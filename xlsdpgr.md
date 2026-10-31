代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://ly.huixiangedu.cn

[R52] 统计行数
来源：http://by.chemitech.net.cn

wc -l a.txt
来源：http://lo.521024.cn

[R53] 查看文件头与实时尾
来源：http://ku.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tu.nszjky.cn

[R54] 比较两个文件
来源：http://vn.shxzukj.cn

diff a.txt b.txt
来源：http://eh.lnxyls.cn

[R55] 压缩与解压
来源：http://yo.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sx.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://xp.yuntaijiaju.cn

scp file user@host:/path/
来源：http://jm.colortex.cn

[R57] 远程执行命令
来源：http://ct.szsharing.cn

ssh user@host 'uptime'
来源：http://cq.szxytkj.cn

[R58] 下载文件
来源：http://cx.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ky.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://si.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zv.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://bw.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ew.lnxyls.cn

[R61] 磁盘占用
来源：http://ea.hnjuh.cn

df -h;  du -sh *
来源：http://mz.shxzukj.cn

[R62] 找最占空间的文件
来源：http://sf.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://ej.yuexingan06.cn

[R63] 内存与进程
来源：http://zd.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://ab.shtwfgs.cn

[R64] 结束进程
来源：http://tr.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://lq.wgjwhj.cn

[R65] 查看端口占用
来源：http://ex.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rm.jianghongdianzi.cn

[R66] 定时任务
来源：http://xk.szsharing.cn

crontab -e;  crontab -l
来源：http://xs.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://ef.yuntaijiaju.cn

openssl rand -hex 16
来源：http://od.huixiangedu.cn

[R68] 计算文件校验值
来源：http://gf.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gf.yuexingan06.cn

[R69] 生成随机密码
来源：http://ie.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://rb.shxzskj.cn

[R70] 时间戳与互转
来源：http://bd.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://fv.huanxung.cn

[R71] 日期格式化
来源：http://sf.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mu.yuexingan06.cn

[R72] 等待端口就绪
来源：http://jm.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ao.shxzukj.cn

[R73] 分割大日志
来源：http://uz.newstarts.cn

split -l 1000 big.log part_
来源：http://us.huanxung.cn

[R74] 批量重命名
来源：http://ef.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cl.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://sj.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://uy.521024.cn

[R76] 使用临时文件
来源：http://lf.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kd.521024.cn

[R77] 读取用户输入
来源：http://sg.yuexingan06.cn

read -rp "请输入: " ans
来源：http://br.nszjky.cn

[R78] 交互式菜单
来源：http://jh.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nc.chemitech.net.cn

[R79] 解析命令行选项
来源：http://bs.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bg.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://xv.muxihuayi.cn

time ./run.sh
来源：http://jf.colortex.cn

================================================================================
来源：http://gm.bookmarksfly.cn

S. C / C++ 专题
来源：http://sd.bjjhwx.cn

================================================================================
来源：http://bg.colortex.cn

[S01] C：Hello World
来源：http://rf.521024.cn

#include <stdio.h>
来源：http://bq.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zy.huanxung.cn

[S02] C：变量与格式化输出
来源：http://cs.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://tb.nszjky.cn

[S03] C：读入整数
来源：http://pr.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://aw.shtwfgs.cn

[S04] C：字符串复制
来源：http://co.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ja.lnxyls.cn

[S05] C：字符串长度
来源：http://op.panjiajie.cn

strlen(s)
来源：http://hy.colortex.cn

[S06] C：字符串比较
来源：http://qe.jctech888.com.cn

strcmp(a, b) == 0
来源：http://gn.huanxung.cn

[S07] C：数组遍历求和
来源：http://uk.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wp.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://di.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pr.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://vy.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mi.huanxung.cn

[S10] C：指针与解引用
来源：http://pf.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://cd.chemitech.net.cn

[S11] C：逐行读文件
来源：http://co.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://gg.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nd.bjjhwx.cn

fclose(f);
来源：http://tp.9csxet.cn

[S12] C：写文件
来源：http://ka.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://us.nicolike.cn

[S13] C：宏定义
来源：http://og.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yf.colortex.cn

[S14] C：枚举
来源：http://pf.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://mb.jianghongdianzi.cn

[S15] C：类型转换
来源：http://zm.bookmarksfly.cn

(double) a / b
来源：http://pp.wgjwhj.cn

[S16] C：位操作置位
来源：http://fb.nszjky.cn

x |= (1 << 3);
来源：http://mz.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://uv.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bs.jctech888.com.cn

