代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://rw.szxytkj.cn

[R70] 时间戳与互转
来源：http://pd.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://ae.shxzskj.cn

[R71] 日期格式化
来源：http://oj.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jh.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://at.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dx.asd995.cn

[R73] 分割大日志
来源：http://ll.nicolike.cn

split -l 1000 big.log part_
来源：http://nh.huanxung.cn

[R74] 批量重命名
来源：http://ve.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://do.hahajie.cn

[R75] 导出环境变量
来源：http://wt.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://of.huixiangedu.cn

[R76] 使用临时文件
来源：http://sd.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uv.newstarts.cn

[R77] 读取用户输入
来源：http://uu.shxzskj.cn

read -rp "请输入: " ans
来源：http://ep.521024.cn

[R78] 交互式菜单
来源：http://tl.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iw.muxihuayi.cn

[R79] 解析命令行选项
来源：http://xx.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lg.521024.cn

[R80] 查看脚本执行耗时
来源：http://mq.chemitech.net.cn

time ./run.sh
来源：http://pm.chemitech.net.cn

================================================================================
来源：http://ci.gzmigu.cn

S. C / C++ 专题
来源：http://nn.yuntaijiaju.cn

================================================================================
来源：http://eh.bookmarksfly.cn

[S01] C：Hello World
来源：http://om.wgjwhj.cn

#include <stdio.h>
来源：http://sz.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hw.newstarts.cn

[S02] C：变量与格式化输出
来源：http://vl.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://uo.shxzukj.cn

[S03] C：读入整数
来源：http://dq.9csxet.cn

int x; scanf("%d", &x);
来源：http://uj.bookmarksfly.cn

[S04] C：字符串复制
来源：http://cs.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ej.haigaiapp.cn

[S05] C：字符串长度
来源：http://uq.panjiajie.cn

strlen(s)
来源：http://xd.wgjwhj.cn

[S06] C：字符串比较
来源：http://ga.panjiajie.cn

strcmp(a, b) == 0
来源：http://hh.nicolike.cn

[S07] C：数组遍历求和
来源：http://rm.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ng.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://sw.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ho.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://tn.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pi.chemitech.net.cn

[S10] C：指针与解引用
来源：http://zs.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://pg.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://br.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://ta.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://be.hnjuh.cn

fclose(f);
来源：http://so.colortex.cn

[S12] C：写文件
来源：http://nb.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tt.wgjwhj.cn

[S13] C：宏定义
来源：http://lh.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://in.hahajie.cn

[S14] C：枚举
来源：http://fj.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://tj.gzmigu.cn

[S15] C：类型转换
来源：http://ad.asd995.cn

(double) a / b
来源：http://on.szxytkj.cn

[S16] C：位操作置位
来源：http://yo.panjiajie.cn

x |= (1 << 3);
来源：http://cf.colortex.cn

[S17] C：安全拼接字符串
来源：http://on.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tl.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://jn.gzmigu.cn

int main(int argc, char **argv)
来源：http://xm.yuexingan06.cn

[S19] C：快速排序
来源：http://wi.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gl.521024.cn

[S20] C：二分查找
来源：http://oq.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cj.yuexingan06.cn

[S21] C：字符类别判断
来源：http://qw.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://na.huixiangedu.cn

[S22] C：字符串转数字
来源：http://sv.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hm.shxzukj.cn

[S23] C：随机数
来源：http://mr.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ha.wgjwhj.cn

[S24] C：获取本地时间
来源：http://ro.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ji.muxihuayi.cn

[S25] C：内存拷贝
来源：http://bq.nicolike.cn

memcpy(dst, src, n);
来源：http://ov.huanxung.cn

[S26] C：内存清零
来源：http://re.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://uc.jianghongdianzi.cn

[S27] C：定义常量
来源：http://mn.panjiajie.cn

const double PI = 3.14159;
来源：http://oq.szxytkj.cn

[S28] C：静态变量
来源：http://ib.shxzskj.cn

static int counter = 0;
来源：http://tf.haigaiapp.cn

[S29] C：变参函数
来源：http://nh.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ey.lnxyls.cn

[S30] C：头文件保护
来源：http://xd.hahajie.cn

#ifndef X_H
来源：http://wa.huixinmuqiang.cn

#define X_H
来源：http://db.szsharing.cn

