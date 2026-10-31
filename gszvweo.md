代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://pv.gzmigu.cn

[R70] 时间戳与互转
来源：http://ud.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://ol.colortex.cn

[R71] 日期格式化
来源：http://oy.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lg.9csxet.cn

[R72] 等待端口就绪
来源：http://mu.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dt.bjjhwx.cn

[R73] 分割大日志
来源：http://zp.hnjuh.cn

split -l 1000 big.log part_
来源：http://iv.gzmigu.cn

[R74] 批量重命名
来源：http://cs.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ki.gzmigu.cn

[R75] 导出环境变量
来源：http://vg.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://eb.huanxung.cn

[R76] 使用临时文件
来源：http://da.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xz.jctech888.com.cn

[R77] 读取用户输入
来源：http://gw.shxzskj.cn

read -rp "请输入: " ans
来源：http://ht.wgjwhj.cn

[R78] 交互式菜单
来源：http://xg.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pu.jctech888.com.cn

[R79] 解析命令行选项
来源：http://ad.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hr.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://zf.szxytkj.cn

time ./run.sh
来源：http://ib.nicolike.cn

================================================================================
来源：http://mh.shtwfgs.cn

S. C / C++ 专题
来源：http://xa.521024.cn

================================================================================
来源：http://es.huanxung.cn

[S01] C：Hello World
来源：http://kk.shtwfgs.cn

#include <stdio.h>
来源：http://hh.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://oh.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://ma.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://sj.9csxet.cn

[S03] C：读入整数
来源：http://nc.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://hc.hahajie.cn

[S04] C：字符串复制
来源：http://fi.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nb.asd995.cn

[S05] C：字符串长度
来源：http://ig.jianghongdianzi.cn

strlen(s)
来源：http://dy.huanxung.cn

[S06] C：字符串比较
来源：http://yw.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://rf.colortex.cn

[S07] C：数组遍历求和
来源：http://gy.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hs.asd995.cn

[S08] C：动态内存分配与释放
来源：http://qq.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://up.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://he.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xu.asd995.cn

[S10] C：指针与解引用
来源：http://hi.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://tw.wgjwhj.cn

[S11] C：逐行读文件
来源：http://jt.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://sj.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hc.gzmigu.cn

fclose(f);
来源：http://qp.szxytkj.cn

[S12] C：写文件
来源：http://fe.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cv.shxzskj.cn

[S13] C：宏定义
来源：http://lj.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jx.huixinmuqiang.cn

[S14] C：枚举
来源：http://wn.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://cw.szxytkj.cn

[S15] C：类型转换
来源：http://cr.lnxyls.cn

(double) a / b
来源：http://nk.nicolike.cn

[S16] C：位操作置位
来源：http://xd.haigaiapp.cn

x |= (1 << 3);
来源：http://xc.nszjky.cn

[S17] C：安全拼接字符串
来源：http://ba.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dg.jctech888.com.cn

[S18] C：命令行参数
来源：http://yy.9csxet.cn

int main(int argc, char **argv)
来源：http://mp.huixinmuqiang.cn

[S19] C：快速排序
来源：http://ay.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ba.huixiangedu.cn

[S20] C：二分查找
来源：http://jb.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cx.shtwfgs.cn

[S21] C：字符类别判断
来源：http://yu.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mz.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://nn.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tu.szxytkj.cn

[S23] C：随机数
来源：http://aa.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oc.hahajie.cn

[S24] C：获取本地时间
来源：http://kt.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fi.bjjhwx.cn

[S25] C：内存拷贝
来源：http://fk.yuexingan06.cn

memcpy(dst, src, n);
来源：http://fv.szsharing.cn

[S26] C：内存清零
来源：http://cx.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://cp.chemitech.net.cn

[S27] C：定义常量
来源：http://sw.hnjuh.cn

const double PI = 3.14159;
来源：http://ak.jctech888.com.cn

[S28] C：静态变量
来源：http://wq.asd995.cn

static int counter = 0;
来源：http://xb.newstarts.cn

[S29] C：变参函数
来源：http://ss.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lm.shtwfgs.cn

[S30] C：头文件保护
来源：http://hk.nicolike.cn

#ifndef X_H
来源：http://wj.jianghongdianzi.cn

#define X_H
来源：http://fr.shtwfgs.cn

#endif
来源：http://uo.colortex.cn

[S31] C++：Hello World
来源：http://ig.colortex.cn

#include <iostream>
来源：http://ev.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://fj.asd995.cn

