代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://rl.muxihuayi.cn

[R48] awk 取指定列
来源：http://ug.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://dp.shxzukj.cn

[R49] awk 带条件
来源：http://xv.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xo.nicolike.cn

[R50] awk 求和
来源：http://os.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tn.hnjuh.cn

[R51] 排序去重取前几
来源：http://ll.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eb.521024.cn

[R52] 统计行数
来源：http://co.yuexingan06.cn

wc -l a.txt
来源：http://hp.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://nb.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://du.hnjuh.cn

[R54] 比较两个文件
来源：http://tt.colortex.cn

diff a.txt b.txt
来源：http://xg.521024.cn

[R55] 压缩与解压
来源：http://ze.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bh.chemitech.net.cn

[R56] 远程拷贝
来源：http://eg.haigaiapp.cn

scp file user@host:/path/
来源：http://dp.newstarts.cn

[R57] 远程执行命令
来源：http://ky.hahajie.cn

ssh user@host 'uptime'
来源：http://pz.shxzukj.cn

[R58] 下载文件
来源：http://sh.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ds.521024.cn

[R59] 发 POST JSON
来源：http://px.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jl.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://ko.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dj.gzmigu.cn

[R61] 磁盘占用
来源：http://hp.lnxyls.cn

df -h;  du -sh *
来源：http://mq.newstarts.cn

[R62] 找最占空间的文件
来源：http://uu.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://ae.jctech888.com.cn

[R63] 内存与进程
来源：http://ue.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://zx.szsharing.cn

[R64] 结束进程
来源：http://xu.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://xv.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://dx.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rj.szsharing.cn

[R66] 定时任务
来源：http://cv.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://qj.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://nn.bjjhwx.cn

openssl rand -hex 16
来源：http://cn.szsharing.cn

[R68] 计算文件校验值
来源：http://xv.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://el.yuexingan06.cn

[R69] 生成随机密码
来源：http://jb.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://et.haigaiapp.cn

[R70] 时间戳与互转
来源：http://ip.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://ln.wgjwhj.cn

[R71] 日期格式化
来源：http://lm.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dd.shxzskj.cn

[R72] 等待端口就绪
来源：http://ei.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sb.jianghongdianzi.cn

[R73] 分割大日志
来源：http://rt.muxihuayi.cn

split -l 1000 big.log part_
来源：http://bh.bjjhwx.cn

[R74] 批量重命名
来源：http://qp.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ew.nszjky.cn

[R75] 导出环境变量
来源：http://rc.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://er.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://zq.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vw.hahajie.cn

[R77] 读取用户输入
来源：http://yv.szxytkj.cn

read -rp "请输入: " ans
来源：http://pm.huixiangedu.cn

[R78] 交互式菜单
来源：http://im.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oz.chemitech.net.cn

[R79] 解析命令行选项
来源：http://cb.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oq.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://zt.521024.cn

time ./run.sh
来源：http://um.wgjwhj.cn

================================================================================
来源：http://kg.wgjwhj.cn

S. C / C++ 专题
来源：http://uz.haigaiapp.cn

================================================================================
来源：http://vt.hahajie.cn

[S01] C：Hello World
来源：http://ew.colortex.cn

#include <stdio.h>
来源：http://bu.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iz.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://mv.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://tf.shtwfgs.cn

[S03] C：读入整数
来源：http://wc.hnjuh.cn

int x; scanf("%d", &x);
来源：http://hw.huixiangedu.cn

[S04] C：字符串复制
来源：http://hu.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rl.521024.cn

[S05] C：字符串长度
来源：http://bb.szxytkj.cn

strlen(s)
来源：http://xr.szxytkj.cn

[S06] C：字符串比较
来源：http://sk.shxzskj.cn

strcmp(a, b) == 0
来源：http://dv.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://ap.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tr.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://ov.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cm.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://nf.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lf.colortex.cn

[S10] C：指针与解引用
来源：http://br.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://hp.lnxyls.cn

[S11] C：逐行读文件
来源：http://jb.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ca.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jx.hahajie.cn

fclose(f);
来源：http://mr.asd995.cn

[S12] C：写文件
来源：http://ny.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mw.hahajie.cn

[S13] C：宏定义
来源：http://io.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sg.huixinmuqiang.cn

[S14] C：枚举
来源：http://mo.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://pt.panjiajie.cn

