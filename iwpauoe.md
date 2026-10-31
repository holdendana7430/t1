代发 wailian999

int main(int argc, char **argv)
来源：http://zo.huixinmuqiang.cn

[S19] C：快速排序
来源：http://rl.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fk.521024.cn

[S20] C：二分查找
来源：http://wa.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mc.wgjwhj.cn

[S21] C：字符类别判断
来源：http://fk.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zr.muxihuayi.cn

[S22] C：字符串转数字
来源：http://vw.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hm.huanxung.cn

[S23] C：随机数
来源：http://pn.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fb.yuexingan06.cn

[S24] C：获取本地时间
来源：http://gz.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mz.gzmigu.cn

[S25] C：内存拷贝
来源：http://qv.colortex.cn

memcpy(dst, src, n);
来源：http://vq.hnjuh.cn

[S26] C：内存清零
来源：http://vb.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://ix.hnjuh.cn

[S27] C：定义常量
来源：http://ic.shxzukj.cn

const double PI = 3.14159;
来源：http://ah.colortex.cn

[S28] C：静态变量
来源：http://zl.jctech888.com.cn

static int counter = 0;
来源：http://qc.shxzskj.cn

[S29] C：变参函数
来源：http://rr.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ut.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://xr.chemitech.net.cn

#ifndef X_H
来源：http://mg.huixiangedu.cn

#define X_H
来源：http://iu.hnjuh.cn

#endif
来源：http://na.521024.cn

[S31] C++：Hello World
来源：http://cf.newstarts.cn

#include <iostream>
来源：http://cq.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://tq.bookmarksfly.cn

[S32] C++：字符串
来源：http://dd.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://ws.bjjhwx.cn

[S33] C++：vector 增删
来源：http://yu.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yi.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://kb.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://qr.chemitech.net.cn

[S35] C++：map
来源：http://zq.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ug.hahajie.cn

[S36] C++：unordered_map
来源：http://kl.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qc.shxzskj.cn

[S37] C++：set
来源：http://jh.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://te.jctech888.com.cn

[S38] C++：排序
来源：http://dh.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://fj.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://fe.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oi.haigaiapp.cn

[S40] C++：查找元素
来源：http://ki.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wc.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://fu.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ez.asd995.cn

[S42] C++：继承与虚函数
来源：http://eo.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://mq.haigaiapp.cn

[S43] C++：智能指针
来源：http://kv.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://zw.colortex.cn

[S44] C++：引用传参
来源：http://ll.hahajie.cn

void inc(int &x) { ++x; }
来源：http://qr.shxzukj.cn

[S45] C++：lambda
来源：http://by.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oa.nicolike.cn

[S46] C++：函数模板
来源：http://gl.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://if.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://ld.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cb.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://uv.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nv.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://ki.chemitech.net.cn

[S49] C++：写文件
来源：http://jt.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lk.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://ny.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://az.lnxyls.cn

[S51] C++：显式类型转换
来源：http://dl.wgjwhj.cn

static_cast<double>(a) / b
来源：http://vw.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://vx.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://tb.nicolike.cn

[S53] C++：移动语义
来源：http://my.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://bw.bjjhwx.cn

[S54] C++：异常处理
来源：http://aa.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://py.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://om.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zq.hahajie.cn

[S56] C++：optional
来源：http://od.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ot.szsharing.cn

[S57] C++：编译期常量
来源：http://uy.nicolike.cn

constexpr int N = 10;
来源：http://wv.haigaiapp.cn

[S58] C++：命名空间
来源：http://vr.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://lv.9csxet.cn

[S59] C++：静态断言
来源：http://pf.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mj.asd995.cn

[S60] C++：遍历并删除元素
来源：http://wb.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qp.wgjwhj.cn

================================================================================
来源：http://co.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pp.hnjuh.cn

================================================================================
来源：http://ud.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://pr.muxihuayi.cn

println("Hello")
来源：http://vf.jctech888.com.cn

[T02] Kotlin：变量
来源：http://qi.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ei.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://bc.szsharing.cn

"值: $b"
来源：http://wa.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://hq.colortex.cn

