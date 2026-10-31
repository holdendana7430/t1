代发 wailian999

free -h;  ps aux | grep nginx
来源：http://pp.jianghongdianzi.cn

[R64] 结束进程
来源：http://jz.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://tz.shxzukj.cn

[R65] 查看端口占用
来源：http://ce.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mz.shtwfgs.cn

[R66] 定时任务
来源：http://lw.hnjuh.cn

crontab -e;  crontab -l
来源：http://al.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://lb.jctech888.com.cn

openssl rand -hex 16
来源：http://ve.muxihuayi.cn

[R68] 计算文件校验值
来源：http://qe.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xw.521024.cn

[R69] 生成随机密码
来源：http://cl.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://qi.nszjky.cn

[R70] 时间戳与互转
来源：http://sz.nicolike.cn

date +%s;  date -d @1700000000
来源：http://rg.huanxung.cn

[R71] 日期格式化
来源：http://hb.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://br.jctech888.com.cn

[R72] 等待端口就绪
来源：http://kx.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hh.huanxung.cn

[R73] 分割大日志
来源：http://dj.haigaiapp.cn

split -l 1000 big.log part_
来源：http://vh.521024.cn

[R74] 批量重命名
来源：http://vm.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gu.bjjhwx.cn

[R75] 导出环境变量
来源：http://my.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://in.haigaiapp.cn

[R76] 使用临时文件
来源：http://ue.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ou.bjjhwx.cn

[R77] 读取用户输入
来源：http://bv.haigaiapp.cn

read -rp "请输入: " ans
来源：http://yg.nicolike.cn

[R78] 交互式菜单
来源：http://ft.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mw.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://jf.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qq.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://pg.nicolike.cn

time ./run.sh
来源：http://bb.jctech888.com.cn

================================================================================
来源：http://wh.jianghongdianzi.cn

S. C / C++ 专题
来源：http://jz.panjiajie.cn

================================================================================
来源：http://hk.hahajie.cn

[S01] C：Hello World
来源：http://ut.asd995.cn

#include <stdio.h>
来源：http://di.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zo.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://ib.521024.cn

int a = 10; printf("%d\n", a);
来源：http://gs.shxzukj.cn

[S03] C：读入整数
来源：http://ou.newstarts.cn

int x; scanf("%d", &x);
来源：http://ad.szsharing.cn

[S04] C：字符串复制
来源：http://rc.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fp.szsharing.cn

[S05] C：字符串长度
来源：http://qi.chemitech.net.cn

strlen(s)
来源：http://ii.szsharing.cn

[S06] C：字符串比较
来源：http://tw.lnxyls.cn

strcmp(a, b) == 0
来源：http://tj.shxzskj.cn

[S07] C：数组遍历求和
来源：http://yr.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fk.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://yi.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wk.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://jh.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lt.9csxet.cn

[S10] C：指针与解引用
来源：http://dz.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://ju.lnxyls.cn

[S11] C：逐行读文件
来源：http://ec.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://ep.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://na.521024.cn

fclose(f);
来源：http://tr.haigaiapp.cn

[S12] C：写文件
来源：http://yv.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nm.szsharing.cn

[S13] C：宏定义
来源：http://tq.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ul.jctech888.com.cn

[S14] C：枚举
来源：http://hs.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://wb.gzmigu.cn

[S15] C：类型转换
来源：http://wa.haigaiapp.cn

(double) a / b
来源：http://ka.9csxet.cn

[S16] C：位操作置位
来源：http://db.haigaiapp.cn

x |= (1 << 3);
来源：http://ox.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://on.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oy.huanxung.cn

[S18] C：命令行参数
来源：http://it.shtwfgs.cn

int main(int argc, char **argv)
来源：http://fr.yuexingan06.cn

[S19] C：快速排序
来源：http://ya.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fh.nszjky.cn

[S20] C：二分查找
来源：http://ip.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iu.muxihuayi.cn

[S21] C：字符类别判断
来源：http://ky.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ds.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://aj.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://as.shtwfgs.cn

[S23] C：随机数
来源：http://xg.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ph.asd995.cn

[S24] C：获取本地时间
来源：http://zd.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fz.haigaiapp.cn

[S25] C：内存拷贝
来源：http://zx.colortex.cn

memcpy(dst, src, n);
来源：http://cs.bookmarksfly.cn

[S26] C：内存清零
来源：http://jo.hahajie.cn

memset(a, 0, sizeof a);
来源：http://hl.bjjhwx.cn

