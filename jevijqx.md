代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zt.shtwfgs.cn

[S21] C：字符类别判断
来源：http://lc.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jg.jctech888.com.cn

[S22] C：字符串转数字
来源：http://ky.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wj.muxihuayi.cn

[S23] C：随机数
来源：http://gn.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hq.newstarts.cn

[S24] C：获取本地时间
来源：http://gq.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ku.colortex.cn

[S25] C：内存拷贝
来源：http://jh.szxytkj.cn

memcpy(dst, src, n);
来源：http://an.jianghongdianzi.cn

[S26] C：内存清零
来源：http://mo.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://ar.haigaiapp.cn

[S27] C：定义常量
来源：http://ny.panjiajie.cn

const double PI = 3.14159;
来源：http://di.nicolike.cn

[S28] C：静态变量
来源：http://sf.huixinmuqiang.cn

static int counter = 0;
来源：http://cw.jianghongdianzi.cn

[S29] C：变参函数
来源：http://ko.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cb.chemitech.net.cn

[S30] C：头文件保护
来源：http://kz.huixiangedu.cn

#ifndef X_H
来源：http://ws.hnjuh.cn

#define X_H
来源：http://kd.bjjhwx.cn

#endif
来源：http://du.9csxet.cn

[S31] C++：Hello World
来源：http://ex.haigaiapp.cn

#include <iostream>
来源：http://vi.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://cn.yuexingan06.cn

[S32] C++：字符串
来源：http://pu.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://mg.wgjwhj.cn

[S33] C++：vector 增删
来源：http://ui.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gd.hnjuh.cn

[S34] C++：遍历 vector
来源：http://zd.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://vp.hahajie.cn

[S35] C++：map
来源：http://nz.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gk.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://nv.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qj.hahajie.cn

[S37] C++：set
来源：http://ul.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tl.gzmigu.cn

[S38] C++：排序
来源：http://cj.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://ig.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://qq.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lh.hnjuh.cn

[S40] C++：查找元素
来源：http://bx.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dl.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://mj.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xg.newstarts.cn

[S42] C++：继承与虚函数
来源：http://vv.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://yp.newstarts.cn

[S43] C++：智能指针
来源：http://bd.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://td.panjiajie.cn

[S44] C++：引用传参
来源：http://ws.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://or.asd995.cn

[S45] C++：lambda
来源：http://ro.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pf.haigaiapp.cn

[S46] C++：函数模板
来源：http://db.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ea.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://ew.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mn.panjiajie.cn

[S48] C++：逐行读文件
来源：http://fh.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sl.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://so.hahajie.cn

[S49] C++：写文件
来源：http://ea.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nd.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://er.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qw.521024.cn

[S51] C++：显式类型转换
来源：http://xn.huixiangedu.cn

static_cast<double>(a) / b
来源：http://ap.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://gx.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://cx.newstarts.cn

[S53] C++：移动语义
来源：http://cw.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://na.gzmigu.cn

[S54] C++：异常处理
来源：http://ng.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lc.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://ph.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://eg.muxihuayi.cn

[S56] C++：optional
来源：http://fn.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://er.asd995.cn

[S57] C++：编译期常量
来源：http://ig.nicolike.cn

constexpr int N = 10;
来源：http://fn.huanxung.cn

[S58] C++：命名空间
来源：http://tu.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://nt.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://zu.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mt.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://ch.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ng.yuexingan06.cn

================================================================================
来源：http://il.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zo.shxzukj.cn

================================================================================
来源：http://bg.521024.cn

[T01] Kotlin：Hello World
来源：http://ha.szxytkj.cn

println("Hello")
来源：http://qa.muxihuayi.cn

[T02] Kotlin：变量
来源：http://ye.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dz.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://og.szxytkj.cn

"值: $b"
来源：http://le.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://ui.shxzukj.cn

val n: String? = null;  n?.length
来源：http://cz.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://kr.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mj.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://ng.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yz.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://jw.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iy.huanxung.cn

[T08] Kotlin：数据类
来源：http://dz.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://bs.521024.cn

[T09] Kotlin：扩展函数
来源：http://tv.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://aj.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://tj.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ec.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://iz.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://po.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://og.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://kk.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://sv.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://eb.nszjky.cn

