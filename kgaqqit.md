代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wa.szsharing.cn

[R56] 远程拷贝
来源：http://sn.lnxyls.cn

scp file user@host:/path/
来源：http://vz.shxzskj.cn

[R57] 远程执行命令
来源：http://cf.panjiajie.cn

ssh user@host 'uptime'
来源：http://up.haigaiapp.cn

[R58] 下载文件
来源：http://th.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://me.chemitech.net.cn

[R59] 发 POST JSON
来源：http://ez.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cw.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://tv.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://li.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://ef.hnjuh.cn

df -h;  du -sh *
来源：http://lg.521024.cn

[R62] 找最占空间的文件
来源：http://os.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://rs.huanxung.cn

[R63] 内存与进程
来源：http://cl.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://sw.huanxung.cn

[R64] 结束进程
来源：http://qt.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://ih.9csxet.cn

[R65] 查看端口占用
来源：http://mo.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ao.yuexingan06.cn

[R66] 定时任务
来源：http://qp.9csxet.cn

crontab -e;  crontab -l
来源：http://hm.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://qc.nicolike.cn

openssl rand -hex 16
来源：http://vv.huanxung.cn

[R68] 计算文件校验值
来源：http://ik.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dr.shxzskj.cn

[R69] 生成随机密码
来源：http://re.521024.cn

head -c 16 /dev/urandom | base64
来源：http://jy.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://mp.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://fp.muxihuayi.cn

[R71] 日期格式化
来源：http://lx.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kw.huixiangedu.cn

[R72] 等待端口就绪
来源：http://db.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://li.szsharing.cn

[R73] 分割大日志
来源：http://vj.haigaiapp.cn

split -l 1000 big.log part_
来源：http://ku.hnjuh.cn

[R74] 批量重命名
来源：http://he.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ty.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://jm.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://sw.gzmigu.cn

[R76] 使用临时文件
来源：http://xf.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mw.panjiajie.cn

[R77] 读取用户输入
来源：http://rv.huixiangedu.cn

read -rp "请输入: " ans
来源：http://ik.hahajie.cn

[R78] 交互式菜单
来源：http://at.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xv.bjjhwx.cn

[R79] 解析命令行选项
来源：http://wo.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ld.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://gt.panjiajie.cn

time ./run.sh
来源：http://cn.shtwfgs.cn

================================================================================
来源：http://me.huixiangedu.cn

S. C / C++ 专题
来源：http://ge.shxzskj.cn

================================================================================
来源：http://oe.chemitech.net.cn

[S01] C：Hello World
来源：http://no.shxzukj.cn

#include <stdio.h>
来源：http://au.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sp.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://kf.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://gm.nicolike.cn

[S03] C：读入整数
来源：http://ka.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://xu.bookmarksfly.cn

[S04] C：字符串复制
来源：http://ov.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wy.nicolike.cn

[S05] C：字符串长度
来源：http://tj.huanxung.cn

strlen(s)
来源：http://wy.shtwfgs.cn

[S06] C：字符串比较
来源：http://vi.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://yr.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://tu.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qx.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://mq.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jv.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://kn.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vg.jctech888.com.cn

[S10] C：指针与解引用
来源：http://yz.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://mc.huixiangedu.cn

[S11] C：逐行读文件
来源：http://qu.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://fc.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cj.521024.cn

fclose(f);
来源：http://cy.shxzukj.cn

[S12] C：写文件
来源：http://df.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gp.nszjky.cn

[S13] C：宏定义
来源：http://of.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wm.huixiangedu.cn

[S14] C：枚举
来源：http://si.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://xv.colortex.cn

[S15] C：类型转换
来源：http://ng.lnxyls.cn

(double) a / b
来源：http://sv.nszjky.cn

[S16] C：位操作置位
来源：http://ww.shxzukj.cn

x |= (1 << 3);
来源：http://nd.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://wn.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ih.huanxung.cn

[S18] C：命令行参数
来源：http://kd.szsharing.cn

int main(int argc, char **argv)
来源：http://mm.shxzukj.cn

[S19] C：快速排序
来源：http://ok.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ml.lnxyls.cn

[S20] C：二分查找
来源：http://eg.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gx.chemitech.net.cn

