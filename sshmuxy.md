代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xo.gzmigu.cn

[R66] 定时任务
来源：http://lh.huanxung.cn

crontab -e;  crontab -l
来源：http://kp.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://bd.jianghongdianzi.cn

openssl rand -hex 16
来源：http://na.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://fx.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://az.shxzskj.cn

[R69] 生成随机密码
来源：http://yi.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://tx.yuexingan06.cn

[R70] 时间戳与互转
来源：http://gu.colortex.cn

date +%s;  date -d @1700000000
来源：http://im.jctech888.com.cn

[R71] 日期格式化
来源：http://iu.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ha.shxzukj.cn

[R72] 等待端口就绪
来源：http://wu.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uq.shxzukj.cn

[R73] 分割大日志
来源：http://dv.9csxet.cn

split -l 1000 big.log part_
来源：http://mg.nszjky.cn

[R74] 批量重命名
来源：http://dk.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tz.panjiajie.cn

[R75] 导出环境变量
来源：http://rg.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://it.jctech888.com.cn

[R76] 使用临时文件
来源：http://aj.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cu.newstarts.cn

[R77] 读取用户输入
来源：http://su.panjiajie.cn

read -rp "请输入: " ans
来源：http://is.gzmigu.cn

[R78] 交互式菜单
来源：http://yu.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nf.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://om.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vj.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://ig.chemitech.net.cn

time ./run.sh
来源：http://fo.huixiangedu.cn

================================================================================
来源：http://pq.nszjky.cn

S. C / C++ 专题
来源：http://ro.9csxet.cn

================================================================================
来源：http://xj.shxzskj.cn

[S01] C：Hello World
来源：http://fd.wgjwhj.cn

#include <stdio.h>
来源：http://du.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fa.nicolike.cn

[S02] C：变量与格式化输出
来源：http://lc.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://jd.huanxung.cn

[S03] C：读入整数
来源：http://qc.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://jq.shtwfgs.cn

[S04] C：字符串复制
来源：http://lz.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jk.nicolike.cn

[S05] C：字符串长度
来源：http://ux.jianghongdianzi.cn

strlen(s)
来源：http://vp.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://hx.shtwfgs.cn

strcmp(a, b) == 0
来源：http://pm.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://rs.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fr.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://jh.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rc.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://nk.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vu.chemitech.net.cn

[S10] C：指针与解引用
来源：http://ix.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://hr.9csxet.cn

[S11] C：逐行读文件
来源：http://el.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://om.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mk.haigaiapp.cn

fclose(f);
来源：http://rz.chemitech.net.cn

[S12] C：写文件
来源：http://nk.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tm.huanxung.cn

[S13] C：宏定义
来源：http://au.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ov.szxytkj.cn

[S14] C：枚举
来源：http://sm.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://sw.wgjwhj.cn

[S15] C：类型转换
来源：http://ks.szxytkj.cn

(double) a / b
来源：http://zb.chemitech.net.cn

[S16] C：位操作置位
来源：http://ji.yuexingan06.cn

x |= (1 << 3);
来源：http://ih.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://cu.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xa.gzmigu.cn

[S18] C：命令行参数
来源：http://ls.asd995.cn

int main(int argc, char **argv)
来源：http://gf.nszjky.cn

[S19] C：快速排序
来源：http://jt.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oe.wgjwhj.cn

[S20] C：二分查找
来源：http://uq.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kg.nicolike.cn

[S21] C：字符类别判断
来源：http://kz.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gi.huixiangedu.cn

[S22] C：字符串转数字
来源：http://vo.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pv.chemitech.net.cn

[S23] C：随机数
来源：http://yn.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yt.hahajie.cn

[S24] C：获取本地时间
来源：http://qd.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ai.huixiangedu.cn

[S25] C：内存拷贝
来源：http://zx.chemitech.net.cn

memcpy(dst, src, n);
来源：http://mv.wgjwhj.cn

[S26] C：内存清零
来源：http://ch.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://lz.szxytkj.cn

[S27] C：定义常量
来源：http://xt.521024.cn

const double PI = 3.14159;
来源：http://kk.bjjhwx.cn

[S28] C：静态变量
来源：http://lw.yuexingan06.cn

static int counter = 0;
来源：http://qv.newstarts.cn

