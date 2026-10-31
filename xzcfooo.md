代发 wailian999

find . -name "*.log" -type f
来源：http://mb.hnjuh.cn

[R44] 按修改时间查找
来源：http://te.9csxet.cn

find . -mtime -7 -type f
来源：http://qn.newstarts.cn

[R45] 批量删除
来源：http://ot.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://gd.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://si.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gz.hnjuh.cn

[R47] sed 单行替换
来源：http://sw.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://be.newstarts.cn

[R48] awk 取指定列
来源：http://pz.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://om.nszjky.cn

[R49] awk 带条件
来源：http://vy.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ix.colortex.cn

[R50] awk 求和
来源：http://kp.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sa.chemitech.net.cn

[R51] 排序去重取前几
来源：http://lj.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qz.jctech888.com.cn

[R52] 统计行数
来源：http://pj.bjjhwx.cn

wc -l a.txt
来源：http://lj.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://of.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yl.gzmigu.cn

[R54] 比较两个文件
来源：http://wa.newstarts.cn

diff a.txt b.txt
来源：http://fj.colortex.cn

[R55] 压缩与解压
来源：http://qn.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://um.hahajie.cn

[R56] 远程拷贝
来源：http://zz.bookmarksfly.cn

scp file user@host:/path/
来源：http://xd.jctech888.com.cn

[R57] 远程执行命令
来源：http://tk.colortex.cn

ssh user@host 'uptime'
来源：http://bd.haigaiapp.cn

[R58] 下载文件
来源：http://uj.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zo.shxzukj.cn

[R59] 发 POST JSON
来源：http://cz.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yf.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://go.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uh.chemitech.net.cn

[R61] 磁盘占用
来源：http://qy.szsharing.cn

df -h;  du -sh *
来源：http://vq.panjiajie.cn

[R62] 找最占空间的文件
来源：http://lm.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://zb.chemitech.net.cn

[R63] 内存与进程
来源：http://bw.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://pd.nicolike.cn

[R64] 结束进程
来源：http://oa.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://ku.shtwfgs.cn

[R65] 查看端口占用
来源：http://de.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://od.huanxung.cn

[R66] 定时任务
来源：http://so.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://tx.colortex.cn

[R67] 生成随机十六进制串
来源：http://pn.lnxyls.cn

openssl rand -hex 16
来源：http://yh.9csxet.cn

[R68] 计算文件校验值
来源：http://il.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cc.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://jv.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://dq.nszjky.cn

[R70] 时间戳与互转
来源：http://ze.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://od.nszjky.cn

[R71] 日期格式化
来源：http://wk.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lu.521024.cn

[R72] 等待端口就绪
来源：http://rw.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://et.panjiajie.cn

[R73] 分割大日志
来源：http://su.shtwfgs.cn

split -l 1000 big.log part_
来源：http://iv.yuexingan06.cn

[R74] 批量重命名
来源：http://cx.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lm.colortex.cn

[R75] 导出环境变量
来源：http://if.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://wy.szsharing.cn

[R76] 使用临时文件
来源：http://pp.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ub.colortex.cn

[R77] 读取用户输入
来源：http://ow.jctech888.com.cn

read -rp "请输入: " ans
来源：http://uc.bjjhwx.cn

[R78] 交互式菜单
来源：http://kb.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ez.nicolike.cn

[R79] 解析命令行选项
来源：http://qr.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tz.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://tk.huixiangedu.cn

time ./run.sh
来源：http://ty.gzmigu.cn

================================================================================
来源：http://os.yuexingan06.cn

S. C / C++ 专题
来源：http://ju.gzmigu.cn

================================================================================
来源：http://tj.9csxet.cn

[S01] C：Hello World
来源：http://ru.lnxyls.cn

#include <stdio.h>
来源：http://oq.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ry.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://kw.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://ju.huixiangedu.cn

[S03] C：读入整数
来源：http://lr.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://fw.wgjwhj.cn

[S04] C：字符串复制
来源：http://qt.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jl.9csxet.cn

[S05] C：字符串长度
来源：http://fi.yuntaijiaju.cn

strlen(s)
来源：http://lr.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://no.shxzskj.cn

strcmp(a, b) == 0
来源：http://is.panjiajie.cn

[S07] C：数组遍历求和
来源：http://pd.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xf.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://xd.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://by.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://rx.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vf.huixiangedu.cn

[S10] C：指针与解引用
来源：http://dx.newstarts.cn

