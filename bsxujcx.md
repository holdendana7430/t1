代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vm.szsharing.cn

[R56] 远程拷贝
来源：http://rk.9csxet.cn

scp file user@host:/path/
来源：http://mu.wgjwhj.cn

[R57] 远程执行命令
来源：http://si.9csxet.cn

ssh user@host 'uptime'
来源：http://wn.bjjhwx.cn

[R58] 下载文件
来源：http://wm.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://to.chemitech.net.cn

[R59] 发 POST JSON
来源：http://kv.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lo.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://ou.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yz.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://cw.wgjwhj.cn

df -h;  du -sh *
来源：http://ka.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://zw.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://xv.asd995.cn

[R63] 内存与进程
来源：http://ah.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://fc.lnxyls.cn

[R64] 结束进程
来源：http://cx.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://df.haigaiapp.cn

[R65] 查看端口占用
来源：http://tn.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nw.shxzukj.cn

[R66] 定时任务
来源：http://kq.lnxyls.cn

crontab -e;  crontab -l
来源：http://kk.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://pj.szxytkj.cn

openssl rand -hex 16
来源：http://gw.hahajie.cn

[R68] 计算文件校验值
来源：http://jm.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kj.nicolike.cn

[R69] 生成随机密码
来源：http://of.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://so.wgjwhj.cn

[R70] 时间戳与互转
来源：http://vq.huanxung.cn

date +%s;  date -d @1700000000
来源：http://rh.nicolike.cn

[R71] 日期格式化
来源：http://zf.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jn.hahajie.cn

[R72] 等待端口就绪
来源：http://kd.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zh.szxytkj.cn

[R73] 分割大日志
来源：http://wd.newstarts.cn

split -l 1000 big.log part_
来源：http://wg.newstarts.cn

[R74] 批量重命名
来源：http://kr.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zz.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://mq.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://np.bjjhwx.cn

[R76] 使用临时文件
来源：http://id.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fc.bookmarksfly.cn

[R77] 读取用户输入
来源：http://yg.nicolike.cn

read -rp "请输入: " ans
来源：http://up.hahajie.cn

[R78] 交互式菜单
来源：http://ga.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ce.chemitech.net.cn

[R79] 解析命令行选项
来源：http://yt.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ut.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://qq.shxzskj.cn

time ./run.sh
来源：http://ec.muxihuayi.cn

================================================================================
来源：http://si.wgjwhj.cn

S. C / C++ 专题
来源：http://lj.lnxyls.cn

================================================================================
来源：http://yr.9csxet.cn

[S01] C：Hello World
来源：http://ou.panjiajie.cn

#include <stdio.h>
来源：http://er.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kr.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://ug.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://ap.wgjwhj.cn

[S03] C：读入整数
来源：http://zi.9csxet.cn

int x; scanf("%d", &x);
来源：http://gb.hnjuh.cn

[S04] C：字符串复制
来源：http://hb.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mi.haigaiapp.cn

[S05] C：字符串长度
来源：http://zz.shxzukj.cn

strlen(s)
来源：http://rs.muxihuayi.cn

[S06] C：字符串比较
来源：http://vu.shxzskj.cn

strcmp(a, b) == 0
来源：http://iy.shxzskj.cn

[S07] C：数组遍历求和
来源：http://xa.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mz.colortex.cn

[S08] C：动态内存分配与释放
来源：http://ve.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wy.521024.cn

[S09] C：结构体定义与初始化
来源：http://je.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cm.yuexingan06.cn

[S10] C：指针与解引用
来源：http://cc.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://xn.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://ep.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://gd.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gg.yuntaijiaju.cn

fclose(f);
来源：http://oy.jianghongdianzi.cn

[S12] C：写文件
来源：http://ib.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ek.szxytkj.cn

[S13] C：宏定义
来源：http://tm.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hv.9csxet.cn

[S14] C：枚举
来源：http://ih.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://zn.yuntaijiaju.cn

[S15] C：类型转换
来源：http://lb.hahajie.cn

(double) a / b
来源：http://nx.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://rd.jctech888.com.cn

x |= (1 << 3);
来源：http://cj.szsharing.cn

[S17] C：安全拼接字符串
来源：http://lr.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://em.gzmigu.cn

[S18] C：命令行参数
来源：http://hu.asd995.cn

int main(int argc, char **argv)
来源：http://eg.jianghongdianzi.cn

