代发 wailian999

free -h;  ps aux | grep nginx
来源：http://rz.shtwfgs.cn

[R64] 结束进程
来源：http://mn.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://xr.huixiangedu.cn

[R65] 查看端口占用
来源：http://tu.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qu.9csxet.cn

[R66] 定时任务
来源：http://mp.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://py.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://yo.haigaiapp.cn

openssl rand -hex 16
来源：http://tn.lnxyls.cn

[R68] 计算文件校验值
来源：http://kg.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qb.lnxyls.cn

[R69] 生成随机密码
来源：http://fe.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://ks.jctech888.com.cn

[R70] 时间戳与互转
来源：http://ap.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://qa.huixinmuqiang.cn

[R71] 日期格式化
来源：http://la.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yg.shxzukj.cn

[R72] 等待端口就绪
来源：http://dx.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pu.huixinmuqiang.cn

[R73] 分割大日志
来源：http://kq.colortex.cn

split -l 1000 big.log part_
来源：http://nv.shtwfgs.cn

[R74] 批量重命名
来源：http://hw.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nb.szxytkj.cn

[R75] 导出环境变量
来源：http://yh.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://ob.shxzukj.cn

[R76] 使用临时文件
来源：http://mt.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mx.colortex.cn

[R77] 读取用户输入
来源：http://ud.bjjhwx.cn

read -rp "请输入: " ans
来源：http://yd.hnjuh.cn

[R78] 交互式菜单
来源：http://yh.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://li.asd995.cn

[R79] 解析命令行选项
来源：http://jx.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mx.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://dn.haigaiapp.cn

time ./run.sh
来源：http://ta.huixiangedu.cn

================================================================================
来源：http://hi.colortex.cn

S. C / C++ 专题
来源：http://kw.huixinmuqiang.cn

================================================================================
来源：http://qx.yuntaijiaju.cn

[S01] C：Hello World
来源：http://pt.gzmigu.cn

#include <stdio.h>
来源：http://as.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://af.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://bf.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://es.bjjhwx.cn

[S03] C：读入整数
来源：http://gj.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://hg.szxytkj.cn

[S04] C：字符串复制
来源：http://xh.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mp.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://zd.huanxung.cn

strlen(s)
来源：http://su.bjjhwx.cn

[S06] C：字符串比较
来源：http://so.hnjuh.cn

strcmp(a, b) == 0
来源：http://jr.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://xi.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yo.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://pc.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qt.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://cs.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uw.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://yx.nszjky.cn

int *p = &a;  *p = 5;
来源：http://ue.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://ha.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://lr.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zn.shtwfgs.cn

fclose(f);
来源：http://wd.gzmigu.cn

[S12] C：写文件
来源：http://jy.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pt.9csxet.cn

[S13] C：宏定义
来源：http://lp.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aa.newstarts.cn

[S14] C：枚举
来源：http://cs.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://sg.haigaiapp.cn

[S15] C：类型转换
来源：http://jt.yuexingan06.cn

(double) a / b
来源：http://de.newstarts.cn

[S16] C：位操作置位
来源：http://fi.hahajie.cn

x |= (1 << 3);
来源：http://jp.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://pl.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ge.9csxet.cn

[S18] C：命令行参数
来源：http://qp.muxihuayi.cn

int main(int argc, char **argv)
来源：http://th.wgjwhj.cn

[S19] C：快速排序
来源：http://jy.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ek.521024.cn

[S20] C：二分查找
来源：http://fh.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pv.huixiangedu.cn

[S21] C：字符类别判断
来源：http://fj.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sq.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://ho.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uf.gzmigu.cn

[S23] C：随机数
来源：http://ff.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gb.521024.cn

[S24] C：获取本地时间
来源：http://ne.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vn.gzmigu.cn

[S25] C：内存拷贝
来源：http://tc.yuexingan06.cn

memcpy(dst, src, n);
来源：http://iu.asd995.cn

[S26] C：内存清零
来源：http://gj.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://tb.521024.cn

[S27] C：定义常量
来源：http://ak.panjiajie.cn

const double PI = 3.14159;
来源：http://hl.szxytkj.cn

[S28] C：静态变量
来源：http://kq.shtwfgs.cn

