代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ok.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://ld.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ur.lnxyls.cn

[S22] C：字符串转数字
来源：http://ns.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jx.panjiajie.cn

[S23] C：随机数
来源：http://bz.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ij.shtwfgs.cn

[S24] C：获取本地时间
来源：http://rt.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qt.hnjuh.cn

[S25] C：内存拷贝
来源：http://vt.szxytkj.cn

memcpy(dst, src, n);
来源：http://iy.shxzskj.cn

[S26] C：内存清零
来源：http://ab.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://qj.jctech888.com.cn

[S27] C：定义常量
来源：http://ls.gzmigu.cn

const double PI = 3.14159;
来源：http://ax.jianghongdianzi.cn

[S28] C：静态变量
来源：http://pb.jianghongdianzi.cn

static int counter = 0;
来源：http://yd.szsharing.cn

[S29] C：变参函数
来源：http://yk.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lo.gzmigu.cn

[S30] C：头文件保护
来源：http://lw.huixiangedu.cn

#ifndef X_H
来源：http://jz.gzmigu.cn

#define X_H
来源：http://ib.panjiajie.cn

#endif
来源：http://fv.bjjhwx.cn

[S31] C++：Hello World
来源：http://ap.haigaiapp.cn

#include <iostream>
来源：http://gm.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://kj.jctech888.com.cn

[S32] C++：字符串
来源：http://aw.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://ir.lnxyls.cn

[S33] C++：vector 增删
来源：http://ky.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dw.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://sz.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://kg.bjjhwx.cn

[S35] C++：map
来源：http://rt.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bj.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://cy.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ph.jctech888.com.cn

[S37] C++：set
来源：http://fe.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://es.jianghongdianzi.cn

[S38] C++：排序
来源：http://ym.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://pk.colortex.cn

[S39] C++：自定义比较器排序
来源：http://ey.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nm.521024.cn

[S40] C++：查找元素
来源：http://of.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eh.shxzukj.cn

[S41] C++：类与构造函数
来源：http://bv.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wg.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://nu.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://in.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://sa.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://bq.shtwfgs.cn

[S44] C++：引用传参
来源：http://rh.nicolike.cn

void inc(int &x) { ++x; }
来源：http://wc.shxzskj.cn

[S45] C++：lambda
来源：http://zf.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wf.hahajie.cn

[S46] C++：函数模板
来源：http://ir.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ar.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://rv.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bw.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://qy.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hd.colortex.cn

while (std::getline(in, line)) { }
来源：http://gx.hnjuh.cn

[S49] C++：写文件
来源：http://gp.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ej.colortex.cn

[S50] C++：格式化数字
来源：http://sh.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://md.lnxyls.cn

[S51] C++：显式类型转换
来源：http://uu.jctech888.com.cn

static_cast<double>(a) / b
来源：http://ly.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://yk.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://in.9csxet.cn

[S53] C++：移动语义
来源：http://ml.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://mn.szsharing.cn

[S54] C++：异常处理
来源：http://jr.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fm.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://zi.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bx.jianghongdianzi.cn

[S56] C++：optional
来源：http://fq.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ar.szxytkj.cn

[S57] C++：编译期常量
来源：http://ro.jctech888.com.cn

constexpr int N = 10;
来源：http://kc.gzmigu.cn

[S58] C++：命名空间
来源：http://ds.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://po.yuexingan06.cn

[S59] C++：静态断言
来源：http://du.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://it.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://by.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qc.huanxung.cn

================================================================================
来源：http://fq.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jn.chemitech.net.cn

================================================================================
来源：http://lt.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://bm.asd995.cn

println("Hello")
来源：http://gg.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://nh.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ov.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://kp.shxzukj.cn

"值: $b"
来源：http://cq.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://zx.shxzskj.cn

val n: String? = null;  n?.length
来源：http://vv.521024.cn

[T05] Kotlin：when 表达式
来源：http://yw.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iz.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://ag.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kp.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://am.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://st.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://bg.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://ym.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://md.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://we.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://mk.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ko.szsharing.cn

[T11] Kotlin：协程
来源：http://pn.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ua.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://bm.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://nb.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://ms.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://xt.nszjky.cn

