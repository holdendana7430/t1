代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ir.hahajie.cn

[R54] 比较两个文件
来源：http://zh.hnjuh.cn

diff a.txt b.txt
来源：http://cs.chemitech.net.cn

[R55] 压缩与解压
来源：http://np.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qw.asd995.cn

[R56] 远程拷贝
来源：http://xb.colortex.cn

scp file user@host:/path/
来源：http://zw.huanxung.cn

[R57] 远程执行命令
来源：http://wf.nicolike.cn

ssh user@host 'uptime'
来源：http://bn.asd995.cn

[R58] 下载文件
来源：http://dw.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qj.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://lb.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pu.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://ia.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wi.hahajie.cn

[R61] 磁盘占用
来源：http://op.yuntaijiaju.cn

df -h;  du -sh *
来源：http://wr.nicolike.cn

[R62] 找最占空间的文件
来源：http://da.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://yl.huanxung.cn

[R63] 内存与进程
来源：http://wu.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://hv.shxzskj.cn

[R64] 结束进程
来源：http://et.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://sw.nicolike.cn

[R65] 查看端口占用
来源：http://br.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tp.huanxung.cn

[R66] 定时任务
来源：http://km.asd995.cn

crontab -e;  crontab -l
来源：http://eg.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://dm.muxihuayi.cn

openssl rand -hex 16
来源：http://ct.asd995.cn

[R68] 计算文件校验值
来源：http://oo.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://do.muxihuayi.cn

[R69] 生成随机密码
来源：http://dk.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://ss.jctech888.com.cn

[R70] 时间戳与互转
来源：http://vk.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://eg.hahajie.cn

[R71] 日期格式化
来源：http://tr.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sb.shtwfgs.cn

[R72] 等待端口就绪
来源：http://ii.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ui.newstarts.cn

[R73] 分割大日志
来源：http://pv.shxzukj.cn

split -l 1000 big.log part_
来源：http://sw.huixiangedu.cn

[R74] 批量重命名
来源：http://vn.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ep.shxzskj.cn

[R75] 导出环境变量
来源：http://gf.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://lr.shtwfgs.cn

[R76] 使用临时文件
来源：http://us.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qo.shxzskj.cn

[R77] 读取用户输入
来源：http://cw.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://xk.chemitech.net.cn

[R78] 交互式菜单
来源：http://rq.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://np.521024.cn

[R79] 解析命令行选项
来源：http://vi.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ty.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://cj.521024.cn

time ./run.sh
来源：http://id.bookmarksfly.cn

================================================================================
来源：http://il.wgjwhj.cn

S. C / C++ 专题
来源：http://ge.huixiangedu.cn

================================================================================
来源：http://ny.yuntaijiaju.cn

[S01] C：Hello World
来源：http://lo.nszjky.cn

#include <stdio.h>
来源：http://ed.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://he.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://ec.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://ma.szsharing.cn

[S03] C：读入整数
来源：http://hl.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://kg.nicolike.cn

[S04] C：字符串复制
来源：http://jc.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qy.nicolike.cn

[S05] C：字符串长度
来源：http://dp.yuexingan06.cn

strlen(s)
来源：http://lo.shxzukj.cn

[S06] C：字符串比较
来源：http://xp.szxytkj.cn

strcmp(a, b) == 0
来源：http://us.newstarts.cn

[S07] C：数组遍历求和
来源：http://id.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oh.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://qg.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yn.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://xw.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vk.shxzukj.cn

[S10] C：指针与解引用
来源：http://oe.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://qh.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://hc.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://vk.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gi.lnxyls.cn

fclose(f);
来源：http://uy.szxytkj.cn

[S12] C：写文件
来源：http://qe.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dv.newstarts.cn

[S13] C：宏定义
来源：http://pt.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jx.shxzukj.cn

[S14] C：枚举
来源：http://sf.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://dx.nicolike.cn

[S15] C：类型转换
来源：http://jg.huixinmuqiang.cn

(double) a / b
来源：http://ti.nicolike.cn

[S16] C：位操作置位
来源：http://bs.yuexingan06.cn

x |= (1 << 3);
来源：http://mc.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://zm.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sm.lnxyls.cn

[S18] C：命令行参数
来源：http://cb.chemitech.net.cn

int main(int argc, char **argv)
来源：http://kq.colortex.cn

[S19] C：快速排序
来源：http://gp.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nj.yuntaijiaju.cn

