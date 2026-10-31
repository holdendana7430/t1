代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://we.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://wd.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://di.haigaiapp.cn

[R61] 磁盘占用
来源：http://uk.nicolike.cn

df -h;  du -sh *
来源：http://kb.lnxyls.cn

[R62] 找最占空间的文件
来源：http://dj.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://vg.huixinmuqiang.cn

[R63] 内存与进程
来源：http://nf.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://mj.bjjhwx.cn

[R64] 结束进程
来源：http://wh.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://dg.bookmarksfly.cn

[R65] 查看端口占用
来源：http://as.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cl.jctech888.com.cn

[R66] 定时任务
来源：http://zj.nszjky.cn

crontab -e;  crontab -l
来源：http://ww.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://wl.yuexingan06.cn

openssl rand -hex 16
来源：http://bj.shtwfgs.cn

[R68] 计算文件校验值
来源：http://ho.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qk.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://vn.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://kd.521024.cn

[R70] 时间戳与互转
来源：http://ha.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://se.huixiangedu.cn

[R71] 日期格式化
来源：http://fg.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tc.shxzskj.cn

[R72] 等待端口就绪
来源：http://sx.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cg.shxzskj.cn

[R73] 分割大日志
来源：http://gb.nszjky.cn

split -l 1000 big.log part_
来源：http://gx.panjiajie.cn

[R74] 批量重命名
来源：http://ht.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ro.shxzukj.cn

[R75] 导出环境变量
来源：http://ol.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://du.lnxyls.cn

[R76] 使用临时文件
来源：http://oy.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://th.hnjuh.cn

[R77] 读取用户输入
来源：http://sl.wgjwhj.cn

read -rp "请输入: " ans
来源：http://oj.jctech888.com.cn

[R78] 交互式菜单
来源：http://vv.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vx.9csxet.cn

[R79] 解析命令行选项
来源：http://me.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ag.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://nc.panjiajie.cn

time ./run.sh
来源：http://wn.jctech888.com.cn

================================================================================
来源：http://ja.9csxet.cn

S. C / C++ 专题
来源：http://rs.shtwfgs.cn

================================================================================
来源：http://gb.hahajie.cn

[S01] C：Hello World
来源：http://cn.lnxyls.cn

#include <stdio.h>
来源：http://ht.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nh.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://lp.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://pm.jctech888.com.cn

[S03] C：读入整数
来源：http://jq.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://zu.nszjky.cn

[S04] C：字符串复制
来源：http://xu.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wu.haigaiapp.cn

[S05] C：字符串长度
来源：http://it.chemitech.net.cn

strlen(s)
来源：http://rc.wgjwhj.cn

[S06] C：字符串比较
来源：http://eh.haigaiapp.cn

strcmp(a, b) == 0
来源：http://sk.asd995.cn

[S07] C：数组遍历求和
来源：http://gj.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jx.asd995.cn

[S08] C：动态内存分配与释放
来源：http://tj.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rw.colortex.cn

[S09] C：结构体定义与初始化
来源：http://tf.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hf.gzmigu.cn

[S10] C：指针与解引用
来源：http://nf.9csxet.cn

int *p = &a;  *p = 5;
来源：http://ms.jctech888.com.cn

[S11] C：逐行读文件
来源：http://yl.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://fr.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ev.panjiajie.cn

fclose(f);
来源：http://uq.shxzukj.cn

[S12] C：写文件
来源：http://ze.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://al.huixinmuqiang.cn

[S13] C：宏定义
来源：http://yz.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vc.huanxung.cn

[S14] C：枚举
来源：http://pc.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://ef.hahajie.cn

[S15] C：类型转换
来源：http://ao.bjjhwx.cn

(double) a / b
来源：http://ho.yuexingan06.cn

[S16] C：位操作置位
来源：http://ka.yuntaijiaju.cn

x |= (1 << 3);
来源：http://td.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://jl.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qz.bookmarksfly.cn

[S18] C：命令行参数
来源：http://kt.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://gs.bookmarksfly.cn

[S19] C：快速排序
来源：http://tc.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fr.panjiajie.cn

[S20] C：二分查找
来源：http://rh.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wv.colortex.cn

[S21] C：字符类别判断
来源：http://mw.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vq.szsharing.cn

[S22] C：字符串转数字
来源：http://uf.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ns.wgjwhj.cn

[S23] C：随机数
来源：http://ve.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ua.newstarts.cn

