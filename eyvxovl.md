代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cq.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://fn.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://is.szxytkj.cn

[R61] 磁盘占用
来源：http://nr.jianghongdianzi.cn

df -h;  du -sh *
来源：http://st.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://zt.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://mg.9csxet.cn

[R63] 内存与进程
来源：http://xo.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://av.jctech888.com.cn

[R64] 结束进程
来源：http://jq.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://ba.521024.cn

[R65] 查看端口占用
来源：http://kz.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dz.colortex.cn

[R66] 定时任务
来源：http://vu.nszjky.cn

crontab -e;  crontab -l
来源：http://uo.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://pe.nszjky.cn

openssl rand -hex 16
来源：http://xh.colortex.cn

[R68] 计算文件校验值
来源：http://kv.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vb.huixiangedu.cn

[R69] 生成随机密码
来源：http://hb.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://jh.bjjhwx.cn

[R70] 时间戳与互转
来源：http://tv.521024.cn

date +%s;  date -d @1700000000
来源：http://pc.wgjwhj.cn

[R71] 日期格式化
来源：http://fo.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vr.jctech888.com.cn

[R72] 等待端口就绪
来源：http://yb.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rk.bookmarksfly.cn

[R73] 分割大日志
来源：http://aj.shxzskj.cn

split -l 1000 big.log part_
来源：http://sj.huanxung.cn

[R74] 批量重命名
来源：http://av.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ls.haigaiapp.cn

[R75] 导出环境变量
来源：http://kw.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://bm.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://ac.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ng.lnxyls.cn

[R77] 读取用户输入
来源：http://yt.9csxet.cn

read -rp "请输入: " ans
来源：http://hg.9csxet.cn

[R78] 交互式菜单
来源：http://qt.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vl.hahajie.cn

[R79] 解析命令行选项
来源：http://aj.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pd.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://ag.wgjwhj.cn

time ./run.sh
来源：http://mh.haigaiapp.cn

================================================================================
来源：http://er.huixinmuqiang.cn

S. C / C++ 专题
来源：http://tk.wgjwhj.cn

================================================================================
来源：http://hj.haigaiapp.cn

[S01] C：Hello World
来源：http://bq.nszjky.cn

#include <stdio.h>
来源：http://fx.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hx.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://zr.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://vf.szxytkj.cn

[S03] C：读入整数
来源：http://ur.hnjuh.cn

int x; scanf("%d", &x);
来源：http://go.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://la.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rp.hnjuh.cn

[S05] C：字符串长度
来源：http://jq.nszjky.cn

strlen(s)
来源：http://gd.haigaiapp.cn

[S06] C：字符串比较
来源：http://lw.colortex.cn

strcmp(a, b) == 0
来源：http://xs.huanxung.cn

[S07] C：数组遍历求和
来源：http://he.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tt.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://pj.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xe.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://sh.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qm.panjiajie.cn

[S10] C：指针与解引用
来源：http://pg.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://du.colortex.cn

[S11] C：逐行读文件
来源：http://zf.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://xd.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cd.wgjwhj.cn

fclose(f);
来源：http://jn.newstarts.cn

[S12] C：写文件
来源：http://pi.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bn.newstarts.cn

[S13] C：宏定义
来源：http://xc.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fi.bjjhwx.cn

[S14] C：枚举
来源：http://wv.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ih.bjjhwx.cn

[S15] C：类型转换
来源：http://kj.huanxung.cn

(double) a / b
来源：http://im.bookmarksfly.cn

[S16] C：位操作置位
来源：http://io.hnjuh.cn

x |= (1 << 3);
来源：http://po.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://fh.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xv.hahajie.cn

[S18] C：命令行参数
来源：http://vc.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://xj.hahajie.cn

[S19] C：快速排序
来源：http://pd.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sq.521024.cn

[S20] C：二分查找
来源：http://wo.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mw.gzmigu.cn

[S21] C：字符类别判断
来源：http://gw.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nr.shxzskj.cn

[S22] C：字符串转数字
来源：http://zq.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ya.huixiangedu.cn

[S23] C：随机数
来源：http://uo.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cc.newstarts.cn

[S24] C：获取本地时间
来源：http://gx.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://so.huanxung.cn

[S25] C：内存拷贝
来源：http://dl.yuexingan06.cn

