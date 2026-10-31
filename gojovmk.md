代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lo.nicolike.cn

[R54] 比较两个文件
来源：http://hh.newstarts.cn

diff a.txt b.txt
来源：http://cj.newstarts.cn

[R55] 压缩与解压
来源：http://vx.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://em.nszjky.cn

[R56] 远程拷贝
来源：http://gw.muxihuayi.cn

scp file user@host:/path/
来源：http://im.shxzukj.cn

[R57] 远程执行命令
来源：http://uy.szsharing.cn

ssh user@host 'uptime'
来源：http://bj.newstarts.cn

[R58] 下载文件
来源：http://tu.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yi.colortex.cn

[R59] 发 POST JSON
来源：http://xg.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uu.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://gg.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vm.huixiangedu.cn

[R61] 磁盘占用
来源：http://bn.521024.cn

df -h;  du -sh *
来源：http://te.huanxung.cn

[R62] 找最占空间的文件
来源：http://fa.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://eu.yuexingan06.cn

[R63] 内存与进程
来源：http://dc.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://tj.huixiangedu.cn

[R64] 结束进程
来源：http://ym.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://gl.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://qv.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uu.shtwfgs.cn

[R66] 定时任务
来源：http://ek.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://cd.9csxet.cn

[R67] 生成随机十六进制串
来源：http://ij.yuntaijiaju.cn

openssl rand -hex 16
来源：http://ap.hahajie.cn

[R68] 计算文件校验值
来源：http://rn.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ug.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://im.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://by.szxytkj.cn

[R70] 时间戳与互转
来源：http://uc.szsharing.cn

date +%s;  date -d @1700000000
来源：http://po.shxzukj.cn

[R71] 日期格式化
来源：http://qw.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xe.huanxung.cn

[R72] 等待端口就绪
来源：http://gj.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wg.szsharing.cn

[R73] 分割大日志
来源：http://qe.huixiangedu.cn

split -l 1000 big.log part_
来源：http://hu.shtwfgs.cn

[R74] 批量重命名
来源：http://eb.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ch.haigaiapp.cn

[R75] 导出环境变量
来源：http://er.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://sk.yuexingan06.cn

[R76] 使用临时文件
来源：http://mp.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://md.hnjuh.cn

[R77] 读取用户输入
来源：http://fs.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://ak.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://zl.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ch.huixiangedu.cn

[R79] 解析命令行选项
来源：http://cs.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yt.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://qp.9csxet.cn

time ./run.sh
来源：http://ww.521024.cn

================================================================================
来源：http://yb.huixiangedu.cn

S. C / C++ 专题
来源：http://oz.lnxyls.cn

================================================================================
来源：http://ce.szsharing.cn

[S01] C：Hello World
来源：http://wm.hahajie.cn

#include <stdio.h>
来源：http://iy.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lx.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://no.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://jj.bookmarksfly.cn

[S03] C：读入整数
来源：http://hx.521024.cn

int x; scanf("%d", &x);
来源：http://id.huixiangedu.cn

[S04] C：字符串复制
来源：http://cf.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vr.hahajie.cn

[S05] C：字符串长度
来源：http://cm.szsharing.cn

strlen(s)
来源：http://qt.hnjuh.cn

[S06] C：字符串比较
来源：http://vu.szsharing.cn

strcmp(a, b) == 0
来源：http://qh.asd995.cn

[S07] C：数组遍历求和
来源：http://pf.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hw.colortex.cn

[S08] C：动态内存分配与释放
来源：http://aj.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fu.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://zl.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qc.hnjuh.cn

[S10] C：指针与解引用
来源：http://ie.nszjky.cn

int *p = &a;  *p = 5;
来源：http://id.colortex.cn

[S11] C：逐行读文件
来源：http://bl.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://fi.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nt.hahajie.cn

fclose(f);
来源：http://qd.panjiajie.cn

[S12] C：写文件
来源：http://fo.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jx.colortex.cn

[S13] C：宏定义
来源：http://nx.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mu.huixinmuqiang.cn

[S14] C：枚举
来源：http://qm.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://fa.asd995.cn

[S15] C：类型转换
来源：http://vp.shtwfgs.cn

(double) a / b
来源：http://qi.nicolike.cn

[S16] C：位操作置位
来源：http://jr.huixinmuqiang.cn

x |= (1 << 3);
来源：http://ik.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://xy.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qm.nszjky.cn

[S18] C：命令行参数
来源：http://ik.9csxet.cn

