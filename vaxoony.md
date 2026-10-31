代发 wailian999

find . -name "*.tmp" -delete
来源：http://go.gzmigu.cn

[R46] 递归替换文件内容
来源：http://on.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ia.hahajie.cn

[R47] sed 单行替换
来源：http://jp.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ty.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://di.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://jf.szxytkj.cn

[R49] awk 带条件
来源：http://bu.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lr.panjiajie.cn

[R50] awk 求和
来源：http://bg.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ry.huixiangedu.cn

[R51] 排序去重取前几
来源：http://su.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jl.chemitech.net.cn

[R52] 统计行数
来源：http://kn.panjiajie.cn

wc -l a.txt
来源：http://rp.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://yp.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dh.wgjwhj.cn

[R54] 比较两个文件
来源：http://mr.nszjky.cn

diff a.txt b.txt
来源：http://sc.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://ga.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nl.szsharing.cn

[R56] 远程拷贝
来源：http://ob.muxihuayi.cn

scp file user@host:/path/
来源：http://hm.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://wg.hnjuh.cn

ssh user@host 'uptime'
来源：http://zu.asd995.cn

[R58] 下载文件
来源：http://bb.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iz.shtwfgs.cn

[R59] 发 POST JSON
来源：http://oe.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uj.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://au.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oo.asd995.cn

[R61] 磁盘占用
来源：http://nr.szsharing.cn

df -h;  du -sh *
来源：http://jj.hahajie.cn

[R62] 找最占空间的文件
来源：http://ha.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://yn.szsharing.cn

[R63] 内存与进程
来源：http://gb.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://wi.muxihuayi.cn

[R64] 结束进程
来源：http://xt.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://wd.colortex.cn

[R65] 查看端口占用
来源：http://sf.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qn.521024.cn

[R66] 定时任务
来源：http://zg.yuexingan06.cn

crontab -e;  crontab -l
来源：http://fy.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://ue.jctech888.com.cn

openssl rand -hex 16
来源：http://rf.yuexingan06.cn

[R68] 计算文件校验值
来源：http://jv.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vz.shxzskj.cn

[R69] 生成随机密码
来源：http://nl.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://gs.chemitech.net.cn

[R70] 时间戳与互转
来源：http://xm.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://io.yuexingan06.cn

[R71] 日期格式化
来源：http://we.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qj.nszjky.cn

[R72] 等待端口就绪
来源：http://bw.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sm.jctech888.com.cn

[R73] 分割大日志
来源：http://fn.newstarts.cn

split -l 1000 big.log part_
来源：http://ig.szsharing.cn

[R74] 批量重命名
来源：http://pd.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gi.shxzukj.cn

[R75] 导出环境变量
来源：http://jl.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://mz.gzmigu.cn

[R76] 使用临时文件
来源：http://rc.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xf.bookmarksfly.cn

[R77] 读取用户输入
来源：http://by.shtwfgs.cn

read -rp "请输入: " ans
来源：http://ar.asd995.cn

[R78] 交互式菜单
来源：http://sn.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pa.shxzukj.cn

[R79] 解析命令行选项
来源：http://qh.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bw.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://nk.nszjky.cn

time ./run.sh
来源：http://gj.newstarts.cn

================================================================================
来源：http://ky.521024.cn

S. C / C++ 专题
来源：http://xg.wgjwhj.cn

================================================================================
来源：http://iq.jctech888.com.cn

[S01] C：Hello World
来源：http://ug.9csxet.cn

#include <stdio.h>
来源：http://tu.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nh.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://xf.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://af.521024.cn

[S03] C：读入整数
来源：http://wa.nszjky.cn

int x; scanf("%d", &x);
来源：http://nu.asd995.cn

[S04] C：字符串复制
来源：http://li.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kx.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://jj.panjiajie.cn

strlen(s)
来源：http://gk.bookmarksfly.cn

[S06] C：字符串比较
来源：http://hx.asd995.cn

strcmp(a, b) == 0
来源：http://ba.colortex.cn

[S07] C：数组遍历求和
来源：http://bn.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lo.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://im.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sj.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://gs.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lo.hahajie.cn

[S10] C：指针与解引用
来源：http://pl.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://ha.asd995.cn

[S11] C：逐行读文件
来源：http://dh.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://le.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mx.hnjuh.cn

fclose(f);
来源：http://kf.lnxyls.cn

