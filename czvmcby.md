代发 wailian999

free -h;  ps aux | grep nginx
来源：http://ca.newstarts.cn

[R64] 结束进程
来源：http://sb.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://oh.asd995.cn

[R65] 查看端口占用
来源：http://oe.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nx.jctech888.com.cn

[R66] 定时任务
来源：http://bf.huixiangedu.cn

crontab -e;  crontab -l
来源：http://bm.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://xr.gzmigu.cn

openssl rand -hex 16
来源：http://sv.shxzukj.cn

[R68] 计算文件校验值
来源：http://cx.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fs.shtwfgs.cn

[R69] 生成随机密码
来源：http://am.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://cb.haigaiapp.cn

[R70] 时间戳与互转
来源：http://do.newstarts.cn

date +%s;  date -d @1700000000
来源：http://cj.wgjwhj.cn

[R71] 日期格式化
来源：http://ga.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yj.shxzskj.cn

[R72] 等待端口就绪
来源：http://se.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fz.chemitech.net.cn

[R73] 分割大日志
来源：http://jx.hnjuh.cn

split -l 1000 big.log part_
来源：http://dk.huanxung.cn

[R74] 批量重命名
来源：http://md.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sm.colortex.cn

[R75] 导出环境变量
来源：http://ia.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://ld.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://dl.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ix.nicolike.cn

[R77] 读取用户输入
来源：http://fl.asd995.cn

read -rp "请输入: " ans
来源：http://lm.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://zw.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ln.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://at.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iq.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://jy.colortex.cn

time ./run.sh
来源：http://fi.jctech888.com.cn

================================================================================
来源：http://as.nszjky.cn

S. C / C++ 专题
来源：http://bi.chemitech.net.cn

================================================================================
来源：http://bc.huixiangedu.cn

[S01] C：Hello World
来源：http://ha.gzmigu.cn

#include <stdio.h>
来源：http://ze.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qt.hahajie.cn

[S02] C：变量与格式化输出
来源：http://pg.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://rm.hahajie.cn

[S03] C：读入整数
来源：http://od.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://ei.panjiajie.cn

[S04] C：字符串复制
来源：http://xo.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vo.bjjhwx.cn

[S05] C：字符串长度
来源：http://ez.nicolike.cn

strlen(s)
来源：http://jb.521024.cn

[S06] C：字符串比较
来源：http://rh.bjjhwx.cn

strcmp(a, b) == 0
来源：http://gn.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://dq.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qo.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://be.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eu.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://jg.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vn.yuexingan06.cn

[S10] C：指针与解引用
来源：http://wy.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://xa.lnxyls.cn

[S11] C：逐行读文件
来源：http://vu.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://dy.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://no.szxytkj.cn

fclose(f);
来源：http://ck.bjjhwx.cn

[S12] C：写文件
来源：http://lj.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qg.shxzskj.cn

[S13] C：宏定义
来源：http://to.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gf.shxzukj.cn

[S14] C：枚举
来源：http://pk.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://mc.bookmarksfly.cn

[S15] C：类型转换
来源：http://cz.lnxyls.cn

(double) a / b
来源：http://hm.colortex.cn

[S16] C：位操作置位
来源：http://pg.wgjwhj.cn

x |= (1 << 3);
来源：http://xh.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://vr.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mw.asd995.cn

[S18] C：命令行参数
来源：http://vg.521024.cn

int main(int argc, char **argv)
来源：http://oa.jctech888.com.cn

[S19] C：快速排序
来源：http://qm.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nd.shxzskj.cn

[S20] C：二分查找
来源：http://hx.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pe.nszjky.cn

[S21] C：字符类别判断
来源：http://fs.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ym.nicolike.cn

[S22] C：字符串转数字
来源：http://en.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pz.szsharing.cn

[S23] C：随机数
来源：http://fa.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://av.521024.cn

[S24] C：获取本地时间
来源：http://nv.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tw.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://bf.colortex.cn

memcpy(dst, src, n);
来源：http://ze.asd995.cn

[S26] C：内存清零
来源：http://vx.asd995.cn

memset(a, 0, sizeof a);
来源：http://mg.shxzskj.cn

[S27] C：定义常量
来源：http://fh.asd995.cn

const double PI = 3.14159;
来源：http://sb.wgjwhj.cn

[S28] C：静态变量
来源：http://dn.bjjhwx.cn