int main(int argc, char **argv)
来源：http://qp.hahajie.cn

[S19] C：快速排序
来源：http://bu.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://et.szsharing.cn

[S20] C：二分查找
来源：http://ef.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gs.nicolike.cn

[S21] C：字符类别判断
来源：http://tk.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fz.chemitech.net.cn

[S22] C：字符串转数字
来源：http://im.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wq.lnxyls.cn

[S23] C：随机数
来源：http://il.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vj.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://qa.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pr.szxytkj.cn

[S25] C：内存拷贝
来源：http://fa.szsharing.cn

memcpy(dst, src, n);
来源：http://vz.newstarts.cn

[S26] C：内存清零
来源：http://nn.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://zt.hahajie.cn

[S27] C：定义常量
来源：http://ec.panjiajie.cn

const double PI = 3.14159;
来源：http://pw.lnxyls.cn

[S28] C：静态变量
来源：http://yr.huanxung.cn

static int counter = 0;
来源：http://eg.jianghongdianzi.cn

[S29] C：变参函数
来源：http://oy.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jv.bjjhwx.cn

[S30] C：头文件保护
来源：http://zk.newstarts.cn

#ifndef X_H
来源：http://ug.bjjhwx.cn

#define X_H
来源：http://sh.huixiangedu.cn

#endif
来源：http://ek.huixiangedu.cn

[S31] C++：Hello World
来源：http://ui.521024.cn

#include <iostream>
来源：http://lz.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://vi.yuexingan06.cn

[S32] C++：字符串
来源：http://ly.asd995.cn

std::string s = "hi";  s += "!";
来源：http://gg.nszjky.cn

[S33] C++：vector 增删
来源：http://ey.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cx.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://mb.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://qf.huixinmuqiang.cn

[S35] C++：map
来源：http://zj.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xy.newstarts.cn

[S36] C++：unordered_map
来源：http://fh.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rj.huixinmuqiang.cn

[S37] C++：set
来源：http://jt.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pi.9csxet.cn

[S38] C++：排序
来源：http://ea.521024.cn

std::sort(v.begin(), v.end());
来源：http://qj.colortex.cn

[S39] C++：自定义比较器排序
来源：http://hj.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oo.colortex.cn

[S40] C++：查找元素
来源：http://ak.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://og.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://ni.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lq.hahajie.cn

[S42] C++：继承与虚函数
来源：http://sl.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://yf.muxihuayi.cn

[S43] C++：智能指针
来源：http://ui.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://ka.wgjwhj.cn

[S44] C++：引用传参
来源：http://is.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://al.chemitech.net.cn

[S45] C++：lambda
来源：http://mz.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ur.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://vq.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ee.521024.cn

[S47] C++：结构化绑定遍历
来源：http://bs.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ju.szsharing.cn

[S48] C++：逐行读文件
来源：http://xs.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gt.hahajie.cn

while (std::getline(in, line)) { }
来源：http://gw.szxytkj.cn

[S49] C++：写文件
来源：http://ep.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xl.bjjhwx.cn

[S50] C++：格式化数字
来源：http://xh.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://um.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://fm.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://js.colortex.cn

[S52] C++：const 与 noexcept
来源：http://jz.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://wc.bookmarksfly.cn

[S53] C++：移动语义
来源：http://qa.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://ry.huanxung.cn

[S54] C++：异常处理
来源：http://ki.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pg.shxzskj.cn

[S55] C++：结构化绑定
来源：http://hq.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dz.shxzskj.cn

[S56] C++：optional
来源：http://mw.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xz.haigaiapp.cn

[S57] C++：编译期常量
来源：http://wa.colortex.cn

constexpr int N = 10;
来源：http://qo.gzmigu.cn

[S58] C++：命名空间
来源：http://wt.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://mc.jctech888.com.cn

[S59] C++：静态断言
来源：http://yz.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fk.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://dl.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ta.szsharing.cn

================================================================================
来源：http://ji.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://et.chemitech.net.cn

================================================================================
来源：http://qy.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://jl.lnxyls.cn

println("Hello")
来源：http://bc.hahajie.cn

[T02] Kotlin：变量
来源：http://qv.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pa.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://ou.huanxung.cn

"值: $b"
来源：http://bx.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://be.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://ql.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://co.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ln.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://tl.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mj.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://mu.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zh.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://qz.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://ty.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://bf.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://dt.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://jh.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tu.wgjwhj.cn

