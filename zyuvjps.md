代发 wailian999

int main(int argc, char **argv)
来源：http://gd.nicolike.cn

[S19] C：快速排序
来源：http://ux.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ft.huanxung.cn

[S20] C：二分查找
来源：http://sv.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ld.gzmigu.cn

[S21] C：字符类别判断
来源：http://mn.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xf.szsharing.cn

[S22] C：字符串转数字
来源：http://rc.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vo.huixiangedu.cn

[S23] C：随机数
来源：http://xr.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hs.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://ou.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vi.huixiangedu.cn

[S25] C：内存拷贝
来源：http://mh.shtwfgs.cn

memcpy(dst, src, n);
来源：http://di.huixinmuqiang.cn

[S26] C：内存清零
来源：http://mt.hahajie.cn

memset(a, 0, sizeof a);
来源：http://lv.haigaiapp.cn

[S27] C：定义常量
来源：http://cv.szxytkj.cn

const double PI = 3.14159;
来源：http://qn.chemitech.net.cn

[S28] C：静态变量
来源：http://tl.521024.cn

static int counter = 0;
来源：http://jd.shxzukj.cn

[S29] C：变参函数
来源：http://al.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vi.huixiangedu.cn

[S30] C：头文件保护
来源：http://su.hahajie.cn

#ifndef X_H
来源：http://gr.wgjwhj.cn

#define X_H
来源：http://ub.jianghongdianzi.cn

#endif
来源：http://wv.newstarts.cn

[S31] C++：Hello World
来源：http://gc.newstarts.cn

#include <iostream>
来源：http://qz.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://js.nszjky.cn

[S32] C++：字符串
来源：http://ra.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://ci.nszjky.cn

[S33] C++：vector 增删
来源：http://ng.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hi.9csxet.cn

[S34] C++：遍历 vector
来源：http://tb.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://bs.lnxyls.cn

[S35] C++：map
来源：http://dj.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pv.newstarts.cn

[S36] C++：unordered_map
来源：http://yh.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fi.nicolike.cn

[S37] C++：set
来源：http://bu.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mj.colortex.cn

[S38] C++：排序
来源：http://nu.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://rf.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://da.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rs.bookmarksfly.cn

[S40] C++：查找元素
来源：http://ct.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ck.huanxung.cn

[S41] C++：类与构造函数
来源：http://oy.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ly.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://vm.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://vh.panjiajie.cn

[S43] C++：智能指针
来源：http://oa.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://mx.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://zl.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://kk.hahajie.cn

[S45] C++：lambda
来源：http://li.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ir.521024.cn

[S46] C++：函数模板
来源：http://ks.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ma.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://lf.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mu.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://cv.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jk.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://uo.newstarts.cn

[S49] C++：写文件
来源：http://xn.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rc.szxytkj.cn

[S50] C++：格式化数字
来源：http://fx.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ou.gzmigu.cn

[S51] C++：显式类型转换
来源：http://hp.shxzukj.cn

static_cast<double>(a) / b
来源：http://xc.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://ps.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://lc.bookmarksfly.cn

[S53] C++：移动语义
来源：http://pt.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://ys.shxzskj.cn

[S54] C++：异常处理
来源：http://xn.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lu.hnjuh.cn

[S55] C++：结构化绑定
来源：http://nv.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fv.yuexingan06.cn

[S56] C++：optional
来源：http://zy.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sw.huanxung.cn

[S57] C++：编译期常量
来源：http://gl.szxytkj.cn

constexpr int N = 10;
来源：http://wb.huanxung.cn

[S58] C++：命名空间
来源：http://lp.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://jg.szsharing.cn

[S59] C++：静态断言
来源：http://nq.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nm.colortex.cn

[S60] C++：遍历并删除元素
来源：http://af.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oq.bookmarksfly.cn

================================================================================
来源：http://co.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fc.szsharing.cn

================================================================================
来源：http://bu.szsharing.cn

[T01] Kotlin：Hello World
来源：http://tu.szxytkj.cn

println("Hello")
来源：http://tx.hnjuh.cn

[T02] Kotlin：变量
来源：http://tq.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vh.colortex.cn

[T03] Kotlin：字符串模板
来源：http://go.wgjwhj.cn

"值: $b"
来源：http://ps.shxzskj.cn

