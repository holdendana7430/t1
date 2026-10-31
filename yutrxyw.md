代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xo.hahajie.cn

[R50] awk 求和
来源：http://wf.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vf.huixiangedu.cn

[R51] 排序去重取前几
来源：http://of.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jx.shxzskj.cn

[R52] 统计行数
来源：http://zb.gzmigu.cn

wc -l a.txt
来源：http://zb.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://fr.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ti.shxzukj.cn

[R54] 比较两个文件
来源：http://dl.9csxet.cn

diff a.txt b.txt
来源：http://lq.shxzskj.cn

[R55] 压缩与解压
来源：http://fy.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yw.huixiangedu.cn

[R56] 远程拷贝
来源：http://hb.hahajie.cn

scp file user@host:/path/
来源：http://vs.jctech888.com.cn

[R57] 远程执行命令
来源：http://pl.shxzukj.cn

ssh user@host 'uptime'
来源：http://yc.huanxung.cn

[R58] 下载文件
来源：http://ca.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dx.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://dd.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gm.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://yp.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kc.shxzukj.cn

[R61] 磁盘占用
来源：http://il.shxzskj.cn

df -h;  du -sh *
来源：http://zh.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://oz.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://rb.haigaiapp.cn

[R63] 内存与进程
来源：http://vm.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://dj.521024.cn

[R64] 结束进程
来源：http://eh.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://cv.bookmarksfly.cn

[R65] 查看端口占用
来源：http://mo.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ta.521024.cn

[R66] 定时任务
来源：http://dj.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://if.521024.cn

[R67] 生成随机十六进制串
来源：http://mc.huixiangedu.cn

openssl rand -hex 16
来源：http://uf.lnxyls.cn

[R68] 计算文件校验值
来源：http://pg.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dm.chemitech.net.cn

[R69] 生成随机密码
来源：http://pe.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://ns.muxihuayi.cn

[R70] 时间戳与互转
来源：http://we.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://jl.yuntaijiaju.cn

[R71] 日期格式化
来源：http://ci.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ir.bjjhwx.cn

[R72] 等待端口就绪
来源：http://rv.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ka.colortex.cn

[R73] 分割大日志
来源：http://jd.szxytkj.cn

split -l 1000 big.log part_
来源：http://fy.9csxet.cn

[R74] 批量重命名
来源：http://sw.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eo.szxytkj.cn

[R75] 导出环境变量
来源：http://dk.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://mq.haigaiapp.cn

[R76] 使用临时文件
来源：http://sx.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cw.huanxung.cn

[R77] 读取用户输入
来源：http://oq.yuexingan06.cn

read -rp "请输入: " ans
来源：http://dw.9csxet.cn

[R78] 交互式菜单
来源：http://ai.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mi.panjiajie.cn

[R79] 解析命令行选项
来源：http://fk.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pd.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://ea.muxihuayi.cn

time ./run.sh
来源：http://nl.newstarts.cn

================================================================================
来源：http://kf.jianghongdianzi.cn

S. C / C++ 专题
来源：http://cc.colortex.cn

================================================================================
来源：http://sv.szxytkj.cn

[S01] C：Hello World
来源：http://mp.gzmigu.cn

#include <stdio.h>
来源：http://vr.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wm.szsharing.cn

[S02] C：变量与格式化输出
来源：http://vi.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://zf.jctech888.com.cn

[S03] C：读入整数
来源：http://mq.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://kc.jctech888.com.cn

[S04] C：字符串复制
来源：http://hh.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jd.9csxet.cn

[S05] C：字符串长度
来源：http://ln.lnxyls.cn

strlen(s)
来源：http://xu.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://fd.colortex.cn

strcmp(a, b) == 0
来源：http://eq.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://ht.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bu.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://yy.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://so.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://xl.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rs.shtwfgs.cn

[S10] C：指针与解引用
来源：http://pf.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://ij.wgjwhj.cn

[S11] C：逐行读文件
来源：http://iv.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://mx.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nm.bookmarksfly.cn

fclose(f);
来源：http://hd.lnxyls.cn

[S12] C：写文件
来源：http://fm.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bw.shtwfgs.cn

[S13] C：宏定义
来源：http://ap.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nl.panjiajie.cn

[S14] C：枚举
来源：http://gv.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://dv.wgjwhj.cn

[S15] C：类型转换
来源：http://kj.huixiangedu.cn

(double) a / b
来源：http://ww.asd995.cn

[S16] C：位操作置位
来源：http://up.newstarts.cn

