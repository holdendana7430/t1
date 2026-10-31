代发 wailian999

find . -name "*.tmp" -delete
来源：http://nk.shxzskj.cn

[R46] 递归替换文件内容
来源：http://jm.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fe.colortex.cn

[R47] sed 单行替换
来源：http://ck.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bu.521024.cn

[R48] awk 取指定列
来源：http://ks.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://nl.nicolike.cn

[R49] awk 带条件
来源：http://ol.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kl.521024.cn

[R50] awk 求和
来源：http://sk.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ck.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://ge.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ek.szsharing.cn

[R52] 统计行数
来源：http://ru.nicolike.cn

wc -l a.txt
来源：http://ta.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://ss.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ls.shxzukj.cn

[R54] 比较两个文件
来源：http://gx.huixiangedu.cn

diff a.txt b.txt
来源：http://my.bjjhwx.cn

[R55] 压缩与解压
来源：http://bd.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yz.chemitech.net.cn

[R56] 远程拷贝
来源：http://fd.bookmarksfly.cn

scp file user@host:/path/
来源：http://re.asd995.cn

[R57] 远程执行命令
来源：http://zf.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://sh.jctech888.com.cn

[R58] 下载文件
来源：http://rb.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tx.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://jc.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fb.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://wp.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fp.chemitech.net.cn

[R61] 磁盘占用
来源：http://vk.colortex.cn

df -h;  du -sh *
来源：http://jc.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://la.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://gs.chemitech.net.cn

[R63] 内存与进程
来源：http://zn.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://bo.yuexingan06.cn

[R64] 结束进程
来源：http://yw.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://tc.szsharing.cn

[R65] 查看端口占用
来源：http://sr.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kn.jctech888.com.cn

[R66] 定时任务
来源：http://wk.shxzskj.cn

crontab -e;  crontab -l
来源：http://lh.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://qr.yuexingan06.cn

openssl rand -hex 16
来源：http://mn.jctech888.com.cn

[R68] 计算文件校验值
来源：http://vu.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fw.szxytkj.cn

[R69] 生成随机密码
来源：http://uy.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://ns.szsharing.cn

[R70] 时间戳与互转
来源：http://et.szsharing.cn

date +%s;  date -d @1700000000
来源：http://xb.asd995.cn

[R71] 日期格式化
来源：http://kp.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hh.yuexingan06.cn

[R72] 等待端口就绪
来源：http://ha.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lf.gzmigu.cn

[R73] 分割大日志
来源：http://er.hnjuh.cn

split -l 1000 big.log part_
来源：http://ec.haigaiapp.cn

[R74] 批量重命名
来源：http://ed.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ej.haigaiapp.cn

[R75] 导出环境变量
来源：http://xh.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://ph.szsharing.cn

[R76] 使用临时文件
来源：http://eh.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ra.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://ti.colortex.cn

read -rp "请输入: " ans
来源：http://ov.newstarts.cn

[R78] 交互式菜单
来源：http://mg.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cf.9csxet.cn

[R79] 解析命令行选项
来源：http://eh.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wj.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://fa.shtwfgs.cn

time ./run.sh
来源：http://cn.panjiajie.cn

================================================================================
来源：http://ad.szxytkj.cn

S. C / C++ 专题
来源：http://ef.jianghongdianzi.cn

================================================================================
来源：http://eb.nszjky.cn

[S01] C：Hello World
来源：http://ws.wgjwhj.cn

#include <stdio.h>
来源：http://bi.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ut.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://rn.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://de.nicolike.cn

[S03] C：读入整数
来源：http://lg.gzmigu.cn

int x; scanf("%d", &x);
来源：http://as.shtwfgs.cn

[S04] C：字符串复制
来源：http://sm.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wd.521024.cn

[S05] C：字符串长度
来源：http://zj.shxzukj.cn

strlen(s)
来源：http://fb.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://zq.nszjky.cn

strcmp(a, b) == 0
来源：http://qu.szsharing.cn

[S07] C：数组遍历求和
来源：http://ih.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bm.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://rp.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vm.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://rr.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gn.chemitech.net.cn

[S10] C：指针与解引用
来源：http://fr.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://my.hnjuh.cn

[S11] C：逐行读文件
来源：http://wn.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://sr.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mj.szxytkj.cn

fclose(f);
来源：http://sn.nicolike.cn

[S12] C：写文件
来源：http://lr.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kr.yuexingan06.cn