[T14] Kotlin：循环
来源：http://aa.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://qb.colortex.cn

[T15] Kotlin：接口
来源：http://zj.szsharing.cn

interface Shape { fun area(): Double }
来源：http://at.hahajie.cn

[T16] Swift：Hello World
来源：http://zi.bjjhwx.cn

print("Hello")
来源：http://bu.lnxyls.cn

[T17] Swift：变量与常量
来源：http://ka.chemitech.net.cn

var a = 1;  let b = 2
来源：http://ht.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://eg.huixinmuqiang.cn

"值: \(b)"
来源：http://rz.lnxyls.cn

[T19] Swift：可选绑定
来源：http://ua.hahajie.cn

if let n = opt { print(n) }
来源：http://fe.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://eh.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vj.hahajie.cn

[T21] Swift：遍历
来源：http://fd.shtwfgs.cn

for x in a { print(x) }
来源：http://ce.lnxyls.cn

[T22] Swift：字典
来源：http://rz.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gu.muxihuayi.cn

[T23] Swift：函数
来源：http://uu.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vz.newstarts.cn

[T24] Swift：闭包
来源：http://th.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hg.gzmigu.cn

[T25] Swift：结构体
来源：http://pg.lnxyls.cn

struct P { var x: Int }
来源：http://kt.hahajie.cn

[T26] Swift：类与重写
来源：http://cn.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://mn.hnjuh.cn

[T27] Swift：错误处理
来源：http://mj.nszjky.cn

do { try f() } catch { print(error) }
来源：http://rn.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://nj.colortex.cn

enum Color { case red, green }
来源：http://of.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://zw.panjiajie.cn

guard let x = opt else { return }
来源：http://bb.huixinmuqiang.cn

[T30] Swift：协议
来源：http://af.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://fi.hnjuh.cn

[T31] Lua：Hello World
来源：http://cp.szxytkj.cn

print("Hello")
来源：http://xq.newstarts.cn

[T32] Lua：局部变量
来源：http://yw.colortex.cn

local a = 1
来源：http://zf.521024.cn

[T33] Lua：表（数组）
来源：http://qb.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rz.szxytkj.cn

[T34] Lua：遍历表
来源：http://fy.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://po.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://vw.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://xo.asd995.cn

[T36] Lua：函数
来源：http://eb.hahajie.cn

function add(a, b) return a + b end
来源：http://bi.nicolike.cn

[T37] Lua：字符串拼接
来源：http://yh.nicolike.cn

"a" .. "b"
来源：http://hl.asd995.cn

[T38] Lua：条件
来源：http://ty.panjiajie.cn

if x > 0 then print("正") end
来源：http://sk.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://em.shtwfgs.cn

string.find(s, "%d+")
来源：http://jd.bookmarksfly.cn

[T40] Lua：元表
来源：http://eu.szsharing.cn

setmetatable({}, { __index = base })
来源：http://xb.colortex.cn

[T41] Perl：Hello World
来源：http://ix.wgjwhj.cn

print "Hello\n";
来源：http://tg.shxzukj.cn

[T42] Perl：变量类型
来源：http://yu.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vp.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://pr.szsharing.cn

"值: $a"
来源：http://gg.shtwfgs.cn

[T44] Perl：条件
来源：http://ca.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://wm.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://nm.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://ia.shxzskj.cn

[T46] Perl：哈希操作
来源：http://yv.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://js.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://ul.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qr.haigaiapp.cn

[T48] Perl：正则替换
来源：http://vb.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://nx.huixiangedu.cn

[T49] Perl：函数
来源：http://pr.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gl.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://id.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oi.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://iw.gzmigu.cn

[T51] Scala：Hello World
来源：http://jy.nicolike.cn

println("Hello")
来源：http://dt.panjiajie.cn

[T52] Scala：变量
来源：http://jo.hnjuh.cn

val a = 1;  var b = 2
来源：http://up.gzmigu.cn

[T53] Scala：字符串插值
来源：http://ra.jctech888.com.cn

s"值: $b"
来源：http://po.nicolike.cn

[T54] Scala：集合映射
来源：http://ev.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://cx.shxzukj.cn

[T55] Scala：集合过滤
来源：http://rz.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cc.9csxet.cn

[T56] Scala：样例类
来源：http://tw.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://sv.nicolike.cn