x |= (1 << 3);
来源：http://wx.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://jt.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qh.nicolike.cn

[S18] C：命令行参数
来源：http://in.panjiajie.cn

int main(int argc, char **argv)
来源：http://il.huanxung.cn

[S19] C：快速排序
来源：http://su.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vo.newstarts.cn

[S20] C：二分查找
来源：http://ha.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ke.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://jg.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ir.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://yr.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iz.hahajie.cn

[S23] C：随机数
来源：http://lu.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://we.jctech888.com.cn

[S24] C：获取本地时间
来源：http://nl.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gl.bjjhwx.cn

[S25] C：内存拷贝
来源：http://os.nicolike.cn

memcpy(dst, src, n);
来源：http://os.yuexingan06.cn

[S26] C：内存清零
来源：http://da.newstarts.cn

memset(a, 0, sizeof a);
来源：http://aw.521024.cn

[S27] C：定义常量
来源：http://fp.hnjuh.cn

const double PI = 3.14159;
来源：http://ca.huixiangedu.cn

[S28] C：静态变量
来源：http://ub.shtwfgs.cn

static int counter = 0;
来源：http://df.asd995.cn

[S29] C：变参函数
来源：http://km.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eq.shxzskj.cn

[S30] C：头文件保护
来源：http://ve.yuexingan06.cn

#ifndef X_H
来源：http://nv.521024.cn

#define X_H
来源：http://qt.9csxet.cn

#endif
来源：http://pj.asd995.cn

[S31] C++：Hello World
来源：http://oi.shxzukj.cn

#include <iostream>
来源：http://js.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://kb.panjiajie.cn

[S32] C++：字符串
来源：http://na.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://tv.asd995.cn

[S33] C++：vector 增删
来源：http://jv.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xv.nicolike.cn

[S34] C++：遍历 vector
来源：http://ge.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://ci.wgjwhj.cn

[S35] C++：map
来源：http://pq.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zi.bjjhwx.cn

[S36] C++：unordered_map
来源：http://mz.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sx.hnjuh.cn

[S37] C++：set
来源：http://ii.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uv.szsharing.cn

[S38] C++：排序
来源：http://rc.colortex.cn

std::sort(v.begin(), v.end());
来源：http://ee.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://dw.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uy.bookmarksfly.cn

[S40] C++：查找元素
来源：http://mc.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hf.huanxung.cn

[S41] C++：类与构造函数
来源：http://kc.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lf.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://jq.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://dt.huanxung.cn

[S43] C++：智能指针
来源：http://ip.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://yx.nszjky.cn

[S44] C++：引用传参
来源：http://mz.nszjky.cn

void inc(int &x) { ++x; }
来源：http://co.nszjky.cn

[S45] C++：lambda
来源：http://eu.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tm.shxzskj.cn

[S46] C++：函数模板
来源：http://ul.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qa.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://du.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qh.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://ag.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wt.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://qh.lnxyls.cn

[S49] C++：写文件
来源：http://gq.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rj.jctech888.com.cn

[S50] C++：格式化数字
来源：http://ra.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://px.shxzukj.cn

[S51] C++：显式类型转换
来源：http://pc.hnjuh.cn

static_cast<double>(a) / b
来源：http://jc.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://qc.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://nf.shxzskj.cn

[S53] C++：移动语义
来源：http://xi.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://ne.chemitech.net.cn

[S54] C++：异常处理
来源：http://er.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zc.huanxung.cn

[S55] C++：结构化绑定
来源：http://ry.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ti.muxihuayi.cn

[S56] C++：optional
来源：http://aj.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://te.szsharing.cn

[S57] C++：编译期常量
来源：http://ry.bjjhwx.cn

constexpr int N = 10;
来源：http://mr.hnjuh.cn

[S58] C++：命名空间
来源：http://sl.521024.cn

namespace ns { int f() { return 1; } }
来源：http://gb.shtwfgs.cn

[S59] C++：静态断言
来源：http://fj.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hm.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://vl.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sz.521024.cn

================================================================================
来源：http://te.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qz.521024.cn

================================================================================
来源：http://nw.hahajie.cn

[T01] Kotlin：Hello World
来源：http://gg.haigaiapp.cn

println("Hello")
来源：http://gx.521024.cn

[T02] Kotlin：变量
来源：http://kr.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nc.asd995.cn

[T03] Kotlin：字符串模板
来源：http://ld.asd995.cn

