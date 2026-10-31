代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ty.szxytkj.cn

[S21] C：字符类别判断
来源：http://hb.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qa.szxytkj.cn

[S22] C：字符串转数字
来源：http://cq.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cm.hahajie.cn

[S23] C：随机数
来源：http://wa.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bv.muxihuayi.cn

[S24] C：获取本地时间
来源：http://gq.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://no.521024.cn

[S25] C：内存拷贝
来源：http://wi.gzmigu.cn

memcpy(dst, src, n);
来源：http://np.yuexingan06.cn

[S26] C：内存清零
来源：http://wn.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://gr.shxzskj.cn

[S27] C：定义常量
来源：http://he.shxzskj.cn

const double PI = 3.14159;
来源：http://nr.chemitech.net.cn

[S28] C：静态变量
来源：http://sy.panjiajie.cn

static int counter = 0;
来源：http://bj.wgjwhj.cn

[S29] C：变参函数
来源：http://sn.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ca.szxytkj.cn

[S30] C：头文件保护
来源：http://np.hahajie.cn

#ifndef X_H
来源：http://ab.yuntaijiaju.cn

#define X_H
来源：http://hg.jianghongdianzi.cn

#endif
来源：http://ik.newstarts.cn

[S31] C++：Hello World
来源：http://gl.szxytkj.cn

#include <iostream>
来源：http://vh.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://sk.nszjky.cn

[S32] C++：字符串
来源：http://ay.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://ie.colortex.cn

[S33] C++：vector 增删
来源：http://km.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ln.gzmigu.cn

[S34] C++：遍历 vector
来源：http://xy.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://br.nicolike.cn

[S35] C++：map
来源：http://wv.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vb.colortex.cn

[S36] C++：unordered_map
来源：http://jk.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hk.yuntaijiaju.cn

[S37] C++：set
来源：http://dt.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vk.bookmarksfly.cn

[S38] C++：排序
来源：http://bn.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://fw.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://ol.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://or.yuexingan06.cn

[S40] C++：查找元素
来源：http://bc.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://no.shxzukj.cn

[S41] C++：类与构造函数
来源：http://yd.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fa.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://pk.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://hh.yuexingan06.cn

[S43] C++：智能指针
来源：http://rd.521024.cn

auto p = std::make_unique<int>(5);
来源：http://nn.wgjwhj.cn

[S44] C++：引用传参
来源：http://tn.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://rb.szsharing.cn

[S45] C++：lambda
来源：http://nf.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ml.asd995.cn

[S46] C++：函数模板
来源：http://jn.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ph.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://bo.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zy.nicolike.cn

[S48] C++：逐行读文件
来源：http://py.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://do.nszjky.cn

while (std::getline(in, line)) { }
来源：http://tv.asd995.cn

[S49] C++：写文件
来源：http://lm.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mt.gzmigu.cn

[S50] C++：格式化数字
来源：http://eu.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ne.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://hz.shtwfgs.cn

static_cast<double>(a) / b
来源：http://sv.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://vk.nicolike.cn

int size() const noexcept { return n_; }
来源：http://wy.asd995.cn

[S53] C++：移动语义
来源：http://wa.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://dl.9csxet.cn

[S54] C++：异常处理
来源：http://kx.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://km.newstarts.cn

[S55] C++：结构化绑定
来源：http://sf.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zx.shxzukj.cn

[S56] C++：optional
来源：http://ob.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sd.szxytkj.cn

[S57] C++：编译期常量
来源：http://bo.yuexingan06.cn

constexpr int N = 10;
来源：http://vd.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://wd.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://ft.521024.cn

[S59] C++：静态断言
来源：http://on.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vx.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://tj.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yc.huixinmuqiang.cn

================================================================================
来源：http://kq.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jn.huixiangedu.cn

================================================================================
来源：http://pk.9csxet.cn

[T01] Kotlin：Hello World
来源：http://im.huanxung.cn

println("Hello")
来源：http://xy.521024.cn

[T02] Kotlin：变量
来源：http://lb.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jx.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://uf.szsharing.cn

"值: $b"
来源：http://kn.shxzskj.cn

[T04] Kotlin：空安全
来源：http://vp.colortex.cn

val n: String? = null;  n?.length
来源：http://vp.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://qw.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dd.huanxung.cn

