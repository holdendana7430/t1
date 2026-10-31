代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sv.bjjhwx.cn

[R56] 远程拷贝
来源：http://rs.bookmarksfly.cn

scp file user@host:/path/
来源：http://ew.panjiajie.cn

[R57] 远程执行命令
来源：http://hc.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://vv.szsharing.cn

[R58] 下载文件
来源：http://sa.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vb.haigaiapp.cn

[R59] 发 POST JSON
来源：http://qv.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ze.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://td.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rr.yuexingan06.cn

[R61] 磁盘占用
来源：http://ru.colortex.cn

df -h;  du -sh *
来源：http://ux.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://jl.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://jh.521024.cn

[R63] 内存与进程
来源：http://ct.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://hh.muxihuayi.cn

[R64] 结束进程
来源：http://dj.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://be.bookmarksfly.cn

[R65] 查看端口占用
来源：http://go.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hn.huixinmuqiang.cn

[R66] 定时任务
来源：http://np.haigaiapp.cn

crontab -e;  crontab -l
来源：http://vs.hahajie.cn

[R67] 生成随机十六进制串
来源：http://bz.szsharing.cn

openssl rand -hex 16
来源：http://ph.hnjuh.cn

[R68] 计算文件校验值
来源：http://oy.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hq.haigaiapp.cn

[R69] 生成随机密码
来源：http://dg.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://lu.shxzskj.cn

[R70] 时间戳与互转
来源：http://zq.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://cy.bookmarksfly.cn

[R71] 日期格式化
来源：http://dw.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ki.haigaiapp.cn

[R72] 等待端口就绪
来源：http://gp.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gq.shxzskj.cn

[R73] 分割大日志
来源：http://pj.shxzskj.cn

split -l 1000 big.log part_
来源：http://fw.szxytkj.cn

[R74] 批量重命名
来源：http://yq.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ev.521024.cn

[R75] 导出环境变量
来源：http://hx.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://fz.szsharing.cn

[R76] 使用临时文件
来源：http://pn.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tx.szxytkj.cn

[R77] 读取用户输入
来源：http://uv.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://za.szxytkj.cn

[R78] 交互式菜单
来源：http://yl.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oj.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://xu.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yu.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://re.wgjwhj.cn

time ./run.sh
来源：http://zv.521024.cn

================================================================================
来源：http://mh.9csxet.cn

S. C / C++ 专题
来源：http://xh.shxzskj.cn

================================================================================
来源：http://tr.hnjuh.cn

[S01] C：Hello World
来源：http://qv.shxzskj.cn

#include <stdio.h>
来源：http://ux.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gq.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://le.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://yn.huanxung.cn

[S03] C：读入整数
来源：http://ll.huanxung.cn

int x; scanf("%d", &x);
来源：http://gn.nszjky.cn

[S04] C：字符串复制
来源：http://od.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gf.shtwfgs.cn

[S05] C：字符串长度
来源：http://uz.yuntaijiaju.cn

strlen(s)
来源：http://yo.hnjuh.cn

[S06] C：字符串比较
来源：http://ku.huixiangedu.cn

strcmp(a, b) == 0
来源：http://fs.huanxung.cn

[S07] C：数组遍历求和
来源：http://hx.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eh.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://fl.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cf.colortex.cn

[S09] C：结构体定义与初始化
来源：http://fd.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lz.szxytkj.cn

[S10] C：指针与解引用
来源：http://um.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://hp.9csxet.cn

[S11] C：逐行读文件
来源：http://kv.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://sa.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yj.muxihuayi.cn

fclose(f);
来源：http://mk.hahajie.cn

[S12] C：写文件
来源：http://of.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ef.521024.cn

[S13] C：宏定义
来源：http://gv.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qg.nszjky.cn

[S14] C：枚举
来源：http://ez.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://zj.gzmigu.cn

[S15] C：类型转换
来源：http://pg.szxytkj.cn

(double) a / b
来源：http://mr.huanxung.cn

[S16] C：位操作置位
来源：http://ez.9csxet.cn

x |= (1 << 3);
来源：http://gn.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://ks.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bz.shtwfgs.cn

[S18] C：命令行参数
来源：http://ea.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://cn.bjjhwx.cn

[S19] C：快速排序
来源：http://tp.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ie.huixinmuqiang.cn

[S20] C：二分查找
来源：http://wb.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lo.nicolike.cn

[S21] C：字符类别判断
来源：http://mx.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fm.huixiangedu.cn

