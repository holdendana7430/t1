代发 wailian999

openssl rand -hex 16
来源：http://we.szxytkj.cn

[R68] 计算文件校验值
来源：http://yg.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vn.huanxung.cn

[R69] 生成随机密码
来源：http://qj.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://al.nszjky.cn

[R70] 时间戳与互转
来源：http://ne.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://nb.jianghongdianzi.cn

[R71] 日期格式化
来源：http://os.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cn.muxihuayi.cn

[R72] 等待端口就绪
来源：http://sr.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fn.wgjwhj.cn

[R73] 分割大日志
来源：http://rq.asd995.cn

split -l 1000 big.log part_
来源：http://xz.bjjhwx.cn

[R74] 批量重命名
来源：http://zl.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gu.hnjuh.cn

[R75] 导出环境变量
来源：http://jz.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://nf.huanxung.cn

[R76] 使用临时文件
来源：http://lb.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ba.muxihuayi.cn

[R77] 读取用户输入
来源：http://tm.szxytkj.cn

read -rp "请输入: " ans
来源：http://jt.hnjuh.cn

[R78] 交互式菜单
来源：http://eq.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gk.szxytkj.cn

[R79] 解析命令行选项
来源：http://tn.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nq.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://dx.9csxet.cn

time ./run.sh
来源：http://jz.lnxyls.cn

================================================================================
来源：http://to.nszjky.cn

S. C / C++ 专题
来源：http://no.shxzskj.cn

================================================================================
来源：http://nv.hahajie.cn

[S01] C：Hello World
来源：http://os.bjjhwx.cn

#include <stdio.h>
来源：http://qd.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hx.newstarts.cn

[S02] C：变量与格式化输出
来源：http://gi.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://bi.muxihuayi.cn

[S03] C：读入整数
来源：http://rs.9csxet.cn

int x; scanf("%d", &x);
来源：http://kz.newstarts.cn

[S04] C：字符串复制
来源：http://ds.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ec.yuexingan06.cn

[S05] C：字符串长度
来源：http://kv.gzmigu.cn

strlen(s)
来源：http://ez.bookmarksfly.cn

[S06] C：字符串比较
来源：http://rc.muxihuayi.cn

strcmp(a, b) == 0
来源：http://ug.newstarts.cn

[S07] C：数组遍历求和
来源：http://ha.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fe.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://gm.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jg.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://sa.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ht.shxzukj.cn

[S10] C：指针与解引用
来源：http://gy.szsharing.cn

int *p = &a;  *p = 5;
来源：http://lw.shtwfgs.cn

[S11] C：逐行读文件
来源：http://uk.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://yb.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ny.huanxung.cn

fclose(f);
来源：http://iw.szsharing.cn

[S12] C：写文件
来源：http://cz.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ps.szsharing.cn

[S13] C：宏定义
来源：http://tc.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lk.nszjky.cn

[S14] C：枚举
来源：http://jk.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://ev.szxytkj.cn

[S15] C：类型转换
来源：http://ko.521024.cn

(double) a / b
来源：http://ix.haigaiapp.cn

[S16] C：位操作置位
来源：http://mc.hahajie.cn

x |= (1 << 3);
来源：http://qm.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://hp.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nq.chemitech.net.cn

[S18] C：命令行参数
来源：http://nf.hnjuh.cn

int main(int argc, char **argv)
来源：http://sz.hnjuh.cn

[S19] C：快速排序
来源：http://vf.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iq.hahajie.cn

[S20] C：二分查找
来源：http://js.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ot.asd995.cn

[S21] C：字符类别判断
来源：http://xa.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nq.muxihuayi.cn

[S22] C：字符串转数字
来源：http://kv.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nw.huixiangedu.cn

[S23] C：随机数
来源：http://xg.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://by.nicolike.cn

[S24] C：获取本地时间
来源：http://cn.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://he.huixiangedu.cn

[S25] C：内存拷贝
来源：http://tg.haigaiapp.cn

memcpy(dst, src, n);
来源：http://ob.shtwfgs.cn

[S26] C：内存清零
来源：http://bk.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://lx.gzmigu.cn

[S27] C：定义常量
来源：http://vo.shtwfgs.cn

const double PI = 3.14159;
来源：http://rc.huanxung.cn

[S28] C：静态变量
来源：http://rh.chemitech.net.cn

static int counter = 0;
来源：http://xh.bookmarksfly.cn

[S29] C：变参函数
来源：http://fu.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wa.lnxyls.cn