[S20] C：二分查找
来源：http://hr.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ht.asd995.cn

[S21] C：字符类别判断
来源：http://ue.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tw.hnjuh.cn

[S22] C：字符串转数字
来源：http://uv.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oo.muxihuayi.cn

[S23] C：随机数
来源：http://vn.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jz.nicolike.cn

[S24] C：获取本地时间
来源：http://ul.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zf.huixiangedu.cn

[S25] C：内存拷贝
来源：http://pp.shtwfgs.cn

memcpy(dst, src, n);
来源：http://ob.jctech888.com.cn

[S26] C：内存清零
来源：http://st.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://vl.asd995.cn

[S27] C：定义常量
来源：http://hr.yuexingan06.cn

const double PI = 3.14159;
来源：http://yx.jctech888.com.cn

[S28] C：静态变量
来源：http://jo.jianghongdianzi.cn

static int counter = 0;
来源：http://fx.szxytkj.cn

[S29] C：变参函数
来源：http://ji.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gw.szsharing.cn

[S30] C：头文件保护
来源：http://ht.9csxet.cn

#ifndef X_H
来源：http://vg.jianghongdianzi.cn

#define X_H
来源：http://cn.bjjhwx.cn

#endif
来源：http://af.shtwfgs.cn

[S31] C++：Hello World
来源：http://ul.521024.cn

#include <iostream>
来源：http://jx.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://vc.nszjky.cn

[S32] C++：字符串
来源：http://bb.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://wm.jctech888.com.cn

[S33] C++：vector 增删
来源：http://xc.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qi.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://ol.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://af.lnxyls.cn

[S35] C++：map
来源：http://ak.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ap.muxihuayi.cn

[S36] C++：unordered_map
来源：http://dc.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://am.panjiajie.cn

[S37] C++：set
来源：http://vv.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xe.szxytkj.cn

[S38] C++：排序
来源：http://ca.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://uw.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://rl.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://um.yuexingan06.cn

[S40] C++：查找元素
来源：http://sv.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hj.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://fe.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cb.nicolike.cn

[S42] C++：继承与虚函数
来源：http://ls.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://jx.muxihuayi.cn

[S43] C++：智能指针
来源：http://fl.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://dn.521024.cn

[S44] C++：引用传参
来源：http://ws.colortex.cn

void inc(int &x) { ++x; }
来源：http://hw.yuntaijiaju.cn

[S45] C++：lambda
来源：http://ni.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dp.gzmigu.cn

[S46] C++：函数模板
来源：http://vt.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yk.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://zt.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vl.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://li.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ea.521024.cn

while (std::getline(in, line)) { }
来源：http://px.newstarts.cn

[S49] C++：写文件
来源：http://sr.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mt.hnjuh.cn

[S50] C++：格式化数字
来源：http://tn.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qm.asd995.cn

[S51] C++：显式类型转换
来源：http://zz.colortex.cn

static_cast<double>(a) / b
来源：http://km.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://gs.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://fi.chemitech.net.cn

[S53] C++：移动语义
来源：http://ke.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://ki.gzmigu.cn

[S54] C++：异常处理
来源：http://su.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ul.shxzskj.cn

[S55] C++：结构化绑定
来源：http://mg.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qf.nicolike.cn

[S56] C++：optional
来源：http://on.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://co.wgjwhj.cn

[S57] C++：编译期常量
来源：http://im.521024.cn

constexpr int N = 10;
来源：http://fh.muxihuayi.cn

[S58] C++：命名空间
来源：http://zf.521024.cn

namespace ns { int f() { return 1; } }
来源：http://yi.wgjwhj.cn

[S59] C++：静态断言
来源：http://aj.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pl.521024.cn

[S60] C++：遍历并删除元素
来源：http://yp.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xu.nszjky.cn

================================================================================
来源：http://vg.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tu.chemitech.net.cn

================================================================================
来源：http://mw.521024.cn

[T01] Kotlin：Hello World
来源：http://ie.szxytkj.cn

println("Hello")
来源：http://cw.wgjwhj.cn

[T02] Kotlin：变量
来源：http://xh.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cn.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://ee.newstarts.cn

"值: $b"
来源：http://yu.shxzukj.cn

[T04] Kotlin：空安全
来源：http://ka.521024.cn

val n: String? = null;  n?.length
来源：http://ea.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://th.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ae.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://yz.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ua.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://cw.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ka.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://pj.521024.cn