#endif
来源：http://ox.huanxung.cn

[S31] C++：Hello World
来源：http://eb.bjjhwx.cn

#include <iostream>
来源：http://ac.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://sz.szsharing.cn

[S32] C++：字符串
来源：http://ms.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://ry.bjjhwx.cn

[S33] C++：vector 增删
来源：http://zw.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ku.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://ud.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://ge.gzmigu.cn

[S35] C++：map
来源：http://rb.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kn.bjjhwx.cn

[S36] C++：unordered_map
来源：http://nt.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xf.jctech888.com.cn

[S37] C++：set
来源：http://ot.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sr.huanxung.cn

[S38] C++：排序
来源：http://rh.521024.cn

std::sort(v.begin(), v.end());
来源：http://xf.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://jw.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wc.chemitech.net.cn

[S40] C++：查找元素
来源：http://le.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ra.hahajie.cn

[S41] C++：类与构造函数
来源：http://jv.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nq.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://hb.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://ig.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://hj.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://mq.bookmarksfly.cn

[S44] C++：引用传参
来源：http://fk.newstarts.cn

void inc(int &x) { ++x; }
来源：http://pu.yuntaijiaju.cn

[S45] C++：lambda
来源：http://vq.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tu.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://hv.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xl.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://ca.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iv.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://jk.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qy.hahajie.cn

while (std::getline(in, line)) { }
来源：http://bb.jctech888.com.cn

[S49] C++：写文件
来源：http://az.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://he.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://wg.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ys.521024.cn

[S51] C++：显式类型转换
来源：http://go.yuexingan06.cn

static_cast<double>(a) / b
来源：http://ns.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://yk.521024.cn

int size() const noexcept { return n_; }
来源：http://tg.chemitech.net.cn

[S53] C++：移动语义
来源：http://ks.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://uj.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://ct.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ia.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://hw.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lx.shxzskj.cn

[S56] C++：optional
来源：http://pm.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hi.newstarts.cn

[S57] C++：编译期常量
来源：http://yl.chemitech.net.cn

constexpr int N = 10;
来源：http://js.bjjhwx.cn

[S58] C++：命名空间
来源：http://ba.521024.cn

namespace ns { int f() { return 1; } }
来源：http://ii.szxytkj.cn

[S59] C++：静态断言
来源：http://cr.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tl.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://ar.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lt.shxzskj.cn

================================================================================
来源：http://lg.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ey.bjjhwx.cn

================================================================================
来源：http://co.9csxet.cn

[T01] Kotlin：Hello World
来源：http://lu.yuntaijiaju.cn

println("Hello")
来源：http://mz.szxytkj.cn

[T02] Kotlin：变量
来源：http://lt.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yu.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://hb.panjiajie.cn

"值: $b"
来源：http://fu.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://pt.colortex.cn

val n: String? = null;  n?.length
来源：http://je.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://rr.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sa.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://gk.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fv.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://ql.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xr.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://td.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://fj.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://ya.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://uc.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://lp.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ma.shxzukj.cn

[T11] Kotlin：协程
来源：http://hj.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jt.9csxet.cn

[T12] Kotlin：解构声明
来源：http://av.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://kg.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://hf.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://ah.muxihuayi.cn

[T14] Kotlin：循环
来源：http://ux.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://xi.bjjhwx.cn

[T15] Kotlin：接口
来源：http://kc.szsharing.cn

interface Shape { fun area(): Double }
来源：http://uo.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://gc.nicolike.cn

print("Hello")
来源：http://iu.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://mm.nszjky.cn

var a = 1;  let b = 2
来源：http://ak.9csxet.cn

[T18] Swift：字符串插值
来源：http://xl.colortex.cn

"值: \(b)"
来源：http://nl.lnxyls.cn

[T19] Swift：可选绑定
来源：http://bn.szsharing.cn

if let n = opt { print(n) }
来源：http://ac.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://uf.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mr.bjjhwx.cn

[T21] Swift：遍历
来源：http://dq.panjiajie.cn

for x in a { print(x) }
来源：http://jj.bjjhwx.cn

[T22] Swift：字典
来源：http://pd.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uw.jctech888.com.cn

[T23] Swift：函数
来源：http://gg.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://py.szxytkj.cn

[T24] Swift：闭包
来源：http://nt.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lx.nszjky.cn