[S22] C：字符串转数字
来源：http://me.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zf.colortex.cn

[S23] C：随机数
来源：http://gy.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mh.newstarts.cn

[S24] C：获取本地时间
来源：http://qv.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://st.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://dw.haigaiapp.cn

memcpy(dst, src, n);
来源：http://pa.haigaiapp.cn

[S26] C：内存清零
来源：http://zi.colortex.cn

memset(a, 0, sizeof a);
来源：http://tx.bjjhwx.cn

[S27] C：定义常量
来源：http://bl.bjjhwx.cn

const double PI = 3.14159;
来源：http://cu.nszjky.cn

[S28] C：静态变量
来源：http://ds.nszjky.cn

static int counter = 0;
来源：http://if.521024.cn

[S29] C：变参函数
来源：http://hm.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ci.newstarts.cn

[S30] C：头文件保护
来源：http://ph.huixinmuqiang.cn

#ifndef X_H
来源：http://ra.hahajie.cn

#define X_H
来源：http://rx.jctech888.com.cn

#endif
来源：http://jy.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://qz.nicolike.cn

#include <iostream>
来源：http://ce.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ad.gzmigu.cn

[S32] C++：字符串
来源：http://th.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://ml.chemitech.net.cn

[S33] C++：vector 增删
来源：http://wl.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mh.asd995.cn

[S34] C++：遍历 vector
来源：http://cv.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://wo.shxzskj.cn

[S35] C++：map
来源：http://dn.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yj.lnxyls.cn

[S36] C++：unordered_map
来源：http://rz.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yq.shxzskj.cn

[S37] C++：set
来源：http://nj.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qo.nszjky.cn

[S38] C++：排序
来源：http://rq.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://uo.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://vz.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hx.lnxyls.cn

[S40] C++：查找元素
来源：http://kz.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://np.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://bd.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tk.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://wu.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://ko.wgjwhj.cn

[S43] C++：智能指针
来源：http://la.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://ss.asd995.cn

[S44] C++：引用传参
来源：http://kj.nszjky.cn

void inc(int &x) { ++x; }
来源：http://ov.jianghongdianzi.cn

[S45] C++：lambda
来源：http://vo.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ah.shxzskj.cn

[S46] C++：函数模板
来源：http://lq.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zf.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://wz.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vf.lnxyls.cn

[S48] C++：逐行读文件
来源：http://jc.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wf.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://vt.colortex.cn

[S49] C++：写文件
来源：http://lm.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://en.nszjky.cn

[S50] C++：格式化数字
来源：http://tl.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bn.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://nl.colortex.cn

static_cast<double>(a) / b
来源：http://sx.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://ns.huanxung.cn

int size() const noexcept { return n_; }
来源：http://iv.colortex.cn

[S53] C++：移动语义
来源：http://gk.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://jb.shxzskj.cn

[S54] C++：异常处理
来源：http://mj.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lk.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://xj.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yk.bookmarksfly.cn

[S56] C++：optional
来源：http://la.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://de.yuexingan06.cn

[S57] C++：编译期常量
来源：http://ly.jianghongdianzi.cn

constexpr int N = 10;
来源：http://oe.szxytkj.cn

[S58] C++：命名空间
来源：http://ki.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://zx.9csxet.cn

[S59] C++：静态断言
来源：http://hy.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gz.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://sz.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ge.panjiajie.cn

================================================================================
来源：http://cv.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zw.bjjhwx.cn

================================================================================
来源：http://zm.521024.cn

[T01] Kotlin：Hello World
来源：http://az.bjjhwx.cn

println("Hello")
来源：http://xg.asd995.cn

[T02] Kotlin：变量
来源：http://md.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sn.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://vd.yuexingan06.cn

"值: $b"
来源：http://jm.colortex.cn

[T04] Kotlin：空安全
来源：http://js.colortex.cn

val n: String? = null;  n?.length
来源：http://ik.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://ck.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zo.nszjky.cn

[T06] Kotlin：集合映射
来源：http://sy.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wf.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://hj.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vz.colortex.cn

[T08] Kotlin：数据类
来源：http://eh.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://ou.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://lj.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://bh.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://zx.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://te.bjjhwx.cn

[T11] Kotlin：协程
来源：http://jb.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xu.asd995.cn

[T12] Kotlin：解构声明
来源：http://re.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://an.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://rr.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://wg.panjiajie.cn

