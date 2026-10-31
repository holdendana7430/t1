代发 wailian999

find . -name "*.log" -type f
来源：http://lq.bjjhwx.cn

[R44] 按修改时间查找
来源：http://zt.nicolike.cn

find . -mtime -7 -type f
来源：http://pp.gzmigu.cn

[R45] 批量删除
来源：http://zh.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://hi.lnxyls.cn

[R46] 递归替换文件内容
来源：http://pw.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yb.haigaiapp.cn

[R47] sed 单行替换
来源：http://bh.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://df.haigaiapp.cn

[R48] awk 取指定列
来源：http://ss.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://tk.chemitech.net.cn

[R49] awk 带条件
来源：http://mx.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gk.huixiangedu.cn

[R50] awk 求和
来源：http://wl.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ge.huixiangedu.cn

[R51] 排序去重取前几
来源：http://cd.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ry.huixinmuqiang.cn

[R52] 统计行数
来源：http://fa.lnxyls.cn

wc -l a.txt
来源：http://hz.colortex.cn

[R53] 查看文件头与实时尾
来源：http://em.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yc.szsharing.cn

[R54] 比较两个文件
来源：http://lt.newstarts.cn

diff a.txt b.txt
来源：http://yw.lnxyls.cn

[R55] 压缩与解压
来源：http://xg.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pm.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://iu.asd995.cn

scp file user@host:/path/
来源：http://se.521024.cn

[R57] 远程执行命令
来源：http://rh.haigaiapp.cn

ssh user@host 'uptime'
来源：http://oj.huixinmuqiang.cn

[R58] 下载文件
来源：http://wr.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://we.huixiangedu.cn

[R59] 发 POST JSON
来源：http://an.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://di.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://hi.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://td.gzmigu.cn

[R61] 磁盘占用
来源：http://by.huixiangedu.cn

df -h;  du -sh *
来源：http://ea.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://wb.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://jj.newstarts.cn

[R63] 内存与进程
来源：http://jq.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://mn.gzmigu.cn

[R64] 结束进程
来源：http://wu.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://tx.nicolike.cn

[R65] 查看端口占用
来源：http://tf.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://av.szxytkj.cn

[R66] 定时任务
来源：http://yh.hnjuh.cn

crontab -e;  crontab -l
来源：http://yi.newstarts.cn

[R67] 生成随机十六进制串
来源：http://zq.newstarts.cn

openssl rand -hex 16
来源：http://yf.jctech888.com.cn

[R68] 计算文件校验值
来源：http://qu.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ay.hnjuh.cn

[R69] 生成随机密码
来源：http://qs.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://hw.nicolike.cn

[R70] 时间戳与互转
来源：http://fn.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://yf.shxzukj.cn

[R71] 日期格式化
来源：http://eg.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vp.nicolike.cn

[R72] 等待端口就绪
来源：http://dk.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cd.wgjwhj.cn

[R73] 分割大日志
来源：http://bb.lnxyls.cn

split -l 1000 big.log part_
来源：http://sy.yuntaijiaju.cn

[R74] 批量重命名
来源：http://ys.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ng.muxihuayi.cn

[R75] 导出环境变量
来源：http://wk.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://mz.shtwfgs.cn

[R76] 使用临时文件
来源：http://dl.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mv.521024.cn

[R77] 读取用户输入
来源：http://vd.lnxyls.cn

read -rp "请输入: " ans
来源：http://ye.jctech888.com.cn

[R78] 交互式菜单
来源：http://rx.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://or.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://vi.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lj.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://qk.haigaiapp.cn

time ./run.sh
来源：http://ci.muxihuayi.cn

================================================================================
来源：http://yd.gzmigu.cn

S. C / C++ 专题
来源：http://pk.huanxung.cn

================================================================================
来源：http://zn.hnjuh.cn

[S01] C：Hello World
来源：http://rr.muxihuayi.cn

#include <stdio.h>
来源：http://pz.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fg.szsharing.cn

[S02] C：变量与格式化输出
来源：http://hm.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://xt.huixinmuqiang.cn

[S03] C：读入整数
来源：http://in.shxzukj.cn

int x; scanf("%d", &x);
来源：http://yj.haigaiapp.cn

[S04] C：字符串复制
来源：http://pe.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ph.haigaiapp.cn

[S05] C：字符串长度
来源：http://tr.hnjuh.cn

strlen(s)
来源：http://hq.nicolike.cn

[S06] C：字符串比较
来源：http://mt.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://my.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://uf.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kc.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://lg.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://es.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://bk.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bu.szsharing.cn

[S10] C：指针与解引用
来源：http://is.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://vn.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://ir.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://ln.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wp.nicolike.cn