[S29] C：变参函数
来源：http://es.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vc.9csxet.cn

[S30] C：头文件保护
来源：http://bl.hahajie.cn

#ifndef X_H
来源：http://ud.jctech888.com.cn

#define X_H
来源：http://lb.gzmigu.cn

#endif
来源：http://mi.haigaiapp.cn

[S31] C++：Hello World
来源：http://ba.colortex.cn

#include <iostream>
来源：http://xv.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://kl.nszjky.cn

[S32] C++：字符串
来源：http://yl.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://ad.shtwfgs.cn

[S33] C++：vector 增删
来源：http://or.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nn.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://lz.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://pn.huixinmuqiang.cn

[S35] C++：map
来源：http://ay.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ss.szxytkj.cn

[S36] C++：unordered_map
来源：http://nt.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kt.huixinmuqiang.cn

[S37] C++：set
来源：http://gy.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dg.bookmarksfly.cn

[S38] C++：排序
来源：http://ub.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://rk.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://iq.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pl.haigaiapp.cn

[S40] C++：查找元素
来源：http://ys.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://le.nicolike.cn

[S41] C++：类与构造函数
来源：http://ys.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ww.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://ts.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://oc.shtwfgs.cn

[S43] C++：智能指针
来源：http://qq.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://hn.newstarts.cn

[S44] C++：引用传参
来源：http://nr.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://za.shxzskj.cn

[S45] C++：lambda
来源：http://yj.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gi.jctech888.com.cn

[S46] C++：函数模板
来源：http://up.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rs.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://sn.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fd.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://lz.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ln.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://bz.wgjwhj.cn

[S49] C++：写文件
来源：http://hw.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xa.haigaiapp.cn

[S50] C++：格式化数字
来源：http://un.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kc.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://ce.lnxyls.cn

static_cast<double>(a) / b
来源：http://hu.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://rv.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://xb.shtwfgs.cn

[S53] C++：移动语义
来源：http://dy.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://cw.hahajie.cn

[S54] C++：异常处理
来源：http://kj.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cg.asd995.cn

[S55] C++：结构化绑定
来源：http://qz.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mf.muxihuayi.cn

[S56] C++：optional
来源：http://og.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://si.wgjwhj.cn

[S57] C++：编译期常量
来源：http://ko.nszjky.cn

constexpr int N = 10;
来源：http://tz.shxzukj.cn

[S58] C++：命名空间
来源：http://jc.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://jv.wgjwhj.cn

[S59] C++：静态断言
来源：http://yj.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nr.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://tz.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wp.nszjky.cn

================================================================================
来源：http://xe.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hv.yuntaijiaju.cn

================================================================================
来源：http://ye.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://sk.nszjky.cn

println("Hello")
来源：http://yt.nicolike.cn

[T02] Kotlin：变量
来源：http://hw.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vp.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://rz.shxzskj.cn

"值: $b"
来源：http://ws.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://vv.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://jk.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://em.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qj.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://az.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gi.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://xw.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://du.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://va.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://aa.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://uw.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://bz.szsharing.cn

[T10] Kotlin：默认参数
来源：http://ao.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nx.hnjuh.cn

[T11] Kotlin：协程
来源：http://uj.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ff.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://uu.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://ho.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://do.newstarts.cn

val m = mapOf("a" to 1)
来源：http://zf.521024.cn

[T14] Kotlin：循环
来源：http://zi.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://gq.yuexingan06.cn

[T15] Kotlin：接口
来源：http://eu.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://jp.jctech888.com.cn

[T16] Swift：Hello World
来源：http://gm.jctech888.com.cn

print("Hello")
来源：http://ya.shxzskj.cn

[T17] Swift：变量与常量
来源：http://nr.shxzskj.cn

var a = 1;  let b = 2
来源：http://jt.gzmigu.cn

[T18] Swift：字符串插值
来源：http://kt.haigaiapp.cn

"值: \(b)"
来源：http://gr.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://oh.shxzskj.cn

if let n = opt { print(n) }
来源：http://dc.lnxyls.cn

[T20] Swift：数组操作
来源：http://wk.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uz.521024.cn

[T21] Swift：遍历
来源：http://zl.yuexingan06.cn

for x in a { print(x) }
来源：http://cz.shxzukj.cn

