代发 wailian999

free -h;  ps aux | grep nginx
来源：http://rb.nicolike.cn

[R64] 结束进程
来源：http://fy.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://qt.bjjhwx.cn

[R65] 查看端口占用
来源：http://sb.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zg.newstarts.cn

[R66] 定时任务
来源：http://ro.shtwfgs.cn

crontab -e;  crontab -l
来源：http://nt.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://xy.szsharing.cn

openssl rand -hex 16
来源：http://oc.jctech888.com.cn

[R68] 计算文件校验值
来源：http://xy.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xv.shtwfgs.cn

[R69] 生成随机密码
来源：http://bk.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://rr.chemitech.net.cn

[R70] 时间戳与互转
来源：http://hn.nicolike.cn

date +%s;  date -d @1700000000
来源：http://ar.haigaiapp.cn

[R71] 日期格式化
来源：http://nl.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ay.szxytkj.cn

[R72] 等待端口就绪
来源：http://ny.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zg.szxytkj.cn

[R73] 分割大日志
来源：http://cn.shxzukj.cn

split -l 1000 big.log part_
来源：http://zv.wgjwhj.cn

[R74] 批量重命名
来源：http://ud.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yg.chemitech.net.cn

[R75] 导出环境变量
来源：http://er.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://uh.muxihuayi.cn

[R76] 使用临时文件
来源：http://lw.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iv.huanxung.cn

[R77] 读取用户输入
来源：http://um.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://ou.nicolike.cn

[R78] 交互式菜单
来源：http://fv.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dd.nszjky.cn

[R79] 解析命令行选项
来源：http://yd.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vm.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://xp.chemitech.net.cn

time ./run.sh
来源：http://lk.shtwfgs.cn

================================================================================
来源：http://oa.colortex.cn

S. C / C++ 专题
来源：http://os.colortex.cn

================================================================================
来源：http://ej.hahajie.cn

[S01] C：Hello World
来源：http://sm.hnjuh.cn

#include <stdio.h>
来源：http://xe.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gr.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://bg.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://lg.colortex.cn

[S03] C：读入整数
来源：http://kp.newstarts.cn

int x; scanf("%d", &x);
来源：http://ox.szxytkj.cn

[S04] C：字符串复制
来源：http://nl.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sk.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://qh.szsharing.cn

strlen(s)
来源：http://xj.gzmigu.cn

[S06] C：字符串比较
来源：http://js.chemitech.net.cn

strcmp(a, b) == 0
来源：http://wj.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://er.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xr.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://gs.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bc.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://cp.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cl.9csxet.cn

[S10] C：指针与解引用
来源：http://mc.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://xi.hnjuh.cn

[S11] C：逐行读文件
来源：http://tf.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://vi.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://er.jianghongdianzi.cn

fclose(f);
来源：http://zf.yuexingan06.cn

[S12] C：写文件
来源：http://cy.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hn.yuexingan06.cn

[S13] C：宏定义
来源：http://mh.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tg.huanxung.cn

[S14] C：枚举
来源：http://vg.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://yw.haigaiapp.cn

[S15] C：类型转换
来源：http://at.bjjhwx.cn

(double) a / b
来源：http://ar.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://nq.hahajie.cn

x |= (1 << 3);
来源：http://mg.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://ng.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tq.shtwfgs.cn

[S18] C：命令行参数
来源：http://ku.colortex.cn

int main(int argc, char **argv)
来源：http://qn.jianghongdianzi.cn

[S19] C：快速排序
来源：http://zp.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hw.wgjwhj.cn

[S20] C：二分查找
来源：http://cr.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ad.asd995.cn

[S21] C：字符类别判断
来源：http://gm.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zf.lnxyls.cn

[S22] C：字符串转数字
来源：http://ff.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://df.haigaiapp.cn

[S23] C：随机数
来源：http://ns.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jt.szsharing.cn

[S24] C：获取本地时间
来源：http://wu.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dx.szxytkj.cn

[S25] C：内存拷贝
来源：http://pt.hnjuh.cn

memcpy(dst, src, n);
来源：http://lj.hahajie.cn

[S26] C：内存清零
来源：http://hn.nicolike.cn

memset(a, 0, sizeof a);
来源：http://ge.lnxyls.cn

[S27] C：定义常量
来源：http://gg.haigaiapp.cn

const double PI = 3.14159;
来源：http://sp.shtwfgs.cn

[S28] C：静态变量
来源：http://oo.nicolike.cn