[S18] C：命令行参数
来源：http://pm.panjiajie.cn

int main(int argc, char **argv)
来源：http://en.asd995.cn

[S19] C：快速排序
来源：http://xg.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kr.szsharing.cn

[S20] C：二分查找
来源：http://rq.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ne.lnxyls.cn

[S21] C：字符类别判断
来源：http://kd.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bs.521024.cn

[S22] C：字符串转数字
来源：http://nm.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://aq.colortex.cn

[S23] C：随机数
来源：http://ze.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kc.chemitech.net.cn

[S24] C：获取本地时间
来源：http://yk.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ar.521024.cn

[S25] C：内存拷贝
来源：http://rf.gzmigu.cn

memcpy(dst, src, n);
来源：http://kf.hnjuh.cn

[S26] C：内存清零
来源：http://kp.colortex.cn

memset(a, 0, sizeof a);
来源：http://ow.lnxyls.cn

[S27] C：定义常量
来源：http://et.bjjhwx.cn

const double PI = 3.14159;
来源：http://ex.gzmigu.cn

[S28] C：静态变量
来源：http://bc.jianghongdianzi.cn

static int counter = 0;
来源：http://rk.yuexingan06.cn

[S29] C：变参函数
来源：http://cg.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ym.szsharing.cn

[S30] C：头文件保护
来源：http://ey.haigaiapp.cn

#ifndef X_H
来源：http://rl.shtwfgs.cn

#define X_H
来源：http://za.nicolike.cn

#endif
来源：http://nn.chemitech.net.cn

[S31] C++：Hello World
来源：http://jb.jctech888.com.cn

#include <iostream>
来源：http://yv.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://pm.shxzskj.cn

[S32] C++：字符串
来源：http://ky.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://wg.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://bb.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pd.colortex.cn

[S34] C++：遍历 vector
来源：http://mn.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://ht.bookmarksfly.cn

[S35] C++：map
来源：http://sp.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sw.lnxyls.cn

[S36] C++：unordered_map
来源：http://cm.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uz.huixinmuqiang.cn

[S37] C++：set
来源：http://qj.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qg.shxzskj.cn

[S38] C++：排序
来源：http://he.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://tt.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://sq.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://by.shxzukj.cn

[S40] C++：查找元素
来源：http://gd.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jt.hahajie.cn

[S41] C++：类与构造函数
来源：http://jz.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ex.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://ad.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://vu.hnjuh.cn

[S43] C++：智能指针
来源：http://gk.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://ja.asd995.cn

[S44] C++：引用传参
来源：http://zo.521024.cn

void inc(int &x) { ++x; }
来源：http://hn.521024.cn

[S45] C++：lambda
来源：http://kt.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kr.shtwfgs.cn

[S46] C++：函数模板
来源：http://ma.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sq.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://yn.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://my.colortex.cn

[S48] C++：逐行读文件
来源：http://kq.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wl.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://ly.yuntaijiaju.cn

[S49] C++：写文件
来源：http://gw.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jb.newstarts.cn

[S50] C++：格式化数字
来源：http://rg.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cx.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://uv.asd995.cn

static_cast<double>(a) / b
来源：http://vy.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://if.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://ne.yuexingan06.cn

[S53] C++：移动语义
来源：http://kf.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://zn.shxzukj.cn

[S54] C++：异常处理
来源：http://ky.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ta.newstarts.cn

[S55] C++：结构化绑定
来源：http://xx.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vc.haigaiapp.cn

[S56] C++：optional
来源：http://kr.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rq.newstarts.cn

[S57] C++：编译期常量
来源：http://to.szxytkj.cn

constexpr int N = 10;
来源：http://se.9csxet.cn

[S58] C++：命名空间
来源：http://sd.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://ts.newstarts.cn

[S59] C++：静态断言
来源：http://xb.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bp.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://ku.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://il.hnjuh.cn

================================================================================
来源：http://xw.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://un.jctech888.com.cn

================================================================================
来源：http://ib.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://lh.haigaiapp.cn

println("Hello")
来源：http://si.gzmigu.cn

[T02] Kotlin：变量
来源：http://kn.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rm.521024.cn

[T03] Kotlin：字符串模板
来源：http://fs.panjiajie.cn

"值: $b"
来源：http://wg.szsharing.cn

[T04] Kotlin：空安全
来源：http://zk.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://zi.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://mi.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gy.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://yl.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vg.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://po.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ti.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://oi.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://jl.colortex.cn