[T04] Kotlin：空安全
来源：http://hc.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://yl.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://ml.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mq.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://uz.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hc.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://lo.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ye.szxytkj.cn

[T08] Kotlin：数据类
来源：http://xd.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://iq.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://cg.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://ql.szsharing.cn

[T10] Kotlin：默认参数
来源：http://pu.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ba.bjjhwx.cn

[T11] Kotlin：协程
来源：http://ef.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wu.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://ku.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://ap.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://xb.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://bj.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://qo.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://pj.gzmigu.cn

[T15] Kotlin：接口
来源：http://kk.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://ei.bjjhwx.cn

[T16] Swift：Hello World
来源：http://vz.jianghongdianzi.cn

print("Hello")
来源：http://bw.szxytkj.cn

[T17] Swift：变量与常量
来源：http://qf.wgjwhj.cn

var a = 1;  let b = 2
来源：http://he.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://of.gzmigu.cn

"值: \(b)"
来源：http://qx.hahajie.cn

[T19] Swift：可选绑定
来源：http://jf.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://la.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://ji.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mr.nszjky.cn

[T21] Swift：遍历
来源：http://ag.bjjhwx.cn

for x in a { print(x) }
来源：http://wc.chemitech.net.cn

[T22] Swift：字典
来源：http://ml.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oq.hahajie.cn

[T23] Swift：函数
来源：http://ud.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fc.jctech888.com.cn

[T24] Swift：闭包
来源：http://ut.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oq.chemitech.net.cn

[T25] Swift：结构体
来源：http://jj.chemitech.net.cn

struct P { var x: Int }
来源：http://yb.hahajie.cn

[T26] Swift：类与重写
来源：http://zd.szxytkj.cn

class A: Base { override func f() {} }
来源：http://wa.newstarts.cn

[T27] Swift：错误处理
来源：http://ej.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://fu.wgjwhj.cn

[T28] Swift：枚举
来源：http://rv.9csxet.cn

enum Color { case red, green }
来源：http://dd.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://vs.huixiangedu.cn

guard let x = opt else { return }
来源：http://qu.yuexingan06.cn

[T30] Swift：协议
来源：http://aj.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://pj.yuexingan06.cn

[T31] Lua：Hello World
来源：http://mp.shtwfgs.cn

print("Hello")
来源：http://es.huixiangedu.cn

[T32] Lua：局部变量
来源：http://qa.haigaiapp.cn

local a = 1
来源：http://vk.hnjuh.cn

[T33] Lua：表（数组）
来源：http://oq.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pe.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://by.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://it.huixiangedu.cn

[T35] Lua：字典表
来源：http://rx.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://cw.shxzukj.cn

[T36] Lua：函数
来源：http://pa.9csxet.cn

function add(a, b) return a + b end
来源：http://ww.szsharing.cn

[T37] Lua：字符串拼接
来源：http://nf.szxytkj.cn

"a" .. "b"
来源：http://kf.jianghongdianzi.cn

[T38] Lua：条件
来源：http://km.panjiajie.cn

if x > 0 then print("正") end
来源：http://kz.colortex.cn

[T39] Lua：模式匹配
来源：http://nn.szxytkj.cn

string.find(s, "%d+")
来源：http://ov.lnxyls.cn

[T40] Lua：元表
来源：http://hy.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://db.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://de.huanxung.cn

print "Hello\n";
来源：http://ka.huanxung.cn

[T42] Perl：变量类型
来源：http://hq.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://st.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://wm.bookmarksfly.cn

"值: $a"
来源：http://db.jctech888.com.cn

[T44] Perl：条件
来源：http://ym.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://gj.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://va.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://hr.lnxyls.cn

[T46] Perl：哈希操作
来源：http://el.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xp.9csxet.cn

[T47] Perl：正则捕获
来源：http://gr.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yz.szsharing.cn

[T48] Perl：正则替换
来源：http://ic.lnxyls.cn

$s =~ s/old/new/g;
来源：http://hn.colortex.cn

[T49] Perl：函数
来源：http://vy.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dk.9csxet.cn

[T50] Perl：逐行读文件
来源：http://le.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xp.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://vt.muxihuayi.cn

[T51] Scala：Hello World
来源：http://gc.521024.cn