memcpy(dst, src, n);
来源：http://hc.bjjhwx.cn

[S26] C：内存清零
来源：http://vd.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://yh.huixiangedu.cn

[S27] C：定义常量
来源：http://oi.yuexingan06.cn

const double PI = 3.14159;
来源：http://xx.huixinmuqiang.cn

[S28] C：静态变量
来源：http://ue.nszjky.cn

static int counter = 0;
来源：http://ge.nszjky.cn

[S29] C：变参函数
来源：http://fi.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://si.shtwfgs.cn

[S30] C：头文件保护
来源：http://gw.hnjuh.cn

#ifndef X_H
来源：http://ml.panjiajie.cn

#define X_H
来源：http://mp.colortex.cn

#endif
来源：http://xm.colortex.cn

[S31] C++：Hello World
来源：http://fk.colortex.cn

#include <iostream>
来源：http://uy.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ww.jianghongdianzi.cn

[S32] C++：字符串
来源：http://vn.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://ds.shxzskj.cn

[S33] C++：vector 增删
来源：http://uu.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yo.gzmigu.cn

[S34] C++：遍历 vector
来源：http://zq.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://wq.asd995.cn

[S35] C++：map
来源：http://jb.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vl.huixiangedu.cn

[S36] C++：unordered_map
来源：http://rw.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zt.bjjhwx.cn

[S37] C++：set
来源：http://vf.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ft.gzmigu.cn

[S38] C++：排序
来源：http://oi.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://em.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://aq.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tg.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://sf.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bk.shxzukj.cn

[S41] C++：类与构造函数
来源：http://am.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fh.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://bv.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://yt.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://xl.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://yx.jctech888.com.cn

[S44] C++：引用传参
来源：http://mf.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://pd.nicolike.cn

[S45] C++：lambda
来源：http://lt.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iw.521024.cn

[S46] C++：函数模板
来源：http://ii.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ww.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://fe.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ab.newstarts.cn

[S48] C++：逐行读文件
来源：http://mt.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cc.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://va.szsharing.cn

[S49] C++：写文件
来源：http://mh.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ma.hnjuh.cn

[S50] C++：格式化数字
来源：http://ju.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://om.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://ro.newstarts.cn

static_cast<double>(a) / b
来源：http://wa.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://yu.521024.cn

int size() const noexcept { return n_; }
来源：http://et.szsharing.cn

[S53] C++：移动语义
来源：http://sj.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://vc.521024.cn

[S54] C++：异常处理
来源：http://da.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ng.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://ng.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jw.szsharing.cn

[S56] C++：optional
来源：http://tm.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qn.szxytkj.cn

[S57] C++：编译期常量
来源：http://ej.nszjky.cn

constexpr int N = 10;
来源：http://ab.shtwfgs.cn

[S58] C++：命名空间
来源：http://uh.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://rx.newstarts.cn

[S59] C++：静态断言
来源：http://ps.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://py.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://ir.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dy.gzmigu.cn

================================================================================
来源：http://qg.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ba.nicolike.cn

================================================================================
来源：http://es.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://bf.shxzukj.cn

println("Hello")
来源：http://dt.gzmigu.cn

[T02] Kotlin：变量
来源：http://lo.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jr.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://hg.jctech888.com.cn

"值: $b"
来源：http://wu.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://pu.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://iz.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://zu.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aw.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://rs.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bi.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://jk.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qi.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://di.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://xo.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://bw.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://yn.szsharing.cn

[T10] Kotlin：默认参数
来源：http://rc.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xp.nicolike.cn

[T11] Kotlin：协程
来源：http://rm.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oy.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://kw.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://ah.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://hj.hahajie.cn

val m = mapOf("a" to 1)
来源：http://kq.shxzukj.cn

[T14] Kotlin：循环
来源：http://hm.newstarts.cn

for (i in 1..10) println(i)
来源：http://kd.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://uw.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://ve.panjiajie.cn

[T16] Swift：Hello World
来源：http://ka.bjjhwx.cn

print("Hello")
来源：http://pe.9csxet.cn

[T17] Swift：变量与常量
来源：http://vi.huixiangedu.cn

var a = 1;  let b = 2
来源：http://xa.nszjky.cn

[T18] Swift：字符串插值
来源：http://wi.yuexingan06.cn