[S21] C：字符类别判断
来源：http://bw.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vv.jctech888.com.cn

[S22] C：字符串转数字
来源：http://jq.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ee.gzmigu.cn

[S23] C：随机数
来源：http://cx.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oe.bjjhwx.cn

[S24] C：获取本地时间
来源：http://jv.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jv.huixiangedu.cn

[S25] C：内存拷贝
来源：http://cd.lnxyls.cn

memcpy(dst, src, n);
来源：http://js.hnjuh.cn

[S26] C：内存清零
来源：http://xs.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://hy.gzmigu.cn

[S27] C：定义常量
来源：http://qw.shxzukj.cn

const double PI = 3.14159;
来源：http://gk.chemitech.net.cn

[S28] C：静态变量
来源：http://ff.shxzskj.cn

static int counter = 0;
来源：http://vo.haigaiapp.cn

[S29] C：变参函数
来源：http://kg.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fv.haigaiapp.cn

[S30] C：头文件保护
来源：http://mp.chemitech.net.cn

#ifndef X_H
来源：http://kb.colortex.cn

#define X_H
来源：http://eh.haigaiapp.cn

#endif
来源：http://uo.szxytkj.cn

[S31] C++：Hello World
来源：http://hn.muxihuayi.cn

#include <iostream>
来源：http://sb.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://of.bookmarksfly.cn

[S32] C++：字符串
来源：http://xa.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://ss.shtwfgs.cn

[S33] C++：vector 增删
来源：http://zg.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pj.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://ew.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://he.chemitech.net.cn

[S35] C++：map
来源：http://vd.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zy.nicolike.cn

[S36] C++：unordered_map
来源：http://xj.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ax.szsharing.cn

[S37] C++：set
来源：http://vp.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ad.huanxung.cn

[S38] C++：排序
来源：http://pk.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://io.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://fx.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://da.chemitech.net.cn

[S40] C++：查找元素
来源：http://wo.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wu.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://kq.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ls.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://io.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://zv.colortex.cn

[S43] C++：智能指针
来源：http://tk.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://jp.asd995.cn

[S44] C++：引用传参
来源：http://bd.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://vf.shxzukj.cn

[S45] C++：lambda
来源：http://mw.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lp.shtwfgs.cn

[S46] C++：函数模板
来源：http://qg.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aq.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://lt.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iy.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://hj.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hn.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://zp.9csxet.cn

[S49] C++：写文件
来源：http://rl.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yo.nicolike.cn

[S50] C++：格式化数字
来源：http://ku.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qz.szxytkj.cn

[S51] C++：显式类型转换
来源：http://kx.panjiajie.cn

static_cast<double>(a) / b
来源：http://pr.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://vp.hahajie.cn

int size() const noexcept { return n_; }
来源：http://tg.huanxung.cn

[S53] C++：移动语义
来源：http://re.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://fn.yuexingan06.cn

[S54] C++：异常处理
来源：http://ej.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nu.hnjuh.cn

[S55] C++：结构化绑定
来源：http://pw.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zk.yuntaijiaju.cn

[S56] C++：optional
来源：http://ne.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ww.huixiangedu.cn

[S57] C++：编译期常量
来源：http://dx.wgjwhj.cn

constexpr int N = 10;
来源：http://tp.asd995.cn

[S58] C++：命名空间
来源：http://nz.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://sw.nszjky.cn

[S59] C++：静态断言
来源：http://mt.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dy.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://id.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ga.nicolike.cn

================================================================================
来源：http://xh.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hq.shxzukj.cn

================================================================================
来源：http://yz.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://kb.colortex.cn

println("Hello")
来源：http://ih.gzmigu.cn

[T02] Kotlin：变量
来源：http://jk.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fd.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://sm.colortex.cn

"值: $b"
来源：http://bl.hahajie.cn

[T04] Kotlin：空安全
来源：http://do.nszjky.cn

val n: String? = null;  n?.length
来源：http://oi.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://tg.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ry.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://sf.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ml.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://lz.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ts.gzmigu.cn

[T08] Kotlin：数据类
来源：http://po.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://gn.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://vw.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://qx.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://zt.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zu.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://dd.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://is.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://hj.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://kw.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://nq.newstarts.cn