int *p = &a;  *p = 5;
来源：http://mz.huanxung.cn

[S11] C：逐行读文件
来源：http://pj.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://mn.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rq.shtwfgs.cn

fclose(f);
来源：http://ri.shtwfgs.cn

[S12] C：写文件
来源：http://sb.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yd.chemitech.net.cn

[S13] C：宏定义
来源：http://ng.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yr.newstarts.cn

[S14] C：枚举
来源：http://be.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://nh.9csxet.cn

[S15] C：类型转换
来源：http://uk.nszjky.cn

(double) a / b
来源：http://rf.nszjky.cn

[S16] C：位操作置位
来源：http://kc.shxzukj.cn

x |= (1 << 3);
来源：http://hd.hahajie.cn

[S17] C：安全拼接字符串
来源：http://ws.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cv.shtwfgs.cn

[S18] C：命令行参数
来源：http://ob.hahajie.cn

int main(int argc, char **argv)
来源：http://uo.wgjwhj.cn

[S19] C：快速排序
来源：http://lx.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jy.521024.cn

[S20] C：二分查找
来源：http://hx.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tc.szxytkj.cn

[S21] C：字符类别判断
来源：http://en.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ph.521024.cn

[S22] C：字符串转数字
来源：http://ke.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://je.yuntaijiaju.cn

[S23] C：随机数
来源：http://gp.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uk.panjiajie.cn

[S24] C：获取本地时间
来源：http://wc.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xz.nicolike.cn

[S25] C：内存拷贝
来源：http://fj.huanxung.cn

memcpy(dst, src, n);
来源：http://zv.jianghongdianzi.cn

[S26] C：内存清零
来源：http://pi.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://mc.newstarts.cn

[S27] C：定义常量
来源：http://gj.szsharing.cn

const double PI = 3.14159;
来源：http://br.newstarts.cn

[S28] C：静态变量
来源：http://if.nicolike.cn

static int counter = 0;
来源：http://nv.huixinmuqiang.cn

[S29] C：变参函数
来源：http://iw.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fn.asd995.cn

[S30] C：头文件保护
来源：http://dc.huixiangedu.cn

#ifndef X_H
来源：http://yu.szsharing.cn

#define X_H
来源：http://wk.shtwfgs.cn

#endif
来源：http://rj.panjiajie.cn

[S31] C++：Hello World
来源：http://vx.panjiajie.cn

#include <iostream>
来源：http://pr.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://gw.9csxet.cn

[S32] C++：字符串
来源：http://ha.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://pq.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://xk.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ia.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://xf.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://gg.hahajie.cn

[S35] C++：map
来源：http://cc.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ef.shxzukj.cn

[S36] C++：unordered_map
来源：http://ld.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lp.huixinmuqiang.cn

[S37] C++：set
来源：http://ss.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gh.wgjwhj.cn

[S38] C++：排序
来源：http://cb.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://mb.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://vb.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ex.shxzskj.cn

[S40] C++：查找元素
来源：http://be.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bt.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://sk.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vm.asd995.cn

[S42] C++：继承与虚函数
来源：http://qc.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://fm.muxihuayi.cn

[S43] C++：智能指针
来源：http://ti.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://pp.bjjhwx.cn

[S44] C++：引用传参
来源：http://ch.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://jm.szsharing.cn

[S45] C++：lambda
来源：http://xh.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ba.wgjwhj.cn

[S46] C++：函数模板
来源：http://qp.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zc.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://fk.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cy.huanxung.cn

[S48] C++：逐行读文件
来源：http://he.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gn.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://gl.521024.cn

[S49] C++：写文件
来源：http://pd.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uy.colortex.cn

[S50] C++：格式化数字
来源：http://gm.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ux.gzmigu.cn

[S51] C++：显式类型转换
来源：http://fc.muxihuayi.cn

static_cast<double>(a) / b
来源：http://vp.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://qu.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://ou.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://uw.asd995.cn

std::vector<int> w = std::move(v);
来源：http://ps.hnjuh.cn

[S54] C++：异常处理
来源：http://ea.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vq.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://vv.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ft.jianghongdianzi.cn

[S56] C++：optional
来源：http://lq.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mq.hnjuh.cn

[S57] C++：编译期常量
来源：http://bo.shxzukj.cn

constexpr int N = 10;
来源：http://zn.yuexingan06.cn

[S58] C++：命名空间
来源：http://gm.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://as.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://gf.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ey.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://hn.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://go.wgjwhj.cn

