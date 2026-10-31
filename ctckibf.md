代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ym.gzmigu.cn

[R50] awk 求和
来源：http://nh.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rf.gzmigu.cn

[R51] 排序去重取前几
来源：http://cx.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bt.wgjwhj.cn

[R52] 统计行数
来源：http://vd.huanxung.cn

wc -l a.txt
来源：http://cj.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://oe.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mz.9csxet.cn

[R54] 比较两个文件
来源：http://sm.jianghongdianzi.cn

diff a.txt b.txt
来源：http://ch.shtwfgs.cn

[R55] 压缩与解压
来源：http://rq.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vk.shxzukj.cn

[R56] 远程拷贝
来源：http://xt.szsharing.cn

scp file user@host:/path/
来源：http://mv.lnxyls.cn

[R57] 远程执行命令
来源：http://ez.jctech888.com.cn

ssh user@host 'uptime'
来源：http://uz.hahajie.cn

[R58] 下载文件
来源：http://xf.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zw.muxihuayi.cn

[R59] 发 POST JSON
来源：http://mc.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ou.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://xn.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ya.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://gu.haigaiapp.cn

df -h;  du -sh *
来源：http://bs.panjiajie.cn

[R62] 找最占空间的文件
来源：http://ne.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://xe.shtwfgs.cn

[R63] 内存与进程
来源：http://mp.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://sl.gzmigu.cn

[R64] 结束进程
来源：http://qn.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://ze.yuexingan06.cn

[R65] 查看端口占用
来源：http://uf.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gl.shxzskj.cn

[R66] 定时任务
来源：http://nr.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://hu.hahajie.cn

[R67] 生成随机十六进制串
来源：http://xn.newstarts.cn

openssl rand -hex 16
来源：http://vw.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://nf.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mv.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://ry.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://de.gzmigu.cn

[R70] 时间戳与互转
来源：http://ml.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://lj.huixinmuqiang.cn

[R71] 日期格式化
来源：http://dc.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gl.yuexingan06.cn

[R72] 等待端口就绪
来源：http://uy.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lu.9csxet.cn

[R73] 分割大日志
来源：http://by.chemitech.net.cn

split -l 1000 big.log part_
来源：http://mo.panjiajie.cn

[R74] 批量重命名
来源：http://yw.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://my.muxihuayi.cn

[R75] 导出环境变量
来源：http://fz.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://mw.jctech888.com.cn

[R76] 使用临时文件
来源：http://vt.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ct.huixiangedu.cn

[R77] 读取用户输入
来源：http://my.hnjuh.cn

read -rp "请输入: " ans
来源：http://sz.wgjwhj.cn

[R78] 交互式菜单
来源：http://xe.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uo.panjiajie.cn

[R79] 解析命令行选项
来源：http://kn.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mb.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://lu.bjjhwx.cn

time ./run.sh
来源：http://pu.521024.cn

================================================================================
来源：http://ld.szxytkj.cn

S. C / C++ 专题
来源：http://fl.huanxung.cn

================================================================================
来源：http://wc.9csxet.cn

[S01] C：Hello World
来源：http://jy.bjjhwx.cn

#include <stdio.h>
来源：http://se.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://go.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://jw.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://mc.nszjky.cn

[S03] C：读入整数
来源：http://mk.nicolike.cn

int x; scanf("%d", &x);
来源：http://lv.nszjky.cn

[S04] C：字符串复制
来源：http://wo.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://se.lnxyls.cn

[S05] C：字符串长度
来源：http://sw.huanxung.cn

strlen(s)
来源：http://vw.asd995.cn

[S06] C：字符串比较
来源：http://ba.bjjhwx.cn

strcmp(a, b) == 0
来源：http://mx.panjiajie.cn

[S07] C：数组遍历求和
来源：http://qr.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qd.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://be.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sw.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://zz.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cf.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://jw.newstarts.cn

int *p = &a;  *p = 5;
来源：http://lw.nicolike.cn

[S11] C：逐行读文件
来源：http://wf.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://py.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kv.jctech888.com.cn

fclose(f);
来源：http://yk.huanxung.cn

[S12] C：写文件
来源：http://cw.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rn.muxihuayi.cn

[S13] C：宏定义
来源：http://qx.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://es.chemitech.net.cn

[S14] C：枚举
来源：http://on.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://ml.hahajie.cn

