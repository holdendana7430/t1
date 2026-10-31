代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://om.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://me.521024.cn

date +%s;  date -d @1700000000
来源：http://nl.521024.cn

[R71] 日期格式化
来源：http://ni.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fd.muxihuayi.cn

[R72] 等待端口就绪
来源：http://dj.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rs.nicolike.cn

[R73] 分割大日志
来源：http://ax.asd995.cn

split -l 1000 big.log part_
来源：http://qd.yuexingan06.cn

[R74] 批量重命名
来源：http://sn.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://na.nszjky.cn

[R75] 导出环境变量
来源：http://sn.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://jo.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://ai.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bh.huixiangedu.cn

[R77] 读取用户输入
来源：http://gn.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://ex.huanxung.cn

[R78] 交互式菜单
来源：http://et.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xs.yuexingan06.cn

[R79] 解析命令行选项
来源：http://wv.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uj.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://vg.muxihuayi.cn

time ./run.sh
来源：http://ii.panjiajie.cn

================================================================================
来源：http://mk.bookmarksfly.cn

S. C / C++ 专题
来源：http://cz.asd995.cn

================================================================================
来源：http://jo.szxytkj.cn

[S01] C：Hello World
来源：http://cl.nszjky.cn

#include <stdio.h>
来源：http://uv.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fu.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://zg.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://tm.lnxyls.cn

[S03] C：读入整数
来源：http://qq.521024.cn

int x; scanf("%d", &x);
来源：http://mq.szsharing.cn

[S04] C：字符串复制
来源：http://sw.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lz.bookmarksfly.cn

[S05] C：字符串长度
来源：http://ex.521024.cn

strlen(s)
来源：http://wj.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://ji.szxytkj.cn

strcmp(a, b) == 0
来源：http://ep.gzmigu.cn

[S07] C：数组遍历求和
来源：http://bj.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dj.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://ni.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://te.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://od.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wi.shxzskj.cn

[S10] C：指针与解引用
来源：http://hp.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://mu.chemitech.net.cn

[S11] C：逐行读文件
来源：http://or.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://eg.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pi.521024.cn

fclose(f);
来源：http://zo.huanxung.cn

[S12] C：写文件
来源：http://ft.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ud.panjiajie.cn

[S13] C：宏定义
来源：http://zx.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cx.shtwfgs.cn

[S14] C：枚举
来源：http://bf.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://kz.wgjwhj.cn

[S15] C：类型转换
来源：http://nu.bjjhwx.cn

(double) a / b
来源：http://kl.lnxyls.cn

[S16] C：位操作置位
来源：http://lv.jctech888.com.cn

x |= (1 << 3);
来源：http://zb.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://su.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ji.haigaiapp.cn

[S18] C：命令行参数
来源：http://ed.gzmigu.cn

int main(int argc, char **argv)
来源：http://pg.szxytkj.cn

[S19] C：快速排序
来源：http://km.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://el.colortex.cn

[S20] C：二分查找
来源：http://va.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ea.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://xd.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xy.newstarts.cn

[S22] C：字符串转数字
来源：http://es.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yx.bjjhwx.cn

[S23] C：随机数
来源：http://oc.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cf.colortex.cn

[S24] C：获取本地时间
来源：http://zg.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kl.muxihuayi.cn

[S25] C：内存拷贝
来源：http://fk.szxytkj.cn

memcpy(dst, src, n);
来源：http://rz.newstarts.cn

[S26] C：内存清零
来源：http://vv.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://xy.nszjky.cn

[S27] C：定义常量
来源：http://il.hahajie.cn

const double PI = 3.14159;
来源：http://cy.9csxet.cn

[S28] C：静态变量
来源：http://tz.9csxet.cn

static int counter = 0;
来源：http://tp.colortex.cn

[S29] C：变参函数
来源：http://qp.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://no.lnxyls.cn

[S30] C：头文件保护
来源：http://ke.hnjuh.cn

#ifndef X_H
来源：http://ec.muxihuayi.cn

#define X_H
来源：http://kh.asd995.cn

#endif
来源：http://eo.szsharing.cn

[S31] C++：Hello World
来源：http://gj.shxzskj.cn