static int counter = 0;
来源：http://ma.panjiajie.cn

[S29] C：变参函数
来源：http://va.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://be.chemitech.net.cn

[S30] C：头文件保护
来源：http://su.bookmarksfly.cn

#ifndef X_H
来源：http://oc.gzmigu.cn

#define X_H
来源：http://rl.lnxyls.cn

#endif
来源：http://vd.521024.cn

[S31] C++：Hello World
来源：http://kj.shtwfgs.cn

#include <iostream>
来源：http://og.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://ej.shxzskj.cn

[S32] C++：字符串
来源：http://ud.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://ey.521024.cn

[S33] C++：vector 增删
来源：http://ns.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vc.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://ty.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://gb.chemitech.net.cn

[S35] C++：map
来源：http://gj.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lh.nszjky.cn

[S36] C++：unordered_map
来源：http://za.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jk.shxzukj.cn

[S37] C++：set
来源：http://qa.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fo.jianghongdianzi.cn

[S38] C++：排序
来源：http://me.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://uc.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://si.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rj.jctech888.com.cn

[S40] C++：查找元素
来源：http://ay.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mw.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://eg.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bh.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://wc.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://ms.9csxet.cn

[S43] C++：智能指针
来源：http://mp.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://nv.gzmigu.cn

[S44] C++：引用传参
来源：http://rb.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://gw.9csxet.cn

[S45] C++：lambda
来源：http://vl.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kh.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://ur.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uw.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://fd.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://px.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://ka.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rr.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://lm.asd995.cn

[S49] C++：写文件
来源：http://cm.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mk.newstarts.cn

[S50] C++：格式化数字
来源：http://ut.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wz.shxzukj.cn

[S51] C++：显式类型转换
来源：http://ee.huanxung.cn

static_cast<double>(a) / b
来源：http://sb.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://bs.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://bg.chemitech.net.cn

[S53] C++：移动语义
来源：http://hg.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://zt.colortex.cn

[S54] C++：异常处理
来源：http://av.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ai.panjiajie.cn

[S55] C++：结构化绑定
来源：http://od.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vn.9csxet.cn

[S56] C++：optional
来源：http://wr.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cc.szxytkj.cn

[S57] C++：编译期常量
来源：http://qc.9csxet.cn

constexpr int N = 10;
来源：http://lr.shxzukj.cn

[S58] C++：命名空间
来源：http://qe.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://dk.shxzukj.cn

[S59] C++：静态断言
来源：http://vr.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kq.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://ru.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ob.shxzskj.cn

================================================================================
来源：http://at.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vf.hahajie.cn

================================================================================
来源：http://hg.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://rv.hahajie.cn

println("Hello")
来源：http://zg.yuexingan06.cn

[T02] Kotlin：变量
来源：http://ua.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uw.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://cw.521024.cn

"值: $b"
来源：http://td.panjiajie.cn

[T04] Kotlin：空安全
来源：http://eu.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://rt.colortex.cn

[T05] Kotlin：when 表达式
来源：http://qo.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ui.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://hq.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gc.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://qh.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ok.shxzukj.cn

[T08] Kotlin：数据类
来源：http://oh.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://lk.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://jo.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://mk.huanxung.cn

[T10] Kotlin：默认参数
来源：http://sc.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jk.shtwfgs.cn

[T11] Kotlin：协程
来源：http://mr.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pg.colortex.cn

[T12] Kotlin：解构声明
来源：http://mk.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://uz.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://jz.szsharing.cn

val m = mapOf("a" to 1)
来源：http://iw.nszjky.cn

[T14] Kotlin：循环
来源：http://ww.hahajie.cn

for (i in 1..10) println(i)
来源：http://zp.nszjky.cn

[T15] Kotlin：接口
来源：http://xu.9csxet.cn

interface Shape { fun area(): Double }
来源：http://lv.huanxung.cn

[T16] Swift：Hello World
来源：http://in.shtwfgs.cn

print("Hello")
来源：http://ku.shxzukj.cn

[T17] Swift：变量与常量
来源：http://aj.szxytkj.cn

var a = 1;  let b = 2
来源：http://vs.nszjky.cn

[T18] Swift：字符串插值
来源：http://dy.yuntaijiaju.cn

