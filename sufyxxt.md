代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uo.shxzukj.cn

[R54] 比较两个文件
来源：http://bq.jctech888.com.cn

diff a.txt b.txt
来源：http://ng.nszjky.cn

[R55] 压缩与解压
来源：http://zi.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kr.shtwfgs.cn

[R56] 远程拷贝
来源：http://gf.huixiangedu.cn

scp file user@host:/path/
来源：http://fz.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://tc.szsharing.cn

ssh user@host 'uptime'
来源：http://hb.wgjwhj.cn

[R58] 下载文件
来源：http://el.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fa.nicolike.cn

[R59] 发 POST JSON
来源：http://ge.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pm.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://od.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yb.bookmarksfly.cn

[R61] 磁盘占用
来源：http://ko.chemitech.net.cn

df -h;  du -sh *
来源：http://pe.panjiajie.cn

[R62] 找最占空间的文件
来源：http://pm.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://hu.bjjhwx.cn

[R63] 内存与进程
来源：http://ed.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://wf.huixinmuqiang.cn

[R64] 结束进程
来源：http://hn.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://mu.muxihuayi.cn

[R65] 查看端口占用
来源：http://tv.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pk.huixiangedu.cn

[R66] 定时任务
来源：http://at.hahajie.cn

crontab -e;  crontab -l
来源：http://zg.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://lw.9csxet.cn

openssl rand -hex 16
来源：http://ra.chemitech.net.cn

[R68] 计算文件校验值
来源：http://nr.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ng.asd995.cn

[R69] 生成随机密码
来源：http://xz.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://gq.nszjky.cn

[R70] 时间戳与互转
来源：http://ti.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://bk.panjiajie.cn

[R71] 日期格式化
来源：http://zx.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://iq.9csxet.cn

[R72] 等待端口就绪
来源：http://si.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lc.wgjwhj.cn

[R73] 分割大日志
来源：http://qh.shxzukj.cn

split -l 1000 big.log part_
来源：http://sj.lnxyls.cn

[R74] 批量重命名
来源：http://hr.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nd.521024.cn

[R75] 导出环境变量
来源：http://ul.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://yj.yuexingan06.cn

[R76] 使用临时文件
来源：http://mp.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bl.szsharing.cn

[R77] 读取用户输入
来源：http://ag.nicolike.cn

read -rp "请输入: " ans
来源：http://yf.nicolike.cn

[R78] 交互式菜单
来源：http://nb.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lc.gzmigu.cn

[R79] 解析命令行选项
来源：http://cq.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dy.521024.cn

[R80] 查看脚本执行耗时
来源：http://uw.gzmigu.cn

time ./run.sh
来源：http://du.huixiangedu.cn

================================================================================
来源：http://ri.shxzskj.cn

S. C / C++ 专题
来源：http://mo.shxzukj.cn

================================================================================
来源：http://ky.521024.cn

[S01] C：Hello World
来源：http://oy.bookmarksfly.cn

#include <stdio.h>
来源：http://ug.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yo.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://pp.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://lx.hahajie.cn

[S03] C：读入整数
来源：http://iy.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://qa.gzmigu.cn

[S04] C：字符串复制
来源：http://ek.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tu.hnjuh.cn

[S05] C：字符串长度
来源：http://sk.jctech888.com.cn

strlen(s)
来源：http://nf.huanxung.cn

[S06] C：字符串比较
来源：http://sc.muxihuayi.cn

strcmp(a, b) == 0
来源：http://kq.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://dg.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gw.colortex.cn

[S08] C：动态内存分配与释放
来源：http://yh.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gk.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://tb.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oq.hnjuh.cn

[S10] C：指针与解引用
来源：http://za.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://fy.shxzukj.cn

[S11] C：逐行读文件
来源：http://ny.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://tn.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iv.gzmigu.cn

fclose(f);
来源：http://cd.9csxet.cn

[S12] C：写文件
来源：http://ga.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ie.jianghongdianzi.cn

[S13] C：宏定义
来源：http://qe.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://la.jianghongdianzi.cn

[S14] C：枚举
来源：http://sk.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://kk.9csxet.cn

[S15] C：类型转换
来源：http://ll.shxzukj.cn

(double) a / b
来源：http://mr.9csxet.cn

[S16] C：位操作置位
来源：http://re.asd995.cn

x |= (1 << 3);
来源：http://np.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://gj.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vy.lnxyls.cn

[S18] C：命令行参数
来源：http://gf.colortex.cn

int main(int argc, char **argv)
来源：http://vx.asd995.cn

