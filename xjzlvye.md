代发 wailian999

int main(int argc, char **argv)
来源：http://td.yuexingan06.cn

[S19] C：快速排序
来源：http://zb.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oy.chemitech.net.cn

[S20] C：二分查找
来源：http://lc.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ny.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://do.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bt.chemitech.net.cn

[S22] C：字符串转数字
来源：http://wh.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ec.hahajie.cn

[S23] C：随机数
来源：http://tz.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dn.yuexingan06.cn

[S24] C：获取本地时间
来源：http://xh.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kl.colortex.cn

[S25] C：内存拷贝
来源：http://cm.hahajie.cn

memcpy(dst, src, n);
来源：http://zo.chemitech.net.cn

[S26] C：内存清零
来源：http://vp.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://rt.521024.cn

[S27] C：定义常量
来源：http://za.wgjwhj.cn

const double PI = 3.14159;
来源：http://rf.huixiangedu.cn

[S28] C：静态变量
来源：http://zh.huixiangedu.cn

static int counter = 0;
来源：http://aa.shxzskj.cn

[S29] C：变参函数
来源：http://pc.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gr.bjjhwx.cn

[S30] C：头文件保护
来源：http://tq.gzmigu.cn

#ifndef X_H
来源：http://jx.huixiangedu.cn

#define X_H
来源：http://wr.hahajie.cn

#endif
来源：http://ll.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://mk.huixiangedu.cn

#include <iostream>
来源：http://ed.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://qm.hahajie.cn

[S32] C++：字符串
来源：http://ja.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://rm.colortex.cn

[S33] C++：vector 增删
来源：http://nt.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uj.shxzskj.cn

[S34] C++：遍历 vector
来源：http://wj.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://zj.jianghongdianzi.cn

[S35] C++：map
来源：http://tp.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mi.hnjuh.cn

[S36] C++：unordered_map
来源：http://vp.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fb.hahajie.cn

[S37] C++：set
来源：http://es.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lg.gzmigu.cn

[S38] C++：排序
来源：http://yy.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://om.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://wo.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://da.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://ak.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ym.szsharing.cn

[S41] C++：类与构造函数
来源：http://gu.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://de.szsharing.cn

[S42] C++：继承与虚函数
来源：http://hq.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://jq.521024.cn

[S43] C++：智能指针
来源：http://jt.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://mj.9csxet.cn

[S44] C++：引用传参
来源：http://wg.9csxet.cn

void inc(int &x) { ++x; }
来源：http://nl.shxzukj.cn

[S45] C++：lambda
来源：http://bu.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jy.shxzukj.cn

[S46] C++：函数模板
来源：http://qq.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mv.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://cb.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dx.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://sz.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ba.9csxet.cn

while (std::getline(in, line)) { }
来源：http://we.wgjwhj.cn

[S49] C++：写文件
来源：http://jn.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ml.yuexingan06.cn

[S50] C++：格式化数字
来源：http://ax.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bq.shxzskj.cn

[S51] C++：显式类型转换
来源：http://mf.asd995.cn

static_cast<double>(a) / b
来源：http://jo.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://kz.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://ih.huanxung.cn

[S53] C++：移动语义
来源：http://hp.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://kr.panjiajie.cn

[S54] C++：异常处理
来源：http://dl.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fx.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://ym.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ky.9csxet.cn

[S56] C++：optional
来源：http://lr.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ke.nicolike.cn

[S57] C++：编译期常量
来源：http://ly.hnjuh.cn

constexpr int N = 10;
来源：http://ji.hnjuh.cn

[S58] C++：命名空间
来源：http://ck.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://vj.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://ou.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xh.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://yo.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ky.gzmigu.cn

================================================================================
来源：http://la.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pr.9csxet.cn

================================================================================
来源：http://dr.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://ws.chemitech.net.cn

println("Hello")
来源：http://mv.hahajie.cn

[T02] Kotlin：变量
来源：http://dy.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gn.colortex.cn

[T03] Kotlin：字符串模板
来源：http://by.newstarts.cn

"值: $b"
来源：http://pp.szsharing.cn

[T04] Kotlin：空安全
来源：http://xn.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://od.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://ax.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qo.nicolike.cn

[T06] Kotlin：集合映射
来源：http://zu.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jh.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://pj.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hr.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://it.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://ch.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://ou.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://wl.9csxet.cn