[S12] C：写文件
来源：http://th.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://je.shxzukj.cn

[S13] C：宏定义
来源：http://hb.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dl.huixinmuqiang.cn

[S14] C：枚举
来源：http://hb.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://nj.yuexingan06.cn

[S15] C：类型转换
来源：http://ps.lnxyls.cn

(double) a / b
来源：http://tv.hahajie.cn

[S16] C：位操作置位
来源：http://mw.colortex.cn

x |= (1 << 3);
来源：http://ck.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://ja.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oj.bjjhwx.cn

[S18] C：命令行参数
来源：http://nn.shtwfgs.cn

int main(int argc, char **argv)
来源：http://cf.muxihuayi.cn

[S19] C：快速排序
来源：http://hq.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pt.hahajie.cn

[S20] C：二分查找
来源：http://zw.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nw.shtwfgs.cn

[S21] C：字符类别判断
来源：http://ll.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ju.bjjhwx.cn

[S22] C：字符串转数字
来源：http://mo.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://be.huixinmuqiang.cn

[S23] C：随机数
来源：http://rr.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xs.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://xk.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hk.hnjuh.cn

[S25] C：内存拷贝
来源：http://ta.nszjky.cn

memcpy(dst, src, n);
来源：http://jp.9csxet.cn

[S26] C：内存清零
来源：http://dw.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://qs.wgjwhj.cn

[S27] C：定义常量
来源：http://nd.szsharing.cn

const double PI = 3.14159;
来源：http://bn.hnjuh.cn

[S28] C：静态变量
来源：http://jv.chemitech.net.cn

static int counter = 0;
来源：http://dw.lnxyls.cn

[S29] C：变参函数
来源：http://pq.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gl.yuexingan06.cn

[S30] C：头文件保护
来源：http://ac.jctech888.com.cn

#ifndef X_H
来源：http://gl.shxzukj.cn

#define X_H
来源：http://pg.lnxyls.cn

#endif
来源：http://bv.chemitech.net.cn

[S31] C++：Hello World
来源：http://zk.newstarts.cn

#include <iostream>
来源：http://fy.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://on.lnxyls.cn

[S32] C++：字符串
来源：http://yb.colortex.cn

std::string s = "hi";  s += "!";
来源：http://dp.szsharing.cn

[S33] C++：vector 增删
来源：http://mz.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kz.hnjuh.cn

[S34] C++：遍历 vector
来源：http://ra.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://as.shxzskj.cn

[S35] C++：map
来源：http://bb.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://av.chemitech.net.cn

[S36] C++：unordered_map
来源：http://po.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gf.muxihuayi.cn

[S37] C++：set
来源：http://cy.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fq.shxzukj.cn

[S38] C++：排序
来源：http://hs.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://sr.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://xs.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ar.szsharing.cn

[S40] C++：查找元素
来源：http://fs.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rp.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://zq.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mk.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://vg.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://is.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://zm.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://ba.szsharing.cn

[S44] C++：引用传参
来源：http://bn.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://wp.shxzskj.cn

[S45] C++：lambda
来源：http://nw.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wc.nszjky.cn

[S46] C++：函数模板
来源：http://ed.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ho.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://cs.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://od.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://ik.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rq.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://yn.szsharing.cn

[S49] C++：写文件
来源：http://lp.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dv.asd995.cn

[S50] C++：格式化数字
来源：http://qj.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nl.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://zo.hnjuh.cn

static_cast<double>(a) / b
来源：http://li.colortex.cn

[S52] C++：const 与 noexcept
来源：http://uw.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://jv.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://la.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://ou.bookmarksfly.cn

[S54] C++：异常处理
来源：http://to.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xo.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://pm.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ww.szxytkj.cn

[S56] C++：optional
来源：http://gt.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ti.chemitech.net.cn

[S57] C++：编译期常量
来源：http://rm.asd995.cn

constexpr int N = 10;
来源：http://vl.szxytkj.cn

[S58] C++：命名空间
来源：http://ts.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://sf.haigaiapp.cn

[S59] C++：静态断言
来源：http://vt.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sb.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://cu.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lz.9csxet.cn

================================================================================
来源：http://nl.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ns.521024.cn

================================================================================
来源：http://rl.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://eq.huixinmuqiang.cn

println("Hello")
来源：http://tq.szsharing.cn

