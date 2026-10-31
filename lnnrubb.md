代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tf.521024.cn

[S21] C：字符类别判断
来源：http://sd.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jx.asd995.cn

[S22] C：字符串转数字
来源：http://dq.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kd.yuntaijiaju.cn

[S23] C：随机数
来源：http://wa.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://az.chemitech.net.cn

[S24] C：获取本地时间
来源：http://ak.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tz.521024.cn

[S25] C：内存拷贝
来源：http://ys.bjjhwx.cn

memcpy(dst, src, n);
来源：http://wv.chemitech.net.cn

[S26] C：内存清零
来源：http://ch.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://ve.haigaiapp.cn

[S27] C：定义常量
来源：http://nm.colortex.cn

const double PI = 3.14159;
来源：http://tz.jctech888.com.cn

[S28] C：静态变量
来源：http://xz.szsharing.cn

static int counter = 0;
来源：http://cg.yuntaijiaju.cn

[S29] C：变参函数
来源：http://qu.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vq.wgjwhj.cn

[S30] C：头文件保护
来源：http://al.nszjky.cn

#ifndef X_H
来源：http://kx.hnjuh.cn

#define X_H
来源：http://ut.szsharing.cn

#endif
来源：http://mo.shxzskj.cn

[S31] C++：Hello World
来源：http://jl.nszjky.cn

#include <iostream>
来源：http://jp.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://ty.asd995.cn

[S32] C++：字符串
来源：http://nr.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://xf.wgjwhj.cn

[S33] C++：vector 增删
来源：http://ty.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://so.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://dj.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://nz.szsharing.cn

[S35] C++：map
来源：http://yq.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ly.szsharing.cn

[S36] C++：unordered_map
来源：http://cc.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ry.gzmigu.cn

[S37] C++：set
来源：http://py.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vq.shxzukj.cn

[S38] C++：排序
来源：http://gu.colortex.cn

std::sort(v.begin(), v.end());
来源：http://jr.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://gm.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://av.colortex.cn

[S40] C++：查找元素
来源：http://yf.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sy.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://kt.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rx.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://fi.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://jj.chemitech.net.cn

[S43] C++：智能指针
来源：http://yy.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://az.lnxyls.cn

[S44] C++：引用传参
来源：http://kd.huanxung.cn

void inc(int &x) { ++x; }
来源：http://ga.huanxung.cn

[S45] C++：lambda
来源：http://li.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ho.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://fz.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sm.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://po.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kr.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://pp.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lj.huanxung.cn

while (std::getline(in, line)) { }
来源：http://qe.gzmigu.cn

[S49] C++：写文件
来源：http://qq.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ui.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://mu.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yw.shxzukj.cn

[S51] C++：显式类型转换
来源：http://bb.gzmigu.cn

static_cast<double>(a) / b
来源：http://rd.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://ip.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://em.hahajie.cn

[S53] C++：移动语义
来源：http://mr.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://ff.hahajie.cn

[S54] C++：异常处理
来源：http://qp.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ja.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://iy.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xq.gzmigu.cn

[S56] C++：optional
来源：http://hc.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ba.newstarts.cn

[S57] C++：编译期常量
来源：http://aw.jctech888.com.cn

constexpr int N = 10;
来源：http://ba.muxihuayi.cn

[S58] C++：命名空间
来源：http://ug.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://aq.panjiajie.cn

[S59] C++：静态断言
来源：http://ht.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ul.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://lp.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zk.nszjky.cn

================================================================================
来源：http://xh.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yl.asd995.cn

================================================================================
来源：http://rc.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://nc.szxytkj.cn

println("Hello")
来源：http://jw.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://in.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ax.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://zj.shxzukj.cn

"值: $b"
来源：http://ty.9csxet.cn

[T04] Kotlin：空安全
来源：http://go.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://ym.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://qc.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vi.huanxung.cn

[T06] Kotlin：集合映射
来源：http://tj.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zn.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://uc.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ni.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://wb.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://iy.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://ne.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://xg.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://mv.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uj.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://cw.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dr.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://yh.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://zm.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://on.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://kt.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://du.lnxyls.cn

for (i in 1..10) println(i)
来源：http://fv.asd995.cn