[T25] Swift：结构体
来源：http://hn.newstarts.cn

struct P { var x: Int }
来源：http://jg.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://eq.asd995.cn

class A: Base { override func f() {} }
来源：http://yc.asd995.cn

[T27] Swift：错误处理
来源：http://yz.colortex.cn

do { try f() } catch { print(error) }
来源：http://dz.yuexingan06.cn

[T28] Swift：枚举
来源：http://nb.hahajie.cn

enum Color { case red, green }
来源：http://kc.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://ug.nicolike.cn

guard let x = opt else { return }
来源：http://sr.colortex.cn

[T30] Swift：协议
来源：http://uk.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://hm.newstarts.cn

[T31] Lua：Hello World
来源：http://ee.newstarts.cn

print("Hello")
来源：http://no.szsharing.cn

[T32] Lua：局部变量
来源：http://vk.colortex.cn

local a = 1
来源：http://se.panjiajie.cn

[T33] Lua：表（数组）
来源：http://rk.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ye.szsharing.cn

[T34] Lua：遍历表
来源：http://or.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oq.bookmarksfly.cn

[T35] Lua：字典表
来源：http://vo.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://rv.huixinmuqiang.cn

[T36] Lua：函数
来源：http://sb.szxytkj.cn

function add(a, b) return a + b end
来源：http://yj.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://ib.shtwfgs.cn

"a" .. "b"
来源：http://ol.hnjuh.cn

[T38] Lua：条件
来源：http://to.yuexingan06.cn

if x > 0 then print("正") end
来源：http://uz.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://em.szsharing.cn

string.find(s, "%d+")
来源：http://vz.9csxet.cn

[T40] Lua：元表
来源：http://jn.colortex.cn

setmetatable({}, { __index = base })
来源：http://ij.panjiajie.cn

[T41] Perl：Hello World
来源：http://ce.jctech888.com.cn

print "Hello\n";
来源：http://ak.bjjhwx.cn

[T42] Perl：变量类型
来源：http://tm.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ut.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://lg.haigaiapp.cn

"值: $a"
来源：http://om.huixinmuqiang.cn

[T44] Perl：条件
来源：http://lp.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://yh.panjiajie.cn

[T45] Perl：数组遍历
来源：http://kg.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://py.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://lx.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ik.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://zd.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xu.nszjky.cn

[T48] Perl：正则替换
来源：http://uw.nicolike.cn

$s =~ s/old/new/g;
来源：http://vl.newstarts.cn

[T49] Perl：函数
来源：http://dh.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gy.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://ti.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pr.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://tl.yuexingan06.cn

[T51] Scala：Hello World
来源：http://ki.shxzukj.cn

println("Hello")
来源：http://up.bjjhwx.cn

[T52] Scala：变量
来源：http://cf.newstarts.cn

val a = 1;  var b = 2
来源：http://ng.nicolike.cn

[T53] Scala：字符串插值
来源：http://cq.szsharing.cn

s"值: $b"
来源：http://ii.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://fj.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://nq.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://if.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://um.chemitech.net.cn

[T56] Scala：样例类
来源：http://yb.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://ke.huanxung.cn

[T57] Scala：模式匹配
来源：http://no.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://be.chemitech.net.cn

[T58] Scala：函数定义
来源：http://rl.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qd.nszjky.cn

[T59] Scala：循环
来源：http://ta.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://gu.chemitech.net.cn

[T60] Scala：折叠
来源：http://kw.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kv.yuntaijiaju.cn

================================================================================
来源：http://ji.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ac.chemitech.net.cn

================================================================================
来源：http://pb.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://as.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fq.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://gz.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gj.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://yf.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xm.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://ch.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bd.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://vy.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://ac.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://lj.szxytkj.cn

{**a, **b}
来源：http://dr.colortex.cn

[U07] Py：反转字典键值
来源：http://uh.szsharing.cn

{v: k for k, v in d.items()}
来源：http://eb.panjiajie.cn

[U08] Py：展平二维列表
来源：http://ky.yuexingan06.cn

[y for x in nested for y in x]
来源：http://ao.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://ju.panjiajie.cn

max(d, key=d.get)
来源：http://du.shxzskj.cn

[U10] Py：按值排序字典
来源：http://qe.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ut.521024.cn


<!-- 参考信息 -->