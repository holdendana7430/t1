代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wg.521024.cn

[S21] C：字符类别判断
来源：http://wc.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lw.521024.cn

[S22] C：字符串转数字
来源：http://nm.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ct.wgjwhj.cn

[S23] C：随机数
来源：http://oe.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kl.szsharing.cn

[S24] C：获取本地时间
来源：http://ds.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pi.9csxet.cn

[S25] C：内存拷贝
来源：http://am.huixiangedu.cn

memcpy(dst, src, n);
来源：http://vy.nicolike.cn

[S26] C：内存清零
来源：http://uw.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://tb.gzmigu.cn

[S27] C：定义常量
来源：http://yn.shtwfgs.cn

const double PI = 3.14159;
来源：http://jk.jctech888.com.cn

[S28] C：静态变量
来源：http://vb.szsharing.cn

static int counter = 0;
来源：http://ab.gzmigu.cn

[S29] C：变参函数
来源：http://ac.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hr.shtwfgs.cn

[S30] C：头文件保护
来源：http://ov.yuexingan06.cn

#ifndef X_H
来源：http://xx.yuntaijiaju.cn

#define X_H
来源：http://sb.panjiajie.cn

#endif
来源：http://iy.szsharing.cn

[S31] C++：Hello World
来源：http://wz.huixiangedu.cn

#include <iostream>
来源：http://qc.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://ar.huixinmuqiang.cn

[S32] C++：字符串
来源：http://yc.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://pu.huanxung.cn

[S33] C++：vector 增删
来源：http://vd.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://da.newstarts.cn

[S34] C++：遍历 vector
来源：http://ct.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://pv.9csxet.cn

[S35] C++：map
来源：http://hm.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fl.hnjuh.cn

[S36] C++：unordered_map
来源：http://dq.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zk.shxzskj.cn

[S37] C++：set
来源：http://hb.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lc.9csxet.cn

[S38] C++：排序
来源：http://bb.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://bu.asd995.cn

[S39] C++：自定义比较器排序
来源：http://ba.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ys.asd995.cn

[S40] C++：查找元素
来源：http://eh.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yf.szxytkj.cn

[S41] C++：类与构造函数
来源：http://pt.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://se.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://og.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://td.shxzskj.cn

[S43] C++：智能指针
来源：http://gs.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://un.szsharing.cn

[S44] C++：引用传参
来源：http://jk.9csxet.cn

void inc(int &x) { ++x; }
来源：http://oa.huixinmuqiang.cn

[S45] C++：lambda
来源：http://qe.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dg.asd995.cn

[S46] C++：函数模板
来源：http://er.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sv.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://fs.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xi.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://zn.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xw.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://bw.yuntaijiaju.cn

[S49] C++：写文件
来源：http://oi.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wz.panjiajie.cn

[S50] C++：格式化数字
来源：http://pe.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pt.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://az.haigaiapp.cn

static_cast<double>(a) / b
来源：http://zw.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://oa.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://oo.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://pr.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://rs.colortex.cn

[S54] C++：异常处理
来源：http://xc.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qj.hahajie.cn

[S55] C++：结构化绑定
来源：http://fe.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ll.jctech888.com.cn

[S56] C++：optional
来源：http://dp.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mv.shxzukj.cn

[S57] C++：编译期常量
来源：http://sb.wgjwhj.cn

constexpr int N = 10;
来源：http://ga.hahajie.cn

[S58] C++：命名空间
来源：http://le.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://ro.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://yb.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bc.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://xk.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yt.huanxung.cn

================================================================================
来源：http://yz.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kt.521024.cn

================================================================================
来源：http://zz.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://tb.szsharing.cn

println("Hello")
来源：http://he.hnjuh.cn

[T02] Kotlin：变量
来源：http://bv.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ag.colortex.cn

[T03] Kotlin：字符串模板
来源：http://hy.hahajie.cn

"值: $b"
来源：http://ha.asd995.cn

[T04] Kotlin：空安全
来源：http://yu.shxzskj.cn

val n: String? = null;  n?.length
来源：http://ek.colortex.cn

[T05] Kotlin：when 表达式
来源：http://rj.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mj.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://he.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mp.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://km.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ak.lnxyls.cn

[T08] Kotlin：数据类
来源：http://kc.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://pe.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://cl.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://cj.hahajie.cn

