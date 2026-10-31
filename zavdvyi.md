代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://if.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://zw.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xp.hahajie.cn

[R61] 磁盘占用
来源：http://pw.newstarts.cn

df -h;  du -sh *
来源：http://zo.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://ds.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://vw.huanxung.cn

[R63] 内存与进程
来源：http://vp.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://ap.asd995.cn

[R64] 结束进程
来源：http://wq.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://gp.muxihuayi.cn

[R65] 查看端口占用
来源：http://hy.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sj.gzmigu.cn

[R66] 定时任务
来源：http://sr.9csxet.cn

crontab -e;  crontab -l
来源：http://mf.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://tp.szsharing.cn

openssl rand -hex 16
来源：http://kj.lnxyls.cn

[R68] 计算文件校验值
来源：http://mn.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yg.szsharing.cn

[R69] 生成随机密码
来源：http://vc.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://gc.chemitech.net.cn

[R70] 时间戳与互转
来源：http://xb.nszjky.cn

date +%s;  date -d @1700000000
来源：http://vw.huixiangedu.cn

[R71] 日期格式化
来源：http://jj.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rm.lnxyls.cn

[R72] 等待端口就绪
来源：http://om.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cj.chemitech.net.cn

[R73] 分割大日志
来源：http://rr.colortex.cn

split -l 1000 big.log part_
来源：http://mf.nszjky.cn

[R74] 批量重命名
来源：http://qy.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bk.huixiangedu.cn

[R75] 导出环境变量
来源：http://tq.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://nw.yuexingan06.cn

[R76] 使用临时文件
来源：http://kv.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ql.shtwfgs.cn

[R77] 读取用户输入
来源：http://wh.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://wq.haigaiapp.cn

[R78] 交互式菜单
来源：http://qm.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gn.9csxet.cn

[R79] 解析命令行选项
来源：http://kv.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zr.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://mq.nicolike.cn

time ./run.sh
来源：http://bx.newstarts.cn

================================================================================
来源：http://bp.hnjuh.cn

S. C / C++ 专题
来源：http://vd.lnxyls.cn

================================================================================
来源：http://hz.hahajie.cn

[S01] C：Hello World
来源：http://pu.haigaiapp.cn

#include <stdio.h>
来源：http://mr.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fn.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://ep.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://gf.szsharing.cn

[S03] C：读入整数
来源：http://ng.gzmigu.cn

int x; scanf("%d", &x);
来源：http://hk.huanxung.cn

[S04] C：字符串复制
来源：http://bf.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lb.9csxet.cn

[S05] C：字符串长度
来源：http://oa.nszjky.cn

strlen(s)
来源：http://qw.muxihuayi.cn

[S06] C：字符串比较
来源：http://ep.lnxyls.cn

strcmp(a, b) == 0
来源：http://dh.shxzskj.cn

[S07] C：数组遍历求和
来源：http://rb.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hq.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://lv.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uy.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://es.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vg.jctech888.com.cn

[S10] C：指针与解引用
来源：http://fa.colortex.cn

int *p = &a;  *p = 5;
来源：http://yl.muxihuayi.cn

[S11] C：逐行读文件
来源：http://vs.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://gp.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ji.bjjhwx.cn

fclose(f);
来源：http://uf.yuexingan06.cn

[S12] C：写文件
来源：http://mo.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dj.shxzskj.cn

[S13] C：宏定义
来源：http://do.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ve.yuntaijiaju.cn

[S14] C：枚举
来源：http://rk.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://rz.bjjhwx.cn

[S15] C：类型转换
来源：http://mb.colortex.cn

(double) a / b
来源：http://ut.yuexingan06.cn

[S16] C：位操作置位
来源：http://wr.jctech888.com.cn

x |= (1 << 3);
来源：http://oo.asd995.cn

[S17] C：安全拼接字符串
来源：http://rv.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lo.colortex.cn

[S18] C：命令行参数
来源：http://ue.hnjuh.cn

int main(int argc, char **argv)
来源：http://my.muxihuayi.cn

[S19] C：快速排序
来源：http://jh.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gk.asd995.cn

[S20] C：二分查找
来源：http://gv.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uj.chemitech.net.cn

[S21] C：字符类别判断
来源：http://at.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://az.521024.cn

[S22] C：字符串转数字
来源：http://dm.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bf.szsharing.cn