"值: $b"
来源：http://ga.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://ny.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://vu.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://fb.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xm.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://ac.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://df.521024.cn

[T07] Kotlin：集合过滤
来源：http://ze.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fd.9csxet.cn

[T08] Kotlin：数据类
来源：http://so.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://dv.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://xf.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://tu.asd995.cn

[T10] Kotlin：默认参数
来源：http://we.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vf.9csxet.cn

[T11] Kotlin：协程
来源：http://kr.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ab.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://ib.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://xm.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://yn.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://wi.bjjhwx.cn

[T14] Kotlin：循环
来源：http://ah.gzmigu.cn

for (i in 1..10) println(i)
来源：http://zn.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://xj.nicolike.cn

interface Shape { fun area(): Double }
来源：http://cv.haigaiapp.cn

[T16] Swift：Hello World
来源：http://ua.shxzskj.cn

print("Hello")
来源：http://yn.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://yn.yuexingan06.cn

var a = 1;  let b = 2
来源：http://fc.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://xa.wgjwhj.cn

"值: \(b)"
来源：http://is.lnxyls.cn

[T19] Swift：可选绑定
来源：http://jn.jctech888.com.cn

if let n = opt { print(n) }
来源：http://ic.chemitech.net.cn

[T20] Swift：数组操作
来源：http://ac.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ur.shtwfgs.cn

[T21] Swift：遍历
来源：http://yo.bjjhwx.cn

for x in a { print(x) }
来源：http://lq.521024.cn

[T22] Swift：字典
来源：http://yh.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nc.haigaiapp.cn

[T23] Swift：函数
来源：http://xr.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qs.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://la.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nz.nszjky.cn

[T25] Swift：结构体
来源：http://ox.hahajie.cn

struct P { var x: Int }
来源：http://ns.shtwfgs.cn

[T26] Swift：类与重写
来源：http://la.hahajie.cn

class A: Base { override func f() {} }
来源：http://lg.colortex.cn

[T27] Swift：错误处理
来源：http://gt.hahajie.cn

do { try f() } catch { print(error) }
来源：http://qk.haigaiapp.cn

[T28] Swift：枚举
来源：http://fl.521024.cn

enum Color { case red, green }
来源：http://hx.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://lp.wgjwhj.cn

guard let x = opt else { return }
来源：http://pq.szsharing.cn

[T30] Swift：协议
来源：http://un.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://qm.hahajie.cn

[T31] Lua：Hello World
来源：http://av.asd995.cn

print("Hello")
来源：http://tj.panjiajie.cn

[T32] Lua：局部变量
来源：http://pi.wgjwhj.cn

local a = 1
来源：http://xb.521024.cn

[T33] Lua：表（数组）
来源：http://ld.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://eu.haigaiapp.cn

[T34] Lua：遍历表
来源：http://tl.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fm.lnxyls.cn

[T35] Lua：字典表
来源：http://ua.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://dc.yuexingan06.cn

[T36] Lua：函数
来源：http://dm.huixiangedu.cn

function add(a, b) return a + b end
来源：http://ex.szsharing.cn

[T37] Lua：字符串拼接
来源：http://xw.jianghongdianzi.cn

"a" .. "b"
来源：http://ik.asd995.cn

[T38] Lua：条件
来源：http://ru.wgjwhj.cn

if x > 0 then print("正") end
来源：http://fw.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://gf.hahajie.cn

string.find(s, "%d+")
来源：http://zt.bookmarksfly.cn

[T40] Lua：元表
来源：http://sd.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://jd.bjjhwx.cn

[T41] Perl：Hello World
来源：http://ew.gzmigu.cn

print "Hello\n";
来源：http://po.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://mn.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zb.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://fq.huanxung.cn

"值: $a"
来源：http://ac.yuntaijiaju.cn

[T44] Perl：条件
来源：http://qn.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://cm.shxzukj.cn

[T45] Perl：数组遍历
来源：http://ty.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://eu.nszjky.cn

[T46] Perl：哈希操作
来源：http://wl.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lq.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://rq.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sg.lnxyls.cn

[T48] Perl：正则替换
来源：http://jf.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://qv.newstarts.cn

[T49] Perl：函数
来源：http://dn.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fg.huanxung.cn

[T50] Perl：逐行读文件
来源：http://dp.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qd.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://bp.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://fs.nszjky.cn

println("Hello")
来源：http://ki.hahajie.cn

[T52] Scala：变量
来源：http://mr.haigaiapp.cn


<!-- 参考信息 -->