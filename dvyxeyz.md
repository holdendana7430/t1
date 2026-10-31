代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://gz.haigaiapp.cn

[R48] awk 取指定列
来源：http://pc.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://yu.bjjhwx.cn

[R49] awk 带条件
来源：http://re.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zg.gzmigu.cn

[R50] awk 求和
来源：http://wv.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vq.jctech888.com.cn

[R51] 排序去重取前几
来源：http://mn.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kd.yuexingan06.cn

[R52] 统计行数
来源：http://yt.huanxung.cn

wc -l a.txt
来源：http://hq.colortex.cn

[R53] 查看文件头与实时尾
来源：http://bw.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jf.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://pg.yuexingan06.cn

diff a.txt b.txt
来源：http://ua.chemitech.net.cn

[R55] 压缩与解压
来源：http://ac.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ls.newstarts.cn

[R56] 远程拷贝
来源：http://mm.521024.cn

scp file user@host:/path/
来源：http://ee.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://bm.haigaiapp.cn

ssh user@host 'uptime'
来源：http://mj.lnxyls.cn

[R58] 下载文件
来源：http://xb.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zk.szxytkj.cn

[R59] 发 POST JSON
来源：http://ol.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xd.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://no.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xv.shtwfgs.cn

[R61] 磁盘占用
来源：http://ew.huanxung.cn

df -h;  du -sh *
来源：http://na.nicolike.cn

[R62] 找最占空间的文件
来源：http://bt.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://rv.haigaiapp.cn

[R63] 内存与进程
来源：http://tn.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://ce.chemitech.net.cn

[R64] 结束进程
来源：http://zx.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://fu.bookmarksfly.cn

[R65] 查看端口占用
来源：http://pf.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mg.chemitech.net.cn

[R66] 定时任务
来源：http://jm.szxytkj.cn

crontab -e;  crontab -l
来源：http://ec.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://nq.shxzukj.cn

openssl rand -hex 16
来源：http://qu.yuexingan06.cn

[R68] 计算文件校验值
来源：http://jv.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tv.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://ir.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://ag.shxzukj.cn

[R70] 时间戳与互转
来源：http://hx.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://se.bjjhwx.cn

[R71] 日期格式化
来源：http://vl.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kh.huanxung.cn

[R72] 等待端口就绪
来源：http://tf.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ng.haigaiapp.cn

[R73] 分割大日志
来源：http://md.muxihuayi.cn

split -l 1000 big.log part_
来源：http://qh.bjjhwx.cn

[R74] 批量重命名
来源：http://as.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mh.bookmarksfly.cn

[R75] 导出环境变量
来源：http://jq.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://zg.newstarts.cn

[R76] 使用临时文件
来源：http://ex.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://va.asd995.cn

[R77] 读取用户输入
来源：http://ob.hnjuh.cn

read -rp "请输入: " ans
来源：http://jw.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://ko.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zl.hahajie.cn

[R79] 解析命令行选项
来源：http://lm.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cf.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://sy.521024.cn

time ./run.sh
来源：http://jw.hahajie.cn

================================================================================
来源：http://ir.szsharing.cn

S. C / C++ 专题
来源：http://ri.newstarts.cn

================================================================================
来源：http://us.haigaiapp.cn

[S01] C：Hello World
来源：http://ba.bookmarksfly.cn

#include <stdio.h>
来源：http://tq.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jo.hahajie.cn

[S02] C：变量与格式化输出
来源：http://dx.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://yj.shxzukj.cn

[S03] C：读入整数
来源：http://et.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://ca.yuexingan06.cn

[S04] C：字符串复制
来源：http://pt.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sw.huanxung.cn

[S05] C：字符串长度
来源：http://kw.panjiajie.cn

strlen(s)
来源：http://ra.521024.cn

[S06] C：字符串比较
来源：http://eh.newstarts.cn

strcmp(a, b) == 0
来源：http://ux.9csxet.cn

[S07] C：数组遍历求和
来源：http://ua.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vu.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://fv.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ed.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://xz.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uk.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://wy.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://rb.521024.cn

[S11] C：逐行读文件
来源：http://un.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://vn.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gm.huixinmuqiang.cn

fclose(f);
来源：http://xu.9csxet.cn

[S12] C：写文件
来源：http://sx.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ei.asd995.cn

[S13] C：宏定义
来源：http://fz.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pi.shxzskj.cn

