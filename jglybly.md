代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nf.wgjwhj.cn

[R54] 比较两个文件
来源：http://pi.muxihuayi.cn

diff a.txt b.txt
来源：http://sz.szxytkj.cn

[R55] 压缩与解压
来源：http://tn.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ox.muxihuayi.cn

[R56] 远程拷贝
来源：http://us.shxzskj.cn

scp file user@host:/path/
来源：http://gw.lnxyls.cn

[R57] 远程执行命令
来源：http://wk.panjiajie.cn

ssh user@host 'uptime'
来源：http://bb.nicolike.cn

[R58] 下载文件
来源：http://vp.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sh.colortex.cn

[R59] 发 POST JSON
来源：http://bl.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eb.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://ny.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wr.asd995.cn

[R61] 磁盘占用
来源：http://rx.shxzukj.cn

df -h;  du -sh *
来源：http://vy.nszjky.cn

[R62] 找最占空间的文件
来源：http://kf.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://gg.muxihuayi.cn

[R63] 内存与进程
来源：http://mo.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://td.gzmigu.cn

[R64] 结束进程
来源：http://mr.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://rs.nicolike.cn

[R65] 查看端口占用
来源：http://uy.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zm.jianghongdianzi.cn

[R66] 定时任务
来源：http://xn.521024.cn

crontab -e;  crontab -l
来源：http://am.9csxet.cn

[R67] 生成随机十六进制串
来源：http://qb.szsharing.cn

openssl rand -hex 16
来源：http://oa.szxytkj.cn

[R68] 计算文件校验值
来源：http://ey.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qe.szxytkj.cn

[R69] 生成随机密码
来源：http://gi.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://wr.szxytkj.cn

[R70] 时间戳与互转
来源：http://ee.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://bb.gzmigu.cn

[R71] 日期格式化
来源：http://pi.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ae.hnjuh.cn

[R72] 等待端口就绪
来源：http://bp.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ii.nicolike.cn

[R73] 分割大日志
来源：http://lh.9csxet.cn

split -l 1000 big.log part_
来源：http://ca.panjiajie.cn

[R74] 批量重命名
来源：http://ny.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tb.shxzskj.cn

[R75] 导出环境变量
来源：http://do.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://rf.hnjuh.cn

[R76] 使用临时文件
来源：http://np.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ay.chemitech.net.cn

[R77] 读取用户输入
来源：http://nc.asd995.cn

read -rp "请输入: " ans
来源：http://mz.szxytkj.cn

[R78] 交互式菜单
来源：http://ap.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lp.shxzukj.cn

[R79] 解析命令行选项
来源：http://bv.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vd.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://bs.hahajie.cn

time ./run.sh
来源：http://pg.9csxet.cn

================================================================================
来源：http://ks.bjjhwx.cn

S. C / C++ 专题
来源：http://ac.yuexingan06.cn

================================================================================
来源：http://lk.yuntaijiaju.cn

[S01] C：Hello World
来源：http://et.gzmigu.cn

#include <stdio.h>
来源：http://pk.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://py.asd995.cn

[S02] C：变量与格式化输出
来源：http://pa.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://lb.bjjhwx.cn

[S03] C：读入整数
来源：http://qp.colortex.cn

int x; scanf("%d", &x);
来源：http://dw.wgjwhj.cn

[S04] C：字符串复制
来源：http://gq.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ry.lnxyls.cn

[S05] C：字符串长度
来源：http://dw.lnxyls.cn

strlen(s)
来源：http://mx.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://ty.shtwfgs.cn

strcmp(a, b) == 0
来源：http://tf.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://fb.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yh.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://um.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cg.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://rf.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xm.jctech888.com.cn

[S10] C：指针与解引用
来源：http://xb.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://hy.nszjky.cn

[S11] C：逐行读文件
来源：http://ia.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://kl.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cd.colortex.cn

fclose(f);
来源：http://ka.muxihuayi.cn

[S12] C：写文件
来源：http://po.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fh.haigaiapp.cn

[S13] C：宏定义
来源：http://xa.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yp.nicolike.cn

[S14] C：枚举
来源：http://hc.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://xk.nszjky.cn

[S15] C：类型转换
来源：http://uq.nszjky.cn

(double) a / b
来源：http://bz.shxzukj.cn

[S16] C：位操作置位
来源：http://oy.chemitech.net.cn

