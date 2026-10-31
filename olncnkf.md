代发 wailian999

int x; scanf("%d", &x);
来源：http://ff.newstarts.cn

[S04] C：字符串复制
来源：http://qt.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jv.newstarts.cn

[S05] C：字符串长度
来源：http://zl.shxzskj.cn

strlen(s)
来源：http://zx.muxihuayi.cn

[S06] C：字符串比较
来源：http://zp.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://cf.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://kr.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pj.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://bl.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ha.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://nr.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cf.nszjky.cn

[S10] C：指针与解引用
来源：http://sr.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://ph.huanxung.cn

[S11] C：逐行读文件
来源：http://af.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://rh.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nt.nicolike.cn

fclose(f);
来源：http://xd.nszjky.cn

[S12] C：写文件
来源：http://ox.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iy.huixinmuqiang.cn

[S13] C：宏定义
来源：http://ao.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ml.bookmarksfly.cn

[S14] C：枚举
来源：http://zk.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://gi.colortex.cn

[S15] C：类型转换
来源：http://ol.gzmigu.cn

(double) a / b
来源：http://ed.szsharing.cn

[S16] C：位操作置位
来源：http://jt.colortex.cn

x |= (1 << 3);
来源：http://xy.nszjky.cn

[S17] C：安全拼接字符串
来源：http://pc.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hp.521024.cn

[S18] C：命令行参数
来源：http://ui.shxzukj.cn

int main(int argc, char **argv)
来源：http://zl.wgjwhj.cn

[S19] C：快速排序
来源：http://yf.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lb.hnjuh.cn

[S20] C：二分查找
来源：http://kg.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ua.asd995.cn

[S21] C：字符类别判断
来源：http://ey.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hi.newstarts.cn

[S22] C：字符串转数字
来源：http://ws.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zu.yuntaijiaju.cn

[S23] C：随机数
来源：http://ia.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ky.jctech888.com.cn

[S24] C：获取本地时间
来源：http://ef.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qm.shxzukj.cn

[S25] C：内存拷贝
来源：http://fg.szxytkj.cn

memcpy(dst, src, n);
来源：http://lp.bookmarksfly.cn

[S26] C：内存清零
来源：http://zf.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://vo.asd995.cn

[S27] C：定义常量
来源：http://vj.asd995.cn

const double PI = 3.14159;
来源：http://ug.yuntaijiaju.cn

[S28] C：静态变量
来源：http://ow.shxzukj.cn

static int counter = 0;
来源：http://nh.szsharing.cn

[S29] C：变参函数
来源：http://ph.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://il.chemitech.net.cn

[S30] C：头文件保护
来源：http://dr.haigaiapp.cn

#ifndef X_H
来源：http://za.hnjuh.cn

#define X_H
来源：http://pv.9csxet.cn

#endif
来源：http://rw.bjjhwx.cn

[S31] C++：Hello World
来源：http://vd.haigaiapp.cn

#include <iostream>
来源：http://xf.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://pr.shxzskj.cn

[S32] C++：字符串
来源：http://pu.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://cn.haigaiapp.cn

[S33] C++：vector 增删
来源：http://vq.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ee.shxzskj.cn

[S34] C++：遍历 vector
来源：http://bp.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://by.yuexingan06.cn

[S35] C++：map
来源：http://mx.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ua.wgjwhj.cn

[S36] C++：unordered_map
来源：http://yr.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bz.9csxet.cn

[S37] C++：set
来源：http://kj.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pf.jianghongdianzi.cn

[S38] C++：排序
来源：http://pu.521024.cn

std::sort(v.begin(), v.end());
来源：http://ct.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://ch.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lj.shxzskj.cn

[S40] C++：查找元素
来源：http://jz.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rz.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://zi.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ig.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://ie.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://bd.haigaiapp.cn

[S43] C++：智能指针
来源：http://ed.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://gf.asd995.cn

[S44] C++：引用传参
来源：http://qd.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://px.shxzskj.cn

[S45] C++：lambda
来源：http://mj.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ph.panjiajie.cn

[S46] C++：函数模板
来源：http://bv.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ra.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://vf.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fo.gzmigu.cn

