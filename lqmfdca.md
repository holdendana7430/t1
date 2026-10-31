代发 wailian999

find . -name "*.tmp" -delete
来源：http://ti.lnxyls.cn

[R46] 递归替换文件内容
来源：http://hq.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hu.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://kd.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wl.521024.cn

[R48] awk 取指定列
来源：http://zm.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://di.shtwfgs.cn

[R49] awk 带条件
来源：http://ij.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xt.nszjky.cn

[R50] awk 求和
来源：http://nd.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://os.lnxyls.cn

[R51] 排序去重取前几
来源：http://po.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sg.hnjuh.cn

[R52] 统计行数
来源：http://vz.szxytkj.cn

wc -l a.txt
来源：http://ku.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://yu.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pj.nicolike.cn

[R54] 比较两个文件
来源：http://go.shxzskj.cn

diff a.txt b.txt
来源：http://jn.colortex.cn

[R55] 压缩与解压
来源：http://af.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ee.nszjky.cn

[R56] 远程拷贝
来源：http://no.colortex.cn

scp file user@host:/path/
来源：http://ed.huanxung.cn

[R57] 远程执行命令
来源：http://kc.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://ri.colortex.cn

[R58] 下载文件
来源：http://sb.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yr.hahajie.cn

[R59] 发 POST JSON
来源：http://io.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://co.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://by.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sv.521024.cn

[R61] 磁盘占用
来源：http://iv.huanxung.cn

df -h;  du -sh *
来源：http://bz.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://un.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://mv.wgjwhj.cn

[R63] 内存与进程
来源：http://zu.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://ib.huixinmuqiang.cn

[R64] 结束进程
来源：http://zf.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://xm.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://xc.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://no.muxihuayi.cn

[R66] 定时任务
来源：http://hc.newstarts.cn

crontab -e;  crontab -l
来源：http://re.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://jz.muxihuayi.cn

openssl rand -hex 16
来源：http://hn.asd995.cn

[R68] 计算文件校验值
来源：http://xo.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vy.huixiangedu.cn

[R69] 生成随机密码
来源：http://sj.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://zr.shtwfgs.cn

[R70] 时间戳与互转
来源：http://aj.newstarts.cn

date +%s;  date -d @1700000000
来源：http://xs.jctech888.com.cn

[R71] 日期格式化
来源：http://jb.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wg.panjiajie.cn

[R72] 等待端口就绪
来源：http://um.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xo.bjjhwx.cn

[R73] 分割大日志
来源：http://bk.bjjhwx.cn

split -l 1000 big.log part_
来源：http://tb.9csxet.cn

[R74] 批量重命名
来源：http://vm.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cb.bjjhwx.cn

[R75] 导出环境变量
来源：http://rx.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://uz.wgjwhj.cn

[R76] 使用临时文件
来源：http://mf.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ct.asd995.cn

[R77] 读取用户输入
来源：http://zr.9csxet.cn

read -rp "请输入: " ans
来源：http://gc.bookmarksfly.cn

[R78] 交互式菜单
来源：http://ev.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://il.colortex.cn

[R79] 解析命令行选项
来源：http://os.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rq.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://yp.nszjky.cn

time ./run.sh
来源：http://dl.chemitech.net.cn

================================================================================
来源：http://ed.nicolike.cn

S. C / C++ 专题
来源：http://im.521024.cn

================================================================================
来源：http://te.huixinmuqiang.cn

[S01] C：Hello World
来源：http://uq.bjjhwx.cn

#include <stdio.h>
来源：http://pg.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tq.szsharing.cn

[S02] C：变量与格式化输出
来源：http://qh.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://hh.jctech888.com.cn

[S03] C：读入整数
来源：http://zz.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://dz.huanxung.cn

[S04] C：字符串复制
来源：http://wd.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://li.colortex.cn

[S05] C：字符串长度
来源：http://kc.jianghongdianzi.cn

strlen(s)
来源：http://zd.9csxet.cn

[S06] C：字符串比较
来源：http://hb.szxytkj.cn

strcmp(a, b) == 0
来源：http://nx.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://ft.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ly.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://rn.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mb.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://sj.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wd.newstarts.cn

[S10] C：指针与解引用
来源：http://qy.asd995.cn

int *p = &a;  *p = 5;
来源：http://fs.huanxung.cn

[S11] C：逐行读文件
来源：http://wy.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://ha.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fp.colortex.cn

