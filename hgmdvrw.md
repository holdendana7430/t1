代发 wailian999

find . -name "*.tmp" -delete
来源：http://bl.shxzskj.cn

[R46] 递归替换文件内容
来源：http://qx.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iq.panjiajie.cn

[R47] sed 单行替换
来源：http://ys.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fo.asd995.cn

[R48] awk 取指定列
来源：http://zu.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://xy.jctech888.com.cn

[R49] awk 带条件
来源：http://em.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ld.gzmigu.cn

[R50] awk 求和
来源：http://sp.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yj.jctech888.com.cn

[R51] 排序去重取前几
来源：http://xa.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://us.szsharing.cn

[R52] 统计行数
来源：http://gi.nszjky.cn

wc -l a.txt
来源：http://lh.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://cw.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jl.hahajie.cn

[R54] 比较两个文件
来源：http://kg.newstarts.cn

diff a.txt b.txt
来源：http://zr.nicolike.cn

[R55] 压缩与解压
来源：http://qa.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yr.bookmarksfly.cn

[R56] 远程拷贝
来源：http://cs.gzmigu.cn

scp file user@host:/path/
来源：http://se.9csxet.cn

[R57] 远程执行命令
来源：http://oz.hahajie.cn

ssh user@host 'uptime'
来源：http://vk.huixiangedu.cn

[R58] 下载文件
来源：http://bs.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zr.gzmigu.cn

[R59] 发 POST JSON
来源：http://tv.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dh.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://mo.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lz.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://fv.521024.cn

df -h;  du -sh *
来源：http://ml.9csxet.cn

[R62] 找最占空间的文件
来源：http://ah.521024.cn

du -ah . | sort -rh | head -10
来源：http://hl.hahajie.cn

[R63] 内存与进程
来源：http://da.521024.cn

free -h;  ps aux | grep nginx
来源：http://md.szxytkj.cn

[R64] 结束进程
来源：http://sp.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://qm.chemitech.net.cn

[R65] 查看端口占用
来源：http://pw.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yl.wgjwhj.cn

[R66] 定时任务
来源：http://pz.shtwfgs.cn

crontab -e;  crontab -l
来源：http://ra.huanxung.cn

[R67] 生成随机十六进制串
来源：http://ca.nszjky.cn

openssl rand -hex 16
来源：http://na.9csxet.cn

[R68] 计算文件校验值
来源：http://ag.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cu.huanxung.cn

[R69] 生成随机密码
来源：http://dl.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://qr.muxihuayi.cn

[R70] 时间戳与互转
来源：http://oe.hahajie.cn

date +%s;  date -d @1700000000
来源：http://op.huixinmuqiang.cn

[R71] 日期格式化
来源：http://fo.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ru.bjjhwx.cn

[R72] 等待端口就绪
来源：http://zz.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://if.jianghongdianzi.cn

[R73] 分割大日志
来源：http://cy.asd995.cn

split -l 1000 big.log part_
来源：http://ja.shxzukj.cn

[R74] 批量重命名
来源：http://ti.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kb.szxytkj.cn

[R75] 导出环境变量
来源：http://vj.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ur.nicolike.cn

[R76] 使用临时文件
来源：http://qd.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://as.chemitech.net.cn

[R77] 读取用户输入
来源：http://eu.panjiajie.cn

read -rp "请输入: " ans
来源：http://jc.shxzukj.cn

[R78] 交互式菜单
来源：http://gm.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lf.shxzskj.cn

[R79] 解析命令行选项
来源：http://jd.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://du.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://df.lnxyls.cn

time ./run.sh
来源：http://rx.lnxyls.cn

================================================================================
来源：http://aa.jianghongdianzi.cn

S. C / C++ 专题
来源：http://hm.muxihuayi.cn

================================================================================
来源：http://co.huanxung.cn

[S01] C：Hello World
来源：http://oj.newstarts.cn

#include <stdio.h>
来源：http://xb.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xs.asd995.cn

[S02] C：变量与格式化输出
来源：http://rg.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://vq.jctech888.com.cn

[S03] C：读入整数
来源：http://pn.shxzukj.cn

int x; scanf("%d", &x);
来源：http://fm.panjiajie.cn

[S04] C：字符串复制
来源：http://gi.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pt.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://ea.chemitech.net.cn

strlen(s)
来源：http://cw.gzmigu.cn

[S06] C：字符串比较
来源：http://om.9csxet.cn

strcmp(a, b) == 0
来源：http://zw.szxytkj.cn

[S07] C：数组遍历求和
来源：http://lx.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ah.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://er.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://as.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://nq.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cm.huanxung.cn