[S30] C：头文件保护
来源：http://hm.panjiajie.cn

#ifndef X_H
来源：http://dh.nszjky.cn

#define X_H
来源：http://gg.nszjky.cn

#endif
来源：http://rx.bookmarksfly.cn

[S31] C++：Hello World
来源：http://mk.hnjuh.cn

#include <iostream>
来源：http://ou.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://zi.yuntaijiaju.cn

[S32] C++：字符串
来源：http://pn.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://yn.chemitech.net.cn

[S33] C++：vector 增删
来源：http://vx.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jv.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://gh.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://rs.yuexingan06.cn

[S35] C++：map
来源：http://jx.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ky.hnjuh.cn

[S36] C++：unordered_map
来源：http://xp.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kr.yuntaijiaju.cn

[S37] C++：set
来源：http://rh.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dk.huixinmuqiang.cn

[S38] C++：排序
来源：http://sw.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://wl.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://kg.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ae.huanxung.cn

[S40] C++：查找元素
来源：http://sl.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aj.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://bn.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ly.huanxung.cn

[S42] C++：继承与虚函数
来源：http://no.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://ao.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://cc.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://nx.szxytkj.cn

[S44] C++：引用传参
来源：http://ib.521024.cn

void inc(int &x) { ++x; }
来源：http://ly.521024.cn

[S45] C++：lambda
来源：http://ez.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pc.huixiangedu.cn

[S46] C++：函数模板
来源：http://zt.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qk.521024.cn

[S47] C++：结构化绑定遍历
来源：http://co.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://of.asd995.cn

[S48] C++：逐行读文件
来源：http://ja.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ph.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://jn.szsharing.cn

[S49] C++：写文件
来源：http://up.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://py.hahajie.cn

[S50] C++：格式化数字
来源：http://ki.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wx.521024.cn

[S51] C++：显式类型转换
来源：http://qx.chemitech.net.cn

static_cast<double>(a) / b
来源：http://el.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://hj.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://jt.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://lt.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://zp.gzmigu.cn

[S54] C++：异常处理
来源：http://ew.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://td.hnjuh.cn

[S55] C++：结构化绑定
来源：http://wy.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ho.yuntaijiaju.cn

[S56] C++：optional
来源：http://sn.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zx.yuexingan06.cn

[S57] C++：编译期常量
来源：http://ez.hahajie.cn

constexpr int N = 10;
来源：http://zf.521024.cn

[S58] C++：命名空间
来源：http://nu.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://nc.lnxyls.cn

[S59] C++：静态断言
来源：http://cz.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mr.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://jq.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kb.shtwfgs.cn

================================================================================
来源：http://vw.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vp.nicolike.cn

================================================================================
来源：http://hg.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://xh.lnxyls.cn

println("Hello")
来源：http://tz.newstarts.cn

[T02] Kotlin：变量
来源：http://fb.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dq.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://wt.jctech888.com.cn

"值: $b"
来源：http://nn.lnxyls.cn

[T04] Kotlin：空安全
来源：http://yu.newstarts.cn

val n: String? = null;  n?.length
来源：http://kd.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://zc.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ju.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://my.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wd.colortex.cn

[T07] Kotlin：集合过滤
来源：http://zv.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tl.hahajie.cn

[T08] Kotlin：数据类
来源：http://yc.colortex.cn

data class User(val name: String, val age: Int)
来源：http://zr.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://hc.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://ya.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://nn.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dp.huixiangedu.cn

[T11] Kotlin：协程
来源：http://ij.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xr.colortex.cn

[T12] Kotlin：解构声明
来源：http://hp.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://cu.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://ik.colortex.cn

val m = mapOf("a" to 1)
来源：http://ys.huixiangedu.cn

[T14] Kotlin：循环
来源：http://dj.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://qb.shtwfgs.cn

[T15] Kotlin：接口
来源：http://gb.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://ye.nszjky.cn

[T16] Swift：Hello World
来源：http://bj.panjiajie.cn

print("Hello")
来源：http://ke.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://vn.lnxyls.cn

var a = 1;  let b = 2
来源：http://kp.hnjuh.cn

[T18] Swift：字符串插值
来源：http://se.521024.cn

"值: \(b)"
来源：http://ia.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://zo.521024.cn

if let n = opt { print(n) }
来源：http://ae.newstarts.cn

[T20] Swift：数组操作
来源：http://xc.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bv.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://zi.shxzskj.cn

for x in a { print(x) }
来源：http://qa.521024.cn

[T22] Swift：字典
来源：http://he.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ys.chemitech.net.cn

