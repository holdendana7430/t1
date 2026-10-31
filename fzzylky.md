代发 wailian999

cmd > out.log 2>&1
来源：http://al.shxzskj.cn

[R40] 追加写日志
来源：http://yt.hnjuh.cn

echo "log" >> out.log
来源：http://oc.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://ix.nszjky.cn

cmd >/dev/null 2>&1
来源：http://uk.szsharing.cn

[R42] 输入重定向
来源：http://tu.hnjuh.cn

wc -l < a.txt
来源：http://ii.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://fw.hahajie.cn

find . -name "*.log" -type f
来源：http://ih.bjjhwx.cn

[R44] 按修改时间查找
来源：http://jx.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://sv.asd995.cn

[R45] 批量删除
来源：http://gq.9csxet.cn

find . -name "*.tmp" -delete
来源：http://fg.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://wp.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yy.hahajie.cn

[R47] sed 单行替换
来源：http://jk.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ug.shxzskj.cn

[R48] awk 取指定列
来源：http://ox.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://ts.jianghongdianzi.cn

[R49] awk 带条件
来源：http://db.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tg.hnjuh.cn

[R50] awk 求和
来源：http://ma.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gf.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://gc.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wf.huixinmuqiang.cn

[R52] 统计行数
来源：http://ew.szsharing.cn

wc -l a.txt
来源：http://ih.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://fa.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://md.nicolike.cn

[R54] 比较两个文件
来源：http://yj.lnxyls.cn

diff a.txt b.txt
来源：http://ll.haigaiapp.cn

[R55] 压缩与解压
来源：http://am.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://su.hnjuh.cn

[R56] 远程拷贝
来源：http://ey.newstarts.cn

scp file user@host:/path/
来源：http://rr.yuexingan06.cn

[R57] 远程执行命令
来源：http://lw.9csxet.cn

ssh user@host 'uptime'
来源：http://lo.hahajie.cn

[R58] 下载文件
来源：http://ea.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fp.panjiajie.cn

[R59] 发 POST JSON
来源：http://se.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ru.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://zb.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mo.colortex.cn

[R61] 磁盘占用
来源：http://vx.yuexingan06.cn

df -h;  du -sh *
来源：http://ti.gzmigu.cn

[R62] 找最占空间的文件
来源：http://ja.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://ov.panjiajie.cn

[R63] 内存与进程
来源：http://ua.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://xi.hnjuh.cn

[R64] 结束进程
来源：http://ty.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://bt.9csxet.cn

[R65] 查看端口占用
来源：http://dx.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ux.bookmarksfly.cn

[R66] 定时任务
来源：http://fc.nicolike.cn

crontab -e;  crontab -l
来源：http://yc.colortex.cn

[R67] 生成随机十六进制串
来源：http://or.haigaiapp.cn

openssl rand -hex 16
来源：http://cb.haigaiapp.cn

[R68] 计算文件校验值
来源：http://kg.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mo.haigaiapp.cn

[R69] 生成随机密码
来源：http://uq.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://vl.muxihuayi.cn

[R70] 时间戳与互转
来源：http://ti.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://xh.bjjhwx.cn

[R71] 日期格式化
来源：http://ej.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mo.nicolike.cn

[R72] 等待端口就绪
来源：http://cb.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sa.szsharing.cn

[R73] 分割大日志
来源：http://eg.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://ly.panjiajie.cn

[R74] 批量重命名
来源：http://jz.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ql.huanxung.cn

[R75] 导出环境变量
来源：http://ec.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://px.newstarts.cn

[R76] 使用临时文件
来源：http://iq.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://az.muxihuayi.cn

[R77] 读取用户输入
来源：http://an.shxzukj.cn

read -rp "请输入: " ans
来源：http://yb.hnjuh.cn

[R78] 交互式菜单
来源：http://dg.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wf.colortex.cn

[R79] 解析命令行选项
来源：http://oa.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ia.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://ym.szsharing.cn

time ./run.sh
来源：http://vo.huixiangedu.cn

================================================================================
来源：http://jf.lnxyls.cn

S. C / C++ 专题
来源：http://wz.lnxyls.cn

================================================================================
来源：http://rg.jianghongdianzi.cn

[S01] C：Hello World
来源：http://sz.bjjhwx.cn

#include <stdio.h>
来源：http://jw.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kn.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://eo.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://jv.chemitech.net.cn

[S03] C：读入整数
来源：http://bn.hahajie.cn

int x; scanf("%d", &x);
来源：http://xe.lnxyls.cn

