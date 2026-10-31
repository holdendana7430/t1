代发 wailian999

cmd >/dev/null 2>&1
来源：http://om.szxytkj.cn

[R42] 输入重定向
来源：http://se.yuntaijiaju.cn

wc -l < a.txt
来源：http://eu.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://ko.hahajie.cn

find . -name "*.log" -type f
来源：http://tk.szxytkj.cn

[R44] 按修改时间查找
来源：http://bf.lnxyls.cn

find . -mtime -7 -type f
来源：http://fa.jctech888.com.cn

[R45] 批量删除
来源：http://ha.asd995.cn

find . -name "*.tmp" -delete
来源：http://xy.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://yy.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nx.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://gg.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wi.shxzskj.cn

[R48] awk 取指定列
来源：http://wo.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://yj.szxytkj.cn

[R49] awk 带条件
来源：http://of.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xi.szxytkj.cn

[R50] awk 求和
来源：http://zk.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://az.huanxung.cn

[R51] 排序去重取前几
来源：http://gr.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xu.bjjhwx.cn

[R52] 统计行数
来源：http://xh.asd995.cn

wc -l a.txt
来源：http://sz.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://up.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://by.panjiajie.cn

[R54] 比较两个文件
来源：http://iw.haigaiapp.cn

diff a.txt b.txt
来源：http://rh.yuexingan06.cn

[R55] 压缩与解压
来源：http://dp.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ti.bookmarksfly.cn

[R56] 远程拷贝
来源：http://zx.gzmigu.cn

scp file user@host:/path/
来源：http://qy.nicolike.cn

[R57] 远程执行命令
来源：http://hy.szsharing.cn

ssh user@host 'uptime'
来源：http://ik.shxzskj.cn

[R58] 下载文件
来源：http://go.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oo.lnxyls.cn

[R59] 发 POST JSON
来源：http://ts.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ma.521024.cn

[R60] 只看 HTTP 状态码
来源：http://nm.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zp.bookmarksfly.cn

[R61] 磁盘占用
来源：http://ey.shtwfgs.cn

df -h;  du -sh *
来源：http://os.lnxyls.cn

[R62] 找最占空间的文件
来源：http://my.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://bg.chemitech.net.cn

[R63] 内存与进程
来源：http://bb.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://iy.asd995.cn

[R64] 结束进程
来源：http://sw.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://yt.newstarts.cn

[R65] 查看端口占用
来源：http://hv.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oa.hahajie.cn

[R66] 定时任务
来源：http://hz.hahajie.cn

crontab -e;  crontab -l
来源：http://lw.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://mo.gzmigu.cn

openssl rand -hex 16
来源：http://tc.gzmigu.cn

[R68] 计算文件校验值
来源：http://uv.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lg.521024.cn

[R69] 生成随机密码
来源：http://gh.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://ap.wgjwhj.cn

[R70] 时间戳与互转
来源：http://ac.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://yw.huixinmuqiang.cn

[R71] 日期格式化
来源：http://lb.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ks.bjjhwx.cn

[R72] 等待端口就绪
来源：http://ks.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ws.nicolike.cn

[R73] 分割大日志
来源：http://qb.panjiajie.cn

split -l 1000 big.log part_
来源：http://ic.hnjuh.cn

[R74] 批量重命名
来源：http://sr.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wo.hnjuh.cn

[R75] 导出环境变量
来源：http://ce.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://dp.asd995.cn

[R76] 使用临时文件
来源：http://sn.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pp.haigaiapp.cn

[R77] 读取用户输入
来源：http://ud.521024.cn

read -rp "请输入: " ans
来源：http://rk.huanxung.cn

[R78] 交互式菜单
来源：http://ps.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ri.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://tz.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://av.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://os.haigaiapp.cn

time ./run.sh
来源：http://dg.9csxet.cn

================================================================================
来源：http://yc.nicolike.cn

S. C / C++ 专题
来源：http://ki.yuntaijiaju.cn

================================================================================
来源：http://mt.hnjuh.cn

[S01] C：Hello World
来源：http://sa.hnjuh.cn

#include <stdio.h>
来源：http://jt.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sa.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://eu.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://ym.jianghongdianzi.cn

[S03] C：读入整数
来源：http://sk.gzmigu.cn

int x; scanf("%d", &x);
来源：http://su.yuexingan06.cn

[S04] C：字符串复制
来源：http://mt.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sd.huixiangedu.cn

[S05] C：字符串长度
来源：http://tq.nszjky.cn

strlen(s)
来源：http://qa.muxihuayi.cn

[S06] C：字符串比较
来源：http://wn.muxihuayi.cn