x |= (1 << 3);
来源：http://yd.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://pd.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ew.nicolike.cn

[S18] C：命令行参数
来源：http://vh.shtwfgs.cn

int main(int argc, char **argv)
来源：http://hb.yuexingan06.cn

[S19] C：快速排序
来源：http://ms.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gm.jianghongdianzi.cn

[S20] C：二分查找
来源：http://hd.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qt.shtwfgs.cn

[S21] C：字符类别判断
来源：http://zr.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hf.shtwfgs.cn

[S22] C：字符串转数字
来源：http://nx.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jy.nicolike.cn

[S23] C：随机数
来源：http://xa.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rg.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://mo.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qg.szxytkj.cn

[S25] C：内存拷贝
来源：http://wd.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://jr.shtwfgs.cn

[S26] C：内存清零
来源：http://mm.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://gp.yuexingan06.cn

[S27] C：定义常量
来源：http://tu.huanxung.cn

const double PI = 3.14159;
来源：http://zz.haigaiapp.cn

[S28] C：静态变量
来源：http://zj.wgjwhj.cn

static int counter = 0;
来源：http://qt.jianghongdianzi.cn

[S29] C：变参函数
来源：http://ww.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fs.asd995.cn

[S30] C：头文件保护
来源：http://ld.huixiangedu.cn

#ifndef X_H
来源：http://dp.bookmarksfly.cn

#define X_H
来源：http://kl.yuntaijiaju.cn

#endif
来源：http://ib.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://es.hahajie.cn

#include <iostream>
来源：http://ho.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://lt.asd995.cn

[S32] C++：字符串
来源：http://wl.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://lj.panjiajie.cn

[S33] C++：vector 增删
来源：http://wu.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nm.nicolike.cn

[S34] C++：遍历 vector
来源：http://lu.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://yr.shxzukj.cn

[S35] C++：map
来源：http://zc.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bq.newstarts.cn

[S36] C++：unordered_map
来源：http://vo.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ss.shxzukj.cn

[S37] C++：set
来源：http://cc.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iz.yuexingan06.cn

[S38] C++：排序
来源：http://br.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://do.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://vi.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mj.nicolike.cn

[S40] C++：查找元素
来源：http://ti.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sv.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://zf.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zg.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://jl.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://ad.szxytkj.cn

[S43] C++：智能指针
来源：http://ay.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://aw.jctech888.com.cn

[S44] C++：引用传参
来源：http://fd.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://rn.yuntaijiaju.cn

[S45] C++：lambda
来源：http://lx.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qm.bookmarksfly.cn

[S46] C++：函数模板
来源：http://am.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gr.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://mh.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qm.9csxet.cn

[S48] C++：逐行读文件
来源：http://ec.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kz.colortex.cn

while (std::getline(in, line)) { }
来源：http://js.asd995.cn

[S49] C++：写文件
来源：http://xe.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hw.nszjky.cn

[S50] C++：格式化数字
来源：http://ga.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sh.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://hl.szsharing.cn

static_cast<double>(a) / b
来源：http://ra.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://fd.colortex.cn

int size() const noexcept { return n_; }
来源：http://tg.hnjuh.cn

[S53] C++：移动语义
来源：http://wc.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://ig.521024.cn

[S54] C++：异常处理
来源：http://sm.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ra.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://gs.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vl.szxytkj.cn

[S56] C++：optional
来源：http://cp.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qv.panjiajie.cn

[S57] C++：编译期常量
来源：http://qw.colortex.cn

constexpr int N = 10;
来源：http://cl.szxytkj.cn

[S58] C++：命名空间
来源：http://kx.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://fd.colortex.cn

[S59] C++：静态断言
来源：http://id.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ns.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://fo.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qb.lnxyls.cn

================================================================================
来源：http://dz.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pq.chemitech.net.cn

================================================================================
来源：http://ox.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://rk.bjjhwx.cn

println("Hello")
来源：http://up.colortex.cn

[T02] Kotlin：变量
来源：http://xr.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bc.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://jn.lnxyls.cn

"值: $b"
来源：http://tw.9csxet.cn

[T04] Kotlin：空安全
来源：http://zd.shxzskj.cn

val n: String? = null;  n?.length
来源：http://hr.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://of.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tm.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://cm.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ob.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://so.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xw.asd995.cn

[T08] Kotlin：数据类
来源：http://cg.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://cn.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://cj.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://fb.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://me.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cg.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://qt.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bi.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://oz.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://co.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://nc.nicolike.cn