"值: \(b)"
来源：http://ml.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://dw.shxzukj.cn

if let n = opt { print(n) }
来源：http://ze.asd995.cn

[T20] Swift：数组操作
来源：http://yl.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://al.chemitech.net.cn

[T21] Swift：遍历
来源：http://qn.yuexingan06.cn

for x in a { print(x) }
来源：http://nd.shxzskj.cn

[T22] Swift：字典
来源：http://xw.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vq.shtwfgs.cn

[T23] Swift：函数
来源：http://vo.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ey.nszjky.cn

[T24] Swift：闭包
来源：http://lf.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tz.szxytkj.cn

[T25] Swift：结构体
来源：http://fe.yuntaijiaju.cn

struct P { var x: Int }
来源：http://fv.yuexingan06.cn

[T26] Swift：类与重写
来源：http://eu.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://cr.huanxung.cn

[T27] Swift：错误处理
来源：http://aw.newstarts.cn

do { try f() } catch { print(error) }
来源：http://iy.muxihuayi.cn

[T28] Swift：枚举
来源：http://hb.9csxet.cn

enum Color { case red, green }
来源：http://hm.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://ek.hnjuh.cn

guard let x = opt else { return }
来源：http://mu.nszjky.cn

[T30] Swift：协议
来源：http://vr.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://ko.yuexingan06.cn

[T31] Lua：Hello World
来源：http://ln.nicolike.cn

print("Hello")
来源：http://cl.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://wm.bjjhwx.cn

local a = 1
来源：http://jq.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://at.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ns.panjiajie.cn

[T34] Lua：遍历表
来源：http://bq.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kh.muxihuayi.cn

[T35] Lua：字典表
来源：http://mj.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://yp.nicolike.cn

[T36] Lua：函数
来源：http://sw.jctech888.com.cn

function add(a, b) return a + b end
来源：http://pu.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://zm.nicolike.cn

"a" .. "b"
来源：http://ry.gzmigu.cn

[T38] Lua：条件
来源：http://mx.chemitech.net.cn

if x > 0 then print("正") end
来源：http://vf.szxytkj.cn

[T39] Lua：模式匹配
来源：http://ew.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://yk.muxihuayi.cn

[T40] Lua：元表
来源：http://hk.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://yb.gzmigu.cn

[T41] Perl：Hello World
来源：http://kx.szsharing.cn

print "Hello\n";
来源：http://da.shxzukj.cn

[T42] Perl：变量类型
来源：http://sk.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fw.gzmigu.cn

[T43] Perl：字符串插值
来源：http://wc.gzmigu.cn

"值: $a"
来源：http://ex.huixiangedu.cn

[T44] Perl：条件
来源：http://va.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://dy.lnxyls.cn

[T45] Perl：数组遍历
来源：http://qz.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://sb.huanxung.cn

[T46] Perl：哈希操作
来源：http://tn.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pk.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://ov.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xl.huixinmuqiang.cn

[T48] Perl：正则替换
来源：http://rw.panjiajie.cn

$s =~ s/old/new/g;
来源：http://uz.asd995.cn

[T49] Perl：函数
来源：http://mt.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vh.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://fw.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xh.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://qe.shtwfgs.cn

[T51] Scala：Hello World
来源：http://fa.521024.cn

println("Hello")
来源：http://uw.hahajie.cn

[T52] Scala：变量
来源：http://xr.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://yw.newstarts.cn

[T53] Scala：字符串插值
来源：http://ep.huanxung.cn

s"值: $b"
来源：http://np.chemitech.net.cn

[T54] Scala：集合映射
来源：http://ib.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://qg.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://zu.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pl.shtwfgs.cn

[T56] Scala：样例类
来源：http://gy.9csxet.cn

case class User(name: String, age: Int)
来源：http://kx.colortex.cn

[T57] Scala：模式匹配
来源：http://ds.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bu.shtwfgs.cn

[T58] Scala：函数定义
来源：http://xe.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fh.asd995.cn

[T59] Scala：循环
来源：http://os.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://vq.yuexingan06.cn

[T60] Scala：折叠
来源：http://ll.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ww.chemitech.net.cn

================================================================================
来源：http://ku.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kz.panjiajie.cn

================================================================================
来源：http://ai.hnjuh.cn


<!-- 参考信息 -->