[S10] C：指针与解引用
来源：http://xc.521024.cn

int *p = &a;  *p = 5;
来源：http://ui.szsharing.cn

[S11] C：逐行读文件
来源：http://ph.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://hd.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cw.haigaiapp.cn

fclose(f);
来源：http://ca.asd995.cn

[S12] C：写文件
来源：http://so.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zu.newstarts.cn

[S13] C：宏定义
来源：http://uv.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yb.yuntaijiaju.cn

[S14] C：枚举
来源：http://ga.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://km.szxytkj.cn

[S15] C：类型转换
来源：http://zx.yuexingan06.cn

(double) a / b
来源：http://lx.bookmarksfly.cn

[S16] C：位操作置位
来源：http://sh.chemitech.net.cn

x |= (1 << 3);
来源：http://ok.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://ah.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nc.521024.cn

[S18] C：命令行参数
来源：http://rt.newstarts.cn

int main(int argc, char **argv)
来源：http://yt.gzmigu.cn

[S19] C：快速排序
来源：http://sg.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yo.huixiangedu.cn

[S20] C：二分查找
来源：http://of.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ks.shxzskj.cn

[S21] C：字符类别判断
来源：http://mo.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qu.9csxet.cn

[S22] C：字符串转数字
来源：http://my.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://io.colortex.cn

[S23] C：随机数
来源：http://jd.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cw.shxzskj.cn

[S24] C：获取本地时间
来源：http://sl.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://al.shtwfgs.cn

[S25] C：内存拷贝
来源：http://qo.shxzskj.cn

memcpy(dst, src, n);
来源：http://sa.szsharing.cn

[S26] C：内存清零
来源：http://ev.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://dp.nszjky.cn

[S27] C：定义常量
来源：http://xo.panjiajie.cn

const double PI = 3.14159;
来源：http://gr.hahajie.cn

[S28] C：静态变量
来源：http://sy.panjiajie.cn

static int counter = 0;
来源：http://gs.gzmigu.cn

[S29] C：变参函数
来源：http://pj.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://me.521024.cn

[S30] C：头文件保护
来源：http://ay.hnjuh.cn

#ifndef X_H
来源：http://ch.huixiangedu.cn

#define X_H
来源：http://wr.jctech888.com.cn

#endif
来源：http://lc.panjiajie.cn

[S31] C++：Hello World
来源：http://ic.yuexingan06.cn

#include <iostream>
来源：http://xe.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://ya.huanxung.cn

[S32] C++：字符串
来源：http://da.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://lw.newstarts.cn

[S33] C++：vector 增删
来源：http://dz.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://da.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://yj.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://tb.muxihuayi.cn

[S35] C++：map
来源：http://qg.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://od.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://sf.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://um.szsharing.cn

[S37] C++：set
来源：http://hp.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ru.nicolike.cn

[S38] C++：排序
来源：http://uq.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://gb.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://mh.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yy.bjjhwx.cn

[S40] C++：查找元素
来源：http://dr.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://as.colortex.cn

[S41] C++：类与构造函数
来源：http://ha.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sc.huanxung.cn

[S42] C++：继承与虚函数
来源：http://er.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://sh.shxzukj.cn

[S43] C++：智能指针
来源：http://xa.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://ah.panjiajie.cn

[S44] C++：引用传参
来源：http://au.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://lr.panjiajie.cn

[S45] C++：lambda
来源：http://ar.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ai.shxzukj.cn

[S46] C++：函数模板
来源：http://nz.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qd.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://va.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dp.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://yv.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zr.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://is.jianghongdianzi.cn

[S49] C++：写文件
来源：http://az.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sj.panjiajie.cn

[S50] C++：格式化数字
来源：http://ac.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kn.colortex.cn

[S51] C++：显式类型转换
来源：http://ib.panjiajie.cn

static_cast<double>(a) / b
来源：http://hl.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://ev.hahajie.cn

int size() const noexcept { return n_; }
来源：http://jn.szxytkj.cn

[S53] C++：移动语义
来源：http://nk.colortex.cn

std::vector<int> w = std::move(v);
来源：http://up.huanxung.cn

[S54] C++：异常处理
来源：http://lf.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ys.panjiajie.cn

[S55] C++：结构化绑定
来源：http://mu.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://le.huanxung.cn

[S56] C++：optional
来源：http://lz.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qz.shtwfgs.cn

[S57] C++：编译期常量
来源：http://fo.521024.cn

constexpr int N = 10;
来源：http://qt.muxihuayi.cn

[S58] C++：命名空间
来源：http://ws.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://sd.yuexingan06.cn