[T14] Kotlin：循环
来源：http://au.9csxet.cn

for (i in 1..10) println(i)
来源：http://mi.shxzukj.cn

[T15] Kotlin：接口
来源：http://ry.521024.cn

interface Shape { fun area(): Double }
来源：http://dg.asd995.cn

[T16] Swift：Hello World
来源：http://ch.521024.cn

print("Hello")
来源：http://cp.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://mi.colortex.cn

var a = 1;  let b = 2
来源：http://nm.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://ng.wgjwhj.cn

"值: \(b)"
来源：http://yi.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://sz.lnxyls.cn

if let n = opt { print(n) }
来源：http://nv.gzmigu.cn

[T20] Swift：数组操作
来源：http://po.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ca.yuexingan06.cn

[T21] Swift：遍历
来源：http://ro.haigaiapp.cn

for x in a { print(x) }
来源：http://bh.lnxyls.cn

[T22] Swift：字典
来源：http://aw.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cc.nszjky.cn

[T23] Swift：函数
来源：http://po.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yy.newstarts.cn

[T24] Swift：闭包
来源：http://jy.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ch.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://tb.szxytkj.cn

struct P { var x: Int }
来源：http://dx.hahajie.cn

[T26] Swift：类与重写
来源：http://xz.huanxung.cn

class A: Base { override func f() {} }
来源：http://my.shxzukj.cn

[T27] Swift：错误处理
来源：http://da.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://en.muxihuayi.cn

[T28] Swift：枚举
来源：http://nc.haigaiapp.cn

enum Color { case red, green }
来源：http://lr.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://wj.newstarts.cn

guard let x = opt else { return }
来源：http://hn.hahajie.cn

[T30] Swift：协议
来源：http://hi.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://lx.nicolike.cn

[T31] Lua：Hello World
来源：http://yh.huixiangedu.cn

print("Hello")
来源：http://sh.gzmigu.cn

[T32] Lua：局部变量
来源：http://kn.wgjwhj.cn

local a = 1
来源：http://lm.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://nd.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uf.asd995.cn

[T34] Lua：遍历表
来源：http://ye.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hx.wgjwhj.cn

[T35] Lua：字典表
来源：http://pw.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://rq.yuntaijiaju.cn

[T36] Lua：函数
来源：http://yk.szxytkj.cn

function add(a, b) return a + b end
来源：http://jm.hahajie.cn

[T37] Lua：字符串拼接
来源：http://zu.yuntaijiaju.cn

"a" .. "b"
来源：http://hz.hnjuh.cn

[T38] Lua：条件
来源：http://je.newstarts.cn

if x > 0 then print("正") end
来源：http://pt.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://jf.muxihuayi.cn

string.find(s, "%d+")
来源：http://ph.muxihuayi.cn

[T40] Lua：元表
来源：http://rj.nicolike.cn

setmetatable({}, { __index = base })
来源：http://bo.lnxyls.cn

[T41] Perl：Hello World
来源：http://vd.bookmarksfly.cn

print "Hello\n";
来源：http://cu.chemitech.net.cn

[T42] Perl：变量类型
来源：http://fr.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ti.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://pq.nszjky.cn

"值: $a"
来源：http://fs.jianghongdianzi.cn

[T44] Perl：条件
来源：http://rk.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://ln.hahajie.cn

[T45] Perl：数组遍历
来源：http://hn.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://bc.lnxyls.cn

[T46] Perl：哈希操作
来源：http://ka.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bh.lnxyls.cn

[T47] Perl：正则捕获
来源：http://vc.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vf.wgjwhj.cn

[T48] Perl：正则替换
来源：http://nu.nicolike.cn

$s =~ s/old/new/g;
来源：http://il.bjjhwx.cn

[T49] Perl：函数
来源：http://gf.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ej.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://ei.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bl.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://kb.panjiajie.cn

[T51] Scala：Hello World
来源：http://cd.nicolike.cn

println("Hello")
来源：http://jw.yuexingan06.cn

[T52] Scala：变量
来源：http://cg.bjjhwx.cn

val a = 1;  var b = 2
来源：http://us.panjiajie.cn

[T53] Scala：字符串插值
来源：http://um.huanxung.cn

