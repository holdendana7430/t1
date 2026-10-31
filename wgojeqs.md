代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rl.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://at.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ak.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://yo.szxytkj.cn

df -h;  du -sh *
来源：http://is.panjiajie.cn

[R62] 找最占空间的文件
来源：http://te.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://hz.jctech888.com.cn

[R63] 内存与进程
来源：http://rd.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://fh.huanxung.cn

[R64] 结束进程
来源：http://hr.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://ul.jctech888.com.cn

[R65] 查看端口占用
来源：http://yl.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mu.nicolike.cn

[R66] 定时任务
来源：http://yl.shtwfgs.cn

crontab -e;  crontab -l
来源：http://xq.nszjky.cn

[R67] 生成随机十六进制串
来源：http://ny.bookmarksfly.cn

openssl rand -hex 16
来源：http://qs.haigaiapp.cn

[R68] 计算文件校验值
来源：http://tm.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dd.shxzskj.cn

[R69] 生成随机密码
来源：http://ns.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://qg.nszjky.cn

[R70] 时间戳与互转
来源：http://xp.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://rv.wgjwhj.cn

[R71] 日期格式化
来源：http://mg.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://me.szsharing.cn

[R72] 等待端口就绪
来源：http://oi.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nq.wgjwhj.cn

[R73] 分割大日志
来源：http://ke.colortex.cn

split -l 1000 big.log part_
来源：http://mi.shxzukj.cn

[R74] 批量重命名
来源：http://gx.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lt.shtwfgs.cn

[R75] 导出环境变量
来源：http://vc.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://ms.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://ll.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qp.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://sp.szsharing.cn

read -rp "请输入: " ans
来源：http://hs.nszjky.cn

[R78] 交互式菜单
来源：http://au.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ns.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://am.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://au.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://pj.muxihuayi.cn

time ./run.sh
来源：http://xh.yuexingan06.cn

================================================================================
来源：http://yv.bookmarksfly.cn

S. C / C++ 专题
来源：http://fb.huixinmuqiang.cn

================================================================================
来源：http://nu.panjiajie.cn

[S01] C：Hello World
来源：http://tg.haigaiapp.cn

#include <stdio.h>
来源：http://or.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://en.asd995.cn

[S02] C：变量与格式化输出
来源：http://my.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://ej.newstarts.cn

[S03] C：读入整数
来源：http://mw.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://vk.bjjhwx.cn

[S04] C：字符串复制
来源：http://mf.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jg.wgjwhj.cn

[S05] C：字符串长度
来源：http://uu.yuntaijiaju.cn

strlen(s)
来源：http://jb.hahajie.cn

[S06] C：字符串比较
来源：http://jo.panjiajie.cn

strcmp(a, b) == 0
来源：http://qt.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://iq.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bp.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://vd.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rw.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://zz.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lf.asd995.cn

[S10] C：指针与解引用
来源：http://ok.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://do.panjiajie.cn

[S11] C：逐行读文件
来源：http://pf.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://sy.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://em.yuexingan06.cn

fclose(f);
来源：http://os.newstarts.cn

[S12] C：写文件
来源：http://zc.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://la.bjjhwx.cn

[S13] C：宏定义
来源：http://so.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tu.shtwfgs.cn

[S14] C：枚举
来源：http://rt.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://te.chemitech.net.cn

[S15] C：类型转换
来源：http://yt.huixiangedu.cn

(double) a / b
来源：http://yf.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://ta.hnjuh.cn

x |= (1 << 3);
来源：http://vb.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://lw.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://il.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://yz.nicolike.cn

int main(int argc, char **argv)
来源：http://vu.shtwfgs.cn

[S19] C：快速排序
来源：http://lo.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yj.hnjuh.cn

[S20] C：二分查找
来源：http://so.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hx.shxzskj.cn

[S21] C：字符类别判断
来源：http://au.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ro.szxytkj.cn

[S22] C：字符串转数字
来源：http://oc.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fd.bjjhwx.cn

[S23] C：随机数
来源：http://jm.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kd.521024.cn

[S24] C：获取本地时间
来源：http://eu.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://li.szsharing.cn