[T11] Kotlin：协程
来源：http://ys.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rj.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://bt.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://ac.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://ky.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://hb.asd995.cn

[T14] Kotlin：循环
来源：http://ts.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://re.huanxung.cn

[T15] Kotlin：接口
来源：http://rp.szsharing.cn

interface Shape { fun area(): Double }
来源：http://cx.asd995.cn

[T16] Swift：Hello World
来源：http://cc.jianghongdianzi.cn

print("Hello")
来源：http://zg.szsharing.cn

[T17] Swift：变量与常量
来源：http://hv.yuexingan06.cn

var a = 1;  let b = 2
来源：http://ya.nicolike.cn

[T18] Swift：字符串插值
来源：http://qs.nicolike.cn

"值: \(b)"
来源：http://up.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://es.haigaiapp.cn

if let n = opt { print(n) }
来源：http://qn.huixiangedu.cn

[T20] Swift：数组操作
来源：http://lc.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ld.bjjhwx.cn

[T21] Swift：遍历
来源：http://ay.lnxyls.cn

for x in a { print(x) }
来源：http://cf.nicolike.cn

[T22] Swift：字典
来源：http://ep.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tt.newstarts.cn

[T23] Swift：函数
来源：http://yi.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bl.muxihuayi.cn

[T24] Swift：闭包
来源：http://jo.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tm.huixiangedu.cn

[T25] Swift：结构体
来源：http://ah.shxzukj.cn

struct P { var x: Int }
来源：http://fq.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://bs.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://sv.9csxet.cn

[T27] Swift：错误处理
来源：http://pk.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://mt.muxihuayi.cn

[T28] Swift：枚举
来源：http://nl.9csxet.cn

enum Color { case red, green }
来源：http://kd.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://go.nszjky.cn

guard let x = opt else { return }
来源：http://wn.colortex.cn

[T30] Swift：协议
来源：http://px.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://ku.gzmigu.cn

[T31] Lua：Hello World
来源：http://zc.newstarts.cn

print("Hello")
来源：http://ad.lnxyls.cn

[T32] Lua：局部变量
来源：http://ec.hnjuh.cn

local a = 1
来源：http://we.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://da.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fq.asd995.cn

[T34] Lua：遍历表
来源：http://ag.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ie.521024.cn

[T35] Lua：字典表
来源：http://aq.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://rk.hahajie.cn

[T36] Lua：函数
来源：http://et.szxytkj.cn

function add(a, b) return a + b end
来源：http://ek.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://ex.chemitech.net.cn

"a" .. "b"
来源：http://bu.hahajie.cn

[T38] Lua：条件
来源：http://kp.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://ba.newstarts.cn

[T39] Lua：模式匹配
来源：http://tl.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://os.yuexingan06.cn

[T40] Lua：元表
来源：http://gq.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://ol.hnjuh.cn

[T41] Perl：Hello World
来源：http://ud.9csxet.cn

print "Hello\n";
来源：http://mt.lnxyls.cn

[T42] Perl：变量类型
来源：http://ut.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jj.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://ea.szxytkj.cn

"值: $a"
来源：http://js.panjiajie.cn

[T44] Perl：条件
来源：http://ou.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://ih.hahajie.cn

[T45] Perl：数组遍历
来源：http://sc.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://us.nicolike.cn

[T46] Perl：哈希操作
来源：http://jv.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bd.colortex.cn

[T47] Perl：正则捕获
来源：http://zu.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dt.yuexingan06.cn

[T48] Perl：正则替换
来源：http://pd.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://vk.bookmarksfly.cn

[T49] Perl：函数
来源：http://oy.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ey.521024.cn

[T50] Perl：逐行读文件
来源：http://tl.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ep.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://wi.521024.cn

[T51] Scala：Hello World
来源：http://px.chemitech.net.cn

println("Hello")
来源：http://ne.huanxung.cn

[T52] Scala：变量
来源：http://yf.hnjuh.cn

val a = 1;  var b = 2
来源：http://ax.huanxung.cn

[T53] Scala：字符串插值
来源：http://yc.hnjuh.cn

s"值: $b"
来源：http://sp.huanxung.cn

[T54] Scala：集合映射
来源：http://ut.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://xg.shxzskj.cn

[T55] Scala：集合过滤
来源：http://xm.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://me.gzmigu.cn

[T56] Scala：样例类
来源：http://yg.haigaiapp.cn


<!-- 参考信息 -->