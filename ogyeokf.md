代发 wailian999

cmd > out.log 2>&1
来源：http://ff.jianghongdianzi.cn

[R40] 追加写日志
来源：http://rg.nicolike.cn

echo "log" >> out.log
来源：http://rn.shxzskj.cn

[R41] 丢弃输出
来源：http://rm.newstarts.cn

cmd >/dev/null 2>&1
来源：http://wl.huanxung.cn

[R42] 输入重定向
来源：http://jt.shxzukj.cn

wc -l < a.txt
来源：http://zd.nszjky.cn

[R43] 按名字查找文件
来源：http://zl.panjiajie.cn

find . -name "*.log" -type f
来源：http://hp.hnjuh.cn

[R44] 按修改时间查找
来源：http://bs.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://qs.huanxung.cn

[R45] 批量删除
来源：http://vn.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://xx.hnjuh.cn

[R46] 递归替换文件内容
来源：http://nz.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mb.jctech888.com.cn

[R47] sed 单行替换
来源：http://up.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gq.chemitech.net.cn

[R48] awk 取指定列
来源：http://ge.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://qo.gzmigu.cn

[R49] awk 带条件
来源：http://mb.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ac.bookmarksfly.cn

[R50] awk 求和
来源：http://ed.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mi.521024.cn

[R51] 排序去重取前几
来源：http://zl.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gn.yuntaijiaju.cn

[R52] 统计行数
来源：http://hr.shxzskj.cn

wc -l a.txt
来源：http://vi.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://bl.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wb.shxzukj.cn

[R54] 比较两个文件
来源：http://vg.jctech888.com.cn

diff a.txt b.txt
来源：http://hz.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://sg.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sa.asd995.cn

[R56] 远程拷贝
来源：http://tn.huixiangedu.cn

scp file user@host:/path/
来源：http://tq.shxzskj.cn

[R57] 远程执行命令
来源：http://tj.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://yg.colortex.cn

[R58] 下载文件
来源：http://wi.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ls.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://bz.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lj.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://sv.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bk.lnxyls.cn

[R61] 磁盘占用
来源：http://wu.panjiajie.cn

df -h;  du -sh *
来源：http://hy.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://zh.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://gb.shxzukj.cn

[R63] 内存与进程
来源：http://ts.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://ec.nicolike.cn

[R64] 结束进程
来源：http://ra.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://ho.panjiajie.cn

[R65] 查看端口占用
来源：http://ph.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nh.muxihuayi.cn

[R66] 定时任务
来源：http://xk.bjjhwx.cn

crontab -e;  crontab -l
来源：http://az.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://sq.yuexingan06.cn

openssl rand -hex 16
来源：http://hs.chemitech.net.cn

[R68] 计算文件校验值
来源：http://sj.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qi.gzmigu.cn

[R69] 生成随机密码
来源：http://pk.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://kc.nszjky.cn

[R70] 时间戳与互转
来源：http://iu.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://mc.szxytkj.cn

[R71] 日期格式化
来源：http://xf.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kj.haigaiapp.cn

[R72] 等待端口就绪
来源：http://mc.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ep.huixiangedu.cn

[R73] 分割大日志
来源：http://rq.bjjhwx.cn

split -l 1000 big.log part_
来源：http://cz.muxihuayi.cn

[R74] 批量重命名
来源：http://hh.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kj.521024.cn

[R75] 导出环境变量
来源：http://wo.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://rl.huixiangedu.cn

[R76] 使用临时文件
来源：http://td.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tl.yuexingan06.cn

[R77] 读取用户输入
来源：http://bs.hahajie.cn

read -rp "请输入: " ans
来源：http://xc.newstarts.cn

[R78] 交互式菜单
来源：http://wk.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rw.newstarts.cn

[R79] 解析命令行选项
来源：http://oc.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sz.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://ho.wgjwhj.cn

time ./run.sh
来源：http://iv.shtwfgs.cn

================================================================================
来源：http://mj.huixiangedu.cn

S. C / C++ 专题
来源：http://fi.jctech888.com.cn

================================================================================
来源：http://hl.huixiangedu.cn

[S01] C：Hello World
来源：http://kj.yuexingan06.cn

#include <stdio.h>
来源：http://jd.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gx.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://tl.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://yq.muxihuayi.cn

[S03] C：读入整数
来源：http://by.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://vv.chemitech.net.cn

[S04] C：字符串复制
来源：http://nq.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sy.nszjky.cn

[S05] C：字符串长度
来源：http://ae.newstarts.cn

