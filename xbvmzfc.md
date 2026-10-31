代发 wailian999

cmd > out.log 2>&1
来源：http://jv.colortex.cn

[R40] 追加写日志
来源：http://os.huixiangedu.cn

echo "log" >> out.log
来源：http://bg.huanxung.cn

[R41] 丢弃输出
来源：http://an.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://um.haigaiapp.cn

[R42] 输入重定向
来源：http://xq.shtwfgs.cn

wc -l < a.txt
来源：http://re.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://fz.panjiajie.cn

find . -name "*.log" -type f
来源：http://vx.jctech888.com.cn

[R44] 按修改时间查找
来源：http://wz.gzmigu.cn

find . -mtime -7 -type f
来源：http://sy.yuntaijiaju.cn

[R45] 批量删除
来源：http://aa.521024.cn

find . -name "*.tmp" -delete
来源：http://qt.nicolike.cn

[R46] 递归替换文件内容
来源：http://qg.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ae.lnxyls.cn

[R47] sed 单行替换
来源：http://im.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lw.wgjwhj.cn

[R48] awk 取指定列
来源：http://at.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://vg.newstarts.cn

[R49] awk 带条件
来源：http://yk.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hj.asd995.cn

[R50] awk 求和
来源：http://iu.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uj.szxytkj.cn

[R51] 排序去重取前几
来源：http://xt.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kh.yuntaijiaju.cn

[R52] 统计行数
来源：http://yi.szxytkj.cn

wc -l a.txt
来源：http://fy.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://uh.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tc.panjiajie.cn

[R54] 比较两个文件
来源：http://zm.jianghongdianzi.cn

diff a.txt b.txt
来源：http://lw.huanxung.cn

[R55] 压缩与解压
来源：http://ws.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jm.gzmigu.cn

[R56] 远程拷贝
来源：http://zg.jctech888.com.cn

scp file user@host:/path/
来源：http://nj.chemitech.net.cn

[R57] 远程执行命令
来源：http://yb.nicolike.cn

ssh user@host 'uptime'
来源：http://rg.gzmigu.cn

[R58] 下载文件
来源：http://qv.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nb.hahajie.cn

[R59] 发 POST JSON
来源：http://mi.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tz.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://wc.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ca.9csxet.cn

[R61] 磁盘占用
来源：http://fq.jianghongdianzi.cn

df -h;  du -sh *
来源：http://cm.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://ov.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://jq.wgjwhj.cn

[R63] 内存与进程
来源：http://sp.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://hl.lnxyls.cn

[R64] 结束进程
来源：http://se.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://az.yuexingan06.cn

[R65] 查看端口占用
来源：http://za.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dt.jianghongdianzi.cn

[R66] 定时任务
来源：http://fu.wgjwhj.cn

crontab -e;  crontab -l
来源：http://fq.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://up.shtwfgs.cn

openssl rand -hex 16
来源：http://kb.nszjky.cn

[R68] 计算文件校验值
来源：http://ve.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fq.muxihuayi.cn

[R69] 生成随机密码
来源：http://rs.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://vf.nicolike.cn

[R70] 时间戳与互转
来源：http://wm.huanxung.cn

date +%s;  date -d @1700000000
来源：http://eu.muxihuayi.cn

[R71] 日期格式化
来源：http://nk.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yf.szxytkj.cn

[R72] 等待端口就绪
来源：http://in.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zz.nicolike.cn

[R73] 分割大日志
来源：http://co.hahajie.cn

split -l 1000 big.log part_
来源：http://la.panjiajie.cn

[R74] 批量重命名
来源：http://zw.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qj.szsharing.cn

[R75] 导出环境变量
来源：http://ao.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://gs.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://wh.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xw.hahajie.cn

[R77] 读取用户输入
来源：http://ij.shxzukj.cn

read -rp "请输入: " ans
来源：http://fo.huanxung.cn

[R78] 交互式菜单
来源：http://by.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eo.newstarts.cn

[R79] 解析命令行选项
来源：http://xs.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xf.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://tk.hnjuh.cn

time ./run.sh
来源：http://fp.shxzukj.cn

================================================================================
来源：http://wh.muxihuayi.cn

S. C / C++ 专题
来源：http://bv.szxytkj.cn

================================================================================
来源：http://oc.lnxyls.cn

[S01] C：Hello World
来源：http://dh.haigaiapp.cn

#include <stdio.h>
来源：http://dd.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yi.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://wy.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://ku.huixinmuqiang.cn