[S13] C：宏定义
来源：http://pz.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lj.521024.cn

[S14] C：枚举
来源：http://kp.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://pn.huixinmuqiang.cn

[S15] C：类型转换
来源：http://it.haigaiapp.cn

(double) a / b
来源：http://el.9csxet.cn

[S16] C：位操作置位
来源：http://jl.szxytkj.cn

x |= (1 << 3);
来源：http://fo.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://iv.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://py.huanxung.cn

[S18] C：命令行参数
来源：http://ig.chemitech.net.cn

int main(int argc, char **argv)
来源：http://uw.9csxet.cn

[S19] C：快速排序
来源：http://tm.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jh.gzmigu.cn

[S20] C：二分查找
来源：http://hb.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ui.521024.cn

[S21] C：字符类别判断
来源：http://nn.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uz.szxytkj.cn

[S22] C：字符串转数字
来源：http://dj.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qw.hahajie.cn

[S23] C：随机数
来源：http://lb.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ki.asd995.cn

[S24] C：获取本地时间
来源：http://hd.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jk.bjjhwx.cn

[S25] C：内存拷贝
来源：http://bw.bjjhwx.cn

memcpy(dst, src, n);
来源：http://yf.gzmigu.cn

[S26] C：内存清零
来源：http://pf.nicolike.cn

memset(a, 0, sizeof a);
来源：http://yl.gzmigu.cn

[S27] C：定义常量
来源：http://gt.lnxyls.cn

const double PI = 3.14159;
来源：http://ky.hnjuh.cn

[S28] C：静态变量
来源：http://uf.szsharing.cn

static int counter = 0;
来源：http://hm.lnxyls.cn

[S29] C：变参函数
来源：http://mn.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lo.shxzukj.cn

[S30] C：头文件保护
来源：http://hb.bookmarksfly.cn

#ifndef X_H
来源：http://ai.huixinmuqiang.cn

#define X_H
来源：http://sm.gzmigu.cn

#endif
来源：http://lm.haigaiapp.cn

[S31] C++：Hello World
来源：http://yp.nicolike.cn

#include <iostream>
来源：http://lr.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://lf.shtwfgs.cn

[S32] C++：字符串
来源：http://jl.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://yn.haigaiapp.cn

[S33] C++：vector 增删
来源：http://eb.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kp.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://yj.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://ra.muxihuayi.cn

[S35] C++：map
来源：http://rn.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ra.szxytkj.cn

[S36] C++：unordered_map
来源：http://ut.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pg.haigaiapp.cn

[S37] C++：set
来源：http://mt.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pu.panjiajie.cn

[S38] C++：排序
来源：http://fp.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://jm.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://li.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gf.muxihuayi.cn

[S40] C++：查找元素
来源：http://wk.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yv.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://te.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yc.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://gd.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://qm.haigaiapp.cn

[S43] C++：智能指针
来源：http://af.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://lc.asd995.cn

[S44] C++：引用传参
来源：http://qr.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://lf.nicolike.cn

[S45] C++：lambda
来源：http://ou.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ik.hahajie.cn

[S46] C++：函数模板
来源：http://we.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yp.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://qe.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pc.hnjuh.cn

[S48] C++：逐行读文件
来源：http://ni.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://os.szsharing.cn

while (std::getline(in, line)) { }
来源：http://dy.gzmigu.cn

[S49] C++：写文件
来源：http://wy.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jr.huanxung.cn

[S50] C++：格式化数字
来源：http://ey.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xv.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://ab.asd995.cn

static_cast<double>(a) / b
来源：http://ev.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://tt.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://ut.colortex.cn

[S53] C++：移动语义
来源：http://ov.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://ro.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://la.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vc.panjiajie.cn

[S55] C++：结构化绑定
来源：http://wj.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mu.panjiajie.cn

[S56] C++：optional
来源：http://fi.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yd.newstarts.cn

[S57] C++：编译期常量
来源：http://pe.521024.cn

constexpr int N = 10;
来源：http://du.gzmigu.cn

[S58] C++：命名空间
来源：http://sr.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://yp.asd995.cn

[S59] C++：静态断言
来源：http://lr.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fd.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://dl.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hw.gzmigu.cn

================================================================================
来源：http://xo.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cx.shtwfgs.cn

================================================================================
来源：http://sk.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://us.shtwfgs.cn