[T10] Kotlin：默认参数
来源：http://ex.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lg.colortex.cn

[T11] Kotlin：协程
来源：http://pj.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ce.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://ql.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://mg.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://ch.521024.cn

val m = mapOf("a" to 1)
来源：http://nt.521024.cn

[T14] Kotlin：循环
来源：http://gd.newstarts.cn

for (i in 1..10) println(i)
来源：http://hm.9csxet.cn

[T15] Kotlin：接口
来源：http://zq.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://vd.nicolike.cn

[T16] Swift：Hello World
来源：http://qg.huixiangedu.cn

print("Hello")
来源：http://mn.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://ub.newstarts.cn

var a = 1;  let b = 2
来源：http://na.panjiajie.cn

[T18] Swift：字符串插值
来源：http://km.muxihuayi.cn

"值: \(b)"
来源：http://kf.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://xn.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://lk.gzmigu.cn

[T20] Swift：数组操作
来源：http://qt.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://br.bookmarksfly.cn

[T21] Swift：遍历
来源：http://ti.hahajie.cn

for x in a { print(x) }
来源：http://mg.bjjhwx.cn

[T22] Swift：字典
来源：http://jj.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gv.colortex.cn

[T23] Swift：函数
来源：http://gm.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yo.chemitech.net.cn

[T24] Swift：闭包
来源：http://ys.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ns.szsharing.cn

[T25] Swift：结构体
来源：http://uq.bookmarksfly.cn

struct P { var x: Int }
来源：http://it.521024.cn

[T26] Swift：类与重写
来源：http://qj.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://cu.szxytkj.cn

[T27] Swift：错误处理
来源：http://gs.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://ke.muxihuayi.cn

[T28] Swift：枚举
来源：http://ef.yuntaijiaju.cn

enum Color { case red, green }
来源：http://vc.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://zx.huanxung.cn

guard let x = opt else { return }
来源：http://xt.yuexingan06.cn

[T30] Swift：协议
来源：http://xp.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://lf.lnxyls.cn

[T31] Lua：Hello World
来源：http://qm.huixinmuqiang.cn

print("Hello")
来源：http://dy.haigaiapp.cn

[T32] Lua：局部变量
来源：http://uq.jctech888.com.cn

local a = 1
来源：http://if.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://ip.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ph.chemitech.net.cn

[T34] Lua：遍历表
来源：http://xl.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ag.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://jx.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://lw.bjjhwx.cn

[T36] Lua：函数
来源：http://cd.bjjhwx.cn

function add(a, b) return a + b end
来源：http://vp.huanxung.cn

[T37] Lua：字符串拼接
来源：http://uv.hnjuh.cn

"a" .. "b"
来源：http://kv.haigaiapp.cn

[T38] Lua：条件
来源：http://rj.wgjwhj.cn

if x > 0 then print("正") end
来源：http://kx.521024.cn

[T39] Lua：模式匹配
来源：http://ks.shtwfgs.cn

string.find(s, "%d+")
来源：http://tq.haigaiapp.cn

[T40] Lua：元表
来源：http://yk.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://ow.shxzskj.cn

[T41] Perl：Hello World
来源：http://ta.szxytkj.cn

print "Hello\n";
来源：http://xx.nszjky.cn

[T42] Perl：变量类型
来源：http://tp.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wj.shxzskj.cn

[T43] Perl：字符串插值
来源：http://yy.nszjky.cn

"值: $a"
来源：http://av.shxzukj.cn

[T44] Perl：条件
来源：http://ps.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://vr.colortex.cn

[T45] Perl：数组遍历
来源：http://ew.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://gn.asd995.cn

[T46] Perl：哈希操作
来源：http://xo.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nh.newstarts.cn

[T47] Perl：正则捕获
来源：http://li.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cr.shxzukj.cn

[T48] Perl：正则替换
来源：http://wn.nicolike.cn

$s =~ s/old/new/g;
来源：http://qn.shxzskj.cn

[T49] Perl：函数
来源：http://kc.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ah.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://rp.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kk.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://vr.huixiangedu.cn

[T51] Scala：Hello World
来源：http://qz.shxzukj.cn

println("Hello")
来源：http://tq.yuntaijiaju.cn

[T52] Scala：变量
来源：http://tf.bjjhwx.cn