[T10] Kotlin：默认参数
来源：http://il.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gh.521024.cn

[T11] Kotlin：协程
来源：http://vu.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gy.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://km.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://tu.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://re.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://fs.wgjwhj.cn

[T14] Kotlin：循环
来源：http://yp.nicolike.cn

for (i in 1..10) println(i)
来源：http://yw.hahajie.cn

[T15] Kotlin：接口
来源：http://gh.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://qr.nicolike.cn

[T16] Swift：Hello World
来源：http://za.shxzskj.cn

print("Hello")
来源：http://ra.hnjuh.cn

[T17] Swift：变量与常量
来源：http://aa.wgjwhj.cn

var a = 1;  let b = 2
来源：http://nc.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://hv.jctech888.com.cn

"值: \(b)"
来源：http://ln.shxzukj.cn

[T19] Swift：可选绑定
来源：http://po.wgjwhj.cn

if let n = opt { print(n) }
来源：http://hs.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://ck.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xd.nicolike.cn

[T21] Swift：遍历
来源：http://ao.shxzukj.cn

for x in a { print(x) }
来源：http://im.muxihuayi.cn

[T22] Swift：字典
来源：http://pw.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://su.jianghongdianzi.cn

[T23] Swift：函数
来源：http://dt.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lr.panjiajie.cn

[T24] Swift：闭包
来源：http://zc.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fa.wgjwhj.cn

[T25] Swift：结构体
来源：http://lj.jctech888.com.cn

struct P { var x: Int }
来源：http://yy.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://ei.nszjky.cn

class A: Base { override func f() {} }
来源：http://yt.jctech888.com.cn

[T27] Swift：错误处理
来源：http://ok.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://py.nicolike.cn

[T28] Swift：枚举
来源：http://oo.muxihuayi.cn

enum Color { case red, green }
来源：http://qw.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://od.nszjky.cn

guard let x = opt else { return }
来源：http://bo.shxzukj.cn

[T30] Swift：协议
来源：http://ln.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://ou.521024.cn

[T31] Lua：Hello World
来源：http://ef.gzmigu.cn

print("Hello")
来源：http://uq.muxihuayi.cn

[T32] Lua：局部变量
来源：http://ei.huixinmuqiang.cn

local a = 1
来源：http://sx.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://al.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fn.panjiajie.cn

[T34] Lua：遍历表
来源：http://xd.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zu.szsharing.cn

[T35] Lua：字典表
来源：http://ro.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://kb.shtwfgs.cn

[T36] Lua：函数
来源：http://xb.jctech888.com.cn

function add(a, b) return a + b end
来源：http://np.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://sm.shxzskj.cn

"a" .. "b"
来源：http://bg.chemitech.net.cn

[T38] Lua：条件
来源：http://jc.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://xi.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://yz.asd995.cn

string.find(s, "%d+")
来源：http://wq.nicolike.cn

[T40] Lua：元表
来源：http://tb.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://at.yuexingan06.cn

[T41] Perl：Hello World
来源：http://ws.shxzukj.cn

print "Hello\n";
来源：http://gr.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://vu.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hn.hahajie.cn

[T43] Perl：字符串插值
来源：http://vf.huanxung.cn

"值: $a"
来源：http://ck.huixinmuqiang.cn

[T44] Perl：条件
来源：http://dp.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://gq.shxzskj.cn

[T45] Perl：数组遍历
来源：http://eo.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://ua.521024.cn

[T46] Perl：哈希操作
来源：http://rk.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bt.gzmigu.cn

[T47] Perl：正则捕获
来源：http://to.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sq.hahajie.cn

[T48] Perl：正则替换
来源：http://kz.521024.cn

$s =~ s/old/new/g;
来源：http://ww.lnxyls.cn

[T49] Perl：函数
来源：http://zk.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oa.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://qg.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wn.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://hv.panjiajie.cn

[T51] Scala：Hello World
来源：http://ki.huixinmuqiang.cn

println("Hello")
来源：http://yv.asd995.cn

[T52] Scala：变量
来源：http://nh.9csxet.cn

val a = 1;  var b = 2
来源：http://cb.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://kn.shxzukj.cn

s"值: $b"
来源：http://xl.huanxung.cn

[T54] Scala：集合映射
来源：http://dx.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://kc.shxzskj.cn