val m = mapOf("a" to 1)
来源：http://ml.jctech888.com.cn

[T14] Kotlin：循环
来源：http://sk.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://cx.asd995.cn

[T15] Kotlin：接口
来源：http://wc.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://nj.szxytkj.cn

[T16] Swift：Hello World
来源：http://nl.szxytkj.cn

print("Hello")
来源：http://rb.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://qv.521024.cn

var a = 1;  let b = 2
来源：http://cp.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://bu.yuexingan06.cn

"值: \(b)"
来源：http://du.shxzskj.cn

[T19] Swift：可选绑定
来源：http://nt.shtwfgs.cn

if let n = opt { print(n) }
来源：http://nq.szxytkj.cn

[T20] Swift：数组操作
来源：http://fw.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wq.chemitech.net.cn

[T21] Swift：遍历
来源：http://lm.haigaiapp.cn

for x in a { print(x) }
来源：http://wh.jctech888.com.cn

[T22] Swift：字典
来源：http://xr.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ff.huixinmuqiang.cn

[T23] Swift：函数
来源：http://hi.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wl.huixiangedu.cn

[T24] Swift：闭包
来源：http://xi.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yu.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://ne.huixinmuqiang.cn

struct P { var x: Int }
来源：http://zp.newstarts.cn

[T26] Swift：类与重写
来源：http://zk.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://ni.haigaiapp.cn

[T27] Swift：错误处理
来源：http://ai.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://wf.hnjuh.cn

[T28] Swift：枚举
来源：http://xx.asd995.cn

enum Color { case red, green }
来源：http://hw.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://gd.colortex.cn

guard let x = opt else { return }
来源：http://bn.huixinmuqiang.cn

[T30] Swift：协议
来源：http://ea.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://uu.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://pn.jctech888.com.cn

print("Hello")
来源：http://ul.szxytkj.cn

[T32] Lua：局部变量
来源：http://go.szsharing.cn

local a = 1
来源：http://ox.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://bk.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sm.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://ka.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qc.lnxyls.cn

[T35] Lua：字典表
来源：http://ei.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://qt.hahajie.cn

[T36] Lua：函数
来源：http://jn.yuexingan06.cn

function add(a, b) return a + b end
来源：http://pt.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://fc.szxytkj.cn

"a" .. "b"
来源：http://ss.lnxyls.cn

[T38] Lua：条件
来源：http://gd.shxzskj.cn

if x > 0 then print("正") end
来源：http://nv.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://wv.jctech888.com.cn

string.find(s, "%d+")
来源：http://dy.hahajie.cn

[T40] Lua：元表
来源：http://af.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://nq.9csxet.cn

[T41] Perl：Hello World
来源：http://bx.szsharing.cn

print "Hello\n";
来源：http://pd.huanxung.cn

[T42] Perl：变量类型
来源：http://em.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yd.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://vc.shtwfgs.cn

"值: $a"
来源：http://lx.panjiajie.cn

[T44] Perl：条件
来源：http://ov.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://cp.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://xp.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://qf.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://ce.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xf.szsharing.cn

[T47] Perl：正则捕获
来源：http://gq.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fx.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://nt.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://zw.colortex.cn

[T49] Perl：函数
来源：http://pv.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wx.nszjky.cn

[T50] Perl：逐行读文件
来源：http://bd.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ui.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://xx.chemitech.net.cn

[T51] Scala：Hello World
来源：http://hc.bookmarksfly.cn

println("Hello")
来源：http://ke.jianghongdianzi.cn

[T52] Scala：变量
来源：http://pz.newstarts.cn

val a = 1;  var b = 2
来源：http://hp.lnxyls.cn

[T53] Scala：字符串插值
来源：http://gd.newstarts.cn

s"值: $b"
来源：http://go.shxzukj.cn

[T54] Scala：集合映射
来源：http://yc.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://mv.szxytkj.cn

[T55] Scala：集合过滤
来源：http://ay.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mn.nicolike.cn

[T56] Scala：样例类
来源：http://ct.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://mi.szsharing.cn

[T57] Scala：模式匹配
来源：http://dw.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dz.9csxet.cn

[T58] Scala：函数定义
来源：http://cv.jctech888.com.cn


<!-- 参考信息 -->