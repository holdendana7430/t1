代发 wailian999

find . -name "*.log" -type f
来源：http://ee.hnjuh.cn

[R44] 按修改时间查找
来源：http://vx.shxzskj.cn

find . -mtime -7 -type f
来源：http://kn.yuntaijiaju.cn

[R45] 批量删除
来源：http://ak.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://zq.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://tg.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nf.huixiangedu.cn

[R47] sed 单行替换
来源：http://kb.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ql.hahajie.cn

[R48] awk 取指定列
来源：http://uw.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://mu.muxihuayi.cn

[R49] awk 带条件
来源：http://wx.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ln.521024.cn

[R50] awk 求和
来源：http://ep.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://us.huixiangedu.cn

[R51] 排序去重取前几
来源：http://ds.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://il.newstarts.cn

[R52] 统计行数
来源：http://cf.panjiajie.cn

wc -l a.txt
来源：http://sv.asd995.cn

[R53] 查看文件头与实时尾
来源：http://cv.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wa.huanxung.cn

[R54] 比较两个文件
来源：http://ra.yuntaijiaju.cn

diff a.txt b.txt
来源：http://mo.nicolike.cn

[R55] 压缩与解压
来源：http://ol.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yy.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://tc.newstarts.cn

scp file user@host:/path/
来源：http://xr.hnjuh.cn

[R57] 远程执行命令
来源：http://cr.shxzskj.cn

ssh user@host 'uptime'
来源：http://ay.muxihuayi.cn

[R58] 下载文件
来源：http://oz.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cu.chemitech.net.cn

[R59] 发 POST JSON
来源：http://zc.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://de.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://cg.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tq.huanxung.cn

[R61] 磁盘占用
来源：http://dg.wgjwhj.cn

df -h;  du -sh *
来源：http://kd.newstarts.cn

[R62] 找最占空间的文件
来源：http://qc.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://wa.shxzskj.cn

[R63] 内存与进程
来源：http://ff.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://lo.yuexingan06.cn

[R64] 结束进程
来源：http://od.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://cs.szxytkj.cn

[R65] 查看端口占用
来源：http://ag.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://za.nszjky.cn

[R66] 定时任务
来源：http://pp.panjiajie.cn

crontab -e;  crontab -l
来源：http://af.9csxet.cn

[R67] 生成随机十六进制串
来源：http://bs.521024.cn

openssl rand -hex 16
来源：http://ig.huanxung.cn

[R68] 计算文件校验值
来源：http://ch.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hh.muxihuayi.cn

[R69] 生成随机密码
来源：http://lb.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://kn.nicolike.cn

[R70] 时间戳与互转
来源：http://dn.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://on.asd995.cn

[R71] 日期格式化
来源：http://yb.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wg.jctech888.com.cn

[R72] 等待端口就绪
来源：http://ik.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xa.panjiajie.cn

[R73] 分割大日志
来源：http://do.hahajie.cn

split -l 1000 big.log part_
来源：http://aw.huixinmuqiang.cn

[R74] 批量重命名
来源：http://ku.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ni.panjiajie.cn

[R75] 导出环境变量
来源：http://jk.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://ff.521024.cn

[R76] 使用临时文件
来源：http://vw.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lc.wgjwhj.cn

[R77] 读取用户输入
来源：http://oy.shtwfgs.cn

read -rp "请输入: " ans
来源：http://il.hahajie.cn

[R78] 交互式菜单
来源：http://om.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wa.wgjwhj.cn

[R79] 解析命令行选项
来源：http://la.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xp.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://bw.9csxet.cn

time ./run.sh
来源：http://un.huixinmuqiang.cn

================================================================================
来源：http://fr.521024.cn

S. C / C++ 专题
来源：http://zq.shxzukj.cn

================================================================================
来源：http://ed.chemitech.net.cn

[S01] C：Hello World
来源：http://de.bjjhwx.cn

#include <stdio.h>
来源：http://tr.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://as.newstarts.cn

[S02] C：变量与格式化输出
来源：http://yd.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://wd.wgjwhj.cn

[S03] C：读入整数
来源：http://np.gzmigu.cn

int x; scanf("%d", &x);
来源：http://xn.asd995.cn

[S04] C：字符串复制
来源：http://sw.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ru.gzmigu.cn

[S05] C：字符串长度
来源：http://hv.shxzukj.cn

strlen(s)
来源：http://kf.asd995.cn

[S06] C：字符串比较
来源：http://yv.panjiajie.cn