static int counter = 0;
来源：http://ue.gzmigu.cn

[S29] C：变参函数
来源：http://qg.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dt.szxytkj.cn

[S30] C：头文件保护
来源：http://ki.szsharing.cn

#ifndef X_H
来源：http://ty.9csxet.cn

#define X_H
来源：http://ah.shxzukj.cn

#endif
来源：http://gh.yuexingan06.cn

[S31] C++：Hello World
来源：http://va.panjiajie.cn

#include <iostream>
来源：http://ro.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://qy.shxzukj.cn

[S32] C++：字符串
来源：http://ib.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://np.shxzukj.cn

[S33] C++：vector 增删
来源：http://ef.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hd.hahajie.cn

[S34] C++：遍历 vector
来源：http://ip.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://bz.hnjuh.cn

[S35] C++：map
来源：http://ay.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://an.szsharing.cn

[S36] C++：unordered_map
来源：http://jf.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yz.yuntaijiaju.cn

[S37] C++：set
来源：http://ot.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hf.shxzukj.cn

[S38] C++：排序
来源：http://hy.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://hg.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://gg.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kh.wgjwhj.cn

[S40] C++：查找元素
来源：http://iu.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ww.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://kh.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ah.hahajie.cn

[S42] C++：继承与虚函数
来源：http://ie.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://he.haigaiapp.cn

[S43] C++：智能指针
来源：http://bx.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://qr.nicolike.cn

[S44] C++：引用传参
来源：http://ba.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://me.shxzukj.cn

[S45] C++：lambda
来源：http://yk.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hp.nicolike.cn

[S46] C++：函数模板
来源：http://gj.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yb.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://pj.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zo.newstarts.cn

[S48] C++：逐行读文件
来源：http://ml.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sp.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://az.yuexingan06.cn

[S49] C++：写文件
来源：http://xo.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bu.asd995.cn

[S50] C++：格式化数字
来源：http://kh.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oa.newstarts.cn

[S51] C++：显式类型转换
来源：http://jx.lnxyls.cn

static_cast<double>(a) / b
来源：http://sg.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://mc.nicolike.cn

int size() const noexcept { return n_; }
来源：http://wg.hahajie.cn

[S53] C++：移动语义
来源：http://mf.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://ct.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://sb.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sn.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://iu.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://us.nicolike.cn

[S56] C++：optional
来源：http://eo.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://au.asd995.cn

[S57] C++：编译期常量
来源：http://zj.shtwfgs.cn

constexpr int N = 10;
来源：http://ua.huanxung.cn

[S58] C++：命名空间
来源：http://to.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://ks.shtwfgs.cn

[S59] C++：静态断言
来源：http://qr.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kf.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://ei.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rk.chemitech.net.cn

================================================================================
来源：http://gn.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tx.9csxet.cn

================================================================================
来源：http://ke.huanxung.cn

[T01] Kotlin：Hello World
来源：http://uj.newstarts.cn

println("Hello")
来源：http://os.521024.cn

[T02] Kotlin：变量
来源：http://eb.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ih.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://tq.asd995.cn

"值: $b"
来源：http://aw.hahajie.cn

[T04] Kotlin：空安全
来源：http://uk.hahajie.cn

val n: String? = null;  n?.length
来源：http://tc.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://wo.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sm.nszjky.cn

[T06] Kotlin：集合映射
来源：http://oe.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hs.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://eq.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://aj.huanxung.cn

[T08] Kotlin：数据类
来源：http://cv.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://nl.colortex.cn

[T09] Kotlin：扩展函数
来源：http://jd.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://nn.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://ub.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mo.szsharing.cn

[T11] Kotlin：协程
来源：http://sp.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tr.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://qt.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://fu.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://ej.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://ip.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://qk.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://cx.asd995.cn

[T15] Kotlin：接口
来源：http://hb.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://ry.521024.cn

[T16] Swift：Hello World
来源：http://fo.newstarts.cn

print("Hello")
来源：http://mc.hahajie.cn

[T17] Swift：变量与常量
来源：http://fc.huanxung.cn

var a = 1;  let b = 2
来源：http://na.9csxet.cn

[T18] Swift：字符串插值
来源：http://jc.shxzskj.cn

"值: \(b)"
来源：http://bf.newstarts.cn

[T19] Swift：可选绑定
来源：http://gl.bjjhwx.cn