[S15] C：类型转换
来源：http://uw.9csxet.cn

(double) a / b
来源：http://kf.jctech888.com.cn

[S16] C：位操作置位
来源：http://cl.gzmigu.cn

x |= (1 << 3);
来源：http://vv.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://pn.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://um.szxytkj.cn

[S18] C：命令行参数
来源：http://ux.haigaiapp.cn

int main(int argc, char **argv)
来源：http://mm.szxytkj.cn

[S19] C：快速排序
来源：http://bq.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wl.hahajie.cn

[S20] C：二分查找
来源：http://zb.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ya.lnxyls.cn

[S21] C：字符类别判断
来源：http://hp.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://en.nicolike.cn

[S22] C：字符串转数字
来源：http://nc.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ao.bjjhwx.cn

[S23] C：随机数
来源：http://sy.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dv.hnjuh.cn

[S24] C：获取本地时间
来源：http://rc.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pu.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://qs.wgjwhj.cn

memcpy(dst, src, n);
来源：http://qg.szxytkj.cn

[S26] C：内存清零
来源：http://gh.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://hj.asd995.cn

[S27] C：定义常量
来源：http://xi.hahajie.cn

const double PI = 3.14159;
来源：http://bz.yuexingan06.cn

[S28] C：静态变量
来源：http://dx.huixinmuqiang.cn

static int counter = 0;
来源：http://ij.huanxung.cn

[S29] C：变参函数
来源：http://sy.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ey.521024.cn

[S30] C：头文件保护
来源：http://bv.colortex.cn

#ifndef X_H
来源：http://kp.szsharing.cn

#define X_H
来源：http://ga.jctech888.com.cn

#endif
来源：http://km.bookmarksfly.cn

[S31] C++：Hello World
来源：http://up.lnxyls.cn

#include <iostream>
来源：http://qb.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ne.huanxung.cn

[S32] C++：字符串
来源：http://zs.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://id.shxzskj.cn

[S33] C++：vector 增删
来源：http://mz.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xz.szsharing.cn

[S34] C++：遍历 vector
来源：http://zn.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://kk.jianghongdianzi.cn

[S35] C++：map
来源：http://qd.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://it.shxzskj.cn

[S36] C++：unordered_map
来源：http://pl.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ni.panjiajie.cn

[S37] C++：set
来源：http://pj.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ge.haigaiapp.cn

[S38] C++：排序
来源：http://kj.521024.cn

std::sort(v.begin(), v.end());
来源：http://mh.asd995.cn

[S39] C++：自定义比较器排序
来源：http://fx.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ze.colortex.cn

[S40] C++：查找元素
来源：http://ys.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cm.nszjky.cn

[S41] C++：类与构造函数
来源：http://el.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://co.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://zp.521024.cn

class B : public Base { public: void f() override {} };
来源：http://hp.szsharing.cn

[S43] C++：智能指针
来源：http://ee.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://xt.yuexingan06.cn

[S44] C++：引用传参
来源：http://zo.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://fq.hahajie.cn

[S45] C++：lambda
来源：http://ua.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xm.szsharing.cn

[S46] C++：函数模板
来源：http://bq.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tu.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://we.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://di.newstarts.cn

[S48] C++：逐行读文件
来源：http://mv.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hj.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://og.haigaiapp.cn

[S49] C++：写文件
来源：http://tw.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dv.jctech888.com.cn

[S50] C++：格式化数字
来源：http://hv.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gj.panjiajie.cn

[S51] C++：显式类型转换
来源：http://gm.huanxung.cn

static_cast<double>(a) / b
来源：http://nh.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://nh.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://ql.jctech888.com.cn

[S53] C++：移动语义
来源：http://ha.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://gb.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://jb.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://st.nszjky.cn

[S55] C++：结构化绑定
来源：http://xe.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pi.haigaiapp.cn

[S56] C++：optional
来源：http://eb.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cn.colortex.cn

[S57] C++：编译期常量
来源：http://ag.jianghongdianzi.cn

constexpr int N = 10;
来源：http://kq.521024.cn

[S58] C++：命名空间
来源：http://he.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://zh.szxytkj.cn

[S59] C++：静态断言
来源：http://oo.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jp.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://hj.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://py.yuexingan06.cn

================================================================================
来源：http://hm.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wb.gzmigu.cn

================================================================================
来源：http://cy.nicolike.cn