[S03] C：读入整数
来源：http://cr.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://xb.jctech888.com.cn

[S04] C：字符串复制
来源：http://mz.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dn.panjiajie.cn

[S05] C：字符串长度
来源：http://iw.hnjuh.cn

strlen(s)
来源：http://tu.shxzskj.cn

[S06] C：字符串比较
来源：http://mh.bjjhwx.cn

strcmp(a, b) == 0
来源：http://ve.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://pe.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qk.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://sz.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://al.asd995.cn

[S09] C：结构体定义与初始化
来源：http://lb.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mn.9csxet.cn

[S10] C：指针与解引用
来源：http://es.newstarts.cn

int *p = &a;  *p = 5;
来源：http://uy.shxzskj.cn

[S11] C：逐行读文件
来源：http://qf.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://fe.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sk.bjjhwx.cn

fclose(f);
来源：http://nr.muxihuayi.cn

[S12] C：写文件
来源：http://bc.szxytkj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vf.huanxung.cn

[S13] C：宏定义
来源：http://pj.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ax.9csxet.cn

[S14] C：枚举
来源：http://bd.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://si.wgjwhj.cn

[S15] C：类型转换
来源：http://yf.nicolike.cn

(double) a / b
来源：http://mq.wgjwhj.cn

[S16] C：位操作置位
来源：http://hg.9csxet.cn

x |= (1 << 3);
来源：http://hp.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://gu.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fj.haigaiapp.cn

[S18] C：命令行参数
来源：http://hm.huixiangedu.cn

int main(int argc, char **argv)
来源：http://hq.yuntaijiaju.cn

[S19] C：快速排序
来源：http://lk.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wc.bookmarksfly.cn

[S20] C：二分查找
来源：http://cp.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lc.panjiajie.cn

[S21] C：字符类别判断
来源：http://rk.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cv.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://yd.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yg.nszjky.cn

[S23] C：随机数
来源：http://ps.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zy.haigaiapp.cn

[S24] C：获取本地时间
来源：http://ff.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fz.panjiajie.cn

[S25] C：内存拷贝
来源：http://hj.colortex.cn

memcpy(dst, src, n);
来源：http://ky.shxzskj.cn

[S26] C：内存清零
来源：http://kr.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://wm.nicolike.cn

[S27] C：定义常量
来源：http://ja.shtwfgs.cn

const double PI = 3.14159;
来源：http://ip.shxzukj.cn

[S28] C：静态变量
来源：http://mp.asd995.cn

static int counter = 0;
来源：http://gy.shxzskj.cn

[S29] C：变参函数
来源：http://lr.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vo.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://wt.gzmigu.cn

#ifndef X_H
来源：http://of.gzmigu.cn

#define X_H
来源：http://up.asd995.cn

#endif
来源：http://df.colortex.cn

[S31] C++：Hello World
来源：http://ow.newstarts.cn

#include <iostream>
来源：http://ej.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://pv.shxzskj.cn

[S32] C++：字符串
来源：http://zo.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://ga.shxzskj.cn

[S33] C++：vector 增删
来源：http://an.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fe.521024.cn

[S34] C++：遍历 vector
来源：http://ko.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://rt.yuntaijiaju.cn

[S35] C++：map
来源：http://ex.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pw.hnjuh.cn

[S36] C++：unordered_map
来源：http://gc.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iy.yuntaijiaju.cn

[S37] C++：set
来源：http://zw.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jk.muxihuayi.cn

[S38] C++：排序
来源：http://yw.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://ub.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://fc.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ua.huanxung.cn

[S40] C++：查找元素
来源：http://hq.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hy.9csxet.cn

[S41] C++：类与构造函数
来源：http://km.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ig.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://tp.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://kx.chemitech.net.cn

[S43] C++：智能指针
来源：http://jl.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://af.chemitech.net.cn

[S44] C++：引用传参
来源：http://oj.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://vx.haigaiapp.cn

[S45] C++：lambda
来源：http://pu.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ma.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://oz.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vn.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://qb.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xr.nicolike.cn

[S48] C++：逐行读文件
来源：http://mt.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://so.szsharing.cn

while (std::getline(in, line)) { }
来源：http://et.panjiajie.cn

[S49] C++：写文件
来源：http://hy.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vj.newstarts.cn

[S50] C++：格式化数字
来源：http://af.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hr.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://br.colortex.cn

static_cast<double>(a) / b
来源：http://wy.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://dz.colortex.cn