[S19] C：快速排序
来源：http://wl.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cw.muxihuayi.cn

[S20] C：二分查找
来源：http://xm.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vf.panjiajie.cn

[S21] C：字符类别判断
来源：http://la.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cy.hnjuh.cn

[S22] C：字符串转数字
来源：http://dt.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eh.9csxet.cn

[S23] C：随机数
来源：http://hx.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ow.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://pq.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ej.panjiajie.cn

[S25] C：内存拷贝
来源：http://gj.bjjhwx.cn

memcpy(dst, src, n);
来源：http://px.521024.cn

[S26] C：内存清零
来源：http://tp.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://rg.huanxung.cn

[S27] C：定义常量
来源：http://ds.newstarts.cn

const double PI = 3.14159;
来源：http://jp.asd995.cn

[S28] C：静态变量
来源：http://mp.huanxung.cn

static int counter = 0;
来源：http://nj.asd995.cn

[S29] C：变参函数
来源：http://in.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qa.haigaiapp.cn

[S30] C：头文件保护
来源：http://ft.szsharing.cn

#ifndef X_H
来源：http://ki.szsharing.cn

#define X_H
来源：http://uq.wgjwhj.cn

#endif
来源：http://nd.bookmarksfly.cn

[S31] C++：Hello World
来源：http://vl.lnxyls.cn

#include <iostream>
来源：http://an.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://xj.asd995.cn

[S32] C++：字符串
来源：http://di.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://yl.haigaiapp.cn

[S33] C++：vector 增删
来源：http://aw.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eq.hahajie.cn

[S34] C++：遍历 vector
来源：http://wx.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://wz.jctech888.com.cn

[S35] C++：map
来源：http://ge.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qw.nicolike.cn

[S36] C++：unordered_map
来源：http://do.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fc.muxihuayi.cn

[S37] C++：set
来源：http://hs.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ei.panjiajie.cn

[S38] C++：排序
来源：http://px.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://gv.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://px.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ns.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://az.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qq.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://bb.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qf.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://gf.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://qa.shxzskj.cn

[S43] C++：智能指针
来源：http://bb.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://or.hnjuh.cn

[S44] C++：引用传参
来源：http://ah.asd995.cn

void inc(int &x) { ++x; }
来源：http://ts.chemitech.net.cn

[S45] C++：lambda
来源：http://ol.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://um.asd995.cn

[S46] C++：函数模板
来源：http://jn.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ym.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://ri.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://um.shxzukj.cn

[S48] C++：逐行读文件
来源：http://gn.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gm.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://hu.9csxet.cn

[S49] C++：写文件
来源：http://tj.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ud.muxihuayi.cn

[S50] C++：格式化数字
来源：http://qk.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dz.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://ag.nicolike.cn

static_cast<double>(a) / b
来源：http://ay.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://fj.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://mq.panjiajie.cn

[S53] C++：移动语义
来源：http://bi.colortex.cn

std::vector<int> w = std::move(v);
来源：http://kx.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://mv.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kc.szsharing.cn

[S55] C++：结构化绑定
来源：http://cl.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rv.colortex.cn

[S56] C++：optional
来源：http://jy.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jv.9csxet.cn

[S57] C++：编译期常量
来源：http://rt.chemitech.net.cn

constexpr int N = 10;
来源：http://kz.chemitech.net.cn

[S58] C++：命名空间
来源：http://vv.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://wy.wgjwhj.cn

[S59] C++：静态断言
来源：http://cp.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xs.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://jj.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xn.bookmarksfly.cn

================================================================================
来源：http://sa.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tx.haigaiapp.cn

================================================================================
来源：http://xl.newstarts.cn

[T01] Kotlin：Hello World
来源：http://hu.gzmigu.cn

println("Hello")
来源：http://uj.bjjhwx.cn

[T02] Kotlin：变量
来源：http://zl.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tf.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://gt.521024.cn

"值: $b"
来源：http://ps.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://tq.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://nv.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://ai.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oe.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://ri.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bw.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://ry.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bm.shxzskj.cn

[T08] Kotlin：数据类
来源：http://mt.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://dv.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://le.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://qz.colortex.cn

[T10] Kotlin：默认参数
来源：http://bg.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lq.jctech888.com.cn

[T11] Kotlin：协程
来源：http://ze.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hp.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://jx.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://in.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://sd.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://pw.chemitech.net.cn