[S19] C：快速排序
来源：http://ga.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cb.huixiangedu.cn

[S20] C：二分查找
来源：http://ma.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://if.muxihuayi.cn

[S21] C：字符类别判断
来源：http://jw.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jv.huixiangedu.cn

[S22] C：字符串转数字
来源：http://oh.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xk.shxzskj.cn

[S23] C：随机数
来源：http://sc.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ua.szsharing.cn

[S24] C：获取本地时间
来源：http://js.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kw.wgjwhj.cn

[S25] C：内存拷贝
来源：http://hu.gzmigu.cn

memcpy(dst, src, n);
来源：http://fk.huixinmuqiang.cn

[S26] C：内存清零
来源：http://zs.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://kr.asd995.cn

[S27] C：定义常量
来源：http://zn.bjjhwx.cn

const double PI = 3.14159;
来源：http://mn.gzmigu.cn

[S28] C：静态变量
来源：http://ai.jianghongdianzi.cn

static int counter = 0;
来源：http://is.hahajie.cn

[S29] C：变参函数
来源：http://tn.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nx.hnjuh.cn

[S30] C：头文件保护
来源：http://ku.lnxyls.cn

#ifndef X_H
来源：http://he.szxytkj.cn

#define X_H
来源：http://qk.chemitech.net.cn

#endif
来源：http://yo.muxihuayi.cn

[S31] C++：Hello World
来源：http://gz.lnxyls.cn

#include <iostream>
来源：http://fo.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://pg.bjjhwx.cn

[S32] C++：字符串
来源：http://mn.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://tx.huixiangedu.cn

[S33] C++：vector 增删
来源：http://kx.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tb.hnjuh.cn

[S34] C++：遍历 vector
来源：http://ej.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://wk.hahajie.cn

[S35] C++：map
来源：http://cs.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lm.9csxet.cn

[S36] C++：unordered_map
来源：http://rx.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fy.shxzukj.cn

[S37] C++：set
来源：http://ug.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bn.hnjuh.cn

[S38] C++：排序
来源：http://vo.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://be.asd995.cn

[S39] C++：自定义比较器排序
来源：http://px.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ce.bjjhwx.cn

[S40] C++：查找元素
来源：http://dy.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gt.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://mt.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qu.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://os.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://rx.panjiajie.cn

[S43] C++：智能指针
来源：http://aa.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://lx.newstarts.cn

[S44] C++：引用传参
来源：http://cq.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://fp.huixinmuqiang.cn

[S45] C++：lambda
来源：http://if.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ws.haigaiapp.cn

[S46] C++：函数模板
来源：http://mq.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rv.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://zj.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kt.hahajie.cn

[S48] C++：逐行读文件
来源：http://hj.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yc.521024.cn

while (std::getline(in, line)) { }
来源：http://kx.bookmarksfly.cn

[S49] C++：写文件
来源：http://rt.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dr.huixiangedu.cn

[S50] C++：格式化数字
来源：http://uj.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ou.gzmigu.cn

[S51] C++：显式类型转换
来源：http://za.nszjky.cn

static_cast<double>(a) / b
来源：http://ix.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://om.asd995.cn

int size() const noexcept { return n_; }
来源：http://zu.shtwfgs.cn

[S53] C++：移动语义
来源：http://jv.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://me.szxytkj.cn

[S54] C++：异常处理
来源：http://gm.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xk.panjiajie.cn

[S55] C++：结构化绑定
来源：http://oi.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xd.huixiangedu.cn

[S56] C++：optional
来源：http://yp.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cl.huixiangedu.cn

[S57] C++：编译期常量
来源：http://ba.shxzskj.cn

constexpr int N = 10;
来源：http://ny.szsharing.cn

[S58] C++：命名空间
来源：http://nr.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://tj.9csxet.cn

[S59] C++：静态断言
来源：http://ta.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fm.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://ez.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://me.huixinmuqiang.cn

================================================================================
来源：http://od.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pk.huanxung.cn

================================================================================
来源：http://nn.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://kg.shtwfgs.cn

println("Hello")
来源：http://ka.9csxet.cn

[T02] Kotlin：变量
来源：http://tt.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ha.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://qo.huanxung.cn

"值: $b"
来源：http://rs.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://bd.szsharing.cn

val n: String? = null;  n?.length
来源：http://oe.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://pa.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://js.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://sa.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vp.asd995.cn

[T07] Kotlin：集合过滤
来源：http://lc.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://du.asd995.cn

[T08] Kotlin：数据类
来源：http://vz.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://ec.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://px.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://sk.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://rc.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oo.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://ts.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dl.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://vg.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://af.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://qp.asd995.cn