int size() const noexcept { return n_; }
来源：http://om.lnxyls.cn

[S53] C++：移动语义
来源：http://ra.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://qc.hahajie.cn

[S54] C++：异常处理
来源：http://yp.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mq.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://fi.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dn.shtwfgs.cn

[S56] C++：optional
来源：http://fw.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://og.colortex.cn

[S57] C++：编译期常量
来源：http://pm.gzmigu.cn

constexpr int N = 10;
来源：http://ii.9csxet.cn

[S58] C++：命名空间
来源：http://ie.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://hx.huixiangedu.cn

[S59] C++：静态断言
来源：http://sm.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qx.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://hm.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aw.lnxyls.cn

================================================================================
来源：http://yu.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nw.shxzukj.cn

================================================================================
来源：http://ds.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://pr.nszjky.cn

println("Hello")
来源：http://mk.huanxung.cn

[T02] Kotlin：变量
来源：http://jl.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lp.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://cn.nszjky.cn

"值: $b"
来源：http://rr.szxytkj.cn

[T04] Kotlin：空安全
来源：http://ct.shxzskj.cn

val n: String? = null;  n?.length
来源：http://cy.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://db.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ia.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://dr.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://of.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://ls.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bp.gzmigu.cn

[T08] Kotlin：数据类
来源：http://tk.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://ne.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://mi.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://gr.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://fh.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tm.colortex.cn

[T11] Kotlin：协程
来源：http://vt.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wa.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://ew.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://fw.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://eq.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://zs.9csxet.cn

[T14] Kotlin：循环
来源：http://lv.szxytkj.cn

for (i in 1..10) println(i)
来源：http://ce.wgjwhj.cn

[T15] Kotlin：接口
来源：http://do.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://kl.muxihuayi.cn

[T16] Swift：Hello World
来源：http://ke.panjiajie.cn

print("Hello")
来源：http://bo.colortex.cn

[T17] Swift：变量与常量
来源：http://nv.521024.cn

var a = 1;  let b = 2
来源：http://ik.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://rs.newstarts.cn

"值: \(b)"
来源：http://lu.nszjky.cn

[T19] Swift：可选绑定
来源：http://ix.asd995.cn

if let n = opt { print(n) }
来源：http://va.bjjhwx.cn

[T20] Swift：数组操作
来源：http://jc.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qu.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://oi.huanxung.cn

for x in a { print(x) }
来源：http://jc.yuntaijiaju.cn

[T22] Swift：字典
来源：http://ce.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bo.huixinmuqiang.cn

[T23] Swift：函数
来源：http://ci.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qe.chemitech.net.cn

[T24] Swift：闭包
来源：http://ym.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lj.shxzskj.cn

[T25] Swift：结构体
来源：http://ou.yuexingan06.cn

struct P { var x: Int }
来源：http://pq.hnjuh.cn

[T26] Swift：类与重写
来源：http://cq.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://ow.bjjhwx.cn

[T27] Swift：错误处理
来源：http://le.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://fw.521024.cn

[T28] Swift：枚举
来源：http://wi.szsharing.cn

enum Color { case red, green }
来源：http://wx.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://ic.shtwfgs.cn

guard let x = opt else { return }
来源：http://ot.huixiangedu.cn

[T30] Swift：协议
来源：http://up.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://ds.huixiangedu.cn

[T31] Lua：Hello World
来源：http://cb.hnjuh.cn

print("Hello")
来源：http://ja.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://wp.shxzskj.cn

local a = 1
来源：http://bw.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://yj.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xo.szsharing.cn

[T34] Lua：遍历表
来源：http://tx.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pm.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://xn.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://wl.shtwfgs.cn

[T36] Lua：函数
来源：http://yi.9csxet.cn

function add(a, b) return a + b end
来源：http://vr.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://op.nicolike.cn

"a" .. "b"
来源：http://rz.hahajie.cn

[T38] Lua：条件
来源：http://mn.huixiangedu.cn

if x > 0 then print("正") end
来源：http://gv.hahajie.cn

[T39] Lua：模式匹配
来源：http://fv.newstarts.cn

string.find(s, "%d+")
来源：http://dw.9csxet.cn

[T40] Lua：元表
来源：http://wc.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://qo.gzmigu.cn

[T41] Perl：Hello World
来源：http://uw.szsharing.cn

print "Hello\n";
来源：http://co.szxytkj.cn

[T42] Perl：变量类型
来源：http://vz.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nu.521024.cn


<!-- 参考信息 -->