fclose(f);
来源：http://ei.bookmarksfly.cn

[S12] C：写文件
来源：http://go.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://px.shtwfgs.cn

[S13] C：宏定义
来源：http://eo.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ra.hahajie.cn

[S14] C：枚举
来源：http://hl.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://tc.jianghongdianzi.cn

[S15] C：类型转换
来源：http://qz.colortex.cn

(double) a / b
来源：http://gp.huanxung.cn

[S16] C：位操作置位
来源：http://wd.wgjwhj.cn

x |= (1 << 3);
来源：http://qz.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://zn.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kg.huixiangedu.cn

[S18] C：命令行参数
来源：http://rf.huanxung.cn

int main(int argc, char **argv)
来源：http://wo.chemitech.net.cn

[S19] C：快速排序
来源：http://iz.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tw.muxihuayi.cn

[S20] C：二分查找
来源：http://yd.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mx.hahajie.cn

[S21] C：字符类别判断
来源：http://fm.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wc.shxzukj.cn

[S22] C：字符串转数字
来源：http://xd.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hg.chemitech.net.cn

[S23] C：随机数
来源：http://eu.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ut.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://zq.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rw.shtwfgs.cn

[S25] C：内存拷贝
来源：http://du.colortex.cn

memcpy(dst, src, n);
来源：http://kk.shxzskj.cn

[S26] C：内存清零
来源：http://tz.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://ix.colortex.cn

[S27] C：定义常量
来源：http://lw.newstarts.cn

const double PI = 3.14159;
来源：http://wl.panjiajie.cn

[S28] C：静态变量
来源：http://kj.hahajie.cn

static int counter = 0;
来源：http://vr.chemitech.net.cn

[S29] C：变参函数
来源：http://ef.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zi.muxihuayi.cn

[S30] C：头文件保护
来源：http://ma.nicolike.cn

#ifndef X_H
来源：http://pb.shxzskj.cn

#define X_H
来源：http://nf.panjiajie.cn

#endif
来源：http://ay.hnjuh.cn

[S31] C++：Hello World
来源：http://kz.nszjky.cn

#include <iostream>
来源：http://hq.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://gv.panjiajie.cn

[S32] C++：字符串
来源：http://hy.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://xw.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://oo.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hx.szsharing.cn

[S34] C++：遍历 vector
来源：http://dg.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://zu.bjjhwx.cn

[S35] C++：map
来源：http://qo.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yq.muxihuayi.cn

[S36] C++：unordered_map
来源：http://wt.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dh.szsharing.cn

[S37] C++：set
来源：http://en.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://az.huanxung.cn

[S38] C++：排序
来源：http://cv.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://ya.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://bg.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://no.huanxung.cn

[S40] C++：查找元素
来源：http://zn.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ul.521024.cn

[S41] C++：类与构造函数
来源：http://yt.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tr.hahajie.cn

[S42] C++：继承与虚函数
来源：http://yb.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://yy.chemitech.net.cn

[S43] C++：智能指针
来源：http://fe.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://ua.asd995.cn

[S44] C++：引用传参
来源：http://pb.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://rm.nicolike.cn

[S45] C++：lambda
来源：http://ps.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ku.panjiajie.cn

[S46] C++：函数模板
来源：http://ir.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://da.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://tx.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vl.nszjky.cn

[S48] C++：逐行读文件
来源：http://tu.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cj.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://kx.bookmarksfly.cn

[S49] C++：写文件
来源：http://ny.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ae.huixiangedu.cn

[S50] C++：格式化数字
来源：http://oh.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ao.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://tu.9csxet.cn

static_cast<double>(a) / b
来源：http://ov.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://kv.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://vd.huanxung.cn

[S53] C++：移动语义
来源：http://rd.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://eg.521024.cn

[S54] C++：异常处理
来源：http://bl.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aa.shxzukj.cn

[S55] C++：结构化绑定
来源：http://cv.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pk.wgjwhj.cn

[S56] C++：optional
来源：http://gr.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ng.wgjwhj.cn

[S57] C++：编译期常量
来源：http://sb.shtwfgs.cn

constexpr int N = 10;
来源：http://ax.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://my.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://ee.lnxyls.cn

[S59] C++：静态断言
来源：http://bv.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ps.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://ia.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mo.asd995.cn

================================================================================
来源：http://kq.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qf.nicolike.cn

