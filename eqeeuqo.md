代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ni.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://nf.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wi.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://zx.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vr.nszjky.cn

[S23] C：随机数
来源：http://vq.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fa.huixiangedu.cn

[S24] C：获取本地时间
来源：http://tw.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://km.shtwfgs.cn

[S25] C：内存拷贝
来源：http://kz.colortex.cn

memcpy(dst, src, n);
来源：http://pw.yuntaijiaju.cn

[S26] C：内存清零
来源：http://ex.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://cf.yuntaijiaju.cn

[S27] C：定义常量
来源：http://bk.gzmigu.cn

const double PI = 3.14159;
来源：http://py.nicolike.cn

[S28] C：静态变量
来源：http://ke.gzmigu.cn

static int counter = 0;
来源：http://zo.haigaiapp.cn

[S29] C：变参函数
来源：http://fr.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xp.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://ru.huixiangedu.cn

#ifndef X_H
来源：http://ek.shtwfgs.cn

#define X_H
来源：http://aa.hahajie.cn

#endif
来源：http://rp.shxzukj.cn

[S31] C++：Hello World
来源：http://db.muxihuayi.cn

#include <iostream>
来源：http://ix.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://hf.huixinmuqiang.cn

[S32] C++：字符串
来源：http://vl.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://db.lnxyls.cn

[S33] C++：vector 增删
来源：http://gq.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pf.asd995.cn

[S34] C++：遍历 vector
来源：http://ea.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://bc.yuexingan06.cn

[S35] C++：map
来源：http://ak.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ty.muxihuayi.cn

[S36] C++：unordered_map
来源：http://ps.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pn.9csxet.cn

[S37] C++：set
来源：http://ym.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xv.colortex.cn

[S38] C++：排序
来源：http://id.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://yn.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://md.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zx.lnxyls.cn

[S40] C++：查找元素
来源：http://jp.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ec.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://ql.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gy.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://on.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://jw.521024.cn

[S43] C++：智能指针
来源：http://qe.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://ny.haigaiapp.cn

[S44] C++：引用传参
来源：http://if.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://pd.szxytkj.cn

[S45] C++：lambda
来源：http://cf.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xt.521024.cn

[S46] C++：函数模板
来源：http://lu.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qj.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://fp.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://om.nicolike.cn

[S48] C++：逐行读文件
来源：http://aw.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ph.9csxet.cn

while (std::getline(in, line)) { }
来源：http://ac.newstarts.cn

[S49] C++：写文件
来源：http://mq.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rn.gzmigu.cn

[S50] C++：格式化数字
来源：http://zy.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qz.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://dv.shtwfgs.cn

static_cast<double>(a) / b
来源：http://sh.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://lf.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://hf.bookmarksfly.cn

[S53] C++：移动语义
来源：http://ja.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://ga.hahajie.cn

[S54] C++：异常处理
来源：http://ai.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eu.colortex.cn

[S55] C++：结构化绑定
来源：http://yx.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://iw.szsharing.cn

[S56] C++：optional
来源：http://rc.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://si.chemitech.net.cn

[S57] C++：编译期常量
来源：http://ig.bookmarksfly.cn

constexpr int N = 10;
来源：http://wu.muxihuayi.cn

[S58] C++：命名空间
来源：http://hk.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://rm.9csxet.cn

[S59] C++：静态断言
来源：http://tf.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fu.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://mx.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://le.huixiangedu.cn

================================================================================
来源：http://kx.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hd.gzmigu.cn

================================================================================
来源：http://iz.newstarts.cn

[T01] Kotlin：Hello World
来源：http://nt.szsharing.cn

println("Hello")
来源：http://aw.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://oq.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cp.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://ul.hahajie.cn

"值: $b"
来源：http://pl.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://hz.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://dk.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://ci.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dd.newstarts.cn

[T06] Kotlin：集合映射
来源：http://hh.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fl.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://je.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wr.panjiajie.cn

[T08] Kotlin：数据类
来源：http://uh.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://ii.521024.cn

[T09] Kotlin：扩展函数
来源：http://sn.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://sp.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://zn.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wu.9csxet.cn

[T11] Kotlin：协程
来源：http://de.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xp.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://wk.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://cc.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://dz.szsharing.cn