fclose(f);
来源：http://pi.shxzskj.cn

[S12] C：写文件
来源：http://vs.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mg.huixinmuqiang.cn

[S13] C：宏定义
来源：http://lw.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gr.huixiangedu.cn

[S14] C：枚举
来源：http://ls.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://ky.wgjwhj.cn

[S15] C：类型转换
来源：http://hq.hnjuh.cn

(double) a / b
来源：http://ox.hnjuh.cn

[S16] C：位操作置位
来源：http://go.shxzskj.cn

x |= (1 << 3);
来源：http://pn.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://yj.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wt.yuexingan06.cn

[S18] C：命令行参数
来源：http://mu.muxihuayi.cn

int main(int argc, char **argv)
来源：http://be.jianghongdianzi.cn

[S19] C：快速排序
来源：http://gj.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xn.shxzukj.cn

[S20] C：二分查找
来源：http://wx.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tg.shxzukj.cn

[S21] C：字符类别判断
来源：http://yw.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://je.nicolike.cn

[S22] C：字符串转数字
来源：http://bb.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bp.gzmigu.cn

[S23] C：随机数
来源：http://uf.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ss.panjiajie.cn

[S24] C：获取本地时间
来源：http://wx.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vw.wgjwhj.cn

[S25] C：内存拷贝
来源：http://hw.hnjuh.cn

memcpy(dst, src, n);
来源：http://nc.bookmarksfly.cn

[S26] C：内存清零
来源：http://sd.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://jn.huixinmuqiang.cn

[S27] C：定义常量
来源：http://nr.newstarts.cn

const double PI = 3.14159;
来源：http://pj.chemitech.net.cn

[S28] C：静态变量
来源：http://on.panjiajie.cn

static int counter = 0;
来源：http://gz.colortex.cn

[S29] C：变参函数
来源：http://rq.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bd.wgjwhj.cn

[S30] C：头文件保护
来源：http://ht.haigaiapp.cn

#ifndef X_H
来源：http://vt.hahajie.cn

#define X_H
来源：http://uu.chemitech.net.cn

#endif
来源：http://nw.hahajie.cn

[S31] C++：Hello World
来源：http://fn.lnxyls.cn

#include <iostream>
来源：http://qv.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://dj.bjjhwx.cn

[S32] C++：字符串
来源：http://ng.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://bx.hahajie.cn

[S33] C++：vector 增删
来源：http://ue.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wg.521024.cn

[S34] C++：遍历 vector
来源：http://wa.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://du.hnjuh.cn

[S35] C++：map
来源：http://zm.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zt.bjjhwx.cn

[S36] C++：unordered_map
来源：http://nq.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uh.bookmarksfly.cn

[S37] C++：set
来源：http://rf.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tp.muxihuayi.cn

[S38] C++：排序
来源：http://ya.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://nj.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://he.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ft.yuexingan06.cn

[S40] C++：查找元素
来源：http://hw.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pa.hnjuh.cn

[S41] C++：类与构造函数
来源：http://zq.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://su.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://ng.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://zd.lnxyls.cn

[S43] C++：智能指针
来源：http://tr.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://ii.szxytkj.cn

[S44] C++：引用传参
来源：http://mh.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://xk.colortex.cn

[S45] C++：lambda
来源：http://ik.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rq.wgjwhj.cn

[S46] C++：函数模板
来源：http://ix.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ul.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://qn.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dk.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://ud.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://av.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://st.521024.cn

[S49] C++：写文件
来源：http://hp.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ry.jctech888.com.cn

[S50] C++：格式化数字
来源：http://nz.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aa.colortex.cn

[S51] C++：显式类型转换
来源：http://dr.panjiajie.cn

static_cast<double>(a) / b
来源：http://he.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://to.szsharing.cn

int size() const noexcept { return n_; }
来源：http://lh.nszjky.cn

[S53] C++：移动语义
来源：http://qq.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://sx.bjjhwx.cn

[S54] C++：异常处理
来源：http://jx.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wk.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://io.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gf.chemitech.net.cn

[S56] C++：optional
来源：http://zs.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pg.szsharing.cn

[S57] C++：编译期常量
来源：http://an.shtwfgs.cn

constexpr int N = 10;
来源：http://fp.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://bv.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://bv.bookmarksfly.cn

[S59] C++：静态断言
来源：http://dg.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wd.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://aq.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://al.shxzukj.cn

================================================================================
来源：http://fj.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fw.wgjwhj.cn

================================================================================
来源：http://an.hahajie.cn

[T01] Kotlin：Hello World
来源：http://cv.huixiangedu.cn