[S24] C：获取本地时间
来源：http://jw.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bj.shxzukj.cn

[S25] C：内存拷贝
来源：http://no.shxzukj.cn

memcpy(dst, src, n);
来源：http://ew.asd995.cn

[S26] C：内存清零
来源：http://at.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://rh.hnjuh.cn

[S27] C：定义常量
来源：http://ip.9csxet.cn

const double PI = 3.14159;
来源：http://fo.muxihuayi.cn

[S28] C：静态变量
来源：http://sx.huixiangedu.cn

static int counter = 0;
来源：http://kq.hahajie.cn

[S29] C：变参函数
来源：http://qb.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ew.hnjuh.cn

[S30] C：头文件保护
来源：http://xe.yuntaijiaju.cn

#ifndef X_H
来源：http://xj.asd995.cn

#define X_H
来源：http://fv.newstarts.cn

#endif
来源：http://pr.bjjhwx.cn

[S31] C++：Hello World
来源：http://ie.bookmarksfly.cn

#include <iostream>
来源：http://qa.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://fp.wgjwhj.cn

[S32] C++：字符串
来源：http://si.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://qt.9csxet.cn

[S33] C++：vector 增删
来源：http://zn.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eo.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://yc.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://vp.colortex.cn

[S35] C++：map
来源：http://bo.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yc.shxzukj.cn

[S36] C++：unordered_map
来源：http://yl.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eq.bjjhwx.cn

[S37] C++：set
来源：http://ta.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wi.wgjwhj.cn

[S38] C++：排序
来源：http://qo.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://gt.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://js.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oy.huanxung.cn

[S40] C++：查找元素
来源：http://qo.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://go.panjiajie.cn

[S41] C++：类与构造函数
来源：http://fv.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ks.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://px.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://yb.nicolike.cn

[S43] C++：智能指针
来源：http://ge.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://re.gzmigu.cn

[S44] C++：引用传参
来源：http://ey.asd995.cn

void inc(int &x) { ++x; }
来源：http://vm.szsharing.cn

[S45] C++：lambda
来源：http://kf.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ct.shxzukj.cn

[S46] C++：函数模板
来源：http://fv.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gh.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://qk.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mg.shxzskj.cn

[S48] C++：逐行读文件
来源：http://zm.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://se.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://ob.muxihuayi.cn

[S49] C++：写文件
来源：http://ep.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pv.newstarts.cn

[S50] C++：格式化数字
来源：http://ha.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ip.newstarts.cn

[S51] C++：显式类型转换
来源：http://wf.szxytkj.cn

static_cast<double>(a) / b
来源：http://dy.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://ix.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://fn.szxytkj.cn

[S53] C++：移动语义
来源：http://iz.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://ic.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://wa.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eq.shxzskj.cn

[S55] C++：结构化绑定
来源：http://az.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://id.newstarts.cn

[S56] C++：optional
来源：http://jl.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yr.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://qz.szxytkj.cn

constexpr int N = 10;
来源：http://je.yuexingan06.cn

[S58] C++：命名空间
来源：http://tr.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://wn.muxihuayi.cn

[S59] C++：静态断言
来源：http://kl.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lb.colortex.cn

[S60] C++：遍历并删除元素
来源：http://kp.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wx.haigaiapp.cn

================================================================================
来源：http://og.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mf.newstarts.cn

================================================================================
来源：http://ld.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://yu.bookmarksfly.cn

println("Hello")
来源：http://ft.szsharing.cn

[T02] Kotlin：变量
来源：http://fv.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://le.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://uv.huixinmuqiang.cn

"值: $b"
来源：http://jl.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://mu.gzmigu.cn

val n: String? = null;  n?.length
来源：http://np.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://fx.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ij.hahajie.cn

[T06] Kotlin：集合映射
来源：http://si.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pc.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://ht.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qk.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://ak.521024.cn

data class User(val name: String, val age: Int)
来源：http://fu.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://xo.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://fo.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://sn.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lx.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://jh.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zo.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://ze.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://wo.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://vz.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://hm.hnjuh.cn

[T14] Kotlin：循环
来源：http://px.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://ns.wgjwhj.cn

[T15] Kotlin：接口
来源：http://er.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://zw.szxytkj.cn

[T16] Swift：Hello World
来源：http://mr.shtwfgs.cn

print("Hello")
来源：http://dc.shxzskj.cn

[T17] Swift：变量与常量
来源：http://hb.shxzukj.cn