[T15] Kotlin：接口
来源：http://cj.521024.cn

interface Shape { fun area(): Double }
来源：http://jp.szxytkj.cn

[T16] Swift：Hello World
来源：http://sc.jctech888.com.cn

print("Hello")
来源：http://xv.nszjky.cn

[T17] Swift：变量与常量
来源：http://gr.shxzskj.cn

var a = 1;  let b = 2
来源：http://oj.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://ee.huanxung.cn

"值: \(b)"
来源：http://nw.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://po.huixiangedu.cn

if let n = opt { print(n) }
来源：http://nz.wgjwhj.cn

[T20] Swift：数组操作
来源：http://gu.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lx.szsharing.cn

[T21] Swift：遍历
来源：http://kj.hnjuh.cn

for x in a { print(x) }
来源：http://ao.newstarts.cn

[T22] Swift：字典
来源：http://al.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://iw.jctech888.com.cn

[T23] Swift：函数
来源：http://iq.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rk.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://fn.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qf.nicolike.cn

[T25] Swift：结构体
来源：http://hh.521024.cn

struct P { var x: Int }
来源：http://gq.shtwfgs.cn

[T26] Swift：类与重写
来源：http://np.gzmigu.cn

class A: Base { override func f() {} }
来源：http://cc.nszjky.cn

[T27] Swift：错误处理
来源：http://gt.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://wg.huanxung.cn

[T28] Swift：枚举
来源：http://no.shtwfgs.cn

enum Color { case red, green }
来源：http://pt.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://vl.jctech888.com.cn

guard let x = opt else { return }
来源：http://bz.muxihuayi.cn

[T30] Swift：协议
来源：http://uw.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://ma.shtwfgs.cn

[T31] Lua：Hello World
来源：http://uq.hnjuh.cn

print("Hello")
来源：http://ki.hnjuh.cn

[T32] Lua：局部变量
来源：http://kf.9csxet.cn

local a = 1
来源：http://yl.shxzskj.cn

[T33] Lua：表（数组）
来源：http://zl.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hp.jctech888.com.cn

[T34] Lua：遍历表
来源：http://hz.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vl.bjjhwx.cn

[T35] Lua：字典表
来源：http://xh.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://kb.jianghongdianzi.cn

[T36] Lua：函数
来源：http://cs.huanxung.cn

function add(a, b) return a + b end
来源：http://yg.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://xb.bookmarksfly.cn

"a" .. "b"
来源：http://so.huanxung.cn

[T38] Lua：条件
来源：http://nb.newstarts.cn

if x > 0 then print("正") end
来源：http://vm.hnjuh.cn

[T39] Lua：模式匹配
来源：http://qa.shxzukj.cn

string.find(s, "%d+")
来源：http://kg.shtwfgs.cn

[T40] Lua：元表
来源：http://vn.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://ax.bjjhwx.cn

[T41] Perl：Hello World
来源：http://if.colortex.cn

print "Hello\n";
来源：http://xs.hahajie.cn

[T42] Perl：变量类型
来源：http://pz.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rv.shxzskj.cn

[T43] Perl：字符串插值
来源：http://xf.huixinmuqiang.cn

"值: $a"
来源：http://oo.szxytkj.cn

[T44] Perl：条件
来源：http://et.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://ds.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://jd.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://vk.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://fm.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oe.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://vl.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rr.lnxyls.cn

[T48] Perl：正则替换
来源：http://zd.colortex.cn

$s =~ s/old/new/g;
来源：http://xr.huanxung.cn

[T49] Perl：函数
来源：http://yt.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ax.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://yu.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pm.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://eo.newstarts.cn

[T51] Scala：Hello World
来源：http://kw.hahajie.cn

println("Hello")
来源：http://kq.newstarts.cn

[T52] Scala：变量
来源：http://fn.huanxung.cn

val a = 1;  var b = 2
来源：http://ut.nicolike.cn

[T53] Scala：字符串插值
来源：http://xz.jianghongdianzi.cn

s"值: $b"
来源：http://nl.muxihuayi.cn

[T54] Scala：集合映射
来源：http://yi.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://hg.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://vd.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dq.jctech888.com.cn