[T06] Kotlin：集合映射
来源：http://qv.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qn.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://wb.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vi.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://mv.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://tz.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://qg.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://dn.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://ax.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gg.panjiajie.cn

[T11] Kotlin：协程
来源：http://nk.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://li.colortex.cn

[T12] Kotlin：解构声明
来源：http://qj.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://iw.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://yq.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://ap.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://bf.shxzskj.cn

for (i in 1..10) println(i)
来源：http://ck.shxzukj.cn

[T15] Kotlin：接口
来源：http://ng.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://mf.colortex.cn

[T16] Swift：Hello World
来源：http://aa.shxzukj.cn

print("Hello")
来源：http://cj.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://ot.shtwfgs.cn

var a = 1;  let b = 2
来源：http://bc.lnxyls.cn

[T18] Swift：字符串插值
来源：http://lr.bjjhwx.cn

"值: \(b)"
来源：http://qd.9csxet.cn

[T19] Swift：可选绑定
来源：http://rt.shtwfgs.cn

if let n = opt { print(n) }
来源：http://np.hnjuh.cn

[T20] Swift：数组操作
来源：http://cy.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nx.bjjhwx.cn

[T21] Swift：遍历
来源：http://jt.huanxung.cn

for x in a { print(x) }
来源：http://db.jianghongdianzi.cn

[T22] Swift：字典
来源：http://ii.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nq.9csxet.cn

[T23] Swift：函数
来源：http://yb.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wp.haigaiapp.cn

[T24] Swift：闭包
来源：http://ws.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wh.yuexingan06.cn

[T25] Swift：结构体
来源：http://xv.haigaiapp.cn

struct P { var x: Int }
来源：http://si.panjiajie.cn

[T26] Swift：类与重写
来源：http://in.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://ph.wgjwhj.cn

[T27] Swift：错误处理
来源：http://kr.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://lr.yuexingan06.cn

[T28] Swift：枚举
来源：http://dc.huixiangedu.cn

enum Color { case red, green }
来源：http://ui.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://we.lnxyls.cn

guard let x = opt else { return }
来源：http://xp.521024.cn

[T30] Swift：协议
来源：http://uj.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://us.gzmigu.cn

[T31] Lua：Hello World
来源：http://di.hnjuh.cn

print("Hello")
来源：http://od.gzmigu.cn

[T32] Lua：局部变量
来源：http://uu.huixinmuqiang.cn

local a = 1
来源：http://nv.newstarts.cn

[T33] Lua：表（数组）
来源：http://bj.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jz.bjjhwx.cn

[T34] Lua：遍历表
来源：http://jy.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jm.hnjuh.cn

[T35] Lua：字典表
来源：http://tq.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://ij.chemitech.net.cn

[T36] Lua：函数
来源：http://sw.shxzukj.cn

function add(a, b) return a + b end
来源：http://rz.nszjky.cn

[T37] Lua：字符串拼接
来源：http://kj.huixiangedu.cn

"a" .. "b"
来源：http://uo.bjjhwx.cn

[T38] Lua：条件
来源：http://sm.huixiangedu.cn

if x > 0 then print("正") end
来源：http://iz.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://ww.yuexingan06.cn

string.find(s, "%d+")
来源：http://et.yuntaijiaju.cn

[T40] Lua：元表
来源：http://hc.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://wy.haigaiapp.cn

[T41] Perl：Hello World
来源：http://xz.huanxung.cn

print "Hello\n";
来源：http://bc.bjjhwx.cn

[T42] Perl：变量类型
来源：http://ug.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qd.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://by.lnxyls.cn

"值: $a"
来源：http://ln.shxzukj.cn

[T44] Perl：条件
来源：http://ep.asd995.cn

if ($a > 0) { print "正"; }
来源：http://ap.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://cr.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://ko.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://bq.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vy.lnxyls.cn

[T47] Perl：正则捕获
来源：http://lk.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://iz.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://xf.hahajie.cn

$s =~ s/old/new/g;
来源：http://jw.szxytkj.cn

[T49] Perl：函数
来源：http://bz.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ye.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://th.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bf.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://kh.jctech888.com.cn

[T51] Scala：Hello World
来源：http://nc.jianghongdianzi.cn

println("Hello")
来源：http://pc.yuntaijiaju.cn

[T52] Scala：变量
来源：http://we.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://pr.newstarts.cn

[T53] Scala：字符串插值
来源：http://jj.yuntaijiaju.cn