strcmp(a, b) == 0
来源：http://sz.nszjky.cn

[S07] C：数组遍历求和
来源：http://zj.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ob.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://bw.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tk.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://yx.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://il.muxihuayi.cn

[S10] C：指针与解引用
来源：http://rp.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://ap.shxzskj.cn

[S11] C：逐行读文件
来源：http://uf.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://bw.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sw.yuntaijiaju.cn

fclose(f);
来源：http://ya.shxzukj.cn

[S12] C：写文件
来源：http://qt.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xn.shxzukj.cn

[S13] C：宏定义
来源：http://dl.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wu.jctech888.com.cn

[S14] C：枚举
来源：http://qr.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://vn.huanxung.cn

[S15] C：类型转换
来源：http://pc.szsharing.cn

(double) a / b
来源：http://fk.szsharing.cn

[S16] C：位操作置位
来源：http://ty.haigaiapp.cn

x |= (1 << 3);
来源：http://ic.szsharing.cn

[S17] C：安全拼接字符串
来源：http://zb.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zy.jctech888.com.cn

[S18] C：命令行参数
来源：http://zh.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://wi.haigaiapp.cn

[S19] C：快速排序
来源：http://vm.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ud.huixinmuqiang.cn

[S20] C：二分查找
来源：http://qg.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tk.gzmigu.cn

[S21] C：字符类别判断
来源：http://nw.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zz.bjjhwx.cn

[S22] C：字符串转数字
来源：http://hk.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cf.lnxyls.cn

[S23] C：随机数
来源：http://hm.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ja.hahajie.cn

[S24] C：获取本地时间
来源：http://wr.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://it.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://ej.lnxyls.cn

memcpy(dst, src, n);
来源：http://cr.shxzukj.cn

[S26] C：内存清零
来源：http://di.huanxung.cn

memset(a, 0, sizeof a);
来源：http://pz.wgjwhj.cn

[S27] C：定义常量
来源：http://tc.nszjky.cn

const double PI = 3.14159;
来源：http://ph.9csxet.cn

[S28] C：静态变量
来源：http://po.hahajie.cn

static int counter = 0;
来源：http://qz.nicolike.cn

[S29] C：变参函数
来源：http://gk.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ej.wgjwhj.cn

[S30] C：头文件保护
来源：http://sx.huixinmuqiang.cn

#ifndef X_H
来源：http://mw.nicolike.cn

#define X_H
来源：http://zu.521024.cn

#endif
来源：http://qv.asd995.cn

[S31] C++：Hello World
来源：http://zq.bookmarksfly.cn

#include <iostream>
来源：http://yp.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://co.huixinmuqiang.cn

[S32] C++：字符串
来源：http://wl.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://jj.shxzskj.cn

[S33] C++：vector 增删
来源：http://sh.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qg.shxzskj.cn

[S34] C++：遍历 vector
来源：http://ix.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://sb.shxzukj.cn

[S35] C++：map
来源：http://yf.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cd.hahajie.cn

[S36] C++：unordered_map
来源：http://yc.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qv.hnjuh.cn

[S37] C++：set
来源：http://iz.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://do.muxihuayi.cn

[S38] C++：排序
来源：http://so.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://pn.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://cw.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sv.521024.cn

[S40] C++：查找元素
来源：http://bf.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zg.nszjky.cn

[S41] C++：类与构造函数
来源：http://tr.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ad.newstarts.cn

[S42] C++：继承与虚函数
来源：http://lx.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://ju.521024.cn

[S43] C++：智能指针
来源：http://lv.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://ns.521024.cn

[S44] C++：引用传参
来源：http://kk.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://kl.521024.cn

[S45] C++：lambda
来源：http://ul.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yw.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://ac.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cx.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://nw.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gi.shxzskj.cn

[S48] C++：逐行读文件
来源：http://oh.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://os.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://vl.lnxyls.cn

[S49] C++：写文件
来源：http://fn.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qh.huanxung.cn

[S50] C++：格式化数字
来源：http://en.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://km.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://qj.jctech888.com.cn

static_cast<double>(a) / b
来源：http://hs.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://en.colortex.cn

int size() const noexcept { return n_; }
来源：http://dv.bookmarksfly.cn

[S53] C++：移动语义
来源：http://jc.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://gw.gzmigu.cn

[S54] C++：异常处理
来源：http://tk.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ns.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://hm.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jc.huixinmuqiang.cn

[S56] C++：optional
来源：http://ra.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vw.bjjhwx.cn

[S57] C++：编译期常量
来源：http://ww.shtwfgs.cn

constexpr int N = 10;
来源：http://kb.colortex.cn