[S04] C：字符串复制
来源：http://sy.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ep.szsharing.cn

[S05] C：字符串长度
来源：http://ku.szsharing.cn

strlen(s)
来源：http://jq.colortex.cn

[S06] C：字符串比较
来源：http://ky.newstarts.cn

strcmp(a, b) == 0
来源：http://op.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://ju.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ni.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://na.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yb.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://yr.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vk.521024.cn

[S10] C：指针与解引用
来源：http://ax.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://fa.yuexingan06.cn

[S11] C：逐行读文件
来源：http://bw.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://nm.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qe.huixinmuqiang.cn

fclose(f);
来源：http://zf.nszjky.cn

[S12] C：写文件
来源：http://we.szxytkj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ji.hahajie.cn

[S13] C：宏定义
来源：http://yc.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yk.hnjuh.cn

[S14] C：枚举
来源：http://kj.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ll.chemitech.net.cn

[S15] C：类型转换
来源：http://jl.521024.cn

(double) a / b
来源：http://jm.shxzukj.cn

[S16] C：位操作置位
来源：http://bi.newstarts.cn

x |= (1 << 3);
来源：http://xo.521024.cn

[S17] C：安全拼接字符串
来源：http://hc.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fy.yuexingan06.cn

[S18] C：命令行参数
来源：http://nq.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://yv.muxihuayi.cn

[S19] C：快速排序
来源：http://rj.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ze.9csxet.cn

[S20] C：二分查找
来源：http://jl.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ix.wgjwhj.cn

[S21] C：字符类别判断
来源：http://sd.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lp.gzmigu.cn

[S22] C：字符串转数字
来源：http://yj.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://za.shxzukj.cn

[S23] C：随机数
来源：http://np.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zs.huixiangedu.cn

[S24] C：获取本地时间
来源：http://jl.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qk.jctech888.com.cn

[S25] C：内存拷贝
来源：http://cy.nicolike.cn

memcpy(dst, src, n);
来源：http://jm.9csxet.cn

[S26] C：内存清零
来源：http://fc.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://bs.szsharing.cn

[S27] C：定义常量
来源：http://yq.gzmigu.cn

const double PI = 3.14159;
来源：http://gg.asd995.cn

[S28] C：静态变量
来源：http://qx.hahajie.cn

static int counter = 0;
来源：http://nm.bjjhwx.cn

[S29] C：变参函数
来源：http://bg.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nd.bjjhwx.cn

[S30] C：头文件保护
来源：http://oq.lnxyls.cn

#ifndef X_H
来源：http://na.newstarts.cn

#define X_H
来源：http://vn.panjiajie.cn

#endif
来源：http://wl.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://fr.chemitech.net.cn

#include <iostream>
来源：http://dy.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://fv.gzmigu.cn

[S32] C++：字符串
来源：http://rn.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://bb.bjjhwx.cn

[S33] C++：vector 增删
来源：http://oc.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nr.521024.cn

[S34] C++：遍历 vector
来源：http://hx.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://gq.huanxung.cn

[S35] C++：map
来源：http://zk.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://um.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://ur.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yj.colortex.cn

[S37] C++：set
来源：http://tm.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xu.wgjwhj.cn

[S38] C++：排序
来源：http://mw.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://jm.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://yw.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rx.shxzskj.cn

[S40] C++：查找元素
来源：http://sx.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lh.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://yd.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cn.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://wi.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://cl.jctech888.com.cn

[S43] C++：智能指针
来源：http://jo.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://ru.huixiangedu.cn

[S44] C++：引用传参
来源：http://ff.asd995.cn

void inc(int &x) { ++x; }
来源：http://wq.panjiajie.cn

[S45] C++：lambda
来源：http://kz.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wv.521024.cn

[S46] C++：函数模板
来源：http://fg.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nu.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://pq.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lo.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://bu.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rc.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://en.jianghongdianzi.cn

[S49] C++：写文件
来源：http://sy.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oz.shtwfgs.cn

[S50] C++：格式化数字
来源：http://qg.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bz.panjiajie.cn

[S51] C++：显式类型转换
来源：http://oj.bjjhwx.cn

static_cast<double>(a) / b
来源：http://hl.asd995.cn

[S52] C++：const 与 noexcept
来源：http://ku.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://yq.haigaiapp.cn

[S53] C++：移动语义
来源：http://ta.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://nc.shxzukj.cn

[S54] C++：异常处理
来源：http://tf.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vo.lnxyls.cn

[S55] C++：结构化绑定
来源：http://qh.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sp.szsharing.cn