s"值: $b"
来源：http://eh.newstarts.cn

[T54] Scala：集合映射
来源：http://ia.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://dp.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://bl.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jf.lnxyls.cn

[T56] Scala：样例类
来源：http://fy.hahajie.cn

case class User(name: String, age: Int)
来源：http://nb.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://xd.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kr.panjiajie.cn

[T58] Scala：函数定义
来源：http://ds.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jd.colortex.cn

[T59] Scala：循环
来源：http://gm.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://ia.chemitech.net.cn

[T60] Scala：折叠
来源：http://ze.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yk.lnxyls.cn

================================================================================
来源：http://re.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vp.shxzukj.cn

================================================================================
来源：http://gn.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://hl.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ea.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://zr.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yn.asd995.cn

[U03] Py：加载 .env 配置
来源：http://qe.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bl.nszjky.cn

[U04] Py：变量调试打印
来源：http://ve.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wh.nszjky.cn

[U05] Py：列表去重且保序
来源：http://iq.asd995.cn

list(dict.fromkeys(arr))
来源：http://gp.shxzskj.cn

[U06] Py：合并两个字典
来源：http://uu.nszjky.cn

{**a, **b}
来源：http://bw.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://ub.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://wn.szxytkj.cn

[U08] Py：展平二维列表
来源：http://ug.hnjuh.cn

[y for x in nested for y in x]
来源：http://xc.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://qc.bjjhwx.cn

max(d, key=d.get)
来源：http://ha.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://gc.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://un.panjiajie.cn

[U11] Py：生成器表达式
来源：http://zw.yuexingan06.cn

(x * 2 for x in arr)
来源：http://la.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xq.shxzskj.cn

Counter(arr).most_common(3)
来源：http://wp.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://vi.newstarts.cn

deque(maxlen=10)
来源：http://fa.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://lr.bookmarksfly.cn

defaultdict(list)
来源：http://qe.huixiangedu.cn

[U15] Py：高精度计时
来源：http://eu.wgjwhj.cn

t = time.perf_counter()
来源：http://yj.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://mh.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lw.szxytkj.cn

[U17] Py：初始化日志
来源：http://aj.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://sd.chemitech.net.cn

[U18] Py：预编译正则
来源：http://br.asd995.cn

pat = re.compile(r"\d+")
来源：http://rr.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://ao.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iu.hahajie.cn

[U20] Py：缓存函数结果
来源：http://kk.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://ix.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://ys.szxytkj.cn

@contextlib.contextmanager
来源：http://qi.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://lw.szsharing.cn

list(zip(*m))
来源：http://dv.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://ea.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qg.huixiangedu.cn

[U24] Py：路径操作
来源：http://re.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ql.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://po.hahajie.cn

csv.DictReader(f)
来源：http://ac.bjjhwx.cn

[U26] Py：并发下载
来源：http://ou.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ov.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://dw.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://fg.lnxyls.cn

[U28] Py：类型别名
来源：http://ih.huanxung.cn

UserId = int
来源：http://ks.panjiajie.cn

[U29] Py：属性校验
来源：http://bf.szxytkj.cn

@property 与 @x.setter 配合
来源：http://zi.jctech888.com.cn

[U30] Py：数据类
来源：http://kg.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://uv.yuexingan06.cn

[U31] Py：单测
来源：http://lz.nszjky.cn

python -m pytest -q
来源：http://uq.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://qo.521024.cn

ruff format . && ruff check --fix .
来源：http://lh.newstarts.cn

[U33] Py：打包发布
来源：http://rd.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://rk.shtwfgs.cn

[U34] Py：判断编码
来源：http://ma.haigaiapp.cn

chardet.detect(raw)
来源：http://br.shxzukj.cn

[U35] Py：发送邮件
来源：http://ec.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zk.shxzskj.cn

[U36] Py：定时任务
来源：http://xs.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://xk.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://qq.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xd.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://dt.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://ir.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://kh.shxzskj.cn

sys.stdout.isatty()
来源：http://jq.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://mr.asd995.cn

print("err", file=sys.stderr)
来源：http://uc.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ki.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kq.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://da.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yi.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://il.haigaiapp.cn

namespace App\Http;
来源：http://kp.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://xy.521024.cn

declare(strict_types=1);
来源：http://wa.szxytkj.cn


<!-- 参考信息 -->