[S25] C：内存拷贝
来源：http://rx.lnxyls.cn

memcpy(dst, src, n);
来源：http://nz.nicolike.cn

[S26] C：内存清零
来源：http://xa.9csxet.cn

memset(a, 0, sizeof a);
来源：http://lc.newstarts.cn

[S27] C：定义常量
来源：http://cm.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://yc.bookmarksfly.cn

[S28] C：静态变量
来源：http://pp.lnxyls.cn

static int counter = 0;
来源：http://yo.bookmarksfly.cn

[S29] C：变参函数
来源：http://hm.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pj.wgjwhj.cn

[S30] C：头文件保护
来源：http://ii.shxzskj.cn

#ifndef X_H
来源：http://cc.haigaiapp.cn

#define X_H
来源：http://ge.521024.cn

#endif
来源：http://tl.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://yr.chemitech.net.cn

#include <iostream>
来源：http://ue.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://du.shxzskj.cn

[S32] C++：字符串
来源：http://vg.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://ap.szsharing.cn

[S33] C++：vector 增删
来源：http://dn.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://os.gzmigu.cn

[S34] C++：遍历 vector
来源：http://td.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://hn.colortex.cn

[S35] C++：map
来源：http://ex.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ib.wgjwhj.cn

[S36] C++：unordered_map
来源：http://df.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mu.szsharing.cn

[S37] C++：set
来源：http://tc.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tu.nicolike.cn

[S38] C++：排序
来源：http://jv.asd995.cn

std::sort(v.begin(), v.end());
来源：http://yd.colortex.cn

[S39] C++：自定义比较器排序
来源：http://hl.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ka.newstarts.cn

[S40] C++：查找元素
来源：http://mv.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yl.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://ce.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wz.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://rs.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://ml.shtwfgs.cn

[S43] C++：智能指针
来源：http://gp.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://lq.colortex.cn

[S44] C++：引用传参
来源：http://vg.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://qe.shtwfgs.cn

[S45] C++：lambda
来源：http://ec.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nv.hahajie.cn

[S46] C++：函数模板
来源：http://cc.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xn.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://ve.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://um.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://uh.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ge.nicolike.cn

while (std::getline(in, line)) { }
来源：http://mn.muxihuayi.cn

[S49] C++：写文件
来源：http://nd.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aq.szxytkj.cn

[S50] C++：格式化数字
来源：http://rw.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://af.shxzukj.cn

[S51] C++：显式类型转换
来源：http://eg.asd995.cn

static_cast<double>(a) / b
来源：http://da.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://za.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://ne.521024.cn

[S53] C++：移动语义
来源：http://kf.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://el.szsharing.cn

[S54] C++：异常处理
来源：http://fl.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tj.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://vx.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cv.muxihuayi.cn

[S56] C++：optional
来源：http://zi.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kw.haigaiapp.cn

[S57] C++：编译期常量
来源：http://tp.wgjwhj.cn

constexpr int N = 10;
来源：http://fc.haigaiapp.cn

[S58] C++：命名空间
来源：http://jo.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://rw.jctech888.com.cn

[S59] C++：静态断言
来源：http://dh.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ik.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://ey.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lb.521024.cn

================================================================================
来源：http://eq.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ys.shtwfgs.cn

================================================================================
来源：http://pu.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://df.nicolike.cn

println("Hello")
来源：http://yv.lnxyls.cn

[T02] Kotlin：变量
来源：http://oz.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jw.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://jx.521024.cn

"值: $b"
来源：http://uz.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://sz.nszjky.cn

val n: String? = null;  n?.length
来源：http://kw.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://ld.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aa.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://ez.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jh.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://ml.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rs.hnjuh.cn

[T08] Kotlin：数据类
来源：http://lb.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://rk.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://bs.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://ca.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://qs.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iz.521024.cn

[T11] Kotlin：协程
来源：http://sc.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ue.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://ny.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://io.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://gv.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://jl.colortex.cn

[T14] Kotlin：循环
来源：http://mz.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://ni.asd995.cn

[T15] Kotlin：接口
来源：http://hk.szsharing.cn

interface Shape { fun area(): Double }
来源：http://th.shxzukj.cn

