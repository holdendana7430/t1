代发 wailian999

cmd >/dev/null 2>&1
来源：http://jm.newstarts.cn

[R42] 输入重定向
来源：http://fd.chemitech.net.cn

wc -l < a.txt
来源：http://ey.lnxyls.cn

[R43] 按名字查找文件
来源：http://yv.9csxet.cn

find . -name "*.log" -type f
来源：http://th.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://zj.chemitech.net.cn

find . -mtime -7 -type f
来源：http://kq.yuntaijiaju.cn

[R45] 批量删除
来源：http://xz.newstarts.cn

find . -name "*.tmp" -delete
来源：http://kk.szxytkj.cn

[R46] 递归替换文件内容
来源：http://sk.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rp.panjiajie.cn

[R47] sed 单行替换
来源：http://gb.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ct.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://xm.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://fh.jianghongdianzi.cn

[R49] awk 带条件
来源：http://py.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ej.muxihuayi.cn

[R50] awk 求和
来源：http://lt.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bp.newstarts.cn

[R51] 排序去重取前几
来源：http://hm.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://em.yuexingan06.cn

[R52] 统计行数
来源：http://yh.wgjwhj.cn

wc -l a.txt
来源：http://sr.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://ql.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kz.colortex.cn

[R54] 比较两个文件
来源：http://ox.haigaiapp.cn

diff a.txt b.txt
来源：http://fa.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://qp.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nf.szsharing.cn

[R56] 远程拷贝
来源：http://wt.huanxung.cn

scp file user@host:/path/
来源：http://nx.hnjuh.cn

[R57] 远程执行命令
来源：http://lo.muxihuayi.cn

ssh user@host 'uptime'
来源：http://hn.521024.cn

[R58] 下载文件
来源：http://si.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mn.521024.cn

[R59] 发 POST JSON
来源：http://vd.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zq.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://kt.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uw.chemitech.net.cn

[R61] 磁盘占用
来源：http://jh.haigaiapp.cn

df -h;  du -sh *
来源：http://rv.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://af.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://op.huanxung.cn

[R63] 内存与进程
来源：http://pv.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://kx.shxzskj.cn

[R64] 结束进程
来源：http://qv.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://di.haigaiapp.cn

[R65] 查看端口占用
来源：http://ns.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dw.jianghongdianzi.cn

[R66] 定时任务
来源：http://to.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://dn.newstarts.cn

[R67] 生成随机十六进制串
来源：http://rp.colortex.cn

openssl rand -hex 16
来源：http://qs.9csxet.cn

[R68] 计算文件校验值
来源：http://ll.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ko.huixiangedu.cn

[R69] 生成随机密码
来源：http://pb.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://vh.bjjhwx.cn

[R70] 时间戳与互转
来源：http://oy.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://xs.szsharing.cn

[R71] 日期格式化
来源：http://bx.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jp.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://ys.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qn.huixiangedu.cn

[R73] 分割大日志
来源：http://gf.yuexingan06.cn

split -l 1000 big.log part_
来源：http://ld.shtwfgs.cn

[R74] 批量重命名
来源：http://et.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hu.chemitech.net.cn

[R75] 导出环境变量
来源：http://bv.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://nm.shtwfgs.cn

[R76] 使用临时文件
来源：http://rr.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vw.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://zn.chemitech.net.cn

read -rp "请输入: " ans
来源：http://gt.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://hh.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sn.huanxung.cn

[R79] 解析命令行选项
来源：http://il.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yp.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://dq.shxzukj.cn

time ./run.sh
来源：http://yu.colortex.cn

================================================================================
来源：http://kt.shxzukj.cn

S. C / C++ 专题
来源：http://sz.nicolike.cn

================================================================================
来源：http://vk.bjjhwx.cn

[S01] C：Hello World
来源：http://of.bjjhwx.cn

#include <stdio.h>
来源：http://yv.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kx.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://ra.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://co.panjiajie.cn

[S03] C：读入整数
来源：http://fa.newstarts.cn

int x; scanf("%d", &x);
来源：http://mv.hnjuh.cn

[S04] C：字符串复制
来源：http://mf.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tr.shxzskj.cn

[S05] C：字符串长度
来源：http://ly.shxzukj.cn

strlen(s)
来源：http://kz.chemitech.net.cn

[S06] C：字符串比较
来源：http://zp.gzmigu.cn

strcmp(a, b) == 0
来源：http://mx.521024.cn