[S48] C++：逐行读文件
来源：http://os.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hw.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://iu.jctech888.com.cn

[S49] C++：写文件
来源：http://fm.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://av.yuexingan06.cn

[S50] C++：格式化数字
来源：http://yk.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yy.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://iu.huixiangedu.cn

static_cast<double>(a) / b
来源：http://er.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://je.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://xd.colortex.cn

[S53] C++：移动语义
来源：http://hk.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://gf.haigaiapp.cn

[S54] C++：异常处理
来源：http://nx.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yo.9csxet.cn

[S55] C++：结构化绑定
来源：http://tv.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jh.jctech888.com.cn

[S56] C++：optional
来源：http://fn.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ik.huixiangedu.cn

[S57] C++：编译期常量
来源：http://qj.wgjwhj.cn

constexpr int N = 10;
来源：http://ig.9csxet.cn

[S58] C++：命名空间
来源：http://zy.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://mn.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://an.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xi.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://wz.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hd.szsharing.cn

================================================================================
来源：http://my.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ov.huanxung.cn

================================================================================
来源：http://ta.newstarts.cn

[T01] Kotlin：Hello World
来源：http://kf.panjiajie.cn

println("Hello")
来源：http://gi.hnjuh.cn

[T02] Kotlin：变量
来源：http://gq.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xl.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://gl.hahajie.cn

"值: $b"
来源：http://xy.hahajie.cn

[T04] Kotlin：空安全
来源：http://gm.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://kf.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://hb.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://an.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://sh.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tx.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://eg.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hy.nicolike.cn

[T08] Kotlin：数据类
来源：http://kt.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://eh.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://ic.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://ow.szsharing.cn

[T10] Kotlin：默认参数
来源：http://pc.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jp.asd995.cn

[T11] Kotlin：协程
来源：http://tf.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oo.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://rq.521024.cn

val (a, b) = Pair(1, 2)
来源：http://jl.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://cd.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://sg.muxihuayi.cn

[T14] Kotlin：循环
来源：http://oi.nicolike.cn

for (i in 1..10) println(i)
来源：http://fp.shxzukj.cn

[T15] Kotlin：接口
来源：http://kq.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://ti.lnxyls.cn

[T16] Swift：Hello World
来源：http://lm.colortex.cn

print("Hello")
来源：http://qj.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://bq.shxzukj.cn

var a = 1;  let b = 2
来源：http://gu.huanxung.cn

[T18] Swift：字符串插值
来源：http://nq.newstarts.cn

"值: \(b)"
来源：http://yk.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://mw.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://ul.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://ra.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bn.hnjuh.cn

[T21] Swift：遍历
来源：http://jj.huixinmuqiang.cn

for x in a { print(x) }
来源：http://dl.asd995.cn

[T22] Swift：字典
来源：http://xs.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ry.lnxyls.cn

[T23] Swift：函数
来源：http://mh.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pc.shxzskj.cn

[T24] Swift：闭包
来源：http://gr.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gq.shtwfgs.cn

[T25] Swift：结构体
来源：http://bm.szsharing.cn

struct P { var x: Int }
来源：http://qa.hahajie.cn

[T26] Swift：类与重写
来源：http://zb.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://kg.hnjuh.cn

[T27] Swift：错误处理
来源：http://ca.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://ca.newstarts.cn

[T28] Swift：枚举
来源：http://vg.jctech888.com.cn

enum Color { case red, green }
来源：http://bx.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://ws.jctech888.com.cn

guard let x = opt else { return }
来源：http://oz.lnxyls.cn

[T30] Swift：协议
来源：http://eg.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://bb.nszjky.cn

[T31] Lua：Hello World
来源：http://te.wgjwhj.cn

print("Hello")
来源：http://vz.huixiangedu.cn

[T32] Lua：局部变量
来源：http://rz.huixinmuqiang.cn

local a = 1
来源：http://lm.hahajie.cn

[T33] Lua：表（数组）
来源：http://zi.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://td.newstarts.cn

[T34] Lua：遍历表
来源：http://al.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nm.9csxet.cn