[T16] Swift：Hello World
来源：http://sq.yuexingan06.cn

print("Hello")
来源：http://ll.hahajie.cn

[T17] Swift：变量与常量
来源：http://zf.nszjky.cn

var a = 1;  let b = 2
来源：http://xq.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://yi.newstarts.cn

"值: \(b)"
来源：http://dv.asd995.cn

[T19] Swift：可选绑定
来源：http://bw.chemitech.net.cn

if let n = opt { print(n) }
来源：http://nz.shtwfgs.cn

[T20] Swift：数组操作
来源：http://fq.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cn.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://it.huanxung.cn

for x in a { print(x) }
来源：http://xe.haigaiapp.cn

[T22] Swift：字典
来源：http://st.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mh.muxihuayi.cn

[T23] Swift：函数
来源：http://qh.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://df.colortex.cn

[T24] Swift：闭包
来源：http://cs.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yi.hahajie.cn

[T25] Swift：结构体
来源：http://kf.yuexingan06.cn

struct P { var x: Int }
来源：http://ux.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://xb.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://ds.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://pi.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://xc.9csxet.cn

[T28] Swift：枚举
来源：http://qf.shxzskj.cn

enum Color { case red, green }
来源：http://mg.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://nh.panjiajie.cn

guard let x = opt else { return }
来源：http://ok.hahajie.cn

[T30] Swift：协议
来源：http://fi.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://xe.9csxet.cn

[T31] Lua：Hello World
来源：http://yz.nicolike.cn

print("Hello")
来源：http://us.jctech888.com.cn

[T32] Lua：局部变量
来源：http://ex.wgjwhj.cn

local a = 1
来源：http://vq.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://qx.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cq.gzmigu.cn

[T34] Lua：遍历表
来源：http://ui.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kp.bjjhwx.cn

[T35] Lua：字典表
来源：http://ns.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://ph.colortex.cn

[T36] Lua：函数
来源：http://rn.shxzskj.cn

function add(a, b) return a + b end
来源：http://ti.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://kl.huixiangedu.cn

"a" .. "b"
来源：http://lg.huixiangedu.cn

[T38] Lua：条件
来源：http://bg.haigaiapp.cn

if x > 0 then print("正") end
来源：http://yy.hahajie.cn

[T39] Lua：模式匹配
来源：http://ub.hahajie.cn

string.find(s, "%d+")
来源：http://lk.haigaiapp.cn

[T40] Lua：元表
来源：http://ei.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://iq.shxzskj.cn

[T41] Perl：Hello World
来源：http://nu.hnjuh.cn

print "Hello\n";
来源：http://pf.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://lf.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kl.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://qp.newstarts.cn

"值: $a"
来源：http://vd.wgjwhj.cn

[T44] Perl：条件
来源：http://ol.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://sv.newstarts.cn

[T45] Perl：数组遍历
来源：http://yu.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://rq.huanxung.cn

[T46] Perl：哈希操作
来源：http://he.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vv.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://ob.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jz.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://vr.nszjky.cn

$s =~ s/old/new/g;
来源：http://sd.yuntaijiaju.cn

[T49] Perl：函数
来源：http://xg.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pv.huanxung.cn

[T50] Perl：逐行读文件
来源：http://of.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nm.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://es.huixiangedu.cn

[T51] Scala：Hello World
来源：http://vz.szxytkj.cn

println("Hello")
来源：http://ps.asd995.cn

[T52] Scala：变量
来源：http://sg.gzmigu.cn

val a = 1;  var b = 2
来源：http://um.521024.cn

[T53] Scala：字符串插值
来源：http://wi.shtwfgs.cn

s"值: $b"
来源：http://fw.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://if.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://pl.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://ug.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lw.colortex.cn

[T56] Scala：样例类
来源：http://tm.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://ih.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://hi.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cc.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://qk.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://di.huanxung.cn

[T59] Scala：循环
来源：http://xa.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://up.hnjuh.cn

[T60] Scala：折叠
来源：http://en.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://en.hahajie.cn

================================================================================
来源：http://sl.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xx.muxihuayi.cn

================================================================================
来源：http://rk.bookmarksfly.cn


<!-- 参考信息 -->