val n: String? = null;  n?.length
来源：http://ik.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://ye.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wn.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://it.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ct.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://uf.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fn.lnxyls.cn

[T08] Kotlin：数据类
来源：http://cm.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://lu.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://rl.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://cn.hahajie.cn

[T10] Kotlin：默认参数
来源：http://dl.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://so.jctech888.com.cn

[T11] Kotlin：协程
来源：http://cl.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uz.9csxet.cn

[T12] Kotlin：解构声明
来源：http://ia.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://zo.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://do.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://tq.yuexingan06.cn

[T14] Kotlin：循环
来源：http://xd.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://yq.shxzukj.cn

[T15] Kotlin：接口
来源：http://xs.521024.cn

interface Shape { fun area(): Double }
来源：http://qr.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://xa.yuexingan06.cn

print("Hello")
来源：http://vi.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://ss.yuexingan06.cn

var a = 1;  let b = 2
来源：http://ms.asd995.cn

[T18] Swift：字符串插值
来源：http://wa.asd995.cn

"值: \(b)"
来源：http://ds.nicolike.cn

[T19] Swift：可选绑定
来源：http://sv.huixiangedu.cn

if let n = opt { print(n) }
来源：http://pb.bjjhwx.cn

[T20] Swift：数组操作
来源：http://lp.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://te.bjjhwx.cn

[T21] Swift：遍历
来源：http://po.szxytkj.cn

for x in a { print(x) }
来源：http://bt.jianghongdianzi.cn

[T22] Swift：字典
来源：http://oq.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gq.panjiajie.cn

[T23] Swift：函数
来源：http://ti.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jt.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://ly.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xd.chemitech.net.cn

[T25] Swift：结构体
来源：http://ac.yuntaijiaju.cn

struct P { var x: Int }
来源：http://wx.yuexingan06.cn

[T26] Swift：类与重写
来源：http://zj.521024.cn

class A: Base { override func f() {} }
来源：http://ag.bjjhwx.cn

[T27] Swift：错误处理
来源：http://bq.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://kl.panjiajie.cn

[T28] Swift：枚举
来源：http://ak.newstarts.cn

enum Color { case red, green }
来源：http://ke.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://vz.asd995.cn

guard let x = opt else { return }
来源：http://he.colortex.cn

[T30] Swift：协议
来源：http://ub.asd995.cn

protocol Shape { func area() -> Double }
来源：http://zd.nszjky.cn

[T31] Lua：Hello World
来源：http://xj.bookmarksfly.cn

print("Hello")
来源：http://cb.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://gl.panjiajie.cn

local a = 1
来源：http://pq.shxzukj.cn

[T33] Lua：表（数组）
来源：http://ux.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tk.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://sw.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qx.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://br.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://rl.shxzukj.cn

[T36] Lua：函数
来源：http://zx.szxytkj.cn

function add(a, b) return a + b end
来源：http://mg.newstarts.cn

[T37] Lua：字符串拼接
来源：http://hv.9csxet.cn

"a" .. "b"
来源：http://ny.shxzukj.cn

[T38] Lua：条件
来源：http://cv.asd995.cn

if x > 0 then print("正") end
来源：http://jk.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://ah.hahajie.cn

string.find(s, "%d+")
来源：http://oo.bjjhwx.cn

[T40] Lua：元表
来源：http://vq.newstarts.cn

setmetatable({}, { __index = base })
来源：http://mz.newstarts.cn

[T41] Perl：Hello World
来源：http://kq.nszjky.cn

print "Hello\n";
来源：http://xw.huixiangedu.cn

[T42] Perl：变量类型
来源：http://az.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yy.newstarts.cn

[T43] Perl：字符串插值
来源：http://qj.huanxung.cn

"值: $a"
来源：http://wq.jianghongdianzi.cn

[T44] Perl：条件
来源：http://pk.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://zn.nicolike.cn

[T45] Perl：数组遍历
来源：http://kj.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://jq.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://dm.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ys.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://uz.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hr.jctech888.com.cn

[T48] Perl：正则替换
来源：http://ut.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://tj.newstarts.cn

[T49] Perl：函数
来源：http://hs.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tf.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://dp.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ax.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://rx.muxihuayi.cn