[T01] Kotlin：Hello World
来源：http://js.huanxung.cn

println("Hello")
来源：http://ae.panjiajie.cn

[T02] Kotlin：变量
来源：http://to.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://io.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://br.jctech888.com.cn

"值: $b"
来源：http://sw.shxzskj.cn

[T04] Kotlin：空安全
来源：http://cj.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://kj.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://pk.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://px.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://kl.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ik.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://zc.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://md.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://kr.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://ze.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://br.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://ad.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://im.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://de.9csxet.cn

[T11] Kotlin：协程
来源：http://hm.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://db.colortex.cn

[T12] Kotlin：解构声明
来源：http://wp.521024.cn

val (a, b) = Pair(1, 2)
来源：http://gx.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://er.colortex.cn

val m = mapOf("a" to 1)
来源：http://xh.haigaiapp.cn

[T14] Kotlin：循环
来源：http://bu.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://xo.asd995.cn

[T15] Kotlin：接口
来源：http://ow.newstarts.cn

interface Shape { fun area(): Double }
来源：http://sj.huanxung.cn

[T16] Swift：Hello World
来源：http://bh.shtwfgs.cn

print("Hello")
来源：http://ns.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://zn.521024.cn

var a = 1;  let b = 2
来源：http://sm.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://wj.szxytkj.cn

"值: \(b)"
来源：http://fs.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://ku.hnjuh.cn

if let n = opt { print(n) }
来源：http://pc.shtwfgs.cn

[T20] Swift：数组操作
来源：http://yf.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jx.nszjky.cn

[T21] Swift：遍历
来源：http://yi.lnxyls.cn

for x in a { print(x) }
来源：http://dg.bookmarksfly.cn

[T22] Swift：字典
来源：http://bw.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fq.9csxet.cn

[T23] Swift：函数
来源：http://gf.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ym.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://yn.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zu.huanxung.cn

[T25] Swift：结构体
来源：http://me.bjjhwx.cn

struct P { var x: Int }
来源：http://rr.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://wz.shxzukj.cn

class A: Base { override func f() {} }
来源：http://dj.yuexingan06.cn

[T27] Swift：错误处理
来源：http://yt.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://lg.nszjky.cn

[T28] Swift：枚举
来源：http://kh.shtwfgs.cn

enum Color { case red, green }
来源：http://jr.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://iv.huixiangedu.cn

guard let x = opt else { return }
来源：http://qv.wgjwhj.cn

[T30] Swift：协议
来源：http://yv.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://gv.nszjky.cn

[T31] Lua：Hello World
来源：http://xz.newstarts.cn

print("Hello")
来源：http://il.szxytkj.cn

[T32] Lua：局部变量
来源：http://nf.yuntaijiaju.cn

local a = 1
来源：http://gl.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://ji.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://px.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://er.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xf.panjiajie.cn

[T35] Lua：字典表
来源：http://zu.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://nh.szxytkj.cn

[T36] Lua：函数
来源：http://mt.asd995.cn

function add(a, b) return a + b end
来源：http://mu.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://ry.nicolike.cn

"a" .. "b"
来源：http://xs.9csxet.cn

[T38] Lua：条件
来源：http://jz.haigaiapp.cn

if x > 0 then print("正") end
来源：http://ny.gzmigu.cn

[T39] Lua：模式匹配
来源：http://gy.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://bh.hnjuh.cn

[T40] Lua：元表
来源：http://zi.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://nx.huixiangedu.cn

[T41] Perl：Hello World
来源：http://jn.gzmigu.cn

print "Hello\n";
来源：http://wk.huixiangedu.cn

[T42] Perl：变量类型
来源：http://ym.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oi.szxytkj.cn

[T43] Perl：字符串插值
来源：http://lv.shtwfgs.cn

"值: $a"
来源：http://wq.szsharing.cn

[T44] Perl：条件
来源：http://ji.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://if.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://yd.jianghongdianzi.cn

for my $x (@arr) { print $x; }
来源：http://ef.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://ux.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ko.521024.cn

[T47] Perl：正则捕获
来源：http://wh.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ox.colortex.cn

[T48] Perl：正则替换
来源：http://op.nszjky.cn

$s =~ s/old/new/g;
来源：http://im.huixinmuqiang.cn

[T49] Perl：函数
来源：http://ng.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jj.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://go.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qc.nicolike.cn


<!-- 参考信息 -->