val m = mapOf("a" to 1)
来源：http://rr.521024.cn

[T14] Kotlin：循环
来源：http://mi.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://sw.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://ec.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://mw.szxytkj.cn

[T16] Swift：Hello World
来源：http://zv.jianghongdianzi.cn

print("Hello")
来源：http://in.shxzskj.cn

[T17] Swift：变量与常量
来源：http://ut.nszjky.cn

var a = 1;  let b = 2
来源：http://tw.panjiajie.cn

[T18] Swift：字符串插值
来源：http://bk.panjiajie.cn

"值: \(b)"
来源：http://au.521024.cn

[T19] Swift：可选绑定
来源：http://kk.huanxung.cn

if let n = opt { print(n) }
来源：http://em.szsharing.cn

[T20] Swift：数组操作
来源：http://ek.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mx.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://ng.bjjhwx.cn

for x in a { print(x) }
来源：http://vm.lnxyls.cn

[T22] Swift：字典
来源：http://za.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uh.muxihuayi.cn

[T23] Swift：函数
来源：http://tn.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wh.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://ww.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kd.jctech888.com.cn

[T25] Swift：结构体
来源：http://oy.yuntaijiaju.cn

struct P { var x: Int }
来源：http://he.521024.cn

[T26] Swift：类与重写
来源：http://ri.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://lu.shxzskj.cn

[T27] Swift：错误处理
来源：http://zj.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://eg.bookmarksfly.cn

[T28] Swift：枚举
来源：http://ig.jctech888.com.cn

enum Color { case red, green }
来源：http://ms.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://qu.9csxet.cn

guard let x = opt else { return }
来源：http://vd.asd995.cn

[T30] Swift：协议
来源：http://dp.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://ky.szsharing.cn

[T31] Lua：Hello World
来源：http://xl.nicolike.cn

print("Hello")
来源：http://gv.chemitech.net.cn

[T32] Lua：局部变量
来源：http://qk.shxzskj.cn

local a = 1
来源：http://qh.newstarts.cn

[T33] Lua：表（数组）
来源：http://lk.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dq.haigaiapp.cn

[T34] Lua：遍历表
来源：http://oe.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hk.huanxung.cn

[T35] Lua：字典表
来源：http://ua.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://bx.lnxyls.cn

[T36] Lua：函数
来源：http://sg.hnjuh.cn

function add(a, b) return a + b end
来源：http://eg.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://fe.newstarts.cn

"a" .. "b"
来源：http://ie.jctech888.com.cn

[T38] Lua：条件
来源：http://wn.haigaiapp.cn

if x > 0 then print("正") end
来源：http://nt.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://gk.lnxyls.cn

string.find(s, "%d+")
来源：http://ov.yuexingan06.cn

[T40] Lua：元表
来源：http://mb.szsharing.cn

setmetatable({}, { __index = base })
来源：http://fa.huixiangedu.cn

[T41] Perl：Hello World
来源：http://lc.panjiajie.cn

print "Hello\n";
来源：http://gc.shxzukj.cn

[T42] Perl：变量类型
来源：http://wz.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sm.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://zp.521024.cn

"值: $a"
来源：http://cv.hahajie.cn

[T44] Perl：条件
来源：http://rs.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://vt.9csxet.cn

[T45] Perl：数组遍历
来源：http://wx.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://lg.nszjky.cn

[T46] Perl：哈希操作
来源：http://ja.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bk.szxytkj.cn

[T47] Perl：正则捕获
来源：http://ru.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ot.szsharing.cn

[T48] Perl：正则替换
来源：http://vq.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://qy.szsharing.cn

[T49] Perl：函数
来源：http://zk.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ql.huanxung.cn

[T50] Perl：逐行读文件
来源：http://zr.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://if.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://bk.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://zh.huixinmuqiang.cn

println("Hello")
来源：http://rs.shtwfgs.cn

[T52] Scala：变量
来源：http://zi.shxzskj.cn

val a = 1;  var b = 2
来源：http://ls.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://dh.asd995.cn

s"值: $b"
来源：http://fm.huanxung.cn

[T54] Scala：集合映射
来源：http://ks.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://uo.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://hj.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wc.szsharing.cn

[T56] Scala：样例类
来源：http://yv.shtwfgs.cn


<!-- 参考信息 -->