strlen(s)
来源：http://nu.521024.cn

[S06] C：字符串比较
来源：http://ta.521024.cn

strcmp(a, b) == 0
来源：http://nd.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://xo.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fu.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://jo.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://co.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://hz.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bs.shtwfgs.cn

[S10] C：指针与解引用
来源：http://qy.9csxet.cn

int *p = &a;  *p = 5;
来源：http://kw.hnjuh.cn

[S11] C：逐行读文件
来源：http://zz.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://hg.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ss.nszjky.cn

fclose(f);
来源：http://tm.huixinmuqiang.cn

[S12] C：写文件
来源：http://wy.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yq.muxihuayi.cn

[S13] C：宏定义
来源：http://ls.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://au.asd995.cn

[S14] C：枚举
来源：http://ug.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ql.huixiangedu.cn

[S15] C：类型转换
来源：http://ux.nszjky.cn

(double) a / b
来源：http://cz.szsharing.cn

[S16] C：位操作置位
来源：http://ej.huixinmuqiang.cn

x |= (1 << 3);
来源：http://rz.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://jr.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://io.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://ts.haigaiapp.cn

int main(int argc, char **argv)
来源：http://pv.muxihuayi.cn

[S19] C：快速排序
来源：http://uf.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nw.hahajie.cn

[S20] C：二分查找
来源：http://je.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zr.huixiangedu.cn

[S21] C：字符类别判断
来源：http://ya.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ix.szsharing.cn

[S22] C：字符串转数字
来源：http://mc.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mt.chemitech.net.cn

[S23] C：随机数
来源：http://kz.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iy.jctech888.com.cn

[S24] C：获取本地时间
来源：http://xr.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://og.jctech888.com.cn

[S25] C：内存拷贝
来源：http://xa.panjiajie.cn

memcpy(dst, src, n);
来源：http://oh.9csxet.cn

[S26] C：内存清零
来源：http://dx.asd995.cn

memset(a, 0, sizeof a);
来源：http://ql.huanxung.cn

[S27] C：定义常量
来源：http://rt.huixiangedu.cn

const double PI = 3.14159;
来源：http://dr.asd995.cn

[S28] C：静态变量
来源：http://tw.521024.cn

static int counter = 0;
来源：http://wy.9csxet.cn

[S29] C：变参函数
来源：http://tp.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xf.lnxyls.cn

[S30] C：头文件保护
来源：http://rp.shtwfgs.cn

#ifndef X_H
来源：http://en.bookmarksfly.cn

#define X_H
来源：http://dc.wgjwhj.cn

#endif
来源：http://vz.muxihuayi.cn

[S31] C++：Hello World
来源：http://db.nicolike.cn

#include <iostream>
来源：http://df.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://es.gzmigu.cn

[S32] C++：字符串
来源：http://ou.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://yq.gzmigu.cn

[S33] C++：vector 增删
来源：http://nf.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tw.nicolike.cn

[S34] C++：遍历 vector
来源：http://cy.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://pe.colortex.cn

[S35] C++：map
来源：http://sw.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pq.wgjwhj.cn

[S36] C++：unordered_map
来源：http://oz.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ie.szsharing.cn

[S37] C++：set
来源：http://fr.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ze.panjiajie.cn

[S38] C++：排序
来源：http://za.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://jy.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://hc.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cv.colortex.cn

[S40] C++：查找元素
来源：http://rj.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lm.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://rt.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sv.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://lj.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://vo.nszjky.cn

[S43] C++：智能指针
来源：http://fy.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://aj.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://mv.hahajie.cn

void inc(int &x) { ++x; }
来源：http://wz.bjjhwx.cn

[S45] C++：lambda
来源：http://oy.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hq.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://jw.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fo.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://pv.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://in.nicolike.cn

[S48] C++：逐行读文件
来源：http://bx.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gj.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://ii.nszjky.cn

[S49] C++：写文件
来源：http://ue.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gq.wgjwhj.cn

[S50] C++：格式化数字
来源：http://ro.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://go.gzmigu.cn

[S51] C++：显式类型转换
来源：http://qy.szsharing.cn

static_cast<double>(a) / b
来源：http://ev.521024.cn

[S52] C++：const 与 noexcept
来源：http://gi.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://oo.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://vr.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://hy.colortex.cn

[S54] C++：异常处理
来源：http://il.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ld.szxytkj.cn

[S55] C++：结构化绑定
来源：http://mf.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vy.hnjuh.cn