[T23] Swift：函数
来源：http://eq.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gd.hnjuh.cn

[T24] Swift：闭包
来源：http://to.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zn.panjiajie.cn

[T25] Swift：结构体
来源：http://aa.yuntaijiaju.cn

struct P { var x: Int }
来源：http://pd.asd995.cn

[T26] Swift：类与重写
来源：http://ut.521024.cn

class A: Base { override func f() {} }
来源：http://mu.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://on.nicolike.cn

do { try f() } catch { print(error) }
来源：http://se.wgjwhj.cn

[T28] Swift：枚举
来源：http://zg.szsharing.cn

enum Color { case red, green }
来源：http://bk.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://te.shxzukj.cn

guard let x = opt else { return }
来源：http://yk.yuntaijiaju.cn

[T30] Swift：协议
来源：http://rq.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://yo.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://gh.yuexingan06.cn

print("Hello")
来源：http://wl.hahajie.cn

[T32] Lua：局部变量
来源：http://sd.shtwfgs.cn

local a = 1
来源：http://lx.hnjuh.cn

[T33] Lua：表（数组）
来源：http://tw.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ai.yuexingan06.cn

[T34] Lua：遍历表
来源：http://bx.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tt.521024.cn

[T35] Lua：字典表
来源：http://wy.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://rl.bjjhwx.cn

[T36] Lua：函数
来源：http://cw.haigaiapp.cn

function add(a, b) return a + b end
来源：http://jp.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://qy.9csxet.cn

"a" .. "b"
来源：http://lr.szsharing.cn

[T38] Lua：条件
来源：http://mb.nszjky.cn

if x > 0 then print("正") end
来源：http://dd.newstarts.cn

[T39] Lua：模式匹配
来源：http://su.haigaiapp.cn

string.find(s, "%d+")
来源：http://tp.nicolike.cn

[T40] Lua：元表
来源：http://tj.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://mx.shxzskj.cn

[T41] Perl：Hello World
来源：http://hf.colortex.cn

print "Hello\n";
来源：http://zz.bjjhwx.cn

[T42] Perl：变量类型
来源：http://ew.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oi.panjiajie.cn

[T43] Perl：字符串插值
来源：http://ne.newstarts.cn

"值: $a"
来源：http://yr.hnjuh.cn

[T44] Perl：条件
来源：http://sz.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://eq.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://vy.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://hv.szxytkj.cn

[T46] Perl：哈希操作
来源：http://cm.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sq.colortex.cn

[T47] Perl：正则捕获
来源：http://wt.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://el.szxytkj.cn

[T48] Perl：正则替换
来源：http://mf.gzmigu.cn

$s =~ s/old/new/g;
来源：http://wl.szxytkj.cn

[T49] Perl：函数
来源：http://lz.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://np.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://un.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cn.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://yd.hnjuh.cn

[T51] Scala：Hello World
来源：http://fn.newstarts.cn

println("Hello")
来源：http://ot.shxzskj.cn

[T52] Scala：变量
来源：http://vn.szsharing.cn

val a = 1;  var b = 2
来源：http://jq.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://cb.haigaiapp.cn

s"值: $b"
来源：http://dm.chemitech.net.cn

[T54] Scala：集合映射
来源：http://xq.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://md.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://hn.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zj.haigaiapp.cn

[T56] Scala：样例类
来源：http://mb.nicolike.cn

case class User(name: String, age: Int)
来源：http://sj.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://cd.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ny.lnxyls.cn

[T58] Scala：函数定义
来源：http://sq.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qy.gzmigu.cn

[T59] Scala：循环
来源：http://la.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://cj.shxzukj.cn

[T60] Scala：折叠
来源：http://jp.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wj.gzmigu.cn

================================================================================
来源：http://xf.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zh.asd995.cn

================================================================================
来源：http://bz.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://dv.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ii.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://ck.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://of.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://ht.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bu.asd995.cn

[U04] Py：变量调试打印
来源：http://ww.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vh.521024.cn

[U05] Py：列表去重且保序
来源：http://gk.hnjuh.cn

list(dict.fromkeys(arr))
来源：http://sj.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://dm.newstarts.cn

{**a, **b}
来源：http://cq.521024.cn

[U07] Py：反转字典键值
来源：http://kr.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://uh.shxzukj.cn

[U08] Py：展平二维列表
来源：http://lk.haigaiapp.cn

[y for x in nested for y in x]
来源：http://qx.shxzskj.cn


<!-- 参考信息 -->