[S23] C：随机数
来源：http://lt.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nj.muxihuayi.cn

[S24] C：获取本地时间
来源：http://jg.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oa.hahajie.cn

[S25] C：内存拷贝
来源：http://sc.chemitech.net.cn

memcpy(dst, src, n);
来源：http://sj.nicolike.cn

[S26] C：内存清零
来源：http://xj.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://rl.bookmarksfly.cn

[S27] C：定义常量
来源：http://qh.szxytkj.cn

const double PI = 3.14159;
来源：http://ov.jianghongdianzi.cn

[S28] C：静态变量
来源：http://yc.shtwfgs.cn

static int counter = 0;
来源：http://fg.asd995.cn

[S29] C：变参函数
来源：http://qo.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jn.nicolike.cn

[S30] C：头文件保护
来源：http://ld.szsharing.cn

#ifndef X_H
来源：http://ws.gzmigu.cn

#define X_H
来源：http://fe.wgjwhj.cn

#endif
来源：http://ve.panjiajie.cn

[S31] C++：Hello World
来源：http://rn.shxzukj.cn

#include <iostream>
来源：http://jt.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://dl.szsharing.cn

[S32] C++：字符串
来源：http://ja.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://rn.hahajie.cn

[S33] C++：vector 增删
来源：http://lh.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ir.shxzukj.cn

[S34] C++：遍历 vector
来源：http://wt.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://vh.asd995.cn

[S35] C++：map
来源：http://pb.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yv.huixiangedu.cn

[S36] C++：unordered_map
来源：http://ez.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xm.panjiajie.cn

[S37] C++：set
来源：http://yb.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://os.jianghongdianzi.cn

[S38] C++：排序
来源：http://lm.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://vm.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://ei.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fo.shxzukj.cn

[S40] C++：查找元素
来源：http://gd.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uo.colortex.cn

[S41] C++：类与构造函数
来源：http://zq.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hv.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://mj.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://vi.9csxet.cn

[S43] C++：智能指针
来源：http://kc.521024.cn

auto p = std::make_unique<int>(5);
来源：http://rm.gzmigu.cn

[S44] C++：引用传参
来源：http://nd.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://tw.shxzskj.cn

[S45] C++：lambda
来源：http://vk.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xn.9csxet.cn

[S46] C++：函数模板
来源：http://aq.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mn.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://xw.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zt.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://vw.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bx.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://vm.yuntaijiaju.cn

[S49] C++：写文件
来源：http://mq.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hw.hahajie.cn

[S50] C++：格式化数字
来源：http://uo.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oz.szsharing.cn

[S51] C++：显式类型转换
来源：http://kx.chemitech.net.cn

static_cast<double>(a) / b
来源：http://fk.asd995.cn

[S52] C++：const 与 noexcept
来源：http://xd.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://tn.bookmarksfly.cn

[S53] C++：移动语义
来源：http://ve.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://rp.gzmigu.cn

[S54] C++：异常处理
来源：http://fk.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://do.hnjuh.cn

[S55] C++：结构化绑定
来源：http://yn.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ws.nicolike.cn

[S56] C++：optional
来源：http://ko.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yy.huanxung.cn

[S57] C++：编译期常量
来源：http://ps.asd995.cn

constexpr int N = 10;
来源：http://vf.9csxet.cn

[S58] C++：命名空间
来源：http://lh.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://ce.panjiajie.cn

[S59] C++：静态断言
来源：http://qy.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nr.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://qs.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mh.yuntaijiaju.cn

================================================================================
来源：http://kk.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yc.9csxet.cn

================================================================================
来源：http://ni.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://ud.bookmarksfly.cn

println("Hello")
来源：http://iq.newstarts.cn

[T02] Kotlin：变量
来源：http://wq.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ok.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://or.bjjhwx.cn

"值: $b"
来源：http://ut.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://xa.521024.cn

val n: String? = null;  n?.length
来源：http://jg.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://lj.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wa.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://ay.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://st.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://az.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pi.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://eu.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://om.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://he.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://dg.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://mm.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://au.shtwfgs.cn

[T11] Kotlin：协程
来源：http://go.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kg.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://be.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://af.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://jn.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://ce.shtwfgs.cn

[T14] Kotlin：循环
来源：http://yi.newstarts.cn

for (i in 1..10) println(i)
来源：http://xf.muxihuayi.cn

[T15] Kotlin：接口
来源：http://mr.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://ri.bjjhwx.cn