[T51] Scala：Hello World
来源：http://gk.521024.cn

println("Hello")
来源：http://lz.shtwfgs.cn

[T52] Scala：变量
来源：http://mp.colortex.cn

val a = 1;  var b = 2
来源：http://uf.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://fd.szxytkj.cn

s"值: $b"
来源：http://np.colortex.cn

[T54] Scala：集合映射
来源：http://bl.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://fn.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://kw.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zg.huixiangedu.cn

[T56] Scala：样例类
来源：http://pw.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://df.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://fm.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sr.panjiajie.cn

[T58] Scala：函数定义
来源：http://lc.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bt.chemitech.net.cn

[T59] Scala：循环
来源：http://ut.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://aa.huanxung.cn

[T60] Scala：折叠
来源：http://cb.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lh.jctech888.com.cn

================================================================================
来源：http://qy.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dp.haigaiapp.cn

================================================================================
来源：http://gd.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://fs.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zt.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://cb.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fx.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://hr.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ex.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://zv.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jh.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://qe.huanxung.cn

list(dict.fromkeys(arr))
来源：http://yv.gzmigu.cn

[U06] Py：合并两个字典
来源：http://wy.nicolike.cn

{**a, **b}
来源：http://xb.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://rc.asd995.cn

{v: k for k, v in d.items()}
来源：http://ln.hahajie.cn

[U08] Py：展平二维列表
来源：http://jv.shtwfgs.cn

[y for x in nested for y in x]
来源：http://es.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://of.szsharing.cn

max(d, key=d.get)
来源：http://kl.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://va.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xd.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://fk.hnjuh.cn

(x * 2 for x in arr)
来源：http://jf.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zs.shxzskj.cn

Counter(arr).most_common(3)
来源：http://fg.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://im.nicolike.cn

deque(maxlen=10)
来源：http://zm.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://zc.9csxet.cn

defaultdict(list)
来源：http://hs.colortex.cn

[U15] Py：高精度计时
来源：http://kj.szsharing.cn

t = time.perf_counter()
来源：http://ya.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://nx.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yp.shtwfgs.cn

[U17] Py：初始化日志
来源：http://xk.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://cy.huixiangedu.cn

[U18] Py：预编译正则
来源：http://ga.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://oo.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://fr.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://of.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://dn.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://km.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://ns.bjjhwx.cn

@contextlib.contextmanager
来源：http://po.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://xx.huixinmuqiang.cn

list(zip(*m))
来源：http://iv.colortex.cn

[U23] Py：分块读取大文件
来源：http://lw.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xa.haigaiapp.cn

[U24] Py：路径操作
来源：http://lx.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tf.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://ta.asd995.cn

csv.DictReader(f)
来源：http://na.nicolike.cn

[U26] Py：并发下载
来源：http://he.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jb.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://rs.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://yg.szxytkj.cn

[U28] Py：类型别名
来源：http://yu.muxihuayi.cn

UserId = int
来源：http://os.haigaiapp.cn

[U29] Py：属性校验
来源：http://ko.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://dg.chemitech.net.cn

[U30] Py：数据类
来源：http://vg.panjiajie.cn

@dataclass(slots=True)
来源：http://rz.jianghongdianzi.cn

[U31] Py：单测
来源：http://ks.521024.cn

python -m pytest -q
来源：http://ou.chemitech.net.cn

[U32] Py：代码格式化
来源：http://vu.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://xt.521024.cn

[U33] Py：打包发布
来源：http://oz.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://ab.huanxung.cn

[U34] Py：判断编码
来源：http://ti.muxihuayi.cn

chardet.detect(raw)
来源：http://iu.yuexingan06.cn

[U35] Py：发送邮件
来源：http://xs.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ae.huanxung.cn

[U36] Py：定时任务
来源：http://uq.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://ar.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://st.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ah.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://mo.shxzskj.cn

Path(__file__).resolve().parent
来源：http://pq.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://ol.hahajie.cn

sys.stdout.isatty()
来源：http://fw.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://mq.szsharing.cn

print("err", file=sys.stderr)
来源：http://fm.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://tv.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bg.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://iz.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ye.bookmarksfly.cn


<!-- 参考信息 -->