println("Hello")
来源：http://ie.wgjwhj.cn

[T02] Kotlin：变量
来源：http://om.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qf.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://pl.gzmigu.cn

"值: $b"
来源：http://md.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://lf.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://ja.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://wx.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xz.newstarts.cn

[T06] Kotlin：集合映射
来源：http://kc.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://od.asd995.cn

[T07] Kotlin：集合过滤
来源：http://qt.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oc.newstarts.cn

[T08] Kotlin：数据类
来源：http://dm.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://iq.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://rn.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://hg.nszjky.cn

[T10] Kotlin：默认参数
来源：http://ly.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yq.hahajie.cn

[T11] Kotlin：协程
来源：http://yo.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nr.nszjky.cn

[T12] Kotlin：解构声明
来源：http://yq.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://oj.colortex.cn

[T13] Kotlin：只读 Map
来源：http://ql.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://wq.huanxung.cn

[T14] Kotlin：循环
来源：http://pm.521024.cn

for (i in 1..10) println(i)
来源：http://jx.shxzukj.cn

[T15] Kotlin：接口
来源：http://og.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://ge.huixiangedu.cn

[T16] Swift：Hello World
来源：http://ht.shxzukj.cn

print("Hello")
来源：http://fy.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://li.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://ec.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://jr.9csxet.cn

"值: \(b)"
来源：http://xj.nszjky.cn

[T19] Swift：可选绑定
来源：http://ln.hnjuh.cn

if let n = opt { print(n) }
来源：http://fy.szxytkj.cn

[T20] Swift：数组操作
来源：http://fq.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pm.haigaiapp.cn

[T21] Swift：遍历
来源：http://vz.hnjuh.cn

for x in a { print(x) }
来源：http://qz.bjjhwx.cn

[T22] Swift：字典
来源：http://lq.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cf.shxzukj.cn

[T23] Swift：函数
来源：http://nn.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ms.wgjwhj.cn

[T24] Swift：闭包
来源：http://zg.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sk.szxytkj.cn

[T25] Swift：结构体
来源：http://qr.nicolike.cn

struct P { var x: Int }
来源：http://dr.asd995.cn

[T26] Swift：类与重写
来源：http://pt.gzmigu.cn

class A: Base { override func f() {} }
来源：http://tm.shxzskj.cn

[T27] Swift：错误处理
来源：http://dk.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://gk.panjiajie.cn

[T28] Swift：枚举
来源：http://pw.hnjuh.cn

enum Color { case red, green }
来源：http://ls.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://yh.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://gy.hnjuh.cn

[T30] Swift：协议
来源：http://oa.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://ef.nicolike.cn

[T31] Lua：Hello World
来源：http://ln.yuexingan06.cn

print("Hello")
来源：http://kx.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://te.colortex.cn

local a = 1
来源：http://nj.colortex.cn

[T33] Lua：表（数组）
来源：http://ri.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qj.521024.cn

[T34] Lua：遍历表
来源：http://dk.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ix.szxytkj.cn

[T35] Lua：字典表
来源：http://vm.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://mb.colortex.cn

[T36] Lua：函数
来源：http://zy.jctech888.com.cn

function add(a, b) return a + b end
来源：http://gw.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://sl.haigaiapp.cn

"a" .. "b"
来源：http://gx.huixinmuqiang.cn

[T38] Lua：条件
来源：http://sy.nszjky.cn

if x > 0 then print("正") end
来源：http://cl.nszjky.cn

[T39] Lua：模式匹配
来源：http://hu.panjiajie.cn

string.find(s, "%d+")
来源：http://wo.yuntaijiaju.cn

[T40] Lua：元表
来源：http://cn.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://au.yuexingan06.cn

[T41] Perl：Hello World
来源：http://wp.gzmigu.cn

print "Hello\n";
来源：http://eg.shtwfgs.cn

[T42] Perl：变量类型
来源：http://kx.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vt.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://bt.bjjhwx.cn

"值: $a"
来源：http://bd.jctech888.com.cn

[T44] Perl：条件
来源：http://dr.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://cl.shxzskj.cn

[T45] Perl：数组遍历
来源：http://eg.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://ll.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://sg.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uh.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://zt.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jw.nszjky.cn

[T48] Perl：正则替换
来源：http://sw.panjiajie.cn

$s =~ s/old/new/g;
来源：http://or.szxytkj.cn


<!-- 参考信息 -->