[T14] Kotlin：循环
来源：http://pw.nszjky.cn

for (i in 1..10) println(i)
来源：http://tu.colortex.cn

[T15] Kotlin：接口
来源：http://qb.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://ow.nszjky.cn

[T16] Swift：Hello World
来源：http://px.szsharing.cn

print("Hello")
来源：http://dw.hahajie.cn

[T17] Swift：变量与常量
来源：http://hq.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://xp.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://xx.lnxyls.cn

"值: \(b)"
来源：http://bo.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://qi.bjjhwx.cn

if let n = opt { print(n) }
来源：http://kb.chemitech.net.cn

[T20] Swift：数组操作
来源：http://cv.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qq.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://cb.chemitech.net.cn

for x in a { print(x) }
来源：http://id.521024.cn

[T22] Swift：字典
来源：http://mt.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dn.colortex.cn

[T23] Swift：函数
来源：http://hf.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kr.wgjwhj.cn

[T24] Swift：闭包
来源：http://pr.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vc.gzmigu.cn

[T25] Swift：结构体
来源：http://ba.huixiangedu.cn

struct P { var x: Int }
来源：http://gm.muxihuayi.cn

[T26] Swift：类与重写
来源：http://sw.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://tp.haigaiapp.cn

[T27] Swift：错误处理
来源：http://ch.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://dq.shtwfgs.cn

[T28] Swift：枚举
来源：http://qg.shtwfgs.cn

enum Color { case red, green }
来源：http://ch.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://tz.bookmarksfly.cn

guard let x = opt else { return }
来源：http://uj.hnjuh.cn

[T30] Swift：协议
来源：http://yp.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://fy.hahajie.cn

[T31] Lua：Hello World
来源：http://ry.hnjuh.cn

print("Hello")
来源：http://ik.huanxung.cn

[T32] Lua：局部变量
来源：http://pe.huanxung.cn

local a = 1
来源：http://uc.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://wo.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fs.yuexingan06.cn

[T34] Lua：遍历表
来源：http://ew.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yk.huanxung.cn

[T35] Lua：字典表
来源：http://gh.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://hn.shxzukj.cn

[T36] Lua：函数
来源：http://mk.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://tz.nszjky.cn

[T37] Lua：字符串拼接
来源：http://ov.9csxet.cn

"a" .. "b"
来源：http://jx.nicolike.cn

[T38] Lua：条件
来源：http://xl.muxihuayi.cn

if x > 0 then print("正") end
来源：http://hb.nicolike.cn

[T39] Lua：模式匹配
来源：http://zv.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://nf.huanxung.cn

[T40] Lua：元表
来源：http://cv.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://ca.asd995.cn

[T41] Perl：Hello World
来源：http://pg.nicolike.cn

print "Hello\n";
来源：http://bd.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://qz.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ba.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://rv.9csxet.cn

"值: $a"
来源：http://li.panjiajie.cn

[T44] Perl：条件
来源：http://go.asd995.cn

if ($a > 0) { print "正"; }
来源：http://co.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://zz.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://ir.asd995.cn

[T46] Perl：哈希操作
来源：http://dd.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aj.hnjuh.cn

[T47] Perl：正则捕获
来源：http://gu.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uz.asd995.cn

[T48] Perl：正则替换
来源：http://hb.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://qj.panjiajie.cn

[T49] Perl：函数
来源：http://kj.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://to.asd995.cn

[T50] Perl：逐行读文件
来源：http://sv.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gi.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://pa.colortex.cn

[T51] Scala：Hello World
来源：http://fb.jianghongdianzi.cn

println("Hello")
来源：http://tb.shxzskj.cn

[T52] Scala：变量
来源：http://xj.wgjwhj.cn

val a = 1;  var b = 2
来源：http://ua.szxytkj.cn

[T53] Scala：字符串插值
来源：http://br.lnxyls.cn

s"值: $b"
来源：http://tx.asd995.cn

[T54] Scala：集合映射
来源：http://aw.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ot.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://pl.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nl.asd995.cn

[T56] Scala：样例类
来源：http://gi.newstarts.cn

case class User(name: String, age: Int)
来源：http://ba.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://jr.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jl.shxzskj.cn

[T58] Scala：函数定义
来源：http://rq.gzmigu.cn


<!-- 参考信息 -->