[T09] Kotlin：扩展函数
来源：http://fe.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://ut.colortex.cn

[T10] Kotlin：默认参数
来源：http://ih.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://li.szsharing.cn

[T11] Kotlin：协程
来源：http://mf.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zq.asd995.cn

[T12] Kotlin：解构声明
来源：http://em.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://bx.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://jg.521024.cn

val m = mapOf("a" to 1)
来源：http://eu.hnjuh.cn

[T14] Kotlin：循环
来源：http://qf.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://ew.haigaiapp.cn

[T15] Kotlin：接口
来源：http://tt.huanxung.cn

interface Shape { fun area(): Double }
来源：http://mx.asd995.cn

[T16] Swift：Hello World
来源：http://dn.asd995.cn

print("Hello")
来源：http://is.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://yo.szsharing.cn

var a = 1;  let b = 2
来源：http://rn.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://fj.jianghongdianzi.cn

"值: \(b)"
来源：http://ni.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://eq.panjiajie.cn

if let n = opt { print(n) }
来源：http://az.newstarts.cn

[T20] Swift：数组操作
来源：http://yy.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xp.muxihuayi.cn

[T21] Swift：遍历
来源：http://dz.szxytkj.cn

for x in a { print(x) }
来源：http://vs.9csxet.cn

[T22] Swift：字典
来源：http://up.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ri.bookmarksfly.cn

[T23] Swift：函数
来源：http://nl.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zt.shxzskj.cn

[T24] Swift：闭包
来源：http://nt.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ln.shtwfgs.cn

[T25] Swift：结构体
来源：http://og.chemitech.net.cn

struct P { var x: Int }
来源：http://ei.colortex.cn

[T26] Swift：类与重写
来源：http://bl.hnjuh.cn

class A: Base { override func f() {} }
来源：http://rc.szsharing.cn

[T27] Swift：错误处理
来源：http://dh.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://zw.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://mv.bookmarksfly.cn

enum Color { case red, green }
来源：http://ot.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://jn.bookmarksfly.cn

guard let x = opt else { return }
来源：http://qs.panjiajie.cn

[T30] Swift：协议
来源：http://dv.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://ip.shxzukj.cn

[T31] Lua：Hello World
来源：http://rt.huixinmuqiang.cn

print("Hello")
来源：http://ps.gzmigu.cn

[T32] Lua：局部变量
来源：http://ii.bookmarksfly.cn

local a = 1
来源：http://vj.newstarts.cn

[T33] Lua：表（数组）
来源：http://cl.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ck.chemitech.net.cn

[T34] Lua：遍历表
来源：http://pl.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ft.shtwfgs.cn

[T35] Lua：字典表
来源：http://jz.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://rs.lnxyls.cn

[T36] Lua：函数
来源：http://pg.nszjky.cn

function add(a, b) return a + b end
来源：http://pm.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://bu.huixinmuqiang.cn

"a" .. "b"
来源：http://cu.newstarts.cn

[T38] Lua：条件
来源：http://ch.9csxet.cn

if x > 0 then print("正") end
来源：http://wj.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://ev.newstarts.cn

string.find(s, "%d+")
来源：http://nw.wgjwhj.cn

[T40] Lua：元表
来源：http://pl.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://mp.szsharing.cn

[T41] Perl：Hello World
来源：http://sc.jctech888.com.cn

print "Hello\n";
来源：http://gk.hnjuh.cn

[T42] Perl：变量类型
来源：http://wr.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bn.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://ak.hnjuh.cn

"值: $a"
来源：http://zs.hnjuh.cn

[T44] Perl：条件
来源：http://qu.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://wu.asd995.cn

[T45] Perl：数组遍历
来源：http://kt.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://yk.nicolike.cn

[T46] Perl：哈希操作
来源：http://nv.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nh.shxzskj.cn

[T47] Perl：正则捕获
来源：http://vf.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qf.huixiangedu.cn

[T48] Perl：正则替换
来源：http://xn.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://nt.9csxet.cn

[T49] Perl：函数
来源：http://hv.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ry.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://jr.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ct.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://gg.gzmigu.cn

[T51] Scala：Hello World
来源：http://ez.shxzukj.cn

println("Hello")
来源：http://yg.gzmigu.cn

[T52] Scala：变量
来源：http://om.szxytkj.cn

val a = 1;  var b = 2
来源：http://pa.521024.cn

[T53] Scala：字符串插值
来源：http://wp.newstarts.cn

s"值: $b"
来源：http://ua.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://kr.muxihuayi.cn


<!-- 参考信息 -->