[T14] Kotlin：循环
来源：http://xo.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://qq.nicolike.cn

[T15] Kotlin：接口
来源：http://id.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://np.panjiajie.cn

[T16] Swift：Hello World
来源：http://vb.huixinmuqiang.cn

print("Hello")
来源：http://sy.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://hd.nszjky.cn

var a = 1;  let b = 2
来源：http://pq.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://rg.newstarts.cn

"值: \(b)"
来源：http://cx.lnxyls.cn

[T19] Swift：可选绑定
来源：http://tu.colortex.cn

if let n = opt { print(n) }
来源：http://ee.hahajie.cn

[T20] Swift：数组操作
来源：http://rr.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uv.nszjky.cn

[T21] Swift：遍历
来源：http://sm.asd995.cn

for x in a { print(x) }
来源：http://en.yuntaijiaju.cn

[T22] Swift：字典
来源：http://ky.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vp.gzmigu.cn

[T23] Swift：函数
来源：http://dd.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://km.asd995.cn

[T24] Swift：闭包
来源：http://du.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://em.bjjhwx.cn

[T25] Swift：结构体
来源：http://zj.nszjky.cn

struct P { var x: Int }
来源：http://xq.lnxyls.cn

[T26] Swift：类与重写
来源：http://rm.shxzukj.cn

class A: Base { override func f() {} }
来源：http://qr.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://yv.9csxet.cn

do { try f() } catch { print(error) }
来源：http://qq.bjjhwx.cn

[T28] Swift：枚举
来源：http://mr.hnjuh.cn

enum Color { case red, green }
来源：http://gi.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://vh.huanxung.cn

guard let x = opt else { return }
来源：http://yk.szsharing.cn

[T30] Swift：协议
来源：http://wt.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://ms.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://eu.shxzukj.cn

print("Hello")
来源：http://mx.hahajie.cn

[T32] Lua：局部变量
来源：http://ao.521024.cn

local a = 1
来源：http://sm.asd995.cn

[T33] Lua：表（数组）
来源：http://cg.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ep.szxytkj.cn

[T34] Lua：遍历表
来源：http://ks.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bk.asd995.cn

[T35] Lua：字典表
来源：http://ta.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://ei.muxihuayi.cn

[T36] Lua：函数
来源：http://ht.hahajie.cn

function add(a, b) return a + b end
来源：http://dp.521024.cn

[T37] Lua：字符串拼接
来源：http://rp.shtwfgs.cn

"a" .. "b"
来源：http://is.chemitech.net.cn

[T38] Lua：条件
来源：http://vz.szsharing.cn

if x > 0 then print("正") end
来源：http://zx.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://ad.newstarts.cn

string.find(s, "%d+")
来源：http://ir.jianghongdianzi.cn

[T40] Lua：元表
来源：http://rr.nicolike.cn

setmetatable({}, { __index = base })
来源：http://oj.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://ml.9csxet.cn

print "Hello\n";
来源：http://fq.nszjky.cn

[T42] Perl：变量类型
来源：http://qj.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pc.nicolike.cn

[T43] Perl：字符串插值
来源：http://qr.521024.cn

"值: $a"
来源：http://sq.huanxung.cn

[T44] Perl：条件
来源：http://hl.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://cd.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://wu.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://cb.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://xx.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yd.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://qm.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://um.szsharing.cn

[T48] Perl：正则替换
来源：http://zq.huanxung.cn

$s =~ s/old/new/g;
来源：http://kn.muxihuayi.cn

[T49] Perl：函数
来源：http://lb.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lr.szsharing.cn

[T50] Perl：逐行读文件
来源：http://wn.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ig.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://vn.nicolike.cn

[T51] Scala：Hello World
来源：http://xs.jctech888.com.cn

println("Hello")
来源：http://wd.jianghongdianzi.cn

[T52] Scala：变量
来源：http://hv.shxzukj.cn

val a = 1;  var b = 2
来源：http://xr.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://iu.szxytkj.cn

s"值: $b"
来源：http://ce.asd995.cn

[T54] Scala：集合映射
来源：http://he.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ni.nicolike.cn

[T55] Scala：集合过滤
来源：http://us.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sw.hahajie.cn

[T56] Scala：样例类
来源：http://rs.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://hs.9csxet.cn

[T57] Scala：模式匹配
来源：http://gv.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://om.9csxet.cn

[T58] Scala：函数定义
来源：http://ys.szsharing.cn


<!-- 参考信息 -->