var a = 1;  let b = 2
来源：http://mc.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://mq.huixiangedu.cn

"值: \(b)"
来源：http://ma.shxzskj.cn

[T19] Swift：可选绑定
来源：http://tj.lnxyls.cn

if let n = opt { print(n) }
来源：http://wb.chemitech.net.cn

[T20] Swift：数组操作
来源：http://cf.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qn.huanxung.cn

[T21] Swift：遍历
来源：http://uf.nszjky.cn

for x in a { print(x) }
来源：http://pj.9csxet.cn

[T22] Swift：字典
来源：http://ak.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ui.nicolike.cn

[T23] Swift：函数
来源：http://ov.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ib.shxzskj.cn

[T24] Swift：闭包
来源：http://oe.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lv.bjjhwx.cn

[T25] Swift：结构体
来源：http://bx.jianghongdianzi.cn

struct P { var x: Int }
来源：http://ib.szsharing.cn

[T26] Swift：类与重写
来源：http://lm.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://eh.szxytkj.cn

[T27] Swift：错误处理
来源：http://xa.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://fm.asd995.cn

[T28] Swift：枚举
来源：http://hd.bookmarksfly.cn

enum Color { case red, green }
来源：http://gz.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://wa.haigaiapp.cn

guard let x = opt else { return }
来源：http://fb.panjiajie.cn

[T30] Swift：协议
来源：http://jn.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://yi.lnxyls.cn

[T31] Lua：Hello World
来源：http://py.bookmarksfly.cn

print("Hello")
来源：http://wl.nszjky.cn

[T32] Lua：局部变量
来源：http://ao.muxihuayi.cn

local a = 1
来源：http://ka.asd995.cn

[T33] Lua：表（数组）
来源：http://bz.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ev.nszjky.cn

[T34] Lua：遍历表
来源：http://hu.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ry.panjiajie.cn

[T35] Lua：字典表
来源：http://ua.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://nw.gzmigu.cn

[T36] Lua：函数
来源：http://qx.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://uv.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://tm.jianghongdianzi.cn

"a" .. "b"
来源：http://gb.lnxyls.cn

[T38] Lua：条件
来源：http://pb.521024.cn

if x > 0 then print("正") end
来源：http://wj.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://cl.521024.cn

string.find(s, "%d+")
来源：http://as.huixinmuqiang.cn

[T40] Lua：元表
来源：http://ij.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://uj.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://qx.yuexingan06.cn

print "Hello\n";
来源：http://qw.nszjky.cn

[T42] Perl：变量类型
来源：http://el.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://on.521024.cn

[T43] Perl：字符串插值
来源：http://cv.szxytkj.cn

"值: $a"
来源：http://ie.gzmigu.cn

[T44] Perl：条件
来源：http://qt.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://ho.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://xc.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://gt.shxzukj.cn

[T46] Perl：哈希操作
来源：http://qa.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://el.nszjky.cn

[T47] Perl：正则捕获
来源：http://xu.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mz.yuexingan06.cn

[T48] Perl：正则替换
来源：http://zf.newstarts.cn

$s =~ s/old/new/g;
来源：http://yq.huixiangedu.cn

[T49] Perl：函数
来源：http://qc.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gj.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://ra.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hk.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://ib.wgjwhj.cn

[T51] Scala：Hello World
来源：http://nn.lnxyls.cn

println("Hello")
来源：http://ed.9csxet.cn

[T52] Scala：变量
来源：http://dc.shtwfgs.cn

val a = 1;  var b = 2
来源：http://vy.huanxung.cn

[T53] Scala：字符串插值
来源：http://ie.szxytkj.cn

s"值: $b"
来源：http://wm.9csxet.cn

[T54] Scala：集合映射
来源：http://cu.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://rh.hahajie.cn

[T55] Scala：集合过滤
来源：http://rj.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://un.huanxung.cn

[T56] Scala：样例类
来源：http://nr.hnjuh.cn

case class User(name: String, age: Int)
来源：http://gm.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://my.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dg.shxzskj.cn

[T58] Scala：函数定义
来源：http://pq.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yc.chemitech.net.cn

[T59] Scala：循环
来源：http://tb.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://tn.nicolike.cn

[T60] Scala：折叠
来源：http://oe.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cz.huixinmuqiang.cn

================================================================================
来源：http://ey.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hr.newstarts.cn

================================================================================
来源：http://hm.shxzukj.cn


<!-- 参考信息 -->