[S59] C++：静态断言
来源：http://vk.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ol.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://br.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ek.yuntaijiaju.cn

================================================================================
来源：http://bn.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tf.muxihuayi.cn

================================================================================
来源：http://kr.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://qm.hnjuh.cn

println("Hello")
来源：http://bx.huanxung.cn

[T02] Kotlin：变量
来源：http://qw.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hl.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://qj.bjjhwx.cn

"值: $b"
来源：http://td.newstarts.cn

[T04] Kotlin：空安全
来源：http://vh.nszjky.cn

val n: String? = null;  n?.length
来源：http://xr.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://ax.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nw.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://me.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wa.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://gi.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xb.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://ax.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://gs.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://eb.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://gw.colortex.cn

[T10] Kotlin：默认参数
来源：http://vm.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yw.jctech888.com.cn

[T11] Kotlin：协程
来源：http://jv.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sk.newstarts.cn

[T12] Kotlin：解构声明
来源：http://jw.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://qs.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://lq.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://xm.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://py.asd995.cn

for (i in 1..10) println(i)
来源：http://qk.muxihuayi.cn

[T15] Kotlin：接口
来源：http://yr.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://ib.newstarts.cn

[T16] Swift：Hello World
来源：http://nq.bookmarksfly.cn

print("Hello")
来源：http://wo.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://ie.521024.cn

var a = 1;  let b = 2
来源：http://wt.hahajie.cn

[T18] Swift：字符串插值
来源：http://hl.bjjhwx.cn

"值: \(b)"
来源：http://ic.shxzskj.cn

[T19] Swift：可选绑定
来源：http://ya.panjiajie.cn

if let n = opt { print(n) }
来源：http://nf.yuexingan06.cn

[T20] Swift：数组操作
来源：http://cg.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wg.521024.cn

[T21] Swift：遍历
来源：http://up.shxzukj.cn

for x in a { print(x) }
来源：http://ws.chemitech.net.cn

[T22] Swift：字典
来源：http://qs.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ug.hahajie.cn

[T23] Swift：函数
来源：http://oe.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ip.haigaiapp.cn

[T24] Swift：闭包
来源：http://zl.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sw.huixiangedu.cn

[T25] Swift：结构体
来源：http://bc.huanxung.cn

struct P { var x: Int }
来源：http://qr.chemitech.net.cn

[T26] Swift：类与重写
来源：http://sn.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://ev.wgjwhj.cn

[T27] Swift：错误处理
来源：http://yz.9csxet.cn

do { try f() } catch { print(error) }
来源：http://bn.bjjhwx.cn

[T28] Swift：枚举
来源：http://th.hnjuh.cn

enum Color { case red, green }
来源：http://my.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://lw.asd995.cn

guard let x = opt else { return }
来源：http://cx.colortex.cn

[T30] Swift：协议
来源：http://ux.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://uf.nszjky.cn

[T31] Lua：Hello World
来源：http://vv.9csxet.cn

print("Hello")
来源：http://fh.lnxyls.cn

[T32] Lua：局部变量
来源：http://af.9csxet.cn

local a = 1
来源：http://ip.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://re.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hr.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://od.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rv.panjiajie.cn

[T35] Lua：字典表
来源：http://xj.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://le.521024.cn

[T36] Lua：函数
来源：http://ei.hnjuh.cn

function add(a, b) return a + b end
来源：http://cu.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://sp.asd995.cn

"a" .. "b"
来源：http://pw.yuntaijiaju.cn

[T38] Lua：条件
来源：http://mu.yuexingan06.cn

if x > 0 then print("正") end
来源：http://kn.lnxyls.cn

[T39] Lua：模式匹配
来源：http://ov.newstarts.cn

string.find(s, "%d+")
来源：http://if.jctech888.com.cn

[T40] Lua：元表
来源：http://ze.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://rd.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://xk.huixiangedu.cn

print "Hello\n";
来源：http://qs.haigaiapp.cn

[T42] Perl：变量类型
来源：http://rg.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ww.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://nw.hahajie.cn

"值: $a"
来源：http://lz.gzmigu.cn

[T44] Perl：条件
来源：http://db.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://iv.szsharing.cn

[T45] Perl：数组遍历
来源：http://jb.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://sr.newstarts.cn

[T46] Perl：哈希操作
来源：http://ey.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ki.nicolike.cn

[T47] Perl：正则捕获
来源：http://je.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ul.muxihuayi.cn

[T48] Perl：正则替换
来源：http://mg.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://mg.szxytkj.cn


<!-- 参考信息 -->