[S15] C：类型转换
来源：http://dz.yuntaijiaju.cn

(double) a / b
来源：http://uv.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://ky.huixiangedu.cn

x |= (1 << 3);
来源：http://xy.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://in.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tf.hnjuh.cn

[S18] C：命令行参数
来源：http://kq.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://nk.wgjwhj.cn

[S19] C：快速排序
来源：http://gm.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pe.lnxyls.cn

[S20] C：二分查找
来源：http://tk.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nq.shxzskj.cn

[S21] C：字符类别判断
来源：http://yn.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qy.shtwfgs.cn

[S22] C：字符串转数字
来源：http://xs.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ck.huixinmuqiang.cn

[S23] C：随机数
来源：http://lo.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fu.chemitech.net.cn

[S24] C：获取本地时间
来源：http://et.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bu.chemitech.net.cn

[S25] C：内存拷贝
来源：http://uw.muxihuayi.cn

memcpy(dst, src, n);
来源：http://xp.shxzskj.cn

[S26] C：内存清零
来源：http://gb.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://wp.huanxung.cn

[S27] C：定义常量
来源：http://wk.lnxyls.cn

const double PI = 3.14159;
来源：http://pg.bjjhwx.cn

[S28] C：静态变量
来源：http://tz.wgjwhj.cn

static int counter = 0;
来源：http://zo.nszjky.cn

[S29] C：变参函数
来源：http://bm.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ti.nszjky.cn

[S30] C：头文件保护
来源：http://kx.colortex.cn

#ifndef X_H
来源：http://xn.gzmigu.cn

#define X_H
来源：http://gh.gzmigu.cn

#endif
来源：http://fx.haigaiapp.cn

[S31] C++：Hello World
来源：http://uy.szxytkj.cn

#include <iostream>
来源：http://ql.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://xl.9csxet.cn

[S32] C++：字符串
来源：http://za.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://bq.newstarts.cn

[S33] C++：vector 增删
来源：http://qu.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lb.hnjuh.cn

[S34] C++：遍历 vector
来源：http://up.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://wb.yuntaijiaju.cn

[S35] C++：map
来源：http://zp.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://be.muxihuayi.cn

[S36] C++：unordered_map
来源：http://py.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yt.huanxung.cn

[S37] C++：set
来源：http://ck.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wm.chemitech.net.cn

[S38] C++：排序
来源：http://lz.521024.cn

std::sort(v.begin(), v.end());
来源：http://sm.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://lx.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vp.wgjwhj.cn

[S40] C++：查找元素
来源：http://gs.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zq.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://km.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ps.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://pi.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://bj.panjiajie.cn

[S43] C++：智能指针
来源：http://qu.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://jn.asd995.cn

[S44] C++：引用传参
来源：http://lv.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://fq.521024.cn

[S45] C++：lambda
来源：http://rd.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dm.colortex.cn

[S46] C++：函数模板
来源：http://zm.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bz.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://et.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fd.colortex.cn

[S48] C++：逐行读文件
来源：http://mp.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ws.nszjky.cn

while (std::getline(in, line)) { }
来源：http://lq.shtwfgs.cn

[S49] C++：写文件
来源：http://be.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sf.bjjhwx.cn

[S50] C++：格式化数字
来源：http://gs.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://my.panjiajie.cn

[S51] C++：显式类型转换
来源：http://hc.szsharing.cn

static_cast<double>(a) / b
来源：http://td.521024.cn

[S52] C++：const 与 noexcept
来源：http://cg.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://gy.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://kd.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://mr.panjiajie.cn

[S54] C++：异常处理
来源：http://ot.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tp.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://js.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zo.jianghongdianzi.cn

[S56] C++：optional
来源：http://qa.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nn.shxzskj.cn

[S57] C++：编译期常量
来源：http://yp.muxihuayi.cn

constexpr int N = 10;
来源：http://xm.nszjky.cn

[S58] C++：命名空间
来源：http://kd.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://qc.huanxung.cn

[S59] C++：静态断言
来源：http://ss.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zh.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://rc.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eg.shtwfgs.cn

================================================================================
来源：http://qq.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vm.hnjuh.cn

================================================================================
来源：http://ho.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://od.haigaiapp.cn

println("Hello")
来源：http://jx.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://ml.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bk.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://hp.bookmarksfly.cn

"值: $b"
来源：http://wx.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://vq.hahajie.cn