[S14] C：枚举
来源：http://rt.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://fa.colortex.cn

[S15] C：类型转换
来源：http://fk.hahajie.cn

(double) a / b
来源：http://oy.lnxyls.cn

[S16] C：位操作置位
来源：http://pd.szsharing.cn

x |= (1 << 3);
来源：http://aq.nicolike.cn

[S17] C：安全拼接字符串
来源：http://gs.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kj.shxzukj.cn

[S18] C：命令行参数
来源：http://ii.colortex.cn

int main(int argc, char **argv)
来源：http://fm.chemitech.net.cn

[S19] C：快速排序
来源：http://hs.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yx.521024.cn

[S20] C：二分查找
来源：http://qz.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pl.lnxyls.cn

[S21] C：字符类别判断
来源：http://ub.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zv.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://uj.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://em.chemitech.net.cn

[S23] C：随机数
来源：http://do.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yg.asd995.cn

[S24] C：获取本地时间
来源：http://gl.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xo.panjiajie.cn

[S25] C：内存拷贝
来源：http://in.hnjuh.cn

memcpy(dst, src, n);
来源：http://bh.shxzskj.cn

[S26] C：内存清零
来源：http://bt.hahajie.cn

memset(a, 0, sizeof a);
来源：http://lf.yuntaijiaju.cn

[S27] C：定义常量
来源：http://mj.muxihuayi.cn

const double PI = 3.14159;
来源：http://sj.haigaiapp.cn

[S28] C：静态变量
来源：http://av.haigaiapp.cn

static int counter = 0;
来源：http://zn.wgjwhj.cn

[S29] C：变参函数
来源：http://yv.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qe.wgjwhj.cn

[S30] C：头文件保护
来源：http://dy.shtwfgs.cn

#ifndef X_H
来源：http://ym.bookmarksfly.cn

#define X_H
来源：http://sy.wgjwhj.cn

#endif
来源：http://hg.bookmarksfly.cn

[S31] C++：Hello World
来源：http://bh.panjiajie.cn

#include <iostream>
来源：http://zr.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://tk.shtwfgs.cn

[S32] C++：字符串
来源：http://hl.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://ye.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://ph.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://al.lnxyls.cn

[S34] C++：遍历 vector
来源：http://sa.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://rw.lnxyls.cn

[S35] C++：map
来源：http://kb.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vw.chemitech.net.cn

[S36] C++：unordered_map
来源：http://xx.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ad.huixiangedu.cn

[S37] C++：set
来源：http://zw.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nt.muxihuayi.cn

[S38] C++：排序
来源：http://hu.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://nb.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://pm.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cu.chemitech.net.cn

[S40] C++：查找元素
来源：http://mk.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ce.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://xy.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ud.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://kf.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://oq.yuexingan06.cn

[S43] C++：智能指针
来源：http://vl.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://qs.szsharing.cn

[S44] C++：引用传参
来源：http://ao.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://ts.muxihuayi.cn

[S45] C++：lambda
来源：http://tw.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jt.nszjky.cn

[S46] C++：函数模板
来源：http://or.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://og.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://am.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bl.szxytkj.cn

[S48] C++：逐行读文件
来源：http://kp.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ej.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://ac.shtwfgs.cn

[S49] C++：写文件
来源：http://dj.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cd.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://er.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nr.shxzskj.cn

[S51] C++：显式类型转换
来源：http://vh.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://je.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://ew.huanxung.cn

int size() const noexcept { return n_; }
来源：http://os.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://ea.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://dl.bookmarksfly.cn

[S54] C++：异常处理
来源：http://no.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xf.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://rh.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ud.nicolike.cn

[S56] C++：optional
来源：http://pt.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bz.hnjuh.cn

[S57] C++：编译期常量
来源：http://vm.yuexingan06.cn

constexpr int N = 10;
来源：http://ry.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://im.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://ne.nicolike.cn

[S59] C++：静态断言
来源：http://zh.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ym.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://ye.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tg.wgjwhj.cn

================================================================================
来源：http://sl.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ji.shxzukj.cn

================================================================================
来源：http://sg.nszjky.cn

[T01] Kotlin：Hello World
来源：http://zk.huanxung.cn

println("Hello")
来源：http://ek.shtwfgs.cn

[T02] Kotlin：变量
来源：http://ra.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iy.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://sn.nicolike.cn