[T35] Lua：字典表
来源：http://ng.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://tk.huanxung.cn

[T36] Lua：函数
来源：http://ba.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://zo.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://wu.newstarts.cn

"a" .. "b"
来源：http://yi.yuntaijiaju.cn

[T38] Lua：条件
来源：http://gg.colortex.cn

if x > 0 then print("正") end
来源：http://zr.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://vg.9csxet.cn

string.find(s, "%d+")
来源：http://rt.jianghongdianzi.cn

[T40] Lua：元表
来源：http://ad.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://gz.9csxet.cn

[T41] Perl：Hello World
来源：http://zy.szsharing.cn

print "Hello\n";
来源：http://vz.nszjky.cn

[T42] Perl：变量类型
来源：http://os.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mm.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://ml.szxytkj.cn

"值: $a"
来源：http://fq.panjiajie.cn

[T44] Perl：条件
来源：http://vp.colortex.cn

if ($a > 0) { print "正"; }
来源：http://ft.gzmigu.cn

[T45] Perl：数组遍历
来源：http://cl.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://jo.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://yf.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vj.asd995.cn

[T47] Perl：正则捕获
来源：http://uo.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://au.panjiajie.cn

[T48] Perl：正则替换
来源：http://yw.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://bb.panjiajie.cn

[T49] Perl：函数
来源：http://lc.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tv.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://kr.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fx.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://oi.gzmigu.cn

[T51] Scala：Hello World
来源：http://jz.huanxung.cn

println("Hello")
来源：http://yf.521024.cn

[T52] Scala：变量
来源：http://en.521024.cn

val a = 1;  var b = 2
来源：http://re.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://ko.jianghongdianzi.cn

s"值: $b"
来源：http://oj.muxihuayi.cn

[T54] Scala：集合映射
来源：http://bq.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://so.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://ae.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ai.shxzskj.cn

[T56] Scala：样例类
来源：http://ug.huanxung.cn

case class User(name: String, age: Int)
来源：http://nm.asd995.cn

[T57] Scala：模式匹配
来源：http://ad.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://op.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://ng.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://by.nicolike.cn

[T59] Scala：循环
来源：http://xe.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://rj.newstarts.cn

[T60] Scala：折叠
来源：http://dm.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xj.bjjhwx.cn

================================================================================
来源：http://ag.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pn.bjjhwx.cn

================================================================================
来源：http://lh.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://tk.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tk.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://fs.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ao.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://qi.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gu.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://qe.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://am.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://iu.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://te.hahajie.cn

[U06] Py：合并两个字典
来源：http://ww.huanxung.cn

{**a, **b}
来源：http://oy.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://bz.521024.cn

{v: k for k, v in d.items()}
来源：http://hg.nicolike.cn

[U08] Py：展平二维列表
来源：http://qy.muxihuayi.cn

[y for x in nested for y in x]
来源：http://we.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://yx.lnxyls.cn

max(d, key=d.get)
来源：http://dg.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://fj.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xi.521024.cn

[U11] Py：生成器表达式
来源：http://pn.lnxyls.cn

(x * 2 for x in arr)
来源：http://wz.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kq.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://zr.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://uk.muxihuayi.cn

deque(maxlen=10)
来源：http://mb.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://cl.colortex.cn

defaultdict(list)
来源：http://nc.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://sk.wgjwhj.cn

t = time.perf_counter()
来源：http://hr.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://yy.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gw.shxzskj.cn

[U17] Py：初始化日志
来源：http://dr.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ux.521024.cn

[U18] Py：预编译正则
来源：http://ge.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://ri.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://pa.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ia.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://qt.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://wd.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://dm.chemitech.net.cn

@contextlib.contextmanager
来源：http://xr.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://hm.hahajie.cn

list(zip(*m))
来源：http://qr.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://wk.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bq.shxzukj.cn

[U24] Py：路径操作
来源：http://on.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sv.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://fn.wgjwhj.cn

csv.DictReader(f)
来源：http://kq.bookmarksfly.cn

[U26] Py：并发下载
来源：http://hh.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://te.shtwfgs.cn


<!-- 参考信息 -->