[T57] Scala：模式匹配
来源：http://hb.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ir.szxytkj.cn

[T58] Scala：函数定义
来源：http://xf.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kf.jctech888.com.cn

[T59] Scala：循环
来源：http://rh.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://kh.yuexingan06.cn

[T60] Scala：折叠
来源：http://kt.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wq.hahajie.cn

================================================================================
来源：http://gj.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ut.bjjhwx.cn

================================================================================
来源：http://pt.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://zz.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oo.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://es.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://is.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://af.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tx.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://es.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gc.szsharing.cn

[U05] Py：列表去重且保序
来源：http://gs.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://fb.shxzskj.cn

[U06] Py：合并两个字典
来源：http://go.huixiangedu.cn

{**a, **b}
来源：http://np.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://rb.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://sb.shxzskj.cn

[U08] Py：展平二维列表
来源：http://jg.huixiangedu.cn

[y for x in nested for y in x]
来源：http://ko.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://sa.shxzukj.cn

max(d, key=d.get)
来源：http://fa.colortex.cn

[U10] Py：按值排序字典
来源：http://gm.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ei.huanxung.cn

[U11] Py：生成器表达式
来源：http://ox.muxihuayi.cn

(x * 2 for x in arr)
来源：http://eu.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vt.lnxyls.cn

Counter(arr).most_common(3)
来源：http://af.huanxung.cn

[U13] Py：固定长度队列
来源：http://ec.lnxyls.cn

deque(maxlen=10)
来源：http://ap.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://od.yuexingan06.cn

defaultdict(list)
来源：http://uu.haigaiapp.cn

[U15] Py：高精度计时
来源：http://vf.nicolike.cn

t = time.perf_counter()
来源：http://uf.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://ja.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ku.asd995.cn

[U17] Py：初始化日志
来源：http://ge.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://df.haigaiapp.cn

[U18] Py：预编译正则
来源：http://qu.nszjky.cn

pat = re.compile(r"\d+")
来源：http://wr.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://jp.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sq.asd995.cn

[U20] Py：缓存函数结果
来源：http://jx.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://qp.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://ji.bjjhwx.cn

@contextlib.contextmanager
来源：http://vc.colortex.cn

[U22] Py：矩阵转置
来源：http://mr.shxzukj.cn

list(zip(*m))
来源：http://bj.asd995.cn

[U23] Py：分块读取大文件
来源：http://uc.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rb.wgjwhj.cn

[U24] Py：路径操作
来源：http://is.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://er.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://vn.bjjhwx.cn

csv.DictReader(f)
来源：http://ga.nszjky.cn

[U26] Py：并发下载
来源：http://na.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ll.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://gs.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://ac.szsharing.cn

[U28] Py：类型别名
来源：http://lk.wgjwhj.cn

UserId = int
来源：http://ua.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://yp.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://ab.muxihuayi.cn

[U30] Py：数据类
来源：http://ud.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://uv.shxzskj.cn

[U31] Py：单测
来源：http://dh.hahajie.cn

python -m pytest -q
来源：http://gj.chemitech.net.cn

[U32] Py：代码格式化
来源：http://cj.huanxung.cn

ruff format . && ruff check --fix .
来源：http://bv.szsharing.cn

[U33] Py：打包发布
来源：http://gz.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://yx.shtwfgs.cn

[U34] Py：判断编码
来源：http://cn.bookmarksfly.cn

chardet.detect(raw)
来源：http://ts.szxytkj.cn

[U35] Py：发送邮件
来源：http://hi.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mz.shtwfgs.cn

[U36] Py：定时任务
来源：http://ho.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://fy.huanxung.cn

[U37] Py：读写 Excel
来源：http://jm.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ln.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://yh.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://eu.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://ua.yuexingan06.cn

sys.stdout.isatty()
来源：http://oe.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://yu.lnxyls.cn

print("err", file=sys.stderr)
来源：http://ux.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://lt.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gc.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://wt.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://da.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://nc.9csxet.cn

namespace App\Http;
来源：http://jj.asd995.cn

[U44] PHP：开启严格类型
来源：http://wt.huixinmuqiang.cn

declare(strict_types=1);
来源：http://of.bjjhwx.cn


<!-- 参考信息 -->