[S56] C++：optional
来源：http://cg.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dj.asd995.cn

[S57] C++：编译期常量
来源：http://yd.szxytkj.cn

constexpr int N = 10;
来源：http://qh.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://cr.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://db.wgjwhj.cn

[S59] C++：静态断言
来源：http://jx.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://se.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://hu.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gz.nszjky.cn

================================================================================
来源：http://xu.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wd.shtwfgs.cn

================================================================================
来源：http://dk.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://cj.huanxung.cn

println("Hello")
来源：http://wl.szsharing.cn

[T02] Kotlin：变量
来源：http://az.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nf.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://gd.bookmarksfly.cn

"值: $b"
来源：http://wa.hahajie.cn

[T04] Kotlin：空安全
来源：http://tl.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://dm.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://lw.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ga.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://ag.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sg.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://nt.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ma.szxytkj.cn

[T08] Kotlin：数据类
来源：http://bq.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://ri.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://kg.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://cd.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://if.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xx.hahajie.cn

[T11] Kotlin：协程
来源：http://vd.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oe.9csxet.cn

[T12] Kotlin：解构声明
来源：http://rk.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://ra.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://gv.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://lz.huixiangedu.cn

[T14] Kotlin：循环
来源：http://yl.lnxyls.cn

for (i in 1..10) println(i)
来源：http://mi.yuexingan06.cn

[T15] Kotlin：接口
来源：http://rc.nicolike.cn

interface Shape { fun area(): Double }
来源：http://hv.nicolike.cn

[T16] Swift：Hello World
来源：http://ch.newstarts.cn

print("Hello")
来源：http://mr.szsharing.cn

[T17] Swift：变量与常量
来源：http://fb.nicolike.cn

var a = 1;  let b = 2
来源：http://ca.9csxet.cn

[T18] Swift：字符串插值
来源：http://je.nicolike.cn

"值: \(b)"
来源：http://gh.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://rl.chemitech.net.cn

if let n = opt { print(n) }
来源：http://xm.gzmigu.cn

[T20] Swift：数组操作
来源：http://by.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rm.gzmigu.cn

[T21] Swift：遍历
来源：http://kr.hnjuh.cn

for x in a { print(x) }
来源：http://gz.hahajie.cn

[T22] Swift：字典
来源：http://pg.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bz.shxzukj.cn

[T23] Swift：函数
来源：http://za.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://es.szsharing.cn

[T24] Swift：闭包
来源：http://un.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://at.shxzskj.cn

[T25] Swift：结构体
来源：http://fc.szxytkj.cn

struct P { var x: Int }
来源：http://fl.521024.cn

[T26] Swift：类与重写
来源：http://de.nicolike.cn

class A: Base { override func f() {} }
来源：http://ct.hnjuh.cn

[T27] Swift：错误处理
来源：http://na.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://ft.nicolike.cn

[T28] Swift：枚举
来源：http://up.nicolike.cn

enum Color { case red, green }
来源：http://jz.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://tw.hahajie.cn

guard let x = opt else { return }
来源：http://wq.9csxet.cn

[T30] Swift：协议
来源：http://dq.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://jp.yuexingan06.cn

[T31] Lua：Hello World
来源：http://jv.haigaiapp.cn

print("Hello")
来源：http://rz.huanxung.cn

[T32] Lua：局部变量
来源：http://fr.521024.cn

local a = 1
来源：http://ag.huanxung.cn

[T33] Lua：表（数组）
来源：http://kl.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://py.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://jz.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qr.nicolike.cn

[T35] Lua：字典表
来源：http://hx.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://pt.muxihuayi.cn

[T36] Lua：函数
来源：http://so.shtwfgs.cn

function add(a, b) return a + b end
来源：http://ha.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://ck.gzmigu.cn

"a" .. "b"
来源：http://mj.shtwfgs.cn

[T38] Lua：条件
来源：http://og.hnjuh.cn

if x > 0 then print("正") end
来源：http://nf.9csxet.cn

[T39] Lua：模式匹配
来源：http://ll.hahajie.cn

string.find(s, "%d+")
来源：http://xb.shxzskj.cn

[T40] Lua：元表
来源：http://qz.9csxet.cn

setmetatable({}, { __index = base })
来源：http://xr.szxytkj.cn

[T41] Perl：Hello World
来源：http://tl.huanxung.cn

print "Hello\n";
来源：http://lq.asd995.cn

[T42] Perl：变量类型
来源：http://km.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lf.521024.cn


<!-- 参考信息 -->