data class User(val name: String, val age: Int)
来源：http://hk.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://lh.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://gi.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://qy.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fl.shxzukj.cn

[T11] Kotlin：协程
来源：http://yd.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hu.huanxung.cn

[T12] Kotlin：解构声明
来源：http://nv.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://la.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://xy.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://tm.newstarts.cn

[T14] Kotlin：循环
来源：http://pm.521024.cn

for (i in 1..10) println(i)
来源：http://vg.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://xy.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://va.lnxyls.cn

[T16] Swift：Hello World
来源：http://ju.shxzskj.cn

print("Hello")
来源：http://qe.hahajie.cn

[T17] Swift：变量与常量
来源：http://cl.colortex.cn

var a = 1;  let b = 2
来源：http://bg.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://fh.gzmigu.cn

"值: \(b)"
来源：http://lo.newstarts.cn

[T19] Swift：可选绑定
来源：http://hj.shxzskj.cn

if let n = opt { print(n) }
来源：http://eq.9csxet.cn

[T20] Swift：数组操作
来源：http://hh.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nr.nszjky.cn

[T21] Swift：遍历
来源：http://xq.szxytkj.cn

for x in a { print(x) }
来源：http://xu.asd995.cn

[T22] Swift：字典
来源：http://yy.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lc.huixiangedu.cn

[T23] Swift：函数
来源：http://pl.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ni.newstarts.cn

[T24] Swift：闭包
来源：http://wc.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yq.shtwfgs.cn

[T25] Swift：结构体
来源：http://ou.nicolike.cn

struct P { var x: Int }
来源：http://az.newstarts.cn

[T26] Swift：类与重写
来源：http://ws.colortex.cn

class A: Base { override func f() {} }
来源：http://wf.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://ov.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://kw.shtwfgs.cn

[T28] Swift：枚举
来源：http://qh.jianghongdianzi.cn

enum Color { case red, green }
来源：http://zi.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://gj.bjjhwx.cn

guard let x = opt else { return }
来源：http://hb.yuexingan06.cn

[T30] Swift：协议
来源：http://ix.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://qs.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://hg.gzmigu.cn

print("Hello")
来源：http://pr.gzmigu.cn

[T32] Lua：局部变量
来源：http://st.huixiangedu.cn

local a = 1
来源：http://wm.gzmigu.cn

[T33] Lua：表（数组）
来源：http://jh.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xm.chemitech.net.cn

[T34] Lua：遍历表
来源：http://fd.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jq.yuexingan06.cn

[T35] Lua：字典表
来源：http://ee.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://nf.muxihuayi.cn

[T36] Lua：函数
来源：http://dv.shxzukj.cn

function add(a, b) return a + b end
来源：http://qo.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://xl.panjiajie.cn

"a" .. "b"
来源：http://df.haigaiapp.cn

[T38] Lua：条件
来源：http://po.jctech888.com.cn

if x > 0 then print("正") end
来源：http://ef.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://tw.szxytkj.cn

string.find(s, "%d+")
来源：http://lj.huixinmuqiang.cn

[T40] Lua：元表
来源：http://lw.hahajie.cn

setmetatable({}, { __index = base })
来源：http://gt.jctech888.com.cn

[T41] Perl：Hello World
来源：http://mx.jctech888.com.cn

print "Hello\n";
来源：http://on.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://qy.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vd.panjiajie.cn

[T43] Perl：字符串插值
来源：http://zs.szsharing.cn

"值: $a"
来源：http://ch.hnjuh.cn

[T44] Perl：条件
来源：http://oh.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://yw.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://nt.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://nb.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://du.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dm.szsharing.cn

[T47] Perl：正则捕获
来源：http://ie.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dh.9csxet.cn

[T48] Perl：正则替换
来源：http://zj.asd995.cn

$s =~ s/old/new/g;
来源：http://jq.szxytkj.cn

[T49] Perl：函数
来源：http://vq.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ez.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://fk.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dn.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://vy.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://tv.newstarts.cn

println("Hello")
来源：http://gh.asd995.cn

[T52] Scala：变量
来源：http://bj.nicolike.cn

val a = 1;  var b = 2
来源：http://ay.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://ky.panjiajie.cn

s"值: $b"
来源：http://xk.yuexingan06.cn

[T54] Scala：集合映射
来源：http://wo.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://hz.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://wz.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sj.hnjuh.cn

[T56] Scala：样例类
来源：http://lt.wgjwhj.cn


<!-- 参考信息 -->