[S56] C++：optional
来源：http://wh.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qa.colortex.cn

[S57] C++：编译期常量
来源：http://hp.hahajie.cn

constexpr int N = 10;
来源：http://pc.bookmarksfly.cn

[S58] C++：命名空间
来源：http://eq.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://yv.haigaiapp.cn

[S59] C++：静态断言
来源：http://is.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ym.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://xf.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ch.wgjwhj.cn

================================================================================
来源：http://vm.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vv.lnxyls.cn

================================================================================
来源：http://ob.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://gz.yuexingan06.cn

println("Hello")
来源：http://un.hahajie.cn

[T02] Kotlin：变量
来源：http://wx.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hv.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://nc.nszjky.cn

"值: $b"
来源：http://ha.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://ng.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://eo.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://na.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qu.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://zf.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bk.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://vk.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pp.shxzskj.cn

[T08] Kotlin：数据类
来源：http://zn.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://eq.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://yj.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://yz.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://ea.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dp.shxzukj.cn

[T11] Kotlin：协程
来源：http://gv.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nm.nszjky.cn

[T12] Kotlin：解构声明
来源：http://mq.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://pg.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://ln.newstarts.cn

val m = mapOf("a" to 1)
来源：http://qn.jctech888.com.cn

[T14] Kotlin：循环
来源：http://nd.521024.cn

for (i in 1..10) println(i)
来源：http://ol.huanxung.cn

[T15] Kotlin：接口
来源：http://da.9csxet.cn

interface Shape { fun area(): Double }
来源：http://qq.wgjwhj.cn

[T16] Swift：Hello World
来源：http://zw.colortex.cn

print("Hello")
来源：http://wm.gzmigu.cn

[T17] Swift：变量与常量
来源：http://rl.wgjwhj.cn

var a = 1;  let b = 2
来源：http://pp.hahajie.cn

[T18] Swift：字符串插值
来源：http://tx.521024.cn

"值: \(b)"
来源：http://vl.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://uh.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://ba.521024.cn

[T20] Swift：数组操作
来源：http://vm.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xz.lnxyls.cn

[T21] Swift：遍历
来源：http://ik.lnxyls.cn

for x in a { print(x) }
来源：http://tj.panjiajie.cn

[T22] Swift：字典
来源：http://zi.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vk.asd995.cn

[T23] Swift：函数
来源：http://qd.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tn.521024.cn

[T24] Swift：闭包
来源：http://er.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://en.newstarts.cn

[T25] Swift：结构体
来源：http://vp.lnxyls.cn

struct P { var x: Int }
来源：http://fo.muxihuayi.cn

[T26] Swift：类与重写
来源：http://ni.huanxung.cn

class A: Base { override func f() {} }
来源：http://sd.szsharing.cn

[T27] Swift：错误处理
来源：http://pn.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://fu.panjiajie.cn

[T28] Swift：枚举
来源：http://pr.szsharing.cn

enum Color { case red, green }
来源：http://pt.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://xk.huanxung.cn

guard let x = opt else { return }
来源：http://rv.szsharing.cn

[T30] Swift：协议
来源：http://xd.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://sw.shxzukj.cn

[T31] Lua：Hello World
来源：http://uf.hahajie.cn

print("Hello")
来源：http://be.jctech888.com.cn

[T32] Lua：局部变量
来源：http://nw.huixinmuqiang.cn

local a = 1
来源：http://kg.shxzskj.cn

[T33] Lua：表（数组）
来源：http://hl.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nv.gzmigu.cn

[T34] Lua：遍历表
来源：http://et.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gx.huanxung.cn

[T35] Lua：字典表
来源：http://ih.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://tt.muxihuayi.cn

[T36] Lua：函数
来源：http://ha.jctech888.com.cn

function add(a, b) return a + b end
来源：http://mj.9csxet.cn

[T37] Lua：字符串拼接
来源：http://qn.szsharing.cn

"a" .. "b"
来源：http://se.muxihuayi.cn

[T38] Lua：条件
来源：http://yk.szsharing.cn

if x > 0 then print("正") end
来源：http://hm.panjiajie.cn

[T39] Lua：模式匹配
来源：http://na.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://pw.bookmarksfly.cn

[T40] Lua：元表
来源：http://wo.nicolike.cn

setmetatable({}, { __index = base })
来源：http://el.szsharing.cn

[T41] Perl：Hello World
来源：http://ae.yuntaijiaju.cn

print "Hello\n";
来源：http://gt.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://zs.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://do.colortex.cn


<!-- 参考信息 -->