static int counter = 0;
来源：http://ay.szxytkj.cn

[S29] C：变参函数
来源：http://uu.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mj.asd995.cn

[S30] C：头文件保护
来源：http://fd.wgjwhj.cn

#ifndef X_H
来源：http://cg.haigaiapp.cn

#define X_H
来源：http://io.shxzskj.cn

#endif
来源：http://xp.bjjhwx.cn

[S31] C++：Hello World
来源：http://ox.newstarts.cn

#include <iostream>
来源：http://ay.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://pk.huanxung.cn

[S32] C++：字符串
来源：http://bk.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://da.lnxyls.cn

[S33] C++：vector 增删
来源：http://rp.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qf.colortex.cn

[S34] C++：遍历 vector
来源：http://be.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://eg.newstarts.cn

[S35] C++：map
来源：http://nh.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ly.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://ng.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jc.shxzskj.cn

[S37] C++：set
来源：http://lq.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eu.szsharing.cn

[S38] C++：排序
来源：http://pr.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://ck.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://xw.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tv.yuexingan06.cn

[S40] C++：查找元素
来源：http://gl.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jn.colortex.cn

[S41] C++：类与构造函数
来源：http://qs.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zc.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://vn.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://jp.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://ti.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://ci.hnjuh.cn

[S44] C++：引用传参
来源：http://vv.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://ip.lnxyls.cn

[S45] C++：lambda
来源：http://zz.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mz.hnjuh.cn

[S46] C++：函数模板
来源：http://no.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://co.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://az.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fv.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://nt.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xq.9csxet.cn

while (std::getline(in, line)) { }
来源：http://sa.shxzskj.cn

[S49] C++：写文件
来源：http://cn.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pg.bjjhwx.cn

[S50] C++：格式化数字
来源：http://wy.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ps.asd995.cn

[S51] C++：显式类型转换
来源：http://ui.panjiajie.cn

static_cast<double>(a) / b
来源：http://kf.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://hx.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://lt.nicolike.cn

[S53] C++：移动语义
来源：http://tx.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://uq.shtwfgs.cn

[S54] C++：异常处理
来源：http://fl.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yf.shxzukj.cn

[S55] C++：结构化绑定
来源：http://yz.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://eu.panjiajie.cn

[S56] C++：optional
来源：http://bu.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ot.huanxung.cn

[S57] C++：编译期常量
来源：http://tw.yuexingan06.cn

constexpr int N = 10;
来源：http://ys.huixiangedu.cn

[S58] C++：命名空间
来源：http://tv.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://ep.hnjuh.cn

[S59] C++：静态断言
来源：http://lh.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pg.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://zx.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ae.bookmarksfly.cn

================================================================================
来源：http://sy.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hy.szxytkj.cn

================================================================================
来源：http://vt.huanxung.cn

[T01] Kotlin：Hello World
来源：http://dr.muxihuayi.cn

println("Hello")
来源：http://cq.lnxyls.cn

[T02] Kotlin：变量
来源：http://ah.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://up.asd995.cn

[T03] Kotlin：字符串模板
来源：http://ud.huixiangedu.cn

"值: $b"
来源：http://ht.9csxet.cn

[T04] Kotlin：空安全
来源：http://ih.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://cw.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://yg.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xg.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://vn.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nn.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://rs.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ao.shxzskj.cn

[T08] Kotlin：数据类
来源：http://yu.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://mb.521024.cn

[T09] Kotlin：扩展函数
来源：http://kf.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://re.szsharing.cn

[T10] Kotlin：默认参数
来源：http://ev.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://em.asd995.cn

[T11] Kotlin：协程
来源：http://ee.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kq.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://nt.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://pa.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://zn.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://du.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://ia.hahajie.cn

for (i in 1..10) println(i)
来源：http://rw.huanxung.cn

[T15] Kotlin：接口
来源：http://jq.nszjky.cn

interface Shape { fun area(): Double }
来源：http://wt.szxytkj.cn

[T16] Swift：Hello World
来源：http://rb.jctech888.com.cn

print("Hello")
来源：http://cr.panjiajie.cn

[T17] Swift：变量与常量
来源：http://hj.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://hl.nicolike.cn

[T18] Swift：字符串插值
来源：http://tw.521024.cn

"值: \(b)"
来源：http://qy.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://kw.gzmigu.cn

if let n = opt { print(n) }
来源：http://cr.bjjhwx.cn