println("Hello")
来源：http://qu.bjjhwx.cn

[T02] Kotlin：变量
来源：http://hz.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ut.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://yj.nszjky.cn

"值: $b"
来源：http://yn.szsharing.cn

[T04] Kotlin：空安全
来源：http://wa.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://pb.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://tr.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jt.521024.cn

[T06] Kotlin：集合映射
来源：http://rd.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kr.521024.cn

[T07] Kotlin：集合过滤
来源：http://ei.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fp.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://kb.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://mt.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://gh.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://as.asd995.cn

[T10] Kotlin：默认参数
来源：http://cu.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ig.szxytkj.cn

[T11] Kotlin：协程
来源：http://eq.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nq.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://es.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://xb.521024.cn

[T13] Kotlin：只读 Map
来源：http://cl.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://ca.gzmigu.cn

[T14] Kotlin：循环
来源：http://ti.521024.cn

for (i in 1..10) println(i)
来源：http://jn.wgjwhj.cn

[T15] Kotlin：接口
来源：http://da.szsharing.cn

interface Shape { fun area(): Double }
来源：http://ds.huanxung.cn

[T16] Swift：Hello World
来源：http://ix.jctech888.com.cn

print("Hello")
来源：http://uh.521024.cn

[T17] Swift：变量与常量
来源：http://tf.shtwfgs.cn

var a = 1;  let b = 2
来源：http://gs.hnjuh.cn

[T18] Swift：字符串插值
来源：http://oc.nszjky.cn

"值: \(b)"
来源：http://if.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://vc.9csxet.cn

if let n = opt { print(n) }
来源：http://sb.hahajie.cn

[T20] Swift：数组操作
来源：http://pz.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nz.colortex.cn

[T21] Swift：遍历
来源：http://yr.shtwfgs.cn

for x in a { print(x) }
来源：http://zz.szxytkj.cn

[T22] Swift：字典
来源：http://cq.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mg.muxihuayi.cn

[T23] Swift：函数
来源：http://wy.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qh.panjiajie.cn

[T24] Swift：闭包
来源：http://dj.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vk.wgjwhj.cn

[T25] Swift：结构体
来源：http://vj.lnxyls.cn

struct P { var x: Int }
来源：http://jx.9csxet.cn

[T26] Swift：类与重写
来源：http://oq.shxzukj.cn

class A: Base { override func f() {} }
来源：http://tz.szsharing.cn

[T27] Swift：错误处理
来源：http://nf.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://wq.szsharing.cn

[T28] Swift：枚举
来源：http://jx.jianghongdianzi.cn

enum Color { case red, green }
来源：http://hi.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://ev.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://xv.shxzskj.cn

[T30] Swift：协议
来源：http://av.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://zd.hahajie.cn

[T31] Lua：Hello World
来源：http://pk.hahajie.cn

print("Hello")
来源：http://xw.newstarts.cn

[T32] Lua：局部变量
来源：http://ja.hahajie.cn

local a = 1
来源：http://jc.shxzskj.cn

[T33] Lua：表（数组）
来源：http://hq.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://op.muxihuayi.cn

[T34] Lua：遍历表
来源：http://nu.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ll.szsharing.cn

[T35] Lua：字典表
来源：http://kg.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://me.shxzukj.cn

[T36] Lua：函数
来源：http://dv.szxytkj.cn

function add(a, b) return a + b end
来源：http://pi.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://zp.521024.cn

"a" .. "b"
来源：http://ws.bookmarksfly.cn

[T38] Lua：条件
来源：http://zm.szxytkj.cn

if x > 0 then print("正") end
来源：http://xv.gzmigu.cn

[T39] Lua：模式匹配
来源：http://fc.panjiajie.cn

string.find(s, "%d+")
来源：http://lz.jctech888.com.cn

[T40] Lua：元表
来源：http://cg.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://tr.521024.cn

[T41] Perl：Hello World
来源：http://nk.yuexingan06.cn

print "Hello\n";
来源：http://bq.9csxet.cn

[T42] Perl：变量类型
来源：http://tf.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yl.colortex.cn

[T43] Perl：字符串插值
来源：http://me.bookmarksfly.cn

"值: $a"
来源：http://yi.shtwfgs.cn

[T44] Perl：条件
来源：http://xa.asd995.cn

if ($a > 0) { print "正"; }
来源：http://wv.shxzukj.cn

[T45] Perl：数组遍历
来源：http://er.colortex.cn

for my $x (@arr) { print $x; }
来源：http://hh.521024.cn

[T46] Perl：哈希操作
来源：http://eu.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ij.wgjwhj.cn


<!-- 参考信息 -->