val n: String? = null;  n?.length
来源：http://dp.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://ac.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ng.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://nv.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hv.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://kf.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ol.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://zg.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://fk.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://wf.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://qz.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://sa.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ee.wgjwhj.cn

[T11] Kotlin：协程
来源：http://sl.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://le.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://az.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://wl.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://yt.colortex.cn

val m = mapOf("a" to 1)
来源：http://qf.jctech888.com.cn

[T14] Kotlin：循环
来源：http://wc.shxzukj.cn

for (i in 1..10) println(i)
来源：http://oi.hnjuh.cn

[T15] Kotlin：接口
来源：http://mk.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://xu.shtwfgs.cn

[T16] Swift：Hello World
来源：http://gb.yuntaijiaju.cn

print("Hello")
来源：http://mk.szxytkj.cn

[T17] Swift：变量与常量
来源：http://ks.chemitech.net.cn

var a = 1;  let b = 2
来源：http://xu.hnjuh.cn

[T18] Swift：字符串插值
来源：http://is.wgjwhj.cn

"值: \(b)"
来源：http://nc.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://wm.huixiangedu.cn

if let n = opt { print(n) }
来源：http://rs.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://lw.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zd.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://sp.shxzukj.cn

for x in a { print(x) }
来源：http://la.szxytkj.cn

[T22] Swift：字典
来源：http://cf.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fd.haigaiapp.cn

[T23] Swift：函数
来源：http://yl.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ho.hahajie.cn

[T24] Swift：闭包
来源：http://ek.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pm.huanxung.cn

[T25] Swift：结构体
来源：http://na.panjiajie.cn

struct P { var x: Int }
来源：http://dl.shxzskj.cn

[T26] Swift：类与重写
来源：http://uw.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://cy.nszjky.cn

[T27] Swift：错误处理
来源：http://jm.nicolike.cn

do { try f() } catch { print(error) }
来源：http://hj.chemitech.net.cn

[T28] Swift：枚举
来源：http://gj.jctech888.com.cn

enum Color { case red, green }
来源：http://jq.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://ss.521024.cn

guard let x = opt else { return }
来源：http://vr.muxihuayi.cn

[T30] Swift：协议
来源：http://nr.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://an.szsharing.cn

[T31] Lua：Hello World
来源：http://qj.hnjuh.cn

print("Hello")
来源：http://cd.hahajie.cn

[T32] Lua：局部变量
来源：http://gh.jctech888.com.cn

local a = 1
来源：http://gc.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://kj.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://st.muxihuayi.cn

[T34] Lua：遍历表
来源：http://jr.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qm.newstarts.cn

[T35] Lua：字典表
来源：http://ub.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://oy.nszjky.cn

[T36] Lua：函数
来源：http://ap.nszjky.cn

function add(a, b) return a + b end
来源：http://cp.nicolike.cn

[T37] Lua：字符串拼接
来源：http://wn.shxzskj.cn

"a" .. "b"
来源：http://on.521024.cn

[T38] Lua：条件
来源：http://zu.newstarts.cn

if x > 0 then print("正") end
来源：http://ov.asd995.cn

[T39] Lua：模式匹配
来源：http://xt.521024.cn

string.find(s, "%d+")
来源：http://hx.yuntaijiaju.cn

[T40] Lua：元表
来源：http://ya.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://bz.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://lu.szsharing.cn

print "Hello\n";
来源：http://wl.szxytkj.cn

[T42] Perl：变量类型
来源：http://tm.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://br.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://bh.asd995.cn

"值: $a"
来源：http://ng.yuntaijiaju.cn

[T44] Perl：条件
来源：http://ih.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://ly.nicolike.cn

[T45] Perl：数组遍历
来源：http://tu.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://zv.panjiajie.cn

[T46] Perl：哈希操作
来源：http://ru.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ui.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://il.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dj.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://ta.szsharing.cn

$s =~ s/old/new/g;
来源：http://it.huixinmuqiang.cn

[T49] Perl：函数
来源：http://mu.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ru.nszjky.cn

[T50] Perl：逐行读文件
来源：http://mr.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hb.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://dh.panjiajie.cn

[T51] Scala：Hello World
来源：http://vh.jianghongdianzi.cn

println("Hello")
来源：http://pq.huixiangedu.cn

[T52] Scala：变量
来源：http://nc.muxihuayi.cn


<!-- 参考信息 -->