"值: $b"
来源：http://yj.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://fn.shxzukj.cn

val n: String? = null;  n?.length
来源：http://ez.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://ut.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tz.nszjky.cn

[T06] Kotlin：集合映射
来源：http://vt.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://io.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://zm.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gr.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://jq.521024.cn

data class User(val name: String, val age: Int)
来源：http://ja.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://hm.colortex.cn

fun String.exclaim() = this + "!"
来源：http://dh.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://ed.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tz.muxihuayi.cn

[T11] Kotlin：协程
来源：http://ti.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://om.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://ge.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://fi.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://rf.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://il.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://rt.newstarts.cn

for (i in 1..10) println(i)
来源：http://bx.nicolike.cn

[T15] Kotlin：接口
来源：http://qv.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://uz.shxzukj.cn

[T16] Swift：Hello World
来源：http://tp.szxytkj.cn

print("Hello")
来源：http://xj.9csxet.cn

[T17] Swift：变量与常量
来源：http://xn.9csxet.cn

var a = 1;  let b = 2
来源：http://qv.gzmigu.cn

[T18] Swift：字符串插值
来源：http://mz.yuntaijiaju.cn

"值: \(b)"
来源：http://ie.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://jd.gzmigu.cn

if let n = opt { print(n) }
来源：http://yg.shxzskj.cn

[T20] Swift：数组操作
来源：http://yn.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wc.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://dk.lnxyls.cn

for x in a { print(x) }
来源：http://ha.shxzskj.cn

[T22] Swift：字典
来源：http://dx.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fe.panjiajie.cn

[T23] Swift：函数
来源：http://vz.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bv.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://tq.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cr.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://qf.asd995.cn

struct P { var x: Int }
来源：http://bc.haigaiapp.cn

[T26] Swift：类与重写
来源：http://sb.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://ab.panjiajie.cn

[T27] Swift：错误处理
来源：http://wp.9csxet.cn

do { try f() } catch { print(error) }
来源：http://dl.haigaiapp.cn

[T28] Swift：枚举
来源：http://sd.asd995.cn

enum Color { case red, green }
来源：http://pz.asd995.cn

[T29] Swift：guard 提前返回
来源：http://yp.wgjwhj.cn

guard let x = opt else { return }
来源：http://gz.hahajie.cn

[T30] Swift：协议
来源：http://ay.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://qv.shxzukj.cn

[T31] Lua：Hello World
来源：http://oa.lnxyls.cn

print("Hello")
来源：http://cf.shtwfgs.cn

[T32] Lua：局部变量
来源：http://he.hahajie.cn

local a = 1
来源：http://hg.hnjuh.cn

[T33] Lua：表（数组）
来源：http://oa.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ya.bjjhwx.cn

[T34] Lua：遍历表
来源：http://ll.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yq.hnjuh.cn

[T35] Lua：字典表
来源：http://he.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://nw.szxytkj.cn

[T36] Lua：函数
来源：http://kq.colortex.cn

function add(a, b) return a + b end
来源：http://ln.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://ye.9csxet.cn

"a" .. "b"
来源：http://mz.wgjwhj.cn

[T38] Lua：条件
来源：http://rk.colortex.cn

if x > 0 then print("正") end
来源：http://wv.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://ho.szxytkj.cn

string.find(s, "%d+")
来源：http://hp.huixiangedu.cn

[T40] Lua：元表
来源：http://uq.9csxet.cn

setmetatable({}, { __index = base })
来源：http://sm.colortex.cn

[T41] Perl：Hello World
来源：http://gu.wgjwhj.cn

print "Hello\n";
来源：http://lx.huixiangedu.cn

[T42] Perl：变量类型
来源：http://gb.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jj.newstarts.cn

[T43] Perl：字符串插值
来源：http://qd.bjjhwx.cn

"值: $a"
来源：http://sz.yuntaijiaju.cn

[T44] Perl：条件
来源：http://su.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://sb.szsharing.cn

[T45] Perl：数组遍历
来源：http://zm.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://gz.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://zk.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uy.gzmigu.cn

[T47] Perl：正则捕获
来源：http://lt.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ni.szxytkj.cn

[T48] Perl：正则替换
来源：http://px.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://qq.shxzskj.cn

[T49] Perl：函数
来源：http://aj.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oa.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://sy.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://og.lnxyls.cn


<!-- 参考信息 -->