[T55] Scala：集合过滤
来源：http://yb.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ee.shtwfgs.cn

[T56] Scala：样例类
来源：http://wq.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://ku.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://mi.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vx.nszjky.cn

[T58] Scala：函数定义
来源：http://nf.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iv.panjiajie.cn

[T59] Scala：循环
来源：http://kt.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://ai.hnjuh.cn

[T60] Scala：折叠
来源：http://kx.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nu.szxytkj.cn

================================================================================
来源：http://ki.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://og.haigaiapp.cn

================================================================================
来源：http://ik.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://qa.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://en.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://df.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qp.colortex.cn

[U03] Py：加载 .env 配置
来源：http://zm.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://id.nszjky.cn

[U04] Py：变量调试打印
来源：http://tj.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dp.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://pg.hahajie.cn

list(dict.fromkeys(arr))
来源：http://dm.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://gd.muxihuayi.cn

{**a, **b}
来源：http://pa.gzmigu.cn

[U07] Py：反转字典键值
来源：http://ds.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://tq.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://zp.shxzukj.cn

[y for x in nested for y in x]
来源：http://dj.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://cs.jctech888.com.cn

max(d, key=d.get)
来源：http://sa.hnjuh.cn

[U10] Py：按值排序字典
来源：http://un.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qv.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://id.muxihuayi.cn

(x * 2 for x in arr)
来源：http://qg.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ky.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://im.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://hn.muxihuayi.cn

deque(maxlen=10)
来源：http://yp.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://sn.huixinmuqiang.cn

defaultdict(list)
来源：http://xc.yuexingan06.cn

[U15] Py：高精度计时
来源：http://ou.nszjky.cn

t = time.perf_counter()
来源：http://ya.nszjky.cn

[U16] Py：命令行参数解析
来源：http://fn.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nl.gzmigu.cn

[U17] Py：初始化日志
来源：http://uq.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://aj.hahajie.cn

[U18] Py：预编译正则
来源：http://ak.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://xu.nszjky.cn

[U19] Py：正则替换带回调
来源：http://vm.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hm.521024.cn

[U20] Py：缓存函数结果
来源：http://fc.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://lj.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://zr.bjjhwx.cn

@contextlib.contextmanager
来源：http://xq.panjiajie.cn

[U22] Py：矩阵转置
来源：http://fu.colortex.cn

list(zip(*m))
来源：http://lm.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://cy.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wv.asd995.cn

[U24] Py：路径操作
来源：http://jc.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://le.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://ae.huixinmuqiang.cn

csv.DictReader(f)
来源：http://tu.bjjhwx.cn

[U26] Py：并发下载
来源：http://kq.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zq.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://gj.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://sh.nszjky.cn

[U28] Py：类型别名
来源：http://qh.hahajie.cn

UserId = int
来源：http://dq.hahajie.cn

[U29] Py：属性校验
来源：http://eh.szsharing.cn

@property 与 @x.setter 配合
来源：http://gu.shxzukj.cn

[U30] Py：数据类
来源：http://tx.haigaiapp.cn

@dataclass(slots=True)
来源：http://tt.nicolike.cn

[U31] Py：单测
来源：http://hc.gzmigu.cn

python -m pytest -q
来源：http://hl.9csxet.cn

[U32] Py：代码格式化
来源：http://an.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://nq.huanxung.cn

[U33] Py：打包发布
来源：http://jp.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://fv.panjiajie.cn

[U34] Py：判断编码
来源：http://qf.nicolike.cn

chardet.detect(raw)
来源：http://hb.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://su.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sh.yuexingan06.cn

[U36] Py：定时任务
来源：http://fa.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://jq.9csxet.cn

[U37] Py：读写 Excel
来源：http://yo.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ct.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://yl.9csxet.cn

Path(__file__).resolve().parent
来源：http://ar.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://oy.9csxet.cn

sys.stdout.isatty()
来源：http://gi.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://ux.gzmigu.cn

print("err", file=sys.stderr)
来源：http://cx.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://zy.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dk.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://it.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oh.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://po.chemitech.net.cn

namespace App\Http;
来源：http://uq.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://nu.lnxyls.cn

declare(strict_types=1);
来源：http://ae.shxzskj.cn


<!-- 参考信息 -->