================================================================================
来源：http://ta.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ih.muxihuayi.cn

================================================================================
来源：http://tl.nicolike.cn

[T01] Kotlin：Hello World
来源：http://vr.nszjky.cn

println("Hello")
来源：http://ec.bjjhwx.cn

[T02] Kotlin：变量
来源：http://no.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vd.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://rz.asd995.cn

"值: $b"
来源：http://zz.szsharing.cn

[T04] Kotlin：空安全
来源：http://yp.szsharing.cn

val n: String? = null;  n?.length
来源：http://os.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://ly.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zp.nszjky.cn

[T06] Kotlin：集合映射
来源：http://qf.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gh.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://mo.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zx.nicolike.cn

[T08] Kotlin：数据类
来源：http://pm.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://lc.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://jp.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://dv.huanxung.cn

[T10] Kotlin：默认参数
来源：http://uq.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hj.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://me.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dw.huanxung.cn

[T12] Kotlin：解构声明
来源：http://ft.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://ub.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://yc.9csxet.cn

val m = mapOf("a" to 1)
来源：http://dn.bjjhwx.cn

[T14] Kotlin：循环
来源：http://xn.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://jx.gzmigu.cn

[T15] Kotlin：接口
来源：http://qx.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://ol.nicolike.cn

[T16] Swift：Hello World
来源：http://hh.haigaiapp.cn

print("Hello")
来源：http://ke.asd995.cn

[T17] Swift：变量与常量
来源：http://if.wgjwhj.cn

var a = 1;  let b = 2
来源：http://pm.hnjuh.cn

[T18] Swift：字符串插值
来源：http://zo.yuntaijiaju.cn

"值: \(b)"
来源：http://rv.nszjky.cn

[T19] Swift：可选绑定
来源：http://zw.newstarts.cn

if let n = opt { print(n) }
来源：http://ql.muxihuayi.cn

[T20] Swift：数组操作
来源：http://dv.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kw.9csxet.cn

[T21] Swift：遍历
来源：http://yy.panjiajie.cn

for x in a { print(x) }
来源：http://am.szsharing.cn

[T22] Swift：字典
来源：http://fi.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fc.huanxung.cn

[T23] Swift：函数
来源：http://br.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nb.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://dl.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vz.lnxyls.cn

[T25] Swift：结构体
来源：http://ba.huixinmuqiang.cn

struct P { var x: Int }
来源：http://th.lnxyls.cn

[T26] Swift：类与重写
来源：http://bx.hahajie.cn

class A: Base { override func f() {} }
来源：http://oo.jctech888.com.cn

[T27] Swift：错误处理
来源：http://kx.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://ha.muxihuayi.cn

[T28] Swift：枚举
来源：http://ng.hahajie.cn

enum Color { case red, green }
来源：http://fh.colortex.cn

[T29] Swift：guard 提前返回
来源：http://zh.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://he.newstarts.cn

[T30] Swift：协议
来源：http://tq.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://kt.panjiajie.cn

[T31] Lua：Hello World
来源：http://uh.9csxet.cn

print("Hello")
来源：http://cs.521024.cn

[T32] Lua：局部变量
来源：http://ti.panjiajie.cn

local a = 1
来源：http://ig.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://cr.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kb.muxihuayi.cn

[T34] Lua：遍历表
来源：http://ki.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qw.hnjuh.cn

[T35] Lua：字典表
来源：http://yr.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://xb.nicolike.cn

[T36] Lua：函数
来源：http://tx.huixiangedu.cn

function add(a, b) return a + b end
来源：http://dn.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://bw.bookmarksfly.cn

"a" .. "b"
来源：http://ie.jianghongdianzi.cn

[T38] Lua：条件
来源：http://cl.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://no.hahajie.cn

[T39] Lua：模式匹配
来源：http://nq.muxihuayi.cn

string.find(s, "%d+")
来源：http://tg.panjiajie.cn

[T40] Lua：元表
来源：http://za.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://ye.panjiajie.cn

[T41] Perl：Hello World
来源：http://tm.shxzskj.cn

print "Hello\n";
来源：http://yp.gzmigu.cn

[T42] Perl：变量类型
来源：http://ab.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zw.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://hq.nszjky.cn

"值: $a"
来源：http://ni.huixiangedu.cn

[T44] Perl：条件
来源：http://xz.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://tc.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://kt.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://ji.shxzskj.cn

[T46] Perl：哈希操作
来源：http://bv.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mu.shxzukj.cn


<!-- 参考信息 -->