[S32] C++：字符串
来源：http://ux.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://my.colortex.cn

[S33] C++：vector 增删
来源：http://yk.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kd.colortex.cn

[S34] C++：遍历 vector
来源：http://ql.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://cz.newstarts.cn

[S35] C++：map
来源：http://se.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fw.colortex.cn

[S36] C++：unordered_map
来源：http://xb.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://su.szsharing.cn

[S37] C++：set
来源：http://je.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xu.nszjky.cn

[S38] C++：排序
来源：http://on.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://bf.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://jb.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zx.wgjwhj.cn

[S40] C++：查找元素
来源：http://hb.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fy.9csxet.cn

[S41] C++：类与构造函数
来源：http://tj.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://di.newstarts.cn

[S42] C++：继承与虚函数
来源：http://ve.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://ar.gzmigu.cn

[S43] C++：智能指针
来源：http://wq.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://zj.shxzukj.cn

[S44] C++：引用传参
来源：http://zz.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://vp.yuntaijiaju.cn

[S45] C++：lambda
来源：http://kv.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gq.gzmigu.cn

[S46] C++：函数模板
来源：http://rk.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ap.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://sb.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qh.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://gd.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uu.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://ez.gzmigu.cn

[S49] C++：写文件
来源：http://sp.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rl.nszjky.cn

[S50] C++：格式化数字
来源：http://ec.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://og.hahajie.cn

[S51] C++：显式类型转换
来源：http://xv.lnxyls.cn

static_cast<double>(a) / b
来源：http://qq.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://im.nicolike.cn

int size() const noexcept { return n_; }
来源：http://nr.9csxet.cn

[S53] C++：移动语义
来源：http://mf.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://lr.hnjuh.cn

[S54] C++：异常处理
来源：http://ia.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hx.521024.cn

[S55] C++：结构化绑定
来源：http://so.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zw.bookmarksfly.cn

[S56] C++：optional
来源：http://sf.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qo.panjiajie.cn

[S57] C++：编译期常量
来源：http://wm.wgjwhj.cn

constexpr int N = 10;
来源：http://fl.chemitech.net.cn

[S58] C++：命名空间
来源：http://kd.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://id.jctech888.com.cn

[S59] C++：静态断言
来源：http://lv.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zl.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://fr.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://me.szxytkj.cn

================================================================================
来源：http://hl.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://in.wgjwhj.cn

================================================================================
来源：http://qm.huanxung.cn

[T01] Kotlin：Hello World
来源：http://tp.hnjuh.cn

println("Hello")
来源：http://cg.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://mi.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tr.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://tj.bjjhwx.cn

"值: $b"
来源：http://mo.huanxung.cn

[T04] Kotlin：空安全
来源：http://yk.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://hh.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://vp.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ic.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://si.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jh.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://yw.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cp.hahajie.cn

[T08] Kotlin：数据类
来源：http://ni.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://hc.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://mk.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://xp.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://us.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://aj.asd995.cn

[T11] Kotlin：协程
来源：http://to.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yf.asd995.cn

[T12] Kotlin：解构声明
来源：http://bp.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://ys.colortex.cn

[T13] Kotlin：只读 Map
来源：http://yw.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://tc.jctech888.com.cn

[T14] Kotlin：循环
来源：http://le.colortex.cn

for (i in 1..10) println(i)
来源：http://gv.gzmigu.cn

[T15] Kotlin：接口
来源：http://gx.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://kr.szxytkj.cn

[T16] Swift：Hello World
来源：http://oz.nszjky.cn

print("Hello")
来源：http://br.521024.cn

[T17] Swift：变量与常量
来源：http://qw.muxihuayi.cn

var a = 1;  let b = 2
来源：http://ux.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://om.nszjky.cn

"值: \(b)"
来源：http://tx.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://ca.hnjuh.cn

if let n = opt { print(n) }
来源：http://wa.asd995.cn

[T20] Swift：数组操作
来源：http://ch.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rp.9csxet.cn

[T21] Swift：遍历
来源：http://iy.jctech888.com.cn

for x in a { print(x) }
来源：http://as.hnjuh.cn

[T22] Swift：字典
来源：http://os.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xm.nicolike.cn

[T23] Swift：函数
来源：http://zt.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ua.asd995.cn

[T24] Swift：闭包
来源：http://go.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ow.wgjwhj.cn

[T25] Swift：结构体
来源：http://bb.521024.cn