[S07] C：数组遍历求和
来源：http://ni.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ke.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://xu.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cl.colortex.cn

[S09] C：结构体定义与初始化
来源：http://go.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bp.lnxyls.cn

[S10] C：指针与解引用
来源：http://wk.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://qi.lnxyls.cn

[S11] C：逐行读文件
来源：http://vn.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://vc.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://at.lnxyls.cn

fclose(f);
来源：http://rz.nicolike.cn

[S12] C：写文件
来源：http://kf.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ht.newstarts.cn

[S13] C：宏定义
来源：http://is.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vk.nszjky.cn

[S14] C：枚举
来源：http://ps.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://iq.szsharing.cn

[S15] C：类型转换
来源：http://mz.huanxung.cn

(double) a / b
来源：http://de.colortex.cn

[S16] C：位操作置位
来源：http://er.gzmigu.cn

x |= (1 << 3);
来源：http://pu.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://kk.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uj.colortex.cn

[S18] C：命令行参数
来源：http://mu.521024.cn

int main(int argc, char **argv)
来源：http://vo.shxzukj.cn

[S19] C：快速排序
来源：http://fz.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tp.521024.cn

[S20] C：二分查找
来源：http://kn.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ew.9csxet.cn

[S21] C：字符类别判断
来源：http://hp.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pl.lnxyls.cn

[S22] C：字符串转数字
来源：http://lv.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pm.gzmigu.cn

[S23] C：随机数
来源：http://ox.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fc.wgjwhj.cn

[S24] C：获取本地时间
来源：http://jy.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vl.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://va.colortex.cn

memcpy(dst, src, n);
来源：http://av.jianghongdianzi.cn

[S26] C：内存清零
来源：http://mh.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://cn.hnjuh.cn

[S27] C：定义常量
来源：http://bv.yuexingan06.cn

const double PI = 3.14159;
来源：http://ex.huanxung.cn

[S28] C：静态变量
来源：http://je.colortex.cn

static int counter = 0;
来源：http://bs.nicolike.cn

[S29] C：变参函数
来源：http://uw.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gf.shxzskj.cn

[S30] C：头文件保护
来源：http://hc.muxihuayi.cn

#ifndef X_H
来源：http://uy.shxzukj.cn

#define X_H
来源：http://dr.haigaiapp.cn

#endif
来源：http://nq.asd995.cn

[S31] C++：Hello World
来源：http://vu.nszjky.cn

#include <iostream>
来源：http://ti.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://um.yuexingan06.cn

[S32] C++：字符串
来源：http://yv.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://wz.newstarts.cn

[S33] C++：vector 增删
来源：http://pw.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cu.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://zo.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://cc.szxytkj.cn

[S35] C++：map
来源：http://zb.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vb.chemitech.net.cn

[S36] C++：unordered_map
来源：http://tm.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sr.yuexingan06.cn

[S37] C++：set
来源：http://au.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yl.panjiajie.cn

[S38] C++：排序
来源：http://er.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://zg.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://rc.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pa.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://bk.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rf.hnjuh.cn

[S41] C++：类与构造函数
来源：http://pk.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bk.asd995.cn

[S42] C++：继承与虚函数
来源：http://gh.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://si.shtwfgs.cn

[S43] C++：智能指针
来源：http://gs.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://iq.yuexingan06.cn

[S44] C++：引用传参
来源：http://ei.521024.cn

void inc(int &x) { ++x; }
来源：http://ro.haigaiapp.cn

[S45] C++：lambda
来源：http://fl.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bt.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://zf.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bh.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://zd.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ic.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://wp.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oo.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://bo.jctech888.com.cn

[S49] C++：写文件
来源：http://sa.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nn.shxzukj.cn

[S50] C++：格式化数字
来源：http://ih.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bl.gzmigu.cn

[S51] C++：显式类型转换
来源：http://dd.shtwfgs.cn

static_cast<double>(a) / b
来源：http://ic.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://or.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://le.hahajie.cn

[S53] C++：移动语义
来源：http://ic.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://lo.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://jw.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tu.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://fk.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://at.nicolike.cn

[S56] C++：optional
来源：http://mg.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fd.shxzukj.cn

[S57] C++：编译期常量
来源：http://um.nszjky.cn

constexpr int N = 10;
来源：http://nw.521024.cn

[S58] C++：命名空间
来源：http://iw.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://fk.wgjwhj.cn