[S27] C：定义常量
来源：http://ha.yuexingan06.cn

const double PI = 3.14159;
来源：http://pg.bookmarksfly.cn

[S28] C：静态变量
来源：http://vu.bookmarksfly.cn

static int counter = 0;
来源：http://ld.huixiangedu.cn

[S29] C：变参函数
来源：http://fo.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://km.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://wo.newstarts.cn

#ifndef X_H
来源：http://fs.jianghongdianzi.cn

#define X_H
来源：http://ql.chemitech.net.cn

#endif
来源：http://nz.yuexingan06.cn

[S31] C++：Hello World
来源：http://vi.shxzskj.cn

#include <iostream>
来源：http://mt.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://ix.szsharing.cn

[S32] C++：字符串
来源：http://wx.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://mz.shxzukj.cn

[S33] C++：vector 增删
来源：http://fq.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hl.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://xu.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://cc.jianghongdianzi.cn

[S35] C++：map
来源：http://wq.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hp.newstarts.cn

[S36] C++：unordered_map
来源：http://hm.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eu.jctech888.com.cn

[S37] C++：set
来源：http://ew.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hd.chemitech.net.cn

[S38] C++：排序
来源：http://xx.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://qk.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://xq.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://em.szsharing.cn

[S40] C++：查找元素
来源：http://hc.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ff.521024.cn

[S41] C++：类与构造函数
来源：http://mq.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fb.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://wh.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://we.wgjwhj.cn

[S43] C++：智能指针
来源：http://hd.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://jd.panjiajie.cn

[S44] C++：引用传参
来源：http://dc.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://le.lnxyls.cn

[S45] C++：lambda
来源：http://zu.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vh.nicolike.cn

[S46] C++：函数模板
来源：http://qu.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iv.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://xn.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rz.shxzskj.cn

[S48] C++：逐行读文件
来源：http://ds.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wz.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://qa.nszjky.cn

[S49] C++：写文件
来源：http://zp.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rj.gzmigu.cn

[S50] C++：格式化数字
来源：http://yf.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tg.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://ft.gzmigu.cn

static_cast<double>(a) / b
来源：http://hd.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://th.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://bb.szsharing.cn

[S53] C++：移动语义
来源：http://lt.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://xy.huanxung.cn

[S54] C++：异常处理
来源：http://av.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ao.hahajie.cn

[S55] C++：结构化绑定
来源：http://et.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://as.bjjhwx.cn

[S56] C++：optional
来源：http://sv.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vy.chemitech.net.cn

[S57] C++：编译期常量
来源：http://zy.bookmarksfly.cn

constexpr int N = 10;
来源：http://wt.chemitech.net.cn

[S58] C++：命名空间
来源：http://sr.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://vm.nicolike.cn

[S59] C++：静态断言
来源：http://dr.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bn.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://qe.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gl.yuexingan06.cn

================================================================================
来源：http://ee.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://up.gzmigu.cn

================================================================================
来源：http://it.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://oy.bookmarksfly.cn

println("Hello")
来源：http://hb.nicolike.cn

[T02] Kotlin：变量
来源：http://ea.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ga.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://gs.lnxyls.cn

"值: $b"
来源：http://lc.nszjky.cn

[T04] Kotlin：空安全
来源：http://ct.huanxung.cn

val n: String? = null;  n?.length
来源：http://qu.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://ys.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ev.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://kz.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ui.asd995.cn

[T07] Kotlin：集合过滤
来源：http://fx.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ve.nicolike.cn

[T08] Kotlin：数据类
来源：http://cb.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://om.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://xb.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://pk.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://si.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sk.colortex.cn

[T11] Kotlin：协程
来源：http://aw.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dc.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://vi.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://zp.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://me.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://pd.yuexingan06.cn

[T14] Kotlin：循环
来源：http://dk.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://me.hahajie.cn

[T15] Kotlin：接口
来源：http://wy.asd995.cn

interface Shape { fun area(): Double }
来源：http://fz.nicolike.cn

[T16] Swift：Hello World
来源：http://fq.bjjhwx.cn

print("Hello")
来源：http://wu.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://zo.chemitech.net.cn

var a = 1;  let b = 2
来源：http://pl.asd995.cn

[T18] Swift：字符串插值
来源：http://lj.asd995.cn

"值: \(b)"
来源：http://cu.asd995.cn

[T19] Swift：可选绑定
来源：http://wx.haigaiapp.cn