if let n = opt { print(n) }
来源：http://kd.shtwfgs.cn

[T20] Swift：数组操作
来源：http://vy.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://he.newstarts.cn

[T21] Swift：遍历
来源：http://ws.huixiangedu.cn

for x in a { print(x) }
来源：http://ro.chemitech.net.cn

[T22] Swift：字典
来源：http://xe.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ci.shtwfgs.cn

[T23] Swift：函数
来源：http://uf.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kn.yuexingan06.cn

[T24] Swift：闭包
来源：http://ym.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uz.bookmarksfly.cn

[T25] Swift：结构体
来源：http://pw.521024.cn

struct P { var x: Int }
来源：http://jd.hahajie.cn

[T26] Swift：类与重写
来源：http://bl.szxytkj.cn

class A: Base { override func f() {} }
来源：http://qg.huanxung.cn

[T27] Swift：错误处理
来源：http://pv.huanxung.cn

do { try f() } catch { print(error) }
来源：http://fl.asd995.cn

[T28] Swift：枚举
来源：http://ai.newstarts.cn

enum Color { case red, green }
来源：http://yb.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://uu.szxytkj.cn

guard let x = opt else { return }
来源：http://ai.bookmarksfly.cn

[T30] Swift：协议
来源：http://fe.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://do.szsharing.cn

[T31] Lua：Hello World
来源：http://rx.521024.cn

print("Hello")
来源：http://id.jctech888.com.cn

[T32] Lua：局部变量
来源：http://vf.nszjky.cn

local a = 1
来源：http://vd.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://zb.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ss.wgjwhj.cn

[T34] Lua：遍历表
来源：http://nq.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pf.bookmarksfly.cn

[T35] Lua：字典表
来源：http://hn.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://td.lnxyls.cn

[T36] Lua：函数
来源：http://ns.lnxyls.cn

function add(a, b) return a + b end
来源：http://qn.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://pc.shxzskj.cn

"a" .. "b"
来源：http://cr.muxihuayi.cn

[T38] Lua：条件
来源：http://ex.newstarts.cn

if x > 0 then print("正") end
来源：http://ip.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://rx.bookmarksfly.cn

string.find(s, "%d+")
来源：http://hg.huanxung.cn

[T40] Lua：元表
来源：http://eg.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://kn.muxihuayi.cn

[T41] Perl：Hello World
来源：http://mc.chemitech.net.cn

print "Hello\n";
来源：http://lw.panjiajie.cn

[T42] Perl：变量类型
来源：http://sr.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://um.lnxyls.cn

[T43] Perl：字符串插值
来源：http://sk.asd995.cn

"值: $a"
来源：http://dp.nicolike.cn

[T44] Perl：条件
来源：http://on.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://rp.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://ns.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://lc.asd995.cn

[T46] Perl：哈希操作
来源：http://ws.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nf.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://ff.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vv.lnxyls.cn

[T48] Perl：正则替换
来源：http://sf.shxzukj.cn

$s =~ s/old/new/g;
来源：http://xh.shxzukj.cn

[T49] Perl：函数
来源：http://aw.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wj.nszjky.cn

[T50] Perl：逐行读文件
来源：http://mn.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://os.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://ok.haigaiapp.cn

[T51] Scala：Hello World
来源：http://oj.yuntaijiaju.cn

println("Hello")
来源：http://lv.newstarts.cn

[T52] Scala：变量
来源：http://fk.hnjuh.cn

val a = 1;  var b = 2
来源：http://qr.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://ox.huixiangedu.cn

s"值: $b"
来源：http://ur.szsharing.cn

[T54] Scala：集合映射
来源：http://oo.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://wo.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://kz.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://as.haigaiapp.cn

[T56] Scala：样例类
来源：http://fq.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://ic.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://nx.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ti.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://he.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dm.panjiajie.cn

[T59] Scala：循环
来源：http://nl.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://xo.bookmarksfly.cn

[T60] Scala：折叠
来源：http://wb.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zt.huixinmuqiang.cn

================================================================================
来源：http://pm.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tn.shxzskj.cn

================================================================================
来源：http://hu.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://fm.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ei.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://oy.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sq.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://zi.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mi.szsharing.cn

[U04] Py：变量调试打印
来源：http://sa.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uw.jianghongdianzi.cn


<!-- 参考信息 -->