[S59] C++：静态断言
来源：http://bl.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gj.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://et.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vp.yuexingan06.cn

================================================================================
来源：http://ha.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tp.huixiangedu.cn

================================================================================
来源：http://mn.colortex.cn

[T01] Kotlin：Hello World
来源：http://ak.hahajie.cn

println("Hello")
来源：http://xs.wgjwhj.cn

[T02] Kotlin：变量
来源：http://vy.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xg.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://vy.huanxung.cn

"值: $b"
来源：http://ea.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://jf.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://fx.521024.cn

[T05] Kotlin：when 表达式
来源：http://se.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ba.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://rt.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oz.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://yg.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://af.szxytkj.cn

[T08] Kotlin：数据类
来源：http://mp.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://wl.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://im.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://pd.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://by.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yx.jctech888.com.cn

[T11] Kotlin：协程
来源：http://mf.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://il.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://xv.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://bc.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://lk.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://nr.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://qo.hnjuh.cn

for (i in 1..10) println(i)
来源：http://tz.bjjhwx.cn

[T15] Kotlin：接口
来源：http://fe.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://mv.jctech888.com.cn

[T16] Swift：Hello World
来源：http://ey.wgjwhj.cn

print("Hello")
来源：http://yo.nszjky.cn

[T17] Swift：变量与常量
来源：http://wn.asd995.cn

var a = 1;  let b = 2
来源：http://ij.hnjuh.cn

[T18] Swift：字符串插值
来源：http://ha.gzmigu.cn

"值: \(b)"
来源：http://su.9csxet.cn

[T19] Swift：可选绑定
来源：http://dh.521024.cn

if let n = opt { print(n) }
来源：http://na.shxzskj.cn

[T20] Swift：数组操作
来源：http://ca.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mi.newstarts.cn

[T21] Swift：遍历
来源：http://sn.huixinmuqiang.cn

for x in a { print(x) }
来源：http://ye.521024.cn

[T22] Swift：字典
来源：http://zm.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wn.szxytkj.cn

[T23] Swift：函数
来源：http://ju.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://op.shxzskj.cn

[T24] Swift：闭包
来源：http://bj.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ru.shxzukj.cn

[T25] Swift：结构体
来源：http://xo.bookmarksfly.cn

struct P { var x: Int }
来源：http://uo.jctech888.com.cn

[T26] Swift：类与重写
来源：http://sx.nicolike.cn

class A: Base { override func f() {} }
来源：http://lk.shxzskj.cn

[T27] Swift：错误处理
来源：http://rk.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://xo.wgjwhj.cn

[T28] Swift：枚举
来源：http://su.yuntaijiaju.cn

enum Color { case red, green }
来源：http://as.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://su.newstarts.cn

guard let x = opt else { return }
来源：http://vd.jctech888.com.cn

[T30] Swift：协议
来源：http://dk.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://du.nszjky.cn

[T31] Lua：Hello World
来源：http://kk.shxzukj.cn

print("Hello")
来源：http://rw.haigaiapp.cn

[T32] Lua：局部变量
来源：http://bh.yuexingan06.cn

local a = 1
来源：http://qz.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://sw.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cf.lnxyls.cn

[T34] Lua：遍历表
来源：http://yx.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cm.9csxet.cn

[T35] Lua：字典表
来源：http://fb.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://lo.hnjuh.cn

[T36] Lua：函数
来源：http://jb.wgjwhj.cn

function add(a, b) return a + b end
来源：http://nm.hahajie.cn

[T37] Lua：字符串拼接
来源：http://zi.haigaiapp.cn

"a" .. "b"
来源：http://fc.shtwfgs.cn

[T38] Lua：条件
来源：http://mf.shxzukj.cn

if x > 0 then print("正") end
来源：http://am.9csxet.cn

[T39] Lua：模式匹配
来源：http://lq.newstarts.cn

string.find(s, "%d+")
来源：http://dt.hahajie.cn

[T40] Lua：元表
来源：http://yg.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://qo.hnjuh.cn

[T41] Perl：Hello World
来源：http://re.9csxet.cn

print "Hello\n";
来源：http://je.szsharing.cn

[T42] Perl：变量类型
来源：http://kl.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zg.521024.cn

[T43] Perl：字符串插值
来源：http://ad.jctech888.com.cn

"值: $a"
来源：http://wo.hnjuh.cn

[T44] Perl：条件
来源：http://tn.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://vv.yuntaijiaju.cn


<!-- 参考信息 -->