val m = mapOf("a" to 1)
来源：http://tq.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://gi.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://iy.huixiangedu.cn

[T15] Kotlin：接口
来源：http://mr.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://jc.bjjhwx.cn

[T16] Swift：Hello World
来源：http://tf.wgjwhj.cn

print("Hello")
来源：http://ny.nszjky.cn

[T17] Swift：变量与常量
来源：http://qm.shtwfgs.cn

var a = 1;  let b = 2
来源：http://bu.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://jn.jctech888.com.cn

"值: \(b)"
来源：http://kd.shxzukj.cn

[T19] Swift：可选绑定
来源：http://xp.panjiajie.cn

if let n = opt { print(n) }
来源：http://dn.jctech888.com.cn

[T20] Swift：数组操作
来源：http://mq.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fw.szxytkj.cn

[T21] Swift：遍历
来源：http://oe.szxytkj.cn

for x in a { print(x) }
来源：http://in.hnjuh.cn

[T22] Swift：字典
来源：http://bx.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jf.asd995.cn

[T23] Swift：函数
来源：http://dk.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yt.szsharing.cn

[T24] Swift：闭包
来源：http://xy.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://it.bookmarksfly.cn

[T25] Swift：结构体
来源：http://ho.panjiajie.cn

struct P { var x: Int }
来源：http://ia.panjiajie.cn

[T26] Swift：类与重写
来源：http://re.shxzskj.cn

class A: Base { override func f() {} }
来源：http://xj.asd995.cn

[T27] Swift：错误处理
来源：http://wn.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://no.bookmarksfly.cn

[T28] Swift：枚举
来源：http://gq.huanxung.cn

enum Color { case red, green }
来源：http://os.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://qe.haigaiapp.cn

guard let x = opt else { return }
来源：http://sq.9csxet.cn

[T30] Swift：协议
来源：http://wm.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://zk.haigaiapp.cn

[T31] Lua：Hello World
来源：http://ef.szsharing.cn

print("Hello")
来源：http://ge.szxytkj.cn

[T32] Lua：局部变量
来源：http://ph.bookmarksfly.cn

local a = 1
来源：http://my.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://ts.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gr.huixiangedu.cn

[T34] Lua：遍历表
来源：http://po.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qk.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://yu.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://lv.szxytkj.cn

[T36] Lua：函数
来源：http://ds.shtwfgs.cn

function add(a, b) return a + b end
来源：http://bj.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://vi.szxytkj.cn

"a" .. "b"
来源：http://am.szxytkj.cn

[T38] Lua：条件
来源：http://qm.shtwfgs.cn

if x > 0 then print("正") end
来源：http://zf.shxzukj.cn

[T39] Lua：模式匹配
来源：http://la.bjjhwx.cn

string.find(s, "%d+")
来源：http://vb.bookmarksfly.cn

[T40] Lua：元表
来源：http://no.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://xs.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://pc.panjiajie.cn

print "Hello\n";
来源：http://ap.newstarts.cn

[T42] Perl：变量类型
来源：http://lb.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wv.lnxyls.cn

[T43] Perl：字符串插值
来源：http://dj.yuntaijiaju.cn

"值: $a"
来源：http://fy.haigaiapp.cn

[T44] Perl：条件
来源：http://ak.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://en.huanxung.cn

[T45] Perl：数组遍历
来源：http://uv.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://jw.colortex.cn

[T46] Perl：哈希操作
来源：http://bn.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qd.nszjky.cn

[T47] Perl：正则捕获
来源：http://lf.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yi.521024.cn

[T48] Perl：正则替换
来源：http://px.hahajie.cn

$s =~ s/old/new/g;
来源：http://td.shxzukj.cn

[T49] Perl：函数
来源：http://zj.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://at.nicolike.cn

[T50] Perl：逐行读文件
来源：http://sl.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ot.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://lq.jctech888.com.cn

[T51] Scala：Hello World
来源：http://cu.yuexingan06.cn

println("Hello")
来源：http://wk.yuntaijiaju.cn

[T52] Scala：变量
来源：http://af.yuexingan06.cn

val a = 1;  var b = 2
来源：http://aj.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://is.colortex.cn

s"值: $b"
来源：http://ks.yuexingan06.cn