#include <iostream>
来源：http://nd.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://gk.asd995.cn

[S32] C++：字符串
来源：http://mj.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://jl.wgjwhj.cn

[S33] C++：vector 增删
来源：http://ax.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eh.shxzukj.cn

[S34] C++：遍历 vector
来源：http://vb.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://ja.9csxet.cn

[S35] C++：map
来源：http://mk.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wk.chemitech.net.cn

[S36] C++：unordered_map
来源：http://qw.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tz.nicolike.cn

[S37] C++：set
来源：http://sz.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rl.muxihuayi.cn

[S38] C++：排序
来源：http://sf.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://jf.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://ak.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rq.chemitech.net.cn

[S40] C++：查找元素
来源：http://ll.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://in.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://ao.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lx.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://dh.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://jg.wgjwhj.cn

[S43] C++：智能指针
来源：http://qk.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://lv.shtwfgs.cn

[S44] C++：引用传参
来源：http://yg.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://eb.bookmarksfly.cn

[S45] C++：lambda
来源：http://zp.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pm.asd995.cn

[S46] C++：函数模板
来源：http://zz.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lx.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://dh.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hj.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://ph.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://aw.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://zc.huixiangedu.cn

[S49] C++：写文件
来源：http://yt.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://md.asd995.cn

[S50] C++：格式化数字
来源：http://aa.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zp.newstarts.cn

[S51] C++：显式类型转换
来源：http://yg.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://dm.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://ce.colortex.cn

int size() const noexcept { return n_; }
来源：http://ef.huixiangedu.cn

[S53] C++：移动语义
来源：http://ab.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://ox.huanxung.cn

[S54] C++：异常处理
来源：http://ag.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zx.newstarts.cn

[S55] C++：结构化绑定
来源：http://rz.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://py.shxzukj.cn

[S56] C++：optional
来源：http://cs.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://io.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://sz.wgjwhj.cn

constexpr int N = 10;
来源：http://jj.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://gq.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://vq.nszjky.cn

[S59] C++：静态断言
来源：http://yx.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tw.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://we.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vk.yuntaijiaju.cn

================================================================================
来源：http://wp.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wp.jctech888.com.cn

================================================================================
来源：http://ag.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://pl.lnxyls.cn

println("Hello")
来源：http://ty.lnxyls.cn

[T02] Kotlin：变量
来源：http://ei.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hr.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://na.szxytkj.cn

"值: $b"
来源：http://de.nicolike.cn

[T04] Kotlin：空安全
来源：http://ne.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://ci.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://bn.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zq.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://cw.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ly.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://dk.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dx.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://ir.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://xn.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://xv.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://jn.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://av.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dv.bjjhwx.cn

[T11] Kotlin：协程
来源：http://aw.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ko.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://ya.521024.cn

val (a, b) = Pair(1, 2)
来源：http://ic.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://gc.nicolike.cn

val m = mapOf("a" to 1)
来源：http://wq.muxihuayi.cn

[T14] Kotlin：循环
来源：http://zc.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://iq.newstarts.cn

[T15] Kotlin：接口
来源：http://jg.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://zs.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://pn.9csxet.cn

print("Hello")
来源：http://rp.newstarts.cn

[T17] Swift：变量与常量
来源：http://wl.asd995.cn

var a = 1;  let b = 2
来源：http://hb.hnjuh.cn

[T18] Swift：字符串插值
来源：http://uk.huanxung.cn

"值: \(b)"
来源：http://vh.newstarts.cn

[T19] Swift：可选绑定
来源：http://rt.chemitech.net.cn

if let n = opt { print(n) }
来源：http://hn.shxzukj.cn

[T20] Swift：数组操作
来源：http://gd.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vf.9csxet.cn

[T21] Swift：遍历
来源：http://jb.yuexingan06.cn

for x in a { print(x) }
来源：http://sg.chemitech.net.cn

[T22] Swift：字典
来源：http://wt.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hy.bjjhwx.cn

[T23] Swift：函数
来源：http://gk.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cc.nicolike.cn

[T24] Swift：闭包
来源：http://ur.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kj.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://ow.asd995.cn

struct P { var x: Int }
来源：http://ba.shtwfgs.cn