[T56] Scala：样例类
来源：http://tx.521024.cn

case class User(name: String, age: Int)
来源：http://vj.gzmigu.cn

[T57] Scala：模式匹配
来源：http://tn.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sg.panjiajie.cn

[T58] Scala：函数定义
来源：http://xh.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ni.panjiajie.cn

[T59] Scala：循环
来源：http://qi.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://wi.yuexingan06.cn

[T60] Scala：折叠
来源：http://el.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ph.muxihuayi.cn

================================================================================
来源：http://cn.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://td.newstarts.cn

================================================================================
来源：http://kv.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://tl.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://la.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://dw.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lh.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://my.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pt.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://my.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vz.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://zw.nicolike.cn

list(dict.fromkeys(arr))
来源：http://pv.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://ev.bjjhwx.cn

{**a, **b}
来源：http://rz.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://rv.newstarts.cn

{v: k for k, v in d.items()}
来源：http://vz.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://lt.hnjuh.cn

[y for x in nested for y in x]
来源：http://lu.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://yb.shxzskj.cn

max(d, key=d.get)
来源：http://el.shxzukj.cn

[U10] Py：按值排序字典
来源：http://fk.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pg.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://yb.chemitech.net.cn

(x * 2 for x in arr)
来源：http://kr.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cx.9csxet.cn

Counter(arr).most_common(3)
来源：http://jf.colortex.cn

[U13] Py：固定长度队列
来源：http://cc.bookmarksfly.cn

deque(maxlen=10)
来源：http://hm.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://am.jctech888.com.cn

defaultdict(list)
来源：http://jj.nicolike.cn

[U15] Py：高精度计时
来源：http://zv.wgjwhj.cn

t = time.perf_counter()
来源：http://qs.9csxet.cn

[U16] Py：命令行参数解析
来源：http://xl.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dm.shxzukj.cn

[U17] Py：初始化日志
来源：http://ni.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://ks.shxzskj.cn

[U18] Py：预编译正则
来源：http://fy.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://xr.nicolike.cn

[U19] Py：正则替换带回调
来源：http://nt.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://un.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://ni.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://bu.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://ro.panjiajie.cn

@contextlib.contextmanager
来源：http://uy.szsharing.cn

[U22] Py：矩阵转置
来源：http://vn.asd995.cn

list(zip(*m))
来源：http://op.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://dp.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dm.nszjky.cn

[U24] Py：路径操作
来源：http://oj.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vs.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://vb.wgjwhj.cn

csv.DictReader(f)
来源：http://uj.shxzukj.cn

[U26] Py：并发下载
来源：http://in.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gu.colortex.cn

[U27] Py：异步 HTTP
来源：http://hi.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://lu.huanxung.cn

[U28] Py：类型别名
来源：http://bm.huixinmuqiang.cn

UserId = int
来源：http://hc.chemitech.net.cn

[U29] Py：属性校验
来源：http://rq.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://lo.nszjky.cn

[U30] Py：数据类
来源：http://re.jctech888.com.cn

@dataclass(slots=True)
来源：http://so.newstarts.cn

[U31] Py：单测
来源：http://wz.chemitech.net.cn

python -m pytest -q
来源：http://yi.szsharing.cn

[U32] Py：代码格式化
来源：http://er.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://qr.szsharing.cn

[U33] Py：打包发布
来源：http://cc.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://dl.521024.cn

[U34] Py：判断编码
来源：http://go.yuexingan06.cn

chardet.detect(raw)
来源：http://et.huanxung.cn

[U35] Py：发送邮件
来源：http://ed.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ds.nszjky.cn

[U36] Py：定时任务
来源：http://zm.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://cy.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://vs.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rd.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://cf.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://am.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://bs.shxzukj.cn

sys.stdout.isatty()
来源：http://ur.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://ns.lnxyls.cn

print("err", file=sys.stderr)
来源：http://rd.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://uf.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nk.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://vm.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://df.asd995.cn

[U43] PHP：声明命名空间
来源：http://my.haigaiapp.cn

namespace App\Http;
来源：http://ib.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://rw.huixiangedu.cn

declare(strict_types=1);
来源：http://vr.shxzskj.cn


<!-- 参考信息 -->