[S58] C++：命名空间
来源：http://gi.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://bp.shtwfgs.cn

[S59] C++：静态断言
来源：http://bg.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ym.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://np.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tx.bookmarksfly.cn

================================================================================
来源：http://tn.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://go.hahajie.cn

================================================================================
来源：http://qo.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://yp.nicolike.cn

println("Hello")
来源：http://xy.asd995.cn

[T02] Kotlin：变量
来源：http://yx.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://om.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://mr.gzmigu.cn

"值: $b"
来源：http://hd.shxzukj.cn

[T04] Kotlin：空安全
来源：http://ay.huanxung.cn

val n: String? = null;  n?.length
来源：http://rv.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://al.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://my.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://oo.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ur.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://xj.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mu.gzmigu.cn

[T08] Kotlin：数据类
来源：http://ki.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://le.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://ae.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://so.newstarts.cn

[T10] Kotlin：默认参数
来源：http://qt.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qj.hnjuh.cn

[T11] Kotlin：协程
来源：http://vm.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://js.9csxet.cn

[T12] Kotlin：解构声明
来源：http://gg.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://bf.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://ws.szsharing.cn

val m = mapOf("a" to 1)
来源：http://rh.szxytkj.cn

[T14] Kotlin：循环
来源：http://bu.asd995.cn

for (i in 1..10) println(i)
来源：http://sd.bjjhwx.cn

[T15] Kotlin：接口
来源：http://vz.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://tp.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://ry.haigaiapp.cn

print("Hello")
来源：http://az.newstarts.cn

[T17] Swift：变量与常量
来源：http://os.521024.cn

var a = 1;  let b = 2
来源：http://ce.szxytkj.cn

[T18] Swift：字符串插值
来源：http://vn.9csxet.cn

"值: \(b)"
来源：http://wi.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://nc.asd995.cn

if let n = opt { print(n) }
来源：http://fg.gzmigu.cn

[T20] Swift：数组操作
来源：http://ff.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://us.nicolike.cn

[T21] Swift：遍历
来源：http://hz.9csxet.cn

for x in a { print(x) }
来源：http://lb.szxytkj.cn

[T22] Swift：字典
来源：http://bs.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ii.chemitech.net.cn

[T23] Swift：函数
来源：http://jt.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lj.hnjuh.cn

[T24] Swift：闭包
来源：http://wj.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sn.szsharing.cn

[T25] Swift：结构体
来源：http://jr.huanxung.cn

struct P { var x: Int }
来源：http://yw.huixiangedu.cn

[T26] Swift：类与重写
来源：http://yo.nszjky.cn

class A: Base { override func f() {} }
来源：http://rs.newstarts.cn

[T27] Swift：错误处理
来源：http://to.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://ie.shxzukj.cn

[T28] Swift：枚举
来源：http://tk.jctech888.com.cn

enum Color { case red, green }
来源：http://vl.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://yo.chemitech.net.cn

guard let x = opt else { return }
来源：http://ce.huanxung.cn

[T30] Swift：协议
来源：http://hs.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://zq.lnxyls.cn

[T31] Lua：Hello World
来源：http://lm.asd995.cn

print("Hello")
来源：http://jv.shxzskj.cn

[T32] Lua：局部变量
来源：http://eu.521024.cn

local a = 1
来源：http://nm.hahajie.cn

[T33] Lua：表（数组）
来源：http://er.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://us.huixiangedu.cn

[T34] Lua：遍历表
来源：http://tl.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rc.gzmigu.cn

[T35] Lua：字典表
来源：http://sr.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://cy.asd995.cn

[T36] Lua：函数
来源：http://qa.newstarts.cn

function add(a, b) return a + b end
来源：http://vn.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://dx.hahajie.cn

"a" .. "b"
来源：http://rq.bookmarksfly.cn

[T38] Lua：条件
来源：http://ux.bjjhwx.cn

if x > 0 then print("正") end
来源：http://tr.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://ke.nszjky.cn

string.find(s, "%d+")
来源：http://ed.jianghongdianzi.cn

[T40] Lua：元表
来源：http://rb.huanxung.cn

setmetatable({}, { __index = base })
来源：http://gi.huixiangedu.cn

[T41] Perl：Hello World
来源：http://hy.shtwfgs.cn

print "Hello\n";
来源：http://kq.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://ju.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jq.shxzskj.cn

[T43] Perl：字符串插值
来源：http://nx.bookmarksfly.cn

"值: $a"
来源：http://vn.muxihuayi.cn

[T44] Perl：条件
来源：http://fd.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://iq.szxytkj.cn


<!-- 参考信息 -->