[T20] Swift：数组操作
来源：http://rm.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://br.shxzskj.cn

[T21] Swift：遍历
来源：http://ms.huanxung.cn

for x in a { print(x) }
来源：http://qb.shtwfgs.cn

[T22] Swift：字典
来源：http://ss.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ol.huixiangedu.cn

[T23] Swift：函数
来源：http://vg.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ih.shxzukj.cn

[T24] Swift：闭包
来源：http://uk.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ia.bjjhwx.cn

[T25] Swift：结构体
来源：http://to.yuntaijiaju.cn

struct P { var x: Int }
来源：http://sl.hahajie.cn

[T26] Swift：类与重写
来源：http://ce.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://cw.hahajie.cn

[T27] Swift：错误处理
来源：http://zn.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://wz.colortex.cn

[T28] Swift：枚举
来源：http://rd.lnxyls.cn

enum Color { case red, green }
来源：http://ey.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://wm.jctech888.com.cn

guard let x = opt else { return }
来源：http://yz.9csxet.cn

[T30] Swift：协议
来源：http://et.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://yx.asd995.cn

[T31] Lua：Hello World
来源：http://df.wgjwhj.cn

print("Hello")
来源：http://ok.szsharing.cn

[T32] Lua：局部变量
来源：http://rc.colortex.cn

local a = 1
来源：http://je.521024.cn

[T33] Lua：表（数组）
来源：http://nu.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zi.shxzskj.cn

[T34] Lua：遍历表
来源：http://ii.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ic.colortex.cn

[T35] Lua：字典表
来源：http://xb.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://xb.yuexingan06.cn

[T36] Lua：函数
来源：http://oc.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://ma.9csxet.cn

[T37] Lua：字符串拼接
来源：http://th.jctech888.com.cn

"a" .. "b"
来源：http://rp.521024.cn

[T38] Lua：条件
来源：http://ly.jctech888.com.cn

if x > 0 then print("正") end
来源：http://qc.hnjuh.cn

[T39] Lua：模式匹配
来源：http://pe.newstarts.cn

string.find(s, "%d+")
来源：http://gt.jianghongdianzi.cn

[T40] Lua：元表
来源：http://yn.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://hu.huanxung.cn

[T41] Perl：Hello World
来源：http://by.szsharing.cn

print "Hello\n";
来源：http://bc.bjjhwx.cn

[T42] Perl：变量类型
来源：http://sx.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sx.nszjky.cn

[T43] Perl：字符串插值
来源：http://mg.yuexingan06.cn

"值: $a"
来源：http://sy.haigaiapp.cn

[T44] Perl：条件
来源：http://ms.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://pn.szsharing.cn

[T45] Perl：数组遍历
来源：http://ws.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://ml.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://pu.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dw.hahajie.cn

[T47] Perl：正则捕获
来源：http://lm.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dm.shtwfgs.cn

[T48] Perl：正则替换
来源：http://lb.hahajie.cn

$s =~ s/old/new/g;
来源：http://pn.muxihuayi.cn

[T49] Perl：函数
来源：http://ok.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ot.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://fu.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ir.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://qw.yuexingan06.cn

[T51] Scala：Hello World
来源：http://ck.hnjuh.cn

println("Hello")
来源：http://pm.9csxet.cn

[T52] Scala：变量
来源：http://kj.shtwfgs.cn

val a = 1;  var b = 2
来源：http://az.nszjky.cn

[T53] Scala：字符串插值
来源：http://bf.chemitech.net.cn

s"值: $b"
来源：http://jj.521024.cn

[T54] Scala：集合映射
来源：http://yz.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://eh.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://ln.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wz.haigaiapp.cn

[T56] Scala：样例类
来源：http://hm.521024.cn

case class User(name: String, age: Int)
来源：http://pz.asd995.cn

[T57] Scala：模式匹配
来源：http://en.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kh.hnjuh.cn

[T58] Scala：函数定义
来源：http://ws.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ko.haigaiapp.cn

[T59] Scala：循环
来源：http://xs.521024.cn

for (i <- 1 to 10) println(i)
来源：http://dq.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://rj.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mz.lnxyls.cn

================================================================================
来源：http://sx.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bm.asd995.cn

================================================================================
来源：http://gy.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://nc.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ju.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://qy.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dx.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://au.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bb.szsharing.cn

[U04] Py：变量调试打印
来源：http://cy.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rr.huixiangedu.cn


<!-- 参考信息 -->