s"值: $b"
来源：http://cb.huixiangedu.cn

[T54] Scala：集合映射
来源：http://wa.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://zg.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://ne.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pa.haigaiapp.cn

[T56] Scala：样例类
来源：http://ge.szxytkj.cn

case class User(name: String, age: Int)
来源：http://xo.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://pi.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jm.muxihuayi.cn

[T58] Scala：函数定义
来源：http://ye.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ji.shxzskj.cn

[T59] Scala：循环
来源：http://ce.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://hb.wgjwhj.cn

[T60] Scala：折叠
来源：http://dp.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wb.gzmigu.cn

================================================================================
来源：http://sa.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cb.huanxung.cn

================================================================================
来源：http://zh.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://dy.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wm.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://ay.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lc.asd995.cn

[U03] Py：加载 .env 配置
来源：http://vq.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://po.9csxet.cn

[U04] Py：变量调试打印
来源：http://cf.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ab.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://df.521024.cn

list(dict.fromkeys(arr))
来源：http://qj.shxzskj.cn

[U06] Py：合并两个字典
来源：http://qj.chemitech.net.cn

{**a, **b}
来源：http://sf.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://bu.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://jk.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://hq.haigaiapp.cn

[y for x in nested for y in x]
来源：http://km.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://qr.huanxung.cn

max(d, key=d.get)
来源：http://lo.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://kg.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ge.9csxet.cn

[U11] Py：生成器表达式
来源：http://os.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://mo.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mt.nszjky.cn

Counter(arr).most_common(3)
来源：http://ec.hnjuh.cn

[U13] Py：固定长度队列
来源：http://ga.shtwfgs.cn

deque(maxlen=10)
来源：http://vd.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://lv.muxihuayi.cn

defaultdict(list)
来源：http://ju.yuexingan06.cn

[U15] Py：高精度计时
来源：http://df.newstarts.cn

t = time.perf_counter()
来源：http://zm.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://bj.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pe.yuexingan06.cn

[U17] Py：初始化日志
来源：http://rg.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://ia.asd995.cn

[U18] Py：预编译正则
来源：http://ms.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://aj.asd995.cn

[U19] Py：正则替换带回调
来源：http://pl.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eh.szsharing.cn

[U20] Py：缓存函数结果
来源：http://bx.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://nh.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://dh.muxihuayi.cn

@contextlib.contextmanager
来源：http://by.nszjky.cn

[U22] Py：矩阵转置
来源：http://vf.hahajie.cn

list(zip(*m))
来源：http://ih.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://in.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mb.nszjky.cn

[U24] Py：路径操作
来源：http://pm.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nw.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://wd.haigaiapp.cn

csv.DictReader(f)
来源：http://nt.yuexingan06.cn

[U26] Py：并发下载
来源：http://ad.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oe.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://eg.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://fd.panjiajie.cn

[U28] Py：类型别名
来源：http://wy.muxihuayi.cn

UserId = int
来源：http://st.shxzskj.cn

[U29] Py：属性校验
来源：http://ha.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://pt.bookmarksfly.cn

[U30] Py：数据类
来源：http://pd.521024.cn

@dataclass(slots=True)
来源：http://ks.muxihuayi.cn

[U31] Py：单测
来源：http://rm.hahajie.cn

python -m pytest -q
来源：http://qt.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://lg.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://ml.9csxet.cn

[U33] Py：打包发布
来源：http://ba.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://ab.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://ps.shtwfgs.cn

chardet.detect(raw)
来源：http://jt.bjjhwx.cn

[U35] Py：发送邮件
来源：http://cv.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lj.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://ua.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://fl.9csxet.cn

[U37] Py：读写 Excel
来源：http://xg.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rz.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://cs.newstarts.cn

Path(__file__).resolve().parent
来源：http://ze.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://ly.9csxet.cn

sys.stdout.isatty()
来源：http://tu.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://gl.panjiajie.cn

print("err", file=sys.stderr)
来源：http://on.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://ys.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oc.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://be.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wp.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://qk.szsharing.cn

namespace App\Http;
来源：http://ij.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://nz.yuntaijiaju.cn

declare(strict_types=1);
来源：http://si.szsharing.cn


<!-- 参考信息 -->