strcmp(a, b) == 0
来源：http://cz.panjiajie.cn

[S07] C：数组遍历求和
来源：http://hz.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oi.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://pm.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kh.asd995.cn

[S09] C：结构体定义与初始化
来源：http://lt.jianghongdianzi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lx.nicolike.cn

[S10] C：指针与解引用
来源：http://az.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://fz.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://wt.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://wy.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nn.bjjhwx.cn

fclose(f);
来源：http://dg.bookmarksfly.cn

[S12] C：写文件
来源：http://gh.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rh.huixiangedu.cn

[S13] C：宏定义
来源：http://qy.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://am.wgjwhj.cn

[S14] C：枚举
来源：http://hk.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://oe.jianghongdianzi.cn

[S15] C：类型转换
来源：http://zx.jianghongdianzi.cn

(double) a / b
来源：http://ku.colortex.cn

[S16] C：位操作置位
来源：http://ao.521024.cn

x |= (1 << 3);
来源：http://ud.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://es.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oe.gzmigu.cn

[S18] C：命令行参数
来源：http://sm.gzmigu.cn

int main(int argc, char **argv)
来源：http://hn.jianghongdianzi.cn

[S19] C：快速排序
来源：http://wm.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kq.muxihuayi.cn

[S20] C：二分查找
来源：http://am.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zw.yuexingan06.cn

[S21] C：字符类别判断
来源：http://uq.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mt.shxzukj.cn

[S22] C：字符串转数字
来源：http://ne.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bs.jianghongdianzi.cn

[S23] C：随机数
来源：http://nb.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pb.szxytkj.cn

[S24] C：获取本地时间
来源：http://ca.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pk.huixiangedu.cn

[S25] C：内存拷贝
来源：http://yj.muxihuayi.cn

memcpy(dst, src, n);
来源：http://bo.9csxet.cn

[S26] C：内存清零
来源：http://oc.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://zo.lnxyls.cn

[S27] C：定义常量
来源：http://yn.wgjwhj.cn

const double PI = 3.14159;
来源：http://em.gzmigu.cn

[S28] C：静态变量
来源：http://an.asd995.cn

static int counter = 0;
来源：http://wd.newstarts.cn

[S29] C：变参函数
来源：http://ep.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gn.wgjwhj.cn

[S30] C：头文件保护
来源：http://rq.szxytkj.cn

#ifndef X_H
来源：http://pz.9csxet.cn

#define X_H
来源：http://oy.shxzskj.cn

#endif
来源：http://qr.panjiajie.cn

[S31] C++：Hello World
来源：http://gi.shxzskj.cn

#include <iostream>
来源：http://ww.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://hq.szxytkj.cn

[S32] C++：字符串
来源：http://rl.colortex.cn

std::string s = "hi";  s += "!";
来源：http://kl.521024.cn

[S33] C++：vector 增删
来源：http://uh.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lf.shxzukj.cn

[S34] C++：遍历 vector
来源：http://pl.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://gv.panjiajie.cn

[S35] C++：map
来源：http://gw.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kc.hnjuh.cn

[S36] C++：unordered_map
来源：http://ir.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jh.shxzskj.cn

[S37] C++：set
来源：http://io.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bo.colortex.cn

[S38] C++：排序
来源：http://pw.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://iq.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://hu.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xf.bookmarksfly.cn

[S40] C++：查找元素
来源：http://mz.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qn.szsharing.cn

[S41] C++：类与构造函数
来源：http://hn.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wc.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://ah.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://ep.muxihuayi.cn

[S43] C++：智能指针
来源：http://im.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://ww.nicolike.cn

[S44] C++：引用传参
来源：http://no.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://rx.asd995.cn

[S45] C++：lambda
来源：http://dj.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sk.wgjwhj.cn

[S46] C++：函数模板
来源：http://hl.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cs.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://sh.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hi.huanxung.cn

[S48] C++：逐行读文件
来源：http://qy.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zi.colortex.cn

while (std::getline(in, line)) { }
来源：http://yt.szxytkj.cn

[S49] C++：写文件
来源：http://jx.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://je.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://kk.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qh.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://wd.521024.cn

static_cast<double>(a) / b
来源：http://ok.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://it.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://ir.haigaiapp.cn

[S53] C++：移动语义
来源：http://ov.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://zv.shxzukj.cn

[S54] C++：异常处理
来源：http://uw.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lh.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://db.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ta.newstarts.cn

[S56] C++：optional
来源：http://ni.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://of.521024.cn