================================================================================
来源：http://rz.nicolike.cn

[T01] Kotlin：Hello World
来源：http://ju.bjjhwx.cn

println("Hello")
来源：http://zx.521024.cn

[T02] Kotlin：变量
来源：http://ld.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dt.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://ef.yuntaijiaju.cn

"值: $b"
来源：http://oq.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://hz.szxytkj.cn

val n: String? = null;  n?.length
来源：http://fo.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://nb.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lo.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://se.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mq.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://tb.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zt.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://lz.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://az.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://oe.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://jh.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://qo.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kw.haigaiapp.cn

[T11] Kotlin：协程
来源：http://gh.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wn.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://gs.521024.cn

val (a, b) = Pair(1, 2)
来源：http://yh.521024.cn

[T13] Kotlin：只读 Map
来源：http://fy.nicolike.cn

val m = mapOf("a" to 1)
来源：http://qa.szxytkj.cn

[T14] Kotlin：循环
来源：http://jr.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://pt.szsharing.cn

[T15] Kotlin：接口
来源：http://mt.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://cn.chemitech.net.cn

[T16] Swift：Hello World
来源：http://xe.jctech888.com.cn

print("Hello")
来源：http://dy.shxzukj.cn

[T17] Swift：变量与常量
来源：http://hh.shxzukj.cn

var a = 1;  let b = 2
来源：http://jm.szxytkj.cn

[T18] Swift：字符串插值
来源：http://so.colortex.cn

"值: \(b)"
来源：http://sx.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://ko.huixiangedu.cn

if let n = opt { print(n) }
来源：http://yd.muxihuayi.cn

[T20] Swift：数组操作
来源：http://yh.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ef.521024.cn

[T21] Swift：遍历
来源：http://ed.huixinmuqiang.cn

for x in a { print(x) }
来源：http://uz.szxytkj.cn

[T22] Swift：字典
来源：http://ux.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ki.shxzukj.cn

[T23] Swift：函数
来源：http://vc.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lf.lnxyls.cn

[T24] Swift：闭包
来源：http://gg.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://se.521024.cn

[T25] Swift：结构体
来源：http://md.huanxung.cn

struct P { var x: Int }
来源：http://qb.lnxyls.cn

[T26] Swift：类与重写
来源：http://xe.521024.cn

class A: Base { override func f() {} }
来源：http://pr.wgjwhj.cn

[T27] Swift：错误处理
来源：http://ei.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://kj.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://nt.wgjwhj.cn

enum Color { case red, green }
来源：http://ul.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://jt.hnjuh.cn

guard let x = opt else { return }
来源：http://mb.521024.cn

[T30] Swift：协议
来源：http://yx.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://mk.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://zx.yuntaijiaju.cn

print("Hello")
来源：http://pe.hahajie.cn

[T32] Lua：局部变量
来源：http://dn.newstarts.cn

local a = 1
来源：http://tz.panjiajie.cn

[T33] Lua：表（数组）
来源：http://qh.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ak.asd995.cn

[T34] Lua：遍历表
来源：http://pt.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zh.hnjuh.cn

[T35] Lua：字典表
来源：http://kr.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://rv.jianghongdianzi.cn

[T36] Lua：函数
来源：http://pm.shtwfgs.cn

function add(a, b) return a + b end
来源：http://of.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://gf.jianghongdianzi.cn

"a" .. "b"
来源：http://be.nszjky.cn

[T38] Lua：条件
来源：http://rt.shxzukj.cn

if x > 0 then print("正") end
来源：http://fu.521024.cn

[T39] Lua：模式匹配
来源：http://ti.chemitech.net.cn

string.find(s, "%d+")
来源：http://nd.huixiangedu.cn

[T40] Lua：元表
来源：http://vp.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://bt.huanxung.cn

[T41] Perl：Hello World
来源：http://oi.bookmarksfly.cn

print "Hello\n";
来源：http://yk.gzmigu.cn

[T42] Perl：变量类型
来源：http://eo.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tn.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://so.gzmigu.cn

"值: $a"
来源：http://fh.nszjky.cn

[T44] Perl：条件
来源：http://eh.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://ep.gzmigu.cn

[T45] Perl：数组遍历
来源：http://aq.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://ep.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://iu.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pu.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://hl.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://is.newstarts.cn

[T48] Perl：正则替换
来源：http://yy.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://re.haigaiapp.cn


<!-- 参考信息 -->