[T16] Swift：Hello World
来源：http://za.colortex.cn

print("Hello")
来源：http://ht.lnxyls.cn

[T17] Swift：变量与常量
来源：http://ha.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://fe.colortex.cn

[T18] Swift：字符串插值
来源：http://gn.hahajie.cn

"值: \(b)"
来源：http://nz.huanxung.cn

[T19] Swift：可选绑定
来源：http://sq.huanxung.cn

if let n = opt { print(n) }
来源：http://jl.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://ay.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qn.asd995.cn

[T21] Swift：遍历
来源：http://xh.bookmarksfly.cn

for x in a { print(x) }
来源：http://bi.shxzskj.cn

[T22] Swift：字典
来源：http://hd.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://em.huixiangedu.cn

[T23] Swift：函数
来源：http://ao.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xi.wgjwhj.cn

[T24] Swift：闭包
来源：http://xv.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fq.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://wo.panjiajie.cn

struct P { var x: Int }
来源：http://tt.szsharing.cn

[T26] Swift：类与重写
来源：http://ig.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://op.huixiangedu.cn

[T27] Swift：错误处理
来源：http://ut.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://np.szsharing.cn

[T28] Swift：枚举
来源：http://nk.szsharing.cn

enum Color { case red, green }
来源：http://qw.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://ww.shxzukj.cn

guard let x = opt else { return }
来源：http://pc.hahajie.cn

[T30] Swift：协议
来源：http://yu.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://vv.bjjhwx.cn

[T31] Lua：Hello World
来源：http://tx.gzmigu.cn

print("Hello")
来源：http://mo.huanxung.cn

[T32] Lua：局部变量
来源：http://bl.chemitech.net.cn

local a = 1
来源：http://cp.szxytkj.cn

[T33] Lua：表（数组）
来源：http://pt.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://od.lnxyls.cn

[T34] Lua：遍历表
来源：http://be.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rh.haigaiapp.cn

[T35] Lua：字典表
来源：http://mp.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://up.colortex.cn

[T36] Lua：函数
来源：http://ta.muxihuayi.cn

function add(a, b) return a + b end
来源：http://wv.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://uy.asd995.cn

"a" .. "b"
来源：http://no.huanxung.cn

[T38] Lua：条件
来源：http://ua.521024.cn

if x > 0 then print("正") end
来源：http://yn.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://ca.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://ni.panjiajie.cn

[T40] Lua：元表
来源：http://ez.szsharing.cn

setmetatable({}, { __index = base })
来源：http://iq.nszjky.cn

[T41] Perl：Hello World
来源：http://pq.asd995.cn

print "Hello\n";
来源：http://bf.hahajie.cn

[T42] Perl：变量类型
来源：http://ds.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yt.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://dn.hahajie.cn

"值: $a"
来源：http://cd.nszjky.cn

[T44] Perl：条件
来源：http://da.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://hl.nszjky.cn

[T45] Perl：数组遍历
来源：http://em.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://ua.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://df.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tc.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://gq.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ph.shtwfgs.cn

[T48] Perl：正则替换
来源：http://uf.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://xy.hnjuh.cn

[T49] Perl：函数
来源：http://xr.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ff.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://tp.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bf.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://vh.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://js.shxzukj.cn

println("Hello")
来源：http://bq.gzmigu.cn

[T52] Scala：变量
来源：http://ub.muxihuayi.cn

val a = 1;  var b = 2
来源：http://ln.hahajie.cn

[T53] Scala：字符串插值
来源：http://pq.yuntaijiaju.cn

s"值: $b"
来源：http://gw.szxytkj.cn

[T54] Scala：集合映射
来源：http://ev.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://wm.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://dm.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wn.gzmigu.cn

[T56] Scala：样例类
来源：http://gi.hnjuh.cn

case class User(name: String, age: Int)
来源：http://nx.gzmigu.cn

[T57] Scala：模式匹配
来源：http://un.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xc.newstarts.cn

[T58] Scala：函数定义
来源：http://mp.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ll.szsharing.cn

[T59] Scala：循环
来源：http://ax.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://ss.newstarts.cn

[T60] Scala：折叠
来源：http://mv.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wm.colortex.cn

================================================================================
来源：http://cy.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ww.szxytkj.cn

================================================================================
来源：http://cx.nicolike.cn


<!-- 参考信息 -->