if let n = opt { print(n) }
来源：http://cz.wgjwhj.cn

[T20] Swift：数组操作
来源：http://up.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zm.huixiangedu.cn

[T21] Swift：遍历
来源：http://mv.panjiajie.cn

for x in a { print(x) }
来源：http://fe.9csxet.cn

[T22] Swift：字典
来源：http://vk.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zl.9csxet.cn

[T23] Swift：函数
来源：http://cl.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ii.wgjwhj.cn

[T24] Swift：闭包
来源：http://hq.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ka.521024.cn

[T25] Swift：结构体
来源：http://bj.yuexingan06.cn

struct P { var x: Int }
来源：http://zj.szsharing.cn

[T26] Swift：类与重写
来源：http://jd.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://ra.521024.cn

[T27] Swift：错误处理
来源：http://rh.newstarts.cn

do { try f() } catch { print(error) }
来源：http://cu.wgjwhj.cn

[T28] Swift：枚举
来源：http://vi.newstarts.cn

enum Color { case red, green }
来源：http://wb.521024.cn

[T29] Swift：guard 提前返回
来源：http://xx.bjjhwx.cn

guard let x = opt else { return }
来源：http://wr.haigaiapp.cn

[T30] Swift：协议
来源：http://mb.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://ym.hahajie.cn

[T31] Lua：Hello World
来源：http://by.jianghongdianzi.cn

print("Hello")
来源：http://pn.asd995.cn

[T32] Lua：局部变量
来源：http://jn.9csxet.cn

local a = 1
来源：http://cr.hnjuh.cn

[T33] Lua：表（数组）
来源：http://di.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vl.shtwfgs.cn

[T34] Lua：遍历表
来源：http://sd.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pz.haigaiapp.cn

[T35] Lua：字典表
来源：http://fr.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://mj.jianghongdianzi.cn

[T36] Lua：函数
来源：http://jh.panjiajie.cn

function add(a, b) return a + b end
来源：http://gf.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://tc.hahajie.cn

"a" .. "b"
来源：http://ai.muxihuayi.cn

[T38] Lua：条件
来源：http://ia.huanxung.cn

if x > 0 then print("正") end
来源：http://ly.panjiajie.cn

[T39] Lua：模式匹配
来源：http://yk.hnjuh.cn

string.find(s, "%d+")
来源：http://dd.hnjuh.cn

[T40] Lua：元表
来源：http://dp.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://tw.bjjhwx.cn

[T41] Perl：Hello World
来源：http://dr.yuexingan06.cn

print "Hello\n";
来源：http://sq.hahajie.cn

[T42] Perl：变量类型
来源：http://hm.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ns.9csxet.cn

[T43] Perl：字符串插值
来源：http://kb.szxytkj.cn

"值: $a"
来源：http://sj.newstarts.cn

[T44] Perl：条件
来源：http://ed.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://jx.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://pi.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://le.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://at.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fw.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://sh.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vm.wgjwhj.cn

[T48] Perl：正则替换
来源：http://xp.newstarts.cn

$s =~ s/old/new/g;
来源：http://cg.jctech888.com.cn

[T49] Perl：函数
来源：http://tg.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wk.asd995.cn

[T50] Perl：逐行读文件
来源：http://ko.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cp.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://ac.yuexingan06.cn

[T51] Scala：Hello World
来源：http://el.panjiajie.cn

println("Hello")
来源：http://kr.hnjuh.cn

[T52] Scala：变量
来源：http://jp.hnjuh.cn

val a = 1;  var b = 2
来源：http://sg.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://zb.lnxyls.cn

s"值: $b"
来源：http://wv.hahajie.cn

[T54] Scala：集合映射
来源：http://ku.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://mr.521024.cn

[T55] Scala：集合过滤
来源：http://wa.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://co.shxzukj.cn

[T56] Scala：样例类
来源：http://mk.hahajie.cn

case class User(name: String, age: Int)
来源：http://fw.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://sy.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yk.wgjwhj.cn

[T58] Scala：函数定义
来源：http://dz.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vk.huanxung.cn

[T59] Scala：循环
来源：http://sr.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://ye.jctech888.com.cn

[T60] Scala：折叠
来源：http://nc.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hi.szxytkj.cn

================================================================================
来源：http://hz.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rm.shxzukj.cn

================================================================================
来源：http://lj.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://js.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://we.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://lk.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tb.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://eh.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fd.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://od.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qi.nszjky.cn


<!-- 参考信息 -->