[T22] Swift：字典
来源：http://te.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tx.asd995.cn

[T23] Swift：函数
来源：http://bq.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qt.haigaiapp.cn

[T24] Swift：闭包
来源：http://wt.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vp.asd995.cn

[T25] Swift：结构体
来源：http://ph.colortex.cn

struct P { var x: Int }
来源：http://wy.muxihuayi.cn

[T26] Swift：类与重写
来源：http://no.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://cb.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://mg.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://qq.lnxyls.cn

[T28] Swift：枚举
来源：http://rw.gzmigu.cn

enum Color { case red, green }
来源：http://jk.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://ch.panjiajie.cn

guard let x = opt else { return }
来源：http://sv.yuntaijiaju.cn

[T30] Swift：协议
来源：http://cx.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://gs.shtwfgs.cn

[T31] Lua：Hello World
来源：http://fn.nszjky.cn

print("Hello")
来源：http://kw.shtwfgs.cn

[T32] Lua：局部变量
来源：http://ng.521024.cn

local a = 1
来源：http://cu.szxytkj.cn

[T33] Lua：表（数组）
来源：http://un.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hu.szsharing.cn

[T34] Lua：遍历表
来源：http://qy.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pu.bookmarksfly.cn

[T35] Lua：字典表
来源：http://ns.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://sh.shxzukj.cn

[T36] Lua：函数
来源：http://mo.shxzskj.cn

function add(a, b) return a + b end
来源：http://dp.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://sj.huixiangedu.cn

"a" .. "b"
来源：http://rh.shtwfgs.cn

[T38] Lua：条件
来源：http://iu.shxzskj.cn

if x > 0 then print("正") end
来源：http://wc.521024.cn

[T39] Lua：模式匹配
来源：http://rg.szxytkj.cn

string.find(s, "%d+")
来源：http://eg.chemitech.net.cn

[T40] Lua：元表
来源：http://ct.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://jz.huixiangedu.cn

[T41] Perl：Hello World
来源：http://au.chemitech.net.cn

print "Hello\n";
来源：http://yz.jctech888.com.cn

[T42] Perl：变量类型
来源：http://sb.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://te.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://xr.hahajie.cn

"值: $a"
来源：http://uj.hnjuh.cn

[T44] Perl：条件
来源：http://ud.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://tu.nicolike.cn

[T45] Perl：数组遍历
来源：http://xr.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://lo.lnxyls.cn

[T46] Perl：哈希操作
来源：http://nv.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ak.asd995.cn

[T47] Perl：正则捕获
来源：http://cm.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://un.huixinmuqiang.cn

[T48] Perl：正则替换
来源：http://rl.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://fn.wgjwhj.cn

[T49] Perl：函数
来源：http://gt.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bp.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://cz.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://og.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ii.hahajie.cn

[T51] Scala：Hello World
来源：http://cz.wgjwhj.cn

println("Hello")
来源：http://go.panjiajie.cn

[T52] Scala：变量
来源：http://lo.colortex.cn

val a = 1;  var b = 2
来源：http://zr.shxzukj.cn

[T53] Scala：字符串插值
来源：http://qn.shxzskj.cn

s"值: $b"
来源：http://vt.shxzskj.cn

[T54] Scala：集合映射
来源：http://yo.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://qc.hahajie.cn

[T55] Scala：集合过滤
来源：http://ay.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zk.huixiangedu.cn

[T56] Scala：样例类
来源：http://hq.huanxung.cn

case class User(name: String, age: Int)
来源：http://xi.huanxung.cn

[T57] Scala：模式匹配
来源：http://rq.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yj.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://ya.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lm.shxzukj.cn

[T59] Scala：循环
来源：http://he.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://dg.bjjhwx.cn

[T60] Scala：折叠
来源：http://tc.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gb.hnjuh.cn

================================================================================
来源：http://mn.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://no.jctech888.com.cn

================================================================================
来源：http://tb.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://yx.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sz.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://mw.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yk.asd995.cn

[U03] Py：加载 .env 配置
来源：http://td.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kq.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://pc.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wk.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://pd.huanxung.cn

list(dict.fromkeys(arr))
来源：http://ba.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://kl.huanxung.cn

{**a, **b}
来源：http://so.shxzskj.cn


<!-- 参考信息 -->