[T54] Scala：集合映射
来源：http://pn.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://du.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://ld.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dw.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://rc.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://sf.nicolike.cn

[T57] Scala：模式匹配
来源：http://fs.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://od.jctech888.com.cn

[T58] Scala：函数定义
来源：http://ee.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://md.lnxyls.cn

[T59] Scala：循环
来源：http://vg.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://re.muxihuayi.cn

[T60] Scala：折叠
来源：http://ok.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rh.jctech888.com.cn

================================================================================
来源：http://vh.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iq.szsharing.cn

================================================================================
来源：http://cy.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://qd.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://va.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://bq.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tp.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://ir.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jx.hnjuh.cn

[U04] Py：变量调试打印
来源：http://qs.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wd.9csxet.cn

[U05] Py：列表去重且保序
来源：http://ke.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://xp.newstarts.cn

[U06] Py：合并两个字典
来源：http://kj.bjjhwx.cn

{**a, **b}
来源：http://do.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://hd.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://yt.nicolike.cn

[U08] Py：展平二维列表
来源：http://gb.huanxung.cn

[y for x in nested for y in x]
来源：http://qn.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://mk.huixinmuqiang.cn

max(d, key=d.get)
来源：http://aq.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://wc.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ap.szsharing.cn

[U11] Py：生成器表达式
来源：http://ls.panjiajie.cn

(x * 2 for x in arr)
来源：http://rs.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lk.shxzukj.cn

Counter(arr).most_common(3)
来源：http://ij.asd995.cn

[U13] Py：固定长度队列
来源：http://lk.hnjuh.cn

deque(maxlen=10)
来源：http://dn.asd995.cn

[U14] Py：分组收集到列表
来源：http://ua.szxytkj.cn

defaultdict(list)
来源：http://qx.shxzskj.cn

[U15] Py：高精度计时
来源：http://mc.gzmigu.cn

t = time.perf_counter()
来源：http://rk.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://ci.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ka.szxytkj.cn

[U17] Py：初始化日志
来源：http://qd.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://au.bjjhwx.cn

[U18] Py：预编译正则
来源：http://vv.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://um.colortex.cn

[U19] Py：正则替换带回调
来源：http://co.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sl.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://ae.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://pq.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://jr.yuexingan06.cn

@contextlib.contextmanager
来源：http://ud.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://xp.huixiangedu.cn

list(zip(*m))
来源：http://qi.hahajie.cn

[U23] Py：分块读取大文件
来源：http://wn.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xe.nicolike.cn

[U24] Py：路径操作
来源：http://bq.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://db.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://wj.yuntaijiaju.cn

csv.DictReader(f)
来源：http://go.shxzukj.cn

[U26] Py：并发下载
来源：http://im.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ka.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://sr.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://nm.szxytkj.cn

[U28] Py：类型别名
来源：http://vp.yuntaijiaju.cn

UserId = int
来源：http://ns.9csxet.cn

[U29] Py：属性校验
来源：http://ts.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://hn.yuntaijiaju.cn

[U30] Py：数据类
来源：http://ux.bookmarksfly.cn

@dataclass(slots=True)
来源：http://tg.jianghongdianzi.cn

[U31] Py：单测
来源：http://vk.colortex.cn

python -m pytest -q
来源：http://oc.huixiangedu.cn

[U32] Py：代码格式化
来源：http://tq.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://lx.hahajie.cn

[U33] Py：打包发布
来源：http://qb.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://tz.panjiajie.cn

[U34] Py：判断编码
来源：http://qg.panjiajie.cn

chardet.detect(raw)
来源：http://wm.9csxet.cn

[U35] Py：发送邮件
来源：http://rt.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vj.521024.cn

[U36] Py：定时任务
来源：http://bv.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://py.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://ix.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mz.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://rf.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://qd.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://ib.yuexingan06.cn

sys.stdout.isatty()
来源：http://kp.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://wg.shxzukj.cn

print("err", file=sys.stderr)
来源：http://hu.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://cd.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rd.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://cd.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pc.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://lq.huixinmuqiang.cn

namespace App\Http;
来源：http://mv.521024.cn

[U44] PHP：开启严格类型
来源：http://je.newstarts.cn

declare(strict_types=1);
来源：http://th.panjiajie.cn


<!-- 参考信息 -->