val m = mapOf("a" to 1)
来源：http://aw.nicolike.cn

[T14] Kotlin：循环
来源：http://bp.9csxet.cn

for (i in 1..10) println(i)
来源：http://kc.gzmigu.cn

[T15] Kotlin：接口
来源：http://yu.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://kj.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://xs.shxzukj.cn

print("Hello")
来源：http://fk.szsharing.cn

[T17] Swift：变量与常量
来源：http://of.newstarts.cn

var a = 1;  let b = 2
来源：http://ye.lnxyls.cn

[T18] Swift：字符串插值
来源：http://iu.gzmigu.cn

"值: \(b)"
来源：http://zc.shxzukj.cn

[T19] Swift：可选绑定
来源：http://tg.shxzskj.cn

if let n = opt { print(n) }
来源：http://yu.nszjky.cn

[T20] Swift：数组操作
来源：http://cw.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://og.muxihuayi.cn

[T21] Swift：遍历
来源：http://gp.huixiangedu.cn

for x in a { print(x) }
来源：http://yb.shtwfgs.cn

[T22] Swift：字典
来源：http://xu.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sg.colortex.cn

[T23] Swift：函数
来源：http://gq.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://to.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://wv.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tu.bjjhwx.cn

[T25] Swift：结构体
来源：http://nj.lnxyls.cn

struct P { var x: Int }
来源：http://ud.szxytkj.cn

[T26] Swift：类与重写
来源：http://sq.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://uy.wgjwhj.cn

[T27] Swift：错误处理
来源：http://ii.hahajie.cn

do { try f() } catch { print(error) }
来源：http://hs.gzmigu.cn

[T28] Swift：枚举
来源：http://vc.gzmigu.cn

enum Color { case red, green }
来源：http://tw.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://jc.shxzukj.cn

guard let x = opt else { return }
来源：http://cr.bjjhwx.cn

[T30] Swift：协议
来源：http://cd.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://tv.newstarts.cn

[T31] Lua：Hello World
来源：http://pi.colortex.cn

print("Hello")
来源：http://ur.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://rz.szxytkj.cn

local a = 1
来源：http://qp.szsharing.cn

[T33] Lua：表（数组）
来源：http://yx.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cs.chemitech.net.cn

[T34] Lua：遍历表
来源：http://fm.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zr.bjjhwx.cn

[T35] Lua：字典表
来源：http://tv.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://er.hahajie.cn

[T36] Lua：函数
来源：http://iz.newstarts.cn

function add(a, b) return a + b end
来源：http://xk.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://qr.panjiajie.cn

"a" .. "b"
来源：http://ik.szxytkj.cn

[T38] Lua：条件
来源：http://pf.colortex.cn

if x > 0 then print("正") end
来源：http://av.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://pe.jctech888.com.cn

string.find(s, "%d+")
来源：http://ku.gzmigu.cn

[T40] Lua：元表
来源：http://dp.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://dt.shtwfgs.cn

[T41] Perl：Hello World
来源：http://hn.jianghongdianzi.cn

print "Hello\n";
来源：http://gp.hahajie.cn

[T42] Perl：变量类型
来源：http://sq.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hi.9csxet.cn

[T43] Perl：字符串插值
来源：http://wl.newstarts.cn

"值: $a"
来源：http://qu.hahajie.cn

[T44] Perl：条件
来源：http://yj.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://cg.panjiajie.cn

[T45] Perl：数组遍历
来源：http://ft.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://oy.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://hv.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ja.panjiajie.cn

[T47] Perl：正则捕获
来源：http://sj.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qp.haigaiapp.cn

[T48] Perl：正则替换
来源：http://wt.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://fd.521024.cn

[T49] Perl：函数
来源：http://xt.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gl.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://us.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://am.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://kx.bjjhwx.cn

[T51] Scala：Hello World
来源：http://jg.hnjuh.cn

println("Hello")
来源：http://dc.muxihuayi.cn

[T52] Scala：变量
来源：http://xr.shtwfgs.cn

val a = 1;  var b = 2
来源：http://de.newstarts.cn

[T53] Scala：字符串插值
来源：http://qv.huanxung.cn

s"值: $b"
来源：http://he.szsharing.cn

[T54] Scala：集合映射
来源：http://bh.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://jm.asd995.cn

[T55] Scala：集合过滤
来源：http://fj.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://za.bjjhwx.cn

[T56] Scala：样例类
来源：http://ur.szsharing.cn


<!-- 参考信息 -->