"值: \(b)"
来源：http://iu.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://ay.szsharing.cn

if let n = opt { print(n) }
来源：http://em.huanxung.cn

[T20] Swift：数组操作
来源：http://rm.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://je.panjiajie.cn

[T21] Swift：遍历
来源：http://xy.yuexingan06.cn

for x in a { print(x) }
来源：http://pb.szxytkj.cn

[T22] Swift：字典
来源：http://wd.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://op.yuexingan06.cn

[T23] Swift：函数
来源：http://qa.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eb.hahajie.cn

[T24] Swift：闭包
来源：http://kp.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ho.9csxet.cn

[T25] Swift：结构体
来源：http://aj.hahajie.cn

struct P { var x: Int }
来源：http://fk.yuexingan06.cn

[T26] Swift：类与重写
来源：http://fw.nszjky.cn

class A: Base { override func f() {} }
来源：http://hs.nicolike.cn

[T27] Swift：错误处理
来源：http://si.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://cj.bookmarksfly.cn

[T28] Swift：枚举
来源：http://te.szxytkj.cn

enum Color { case red, green }
来源：http://fg.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://su.huanxung.cn

guard let x = opt else { return }
来源：http://ms.bjjhwx.cn

[T30] Swift：协议
来源：http://wh.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://lt.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://ur.colortex.cn

print("Hello")
来源：http://dk.chemitech.net.cn

[T32] Lua：局部变量
来源：http://jj.huanxung.cn

local a = 1
来源：http://fh.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://aj.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sc.szsharing.cn

[T34] Lua：遍历表
来源：http://dp.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bf.yuexingan06.cn

[T35] Lua：字典表
来源：http://zh.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://gx.hnjuh.cn

[T36] Lua：函数
来源：http://xa.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://dm.huanxung.cn

[T37] Lua：字符串拼接
来源：http://kd.9csxet.cn

"a" .. "b"
来源：http://mb.muxihuayi.cn

[T38] Lua：条件
来源：http://jl.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://pz.gzmigu.cn

[T39] Lua：模式匹配
来源：http://ir.szsharing.cn

string.find(s, "%d+")
来源：http://md.szxytkj.cn

[T40] Lua：元表
来源：http://cd.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://et.newstarts.cn

[T41] Perl：Hello World
来源：http://rw.huixinmuqiang.cn

print "Hello\n";
来源：http://ru.panjiajie.cn

[T42] Perl：变量类型
来源：http://gk.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pz.huanxung.cn

[T43] Perl：字符串插值
来源：http://ck.huanxung.cn

"值: $a"
来源：http://ci.shxzskj.cn

[T44] Perl：条件
来源：http://yw.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://bv.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://ke.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://yk.colortex.cn

[T46] Perl：哈希操作
来源：http://iz.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yz.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://wq.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://iu.shxzskj.cn

[T48] Perl：正则替换
来源：http://lv.521024.cn

$s =~ s/old/new/g;
来源：http://oi.muxihuayi.cn

[T49] Perl：函数
来源：http://lt.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ni.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://qz.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yu.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://ql.9csxet.cn

[T51] Scala：Hello World
来源：http://bk.hahajie.cn

println("Hello")
来源：http://pf.lnxyls.cn

[T52] Scala：变量
来源：http://pf.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://rl.colortex.cn

[T53] Scala：字符串插值
来源：http://cx.szxytkj.cn

s"值: $b"
来源：http://xu.hahajie.cn

[T54] Scala：集合映射
来源：http://jv.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://zr.huanxung.cn

[T55] Scala：集合过滤
来源：http://ff.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qu.panjiajie.cn

[T56] Scala：样例类
来源：http://pz.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://mm.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://cc.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://el.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://hw.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bz.bookmarksfly.cn

[T59] Scala：循环
来源：http://hj.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://ws.bjjhwx.cn

[T60] Scala：折叠
来源：http://jl.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pm.jctech888.com.cn

================================================================================
来源：http://vr.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qx.wgjwhj.cn

================================================================================
来源：http://co.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://az.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sp.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://ht.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fc.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://gj.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ye.szxytkj.cn

[U04] Py：变量调试打印
来源：http://cf.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nw.newstarts.cn


<!-- 参考信息 -->