println("Hello")
来源：http://oo.bookmarksfly.cn

[T52] Scala：变量
来源：http://kc.gzmigu.cn

val a = 1;  var b = 2
来源：http://qf.szsharing.cn

[T53] Scala：字符串插值
来源：http://wb.haigaiapp.cn

s"值: $b"
来源：http://hx.shxzskj.cn

[T54] Scala：集合映射
来源：http://as.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://sm.szsharing.cn

[T55] Scala：集合过滤
来源：http://kl.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wm.panjiajie.cn

[T56] Scala：样例类
来源：http://kl.9csxet.cn

case class User(name: String, age: Int)
来源：http://mn.lnxyls.cn

[T57] Scala：模式匹配
来源：http://ka.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ix.shxzskj.cn

[T58] Scala：函数定义
来源：http://ul.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://es.wgjwhj.cn

[T59] Scala：循环
来源：http://ff.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://qn.szxytkj.cn

[T60] Scala：折叠
来源：http://pc.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ds.nicolike.cn

================================================================================
来源：http://pt.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zs.lnxyls.cn

================================================================================
来源：http://ak.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://we.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xi.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://ec.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fj.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://as.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sp.panjiajie.cn

[U04] Py：变量调试打印
来源：http://yq.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ym.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://cv.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://hm.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://oy.newstarts.cn

{**a, **b}
来源：http://zk.newstarts.cn

[U07] Py：反转字典键值
来源：http://jo.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://gh.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://yt.hahajie.cn

[y for x in nested for y in x]
来源：http://lt.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://ff.yuexingan06.cn

max(d, key=d.get)
来源：http://fr.newstarts.cn

[U10] Py：按值排序字典
来源：http://sa.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yy.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://qk.asd995.cn

(x * 2 for x in arr)
来源：http://ji.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cj.colortex.cn

Counter(arr).most_common(3)
来源：http://nj.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://ti.shtwfgs.cn

deque(maxlen=10)
来源：http://lg.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://qe.9csxet.cn

defaultdict(list)
来源：http://lw.bjjhwx.cn

[U15] Py：高精度计时
来源：http://qz.bjjhwx.cn

t = time.perf_counter()
来源：http://xe.asd995.cn

[U16] Py：命令行参数解析
来源：http://bj.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://az.shxzukj.cn

[U17] Py：初始化日志
来源：http://xc.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://ru.asd995.cn

[U18] Py：预编译正则
来源：http://td.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://el.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://xw.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vx.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://py.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://ov.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://xj.yuexingan06.cn

@contextlib.contextmanager
来源：http://vr.shxzskj.cn

[U22] Py：矩阵转置
来源：http://ax.huixiangedu.cn

list(zip(*m))
来源：http://zy.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://xv.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pc.nicolike.cn

[U24] Py：路径操作
来源：http://yu.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ni.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://wl.huanxung.cn

csv.DictReader(f)
来源：http://qg.bjjhwx.cn

[U26] Py：并发下载
来源：http://gf.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lu.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://tp.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://kw.nszjky.cn

[U28] Py：类型别名
来源：http://yg.muxihuayi.cn

UserId = int
来源：http://av.yuexingan06.cn

[U29] Py：属性校验
来源：http://nw.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://ef.szsharing.cn

[U30] Py：数据类
来源：http://bc.asd995.cn

@dataclass(slots=True)
来源：http://tx.szsharing.cn

[U31] Py：单测
来源：http://lm.asd995.cn

python -m pytest -q
来源：http://iw.lnxyls.cn

[U32] Py：代码格式化
来源：http://uk.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://es.nicolike.cn

[U33] Py：打包发布
来源：http://kw.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://tb.hnjuh.cn

[U34] Py：判断编码
来源：http://ss.jctech888.com.cn

chardet.detect(raw)
来源：http://kt.haigaiapp.cn

[U35] Py：发送邮件
来源：http://pr.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xu.nicolike.cn

[U36] Py：定时任务
来源：http://vf.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://wo.asd995.cn

[U37] Py：读写 Excel
来源：http://an.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ni.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://jv.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://ef.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://eq.gzmigu.cn

sys.stdout.isatty()
来源：http://jh.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://uj.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://mj.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://lm.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ns.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://kv.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://op.asd995.cn


<!-- 参考信息 -->