[T02] Kotlin：变量
来源：http://pv.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sk.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://ug.muxihuayi.cn

"值: $b"
来源：http://go.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://rh.gzmigu.cn

val n: String? = null;  n?.length
来源：http://ig.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://fa.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ev.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://gl.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kc.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://po.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ed.shxzskj.cn

[T08] Kotlin：数据类
来源：http://ae.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://ek.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://li.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://pu.nicolike.cn

[T10] Kotlin：默认参数
来源：http://ex.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nl.hahajie.cn

[T11] Kotlin：协程
来源：http://ni.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jl.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://hq.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://dz.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://mn.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://ur.bjjhwx.cn

[T14] Kotlin：循环
来源：http://es.szsharing.cn

for (i in 1..10) println(i)
来源：http://hs.lnxyls.cn

[T15] Kotlin：接口
来源：http://sf.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://kl.shtwfgs.cn

[T16] Swift：Hello World
来源：http://fy.bjjhwx.cn

print("Hello")
来源：http://ny.colortex.cn

[T17] Swift：变量与常量
来源：http://wp.szxytkj.cn

var a = 1;  let b = 2
来源：http://yk.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://ym.shtwfgs.cn

"值: \(b)"
来源：http://wc.newstarts.cn

[T19] Swift：可选绑定
来源：http://dm.panjiajie.cn

if let n = opt { print(n) }
来源：http://nc.szxytkj.cn

[T20] Swift：数组操作
来源：http://xe.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ga.szxytkj.cn

[T21] Swift：遍历
来源：http://gt.lnxyls.cn

for x in a { print(x) }
来源：http://in.bookmarksfly.cn

[T22] Swift：字典
来源：http://yw.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ls.bjjhwx.cn

[T23] Swift：函数
来源：http://sb.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yg.shxzskj.cn

[T24] Swift：闭包
来源：http://cb.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dc.newstarts.cn

[T25] Swift：结构体
来源：http://hj.szsharing.cn

struct P { var x: Int }
来源：http://cn.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://rt.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://oy.gzmigu.cn

[T27] Swift：错误处理
来源：http://tv.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://hb.shxzukj.cn

[T28] Swift：枚举
来源：http://bj.asd995.cn

enum Color { case red, green }
来源：http://fi.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://dp.9csxet.cn

guard let x = opt else { return }
来源：http://cq.huixiangedu.cn

[T30] Swift：协议
来源：http://ol.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://bz.nszjky.cn

[T31] Lua：Hello World
来源：http://xi.bjjhwx.cn

print("Hello")
来源：http://aq.panjiajie.cn

[T32] Lua：局部变量
来源：http://sz.hnjuh.cn

local a = 1
来源：http://lg.521024.cn

[T33] Lua：表（数组）
来源：http://cq.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sh.panjiajie.cn

[T34] Lua：遍历表
来源：http://oi.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sr.newstarts.cn

[T35] Lua：字典表
来源：http://gl.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://tl.nszjky.cn

[T36] Lua：函数
来源：http://uj.panjiajie.cn

function add(a, b) return a + b end
来源：http://zy.colortex.cn

[T37] Lua：字符串拼接
来源：http://gt.bjjhwx.cn

"a" .. "b"
来源：http://tn.yuntaijiaju.cn

[T38] Lua：条件
来源：http://am.newstarts.cn

if x > 0 then print("正") end
来源：http://oi.colortex.cn

[T39] Lua：模式匹配
来源：http://kz.shxzskj.cn

string.find(s, "%d+")
来源：http://xk.yuexingan06.cn

[T40] Lua：元表
来源：http://ej.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://nl.colortex.cn

[T41] Perl：Hello World
来源：http://lp.yuntaijiaju.cn

print "Hello\n";
来源：http://db.yuexingan06.cn

[T42] Perl：变量类型
来源：http://ao.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uk.shxzukj.cn

[T43] Perl：字符串插值
来源：http://sa.shxzskj.cn

"值: $a"
来源：http://nx.colortex.cn

[T44] Perl：条件
来源：http://vb.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://yq.szsharing.cn

[T45] Perl：数组遍历
来源：http://eb.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://ee.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://zd.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ik.newstarts.cn

[T47] Perl：正则捕获
来源：http://pu.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gz.wgjwhj.cn

[T48] Perl：正则替换
来源：http://wv.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://oy.jianghongdianzi.cn


<!-- 参考信息 -->