struct P { var x: Int }
来源：http://rc.yuexingan06.cn

[T26] Swift：类与重写
来源：http://oq.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://hr.shxzskj.cn

[T27] Swift：错误处理
来源：http://qp.huanxung.cn

do { try f() } catch { print(error) }
来源：http://ei.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://sk.shxzukj.cn

enum Color { case red, green }
来源：http://op.colortex.cn

[T29] Swift：guard 提前返回
来源：http://pe.shxzskj.cn

guard let x = opt else { return }
来源：http://ch.wgjwhj.cn

[T30] Swift：协议
来源：http://jm.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://ak.szsharing.cn

[T31] Lua：Hello World
来源：http://xe.szsharing.cn

print("Hello")
来源：http://qy.nszjky.cn

[T32] Lua：局部变量
来源：http://yd.haigaiapp.cn

local a = 1
来源：http://zx.gzmigu.cn

[T33] Lua：表（数组）
来源：http://ip.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yx.chemitech.net.cn

[T34] Lua：遍历表
来源：http://by.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yu.shtwfgs.cn

[T35] Lua：字典表
来源：http://dx.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://ov.yuexingan06.cn

[T36] Lua：函数
来源：http://mp.shtwfgs.cn

function add(a, b) return a + b end
来源：http://gy.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://yo.jianghongdianzi.cn

"a" .. "b"
来源：http://yx.huixiangedu.cn

[T38] Lua：条件
来源：http://az.shtwfgs.cn

if x > 0 then print("正") end
来源：http://kb.szxytkj.cn

[T39] Lua：模式匹配
来源：http://rb.panjiajie.cn

string.find(s, "%d+")
来源：http://wy.jianghongdianzi.cn

[T40] Lua：元表
来源：http://mn.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://hi.wgjwhj.cn

[T41] Perl：Hello World
来源：http://kp.shxzskj.cn

print "Hello\n";
来源：http://fx.haigaiapp.cn

[T42] Perl：变量类型
来源：http://ki.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yo.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://gn.huanxung.cn

"值: $a"
来源：http://yr.szsharing.cn

[T44] Perl：条件
来源：http://vk.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://pz.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://do.colortex.cn

for my $x (@arr) { print $x; }
来源：http://ht.newstarts.cn

[T46] Perl：哈希操作
来源：http://pp.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ev.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://ml.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ql.nszjky.cn

[T48] Perl：正则替换
来源：http://ft.shxzskj.cn

$s =~ s/old/new/g;
来源：http://ta.9csxet.cn

[T49] Perl：函数
来源：http://pg.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eb.newstarts.cn

[T50] Perl：逐行读文件
来源：http://js.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://je.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://hn.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://sm.asd995.cn

println("Hello")
来源：http://yz.szsharing.cn

[T52] Scala：变量
来源：http://uy.gzmigu.cn

val a = 1;  var b = 2
来源：http://bg.panjiajie.cn

[T53] Scala：字符串插值
来源：http://re.colortex.cn

s"值: $b"
来源：http://jy.szsharing.cn

[T54] Scala：集合映射
来源：http://mt.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ma.gzmigu.cn

[T55] Scala：集合过滤
来源：http://qz.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://db.wgjwhj.cn

[T56] Scala：样例类
来源：http://pz.newstarts.cn

case class User(name: String, age: Int)
来源：http://iu.panjiajie.cn

[T57] Scala：模式匹配
来源：http://pj.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lh.nicolike.cn

[T58] Scala：函数定义
来源：http://gx.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fy.shtwfgs.cn

[T59] Scala：循环
来源：http://ei.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://gj.szxytkj.cn

[T60] Scala：折叠
来源：http://ib.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xs.lnxyls.cn

================================================================================
来源：http://jv.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vv.shtwfgs.cn

================================================================================
来源：http://no.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://cj.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zl.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://ud.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eb.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://qi.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yz.asd995.cn

[U04] Py：变量调试打印
来源：http://yo.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xs.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://tj.nicolike.cn

list(dict.fromkeys(arr))
来源：http://oj.hahajie.cn

[U06] Py：合并两个字典
来源：http://zu.jianghongdianzi.cn

{**a, **b}
来源：http://ui.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://ld.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://yn.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://df.wgjwhj.cn

[y for x in nested for y in x]
来源：http://ed.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://nv.bookmarksfly.cn

max(d, key=d.get)
来源：http://cb.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://ao.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jx.chemitech.net.cn


<!-- 参考信息 -->