[S57] C++：编译期常量
来源：http://cx.huanxung.cn

constexpr int N = 10;
来源：http://db.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://ii.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://yc.muxihuayi.cn

[S59] C++：静态断言
来源：http://ca.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ci.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://mt.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sd.lnxyls.cn

================================================================================
来源：http://kl.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yh.nszjky.cn

================================================================================
来源：http://yj.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://gv.jctech888.com.cn

println("Hello")
来源：http://ht.muxihuayi.cn

[T02] Kotlin：变量
来源：http://on.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sw.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://ky.hnjuh.cn

"值: $b"
来源：http://ts.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://uk.panjiajie.cn

val n: String? = null;  n?.length
来源：http://cy.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://uc.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xy.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://nh.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xq.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://nw.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://er.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://xc.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://ro.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://gk.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://rv.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://ok.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pb.bjjhwx.cn

[T11] Kotlin：协程
来源：http://gh.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yl.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://td.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://ew.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://do.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://kt.hnjuh.cn

[T14] Kotlin：循环
来源：http://vb.shxzukj.cn

for (i in 1..10) println(i)
来源：http://nm.gzmigu.cn

[T15] Kotlin：接口
来源：http://jf.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://tw.521024.cn

[T16] Swift：Hello World
来源：http://be.yuntaijiaju.cn

print("Hello")
来源：http://wh.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://ej.bjjhwx.cn

var a = 1;  let b = 2
来源：http://re.shxzukj.cn

[T18] Swift：字符串插值
来源：http://cl.9csxet.cn

"值: \(b)"
来源：http://fj.szsharing.cn

[T19] Swift：可选绑定
来源：http://aq.jctech888.com.cn

if let n = opt { print(n) }
来源：http://vo.hnjuh.cn

[T20] Swift：数组操作
来源：http://yo.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bq.hahajie.cn

[T21] Swift：遍历
来源：http://yf.521024.cn

for x in a { print(x) }
来源：http://jk.yuexingan06.cn

[T22] Swift：字典
来源：http://qy.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vk.huixinmuqiang.cn

[T23] Swift：函数
来源：http://oo.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ys.hnjuh.cn

[T24] Swift：闭包
来源：http://wi.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yu.shxzukj.cn

[T25] Swift：结构体
来源：http://gm.hahajie.cn

struct P { var x: Int }
来源：http://cs.muxihuayi.cn

[T26] Swift：类与重写
来源：http://tv.shxzskj.cn

class A: Base { override func f() {} }
来源：http://ps.muxihuayi.cn

[T27] Swift：错误处理
来源：http://lc.9csxet.cn

do { try f() } catch { print(error) }
来源：http://cw.haigaiapp.cn

[T28] Swift：枚举
来源：http://ya.newstarts.cn

enum Color { case red, green }
来源：http://zl.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://ki.huixiangedu.cn

guard let x = opt else { return }
来源：http://dq.9csxet.cn

[T30] Swift：协议
来源：http://fb.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://of.newstarts.cn

[T31] Lua：Hello World
来源：http://iz.huixiangedu.cn

print("Hello")
来源：http://ss.nicolike.cn

[T32] Lua：局部变量
来源：http://rf.521024.cn

local a = 1
来源：http://ka.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://br.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mc.jctech888.com.cn

[T34] Lua：遍历表
来源：http://yi.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ce.jctech888.com.cn

[T35] Lua：字典表
来源：http://fh.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://wz.newstarts.cn

[T36] Lua：函数
来源：http://dt.haigaiapp.cn

function add(a, b) return a + b end
来源：http://ok.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://pe.chemitech.net.cn

"a" .. "b"
来源：http://ry.panjiajie.cn

[T38] Lua：条件
来源：http://rd.newstarts.cn

if x > 0 then print("正") end
来源：http://cn.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://tu.bjjhwx.cn

string.find(s, "%d+")
来源：http://wn.huanxung.cn

[T40] Lua：元表
来源：http://pu.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://it.colortex.cn

[T41] Perl：Hello World
来源：http://ay.nicolike.cn

print "Hello\n";
来源：http://bw.nicolike.cn

[T42] Perl：变量类型
来源：http://wi.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sm.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://nt.newstarts.cn

"值: $a"
来源：http://su.nszjky.cn

[T44] Perl：条件
来源：http://vr.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://on.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://dn.521024.cn

for my $x (@arr) { print $x; }
来源：http://tj.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://fd.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oa.9csxet.cn


<!-- 参考信息 -->