val a = 1;  var b = 2
来源：http://wc.shxzukj.cn

[T53] Scala：字符串插值
来源：http://ob.nicolike.cn

s"值: $b"
来源：http://bk.nicolike.cn

[T54] Scala：集合映射
来源：http://xf.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://uc.gzmigu.cn

[T55] Scala：集合过滤
来源：http://qk.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lz.szxytkj.cn

[T56] Scala：样例类
来源：http://lh.hnjuh.cn

case class User(name: String, age: Int)
来源：http://qb.newstarts.cn

[T57] Scala：模式匹配
来源：http://pu.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nq.521024.cn

[T58] Scala：函数定义
来源：http://co.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://im.shxzukj.cn

[T59] Scala：循环
来源：http://oz.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://mn.gzmigu.cn

[T60] Scala：折叠
来源：http://pd.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dv.9csxet.cn

================================================================================
来源：http://gi.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rp.muxihuayi.cn

================================================================================
来源：http://zb.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://oi.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://to.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://qq.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wn.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://ip.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rp.nszjky.cn

[U04] Py：变量调试打印
来源：http://pr.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ra.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://mr.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://rf.shxzukj.cn

[U06] Py：合并两个字典
来源：http://as.chemitech.net.cn

{**a, **b}
来源：http://bs.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://qr.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://qz.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://kf.gzmigu.cn

[y for x in nested for y in x]
来源：http://we.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://zf.hahajie.cn

max(d, key=d.get)
来源：http://dp.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://zg.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ky.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://fd.newstarts.cn

(x * 2 for x in arr)
来源：http://qx.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uz.huanxung.cn

Counter(arr).most_common(3)
来源：http://er.panjiajie.cn

[U13] Py：固定长度队列
来源：http://uf.hnjuh.cn

deque(maxlen=10)
来源：http://lc.9csxet.cn

[U14] Py：分组收集到列表
来源：http://nq.521024.cn

defaultdict(list)
来源：http://xz.szsharing.cn

[U15] Py：高精度计时
来源：http://je.nicolike.cn

t = time.perf_counter()
来源：http://yk.nicolike.cn

[U16] Py：命令行参数解析
来源：http://dm.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://my.chemitech.net.cn

[U17] Py：初始化日志
来源：http://kd.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://st.nszjky.cn

[U18] Py：预编译正则
来源：http://ae.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://jk.9csxet.cn

[U19] Py：正则替换带回调
来源：http://mn.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ys.huanxung.cn

[U20] Py：缓存函数结果
来源：http://kp.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://gz.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://fd.shtwfgs.cn

@contextlib.contextmanager
来源：http://ha.nszjky.cn

[U22] Py：矩阵转置
来源：http://cp.shxzskj.cn

list(zip(*m))
来源：http://qu.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://zg.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tc.yuexingan06.cn

[U24] Py：路径操作
来源：http://lz.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yc.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://uz.panjiajie.cn

csv.DictReader(f)
来源：http://el.shxzskj.cn

[U26] Py：并发下载
来源：http://hn.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iq.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://jx.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://yj.szxytkj.cn

[U28] Py：类型别名
来源：http://hq.huanxung.cn

UserId = int
来源：http://go.jctech888.com.cn

[U29] Py：属性校验
来源：http://eu.shxzskj.cn

@property 与 @x.setter 配合
来源：http://nj.colortex.cn

[U30] Py：数据类
来源：http://jq.jctech888.com.cn

@dataclass(slots=True)
来源：http://lb.yuntaijiaju.cn

[U31] Py：单测
来源：http://ss.9csxet.cn

python -m pytest -q
来源：http://yx.haigaiapp.cn

[U32] Py：代码格式化
来源：http://uf.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://oe.lnxyls.cn

[U33] Py：打包发布
来源：http://be.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://cb.muxihuayi.cn

[U34] Py：判断编码
来源：http://ze.hnjuh.cn

chardet.detect(raw)
来源：http://ww.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://ag.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rl.huanxung.cn

[U36] Py：定时任务
来源：http://lz.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://rr.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://fv.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://no.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://fe.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://uj.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://ww.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://uh.9csxet.cn

[U40] Py：打印到标准错误
来源：http://eh.521024.cn

print("err", file=sys.stderr)
来源：http://xw.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://ga.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lx.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://dq.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ob.panjiajie.cn


<!-- 参考信息 -->