[T26] Swift：类与重写
来源：http://bp.hahajie.cn

class A: Base { override func f() {} }
来源：http://gi.shxzskj.cn

[T27] Swift：错误处理
来源：http://op.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://ik.hnjuh.cn

[T28] Swift：枚举
来源：http://cc.lnxyls.cn

enum Color { case red, green }
来源：http://lp.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://et.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://pz.yuexingan06.cn

[T30] Swift：协议
来源：http://eu.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://po.521024.cn

[T31] Lua：Hello World
来源：http://rp.szxytkj.cn

print("Hello")
来源：http://qb.huixiangedu.cn

[T32] Lua：局部变量
来源：http://lp.chemitech.net.cn

local a = 1
来源：http://qr.521024.cn

[T33] Lua：表（数组）
来源：http://gc.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://aq.lnxyls.cn

[T34] Lua：遍历表
来源：http://kb.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ta.chemitech.net.cn

[T35] Lua：字典表
来源：http://rs.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://bz.muxihuayi.cn

[T36] Lua：函数
来源：http://tg.9csxet.cn

function add(a, b) return a + b end
来源：http://cd.asd995.cn

[T37] Lua：字符串拼接
来源：http://wx.chemitech.net.cn

"a" .. "b"
来源：http://bx.huixinmuqiang.cn

[T38] Lua：条件
来源：http://mp.521024.cn

if x > 0 then print("正") end
来源：http://ck.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://ta.wgjwhj.cn

string.find(s, "%d+")
来源：http://fq.shxzskj.cn

[T40] Lua：元表
来源：http://hf.colortex.cn

setmetatable({}, { __index = base })
来源：http://yb.shxzukj.cn

[T41] Perl：Hello World
来源：http://pd.9csxet.cn

print "Hello\n";
来源：http://fq.lnxyls.cn

[T42] Perl：变量类型
来源：http://mx.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nd.shxzskj.cn

[T43] Perl：字符串插值
来源：http://og.nicolike.cn

"值: $a"
来源：http://eu.newstarts.cn

[T44] Perl：条件
来源：http://jy.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://qg.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://rc.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://bm.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://ib.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sj.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://vp.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xf.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://ke.shxzskj.cn

$s =~ s/old/new/g;
来源：http://dy.yuntaijiaju.cn

[T49] Perl：函数
来源：http://gj.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ve.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://kh.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qa.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://hc.shtwfgs.cn

[T51] Scala：Hello World
来源：http://ve.panjiajie.cn

println("Hello")
来源：http://dx.521024.cn

[T52] Scala：变量
来源：http://bg.lnxyls.cn

val a = 1;  var b = 2
来源：http://ps.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://gg.newstarts.cn

s"值: $b"
来源：http://wl.hahajie.cn

[T54] Scala：集合映射
来源：http://ai.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://jm.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://iq.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ti.muxihuayi.cn

[T56] Scala：样例类
来源：http://li.huanxung.cn

case class User(name: String, age: Int)
来源：http://qc.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://dp.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://na.lnxyls.cn

[T58] Scala：函数定义
来源：http://xu.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://an.newstarts.cn

[T59] Scala：循环
来源：http://az.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://ue.muxihuayi.cn

[T60] Scala：折叠
来源：http://bn.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://js.shxzskj.cn

================================================================================
来源：http://hh.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://et.9csxet.cn

================================================================================
来源：http://gn.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://ew.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tx.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://af.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rv.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://lm.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xo.nszjky.cn

[U04] Py：变量调试打印
来源：http://eh.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://im.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://pt.asd995.cn

list(dict.fromkeys(arr))
来源：http://fc.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://au.szsharing.cn

{**a, **b}
来源：http://lk.huanxung.cn

[U07] Py：反转字典键值
来源：http://xn.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://pt.9csxet.cn

[U08] Py：展平二维列表
来源：http://ri.hnjuh.cn

[y for x in nested for y in x]
来源：http://ha.colortex.cn

[U09] Py：字典取最大值的键
来源：http://vl.panjiajie.cn

max(d, key=d.get)
来源：http://xm.nicolike.cn

[U10] Py：按值排序字典
来源：http://lr.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vj.chemitech.net.cn


<!-- 参考信息 -->