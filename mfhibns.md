代发 wailian999

find . -name "*.log" -type f
来源：http://xa.yuexingan06.cn

[R44] 按修改时间查找
来源：http://nj.chemitech.net.cn

find . -mtime -7 -type f
来源：http://bt.shtwfgs.cn

[R45] 批量删除
来源：http://fj.colortex.cn

find . -name "*.tmp" -delete
来源：http://cj.521024.cn

[R46] 递归替换文件内容
来源：http://md.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cj.szxytkj.cn

[R47] sed 单行替换
来源：http://ze.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cs.huixiangedu.cn

[R48] awk 取指定列
来源：http://dd.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://rv.lnxyls.cn

[R49] awk 带条件
来源：http://qk.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nm.shtwfgs.cn

[R50] awk 求和
来源：http://nf.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jh.hahajie.cn

[R51] 排序去重取前几
来源：http://zg.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://iw.wgjwhj.cn

[R52] 统计行数
来源：http://qt.nszjky.cn

wc -l a.txt
来源：http://gt.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://el.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sk.hnjuh.cn

[R54] 比较两个文件
来源：http://um.yuexingan06.cn

diff a.txt b.txt
来源：http://fi.hnjuh.cn

[R55] 压缩与解压
来源：http://kl.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ho.asd995.cn

[R56] 远程拷贝
来源：http://ae.shtwfgs.cn

scp file user@host:/path/
来源：http://ao.nszjky.cn

[R57] 远程执行命令
来源：http://iu.hahajie.cn

ssh user@host 'uptime'
来源：http://bl.nicolike.cn

[R58] 下载文件
来源：http://ky.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aj.yuexingan06.cn

[R59] 发 POST JSON
来源：http://im.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jr.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://rt.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rg.wgjwhj.cn

[R61] 磁盘占用
来源：http://rl.yuexingan06.cn

df -h;  du -sh *
来源：http://op.colortex.cn

[R62] 找最占空间的文件
来源：http://ol.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://yk.hnjuh.cn

[R63] 内存与进程
来源：http://iu.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://mg.chemitech.net.cn

[R64] 结束进程
来源：http://ay.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://bg.gzmigu.cn

[R65] 查看端口占用
来源：http://no.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ty.szsharing.cn

[R66] 定时任务
来源：http://zd.newstarts.cn

crontab -e;  crontab -l
来源：http://me.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://kd.nszjky.cn

openssl rand -hex 16
来源：http://ab.huanxung.cn

[R68] 计算文件校验值
来源：http://id.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://li.9csxet.cn

[R69] 生成随机密码
来源：http://up.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://pr.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://br.newstarts.cn

date +%s;  date -d @1700000000
来源：http://vp.bookmarksfly.cn

[R71] 日期格式化
来源：http://dd.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kl.hnjuh.cn

[R72] 等待端口就绪
来源：http://cl.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rn.bookmarksfly.cn

[R73] 分割大日志
来源：http://bi.bjjhwx.cn

split -l 1000 big.log part_
来源：http://zy.newstarts.cn

[R74] 批量重命名
来源：http://zn.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bs.asd995.cn

[R75] 导出环境变量
来源：http://rw.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://nm.shxzukj.cn

[R76] 使用临时文件
来源：http://ms.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rh.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://iv.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://yu.bjjhwx.cn

[R78] 交互式菜单
来源：http://kr.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xh.9csxet.cn

[R79] 解析命令行选项
来源：http://hv.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://td.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://zo.hnjuh.cn

time ./run.sh
来源：http://lb.szxytkj.cn

================================================================================
来源：http://eq.chemitech.net.cn

S. C / C++ 专题
来源：http://xz.shxzukj.cn

================================================================================
来源：http://xu.asd995.cn

[S01] C：Hello World
来源：http://ez.yuexingan06.cn

#include <stdio.h>
来源：http://mr.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qc.9csxet.cn

[S02] C：变量与格式化输出
来源：http://xr.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://nt.newstarts.cn

[S03] C：读入整数
来源：http://aw.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://pa.bookmarksfly.cn

[S04] C：字符串复制
来源：http://du.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://at.lnxyls.cn

[S05] C：字符串长度
来源：http://yr.hahajie.cn

strlen(s)
来源：http://sl.jctech888.com.cn

[S06] C：字符串比较
来源：http://cy.shxzskj.cn

strcmp(a, b) == 0
来源：http://za.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://in.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wq.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://tc.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qq.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://py.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tw.huixiangedu.cn

[S10] C：指针与解引用
来源：http://rq.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://xl.hahajie.cn

[S11] C：逐行读文件
来源：http://vq.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://py.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gq.hnjuh.cn

fclose(f);
来源：http://jh.bookmarksfly.cn

[S12] C：写文件
来源：http://fx.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ob.nicolike.cn

[S13] C：宏定义
来源：http://jv.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wj.colortex.cn

[S14] C：枚举
来源：http://mg.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://km.huanxung.cn

[S15] C：类型转换
来源：http://fx.9csxet.cn

(double) a / b
来源：http://yo.huixiangedu.cn

[S16] C：位操作置位
来源：http://ou.hahajie.cn

x |= (1 << 3);
来源：http://pl.nszjky.cn

[S17] C：安全拼接字符串
来源：http://my.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://os.jctech888.com.cn

[S18] C：命令行参数
来源：http://kp.hnjuh.cn

int main(int argc, char **argv)
来源：http://qc.yuntaijiaju.cn

[S19] C：快速排序
来源：http://nz.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dj.hnjuh.cn

[S20] C：二分查找
来源：http://zu.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hp.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://oa.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ac.wgjwhj.cn

[S22] C：字符串转数字
来源：http://xk.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gy.huanxung.cn

[S23] C：随机数
来源：http://dw.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kl.haigaiapp.cn

[S24] C：获取本地时间
来源：http://hc.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ps.huanxung.cn

[S25] C：内存拷贝
来源：http://hc.muxihuayi.cn

memcpy(dst, src, n);
来源：http://wf.521024.cn

[S26] C：内存清零
来源：http://ft.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://ds.colortex.cn

[S27] C：定义常量
来源：http://om.muxihuayi.cn

const double PI = 3.14159;
来源：http://yd.bookmarksfly.cn

[S28] C：静态变量
来源：http://bo.szsharing.cn

static int counter = 0;
来源：http://oh.huixinmuqiang.cn

[S29] C：变参函数
来源：http://iz.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eb.shxzukj.cn

[S30] C：头文件保护
来源：http://ao.wgjwhj.cn

#ifndef X_H
来源：http://on.asd995.cn

#define X_H
来源：http://hi.hahajie.cn

#endif
来源：http://km.newstarts.cn

[S31] C++：Hello World
来源：http://dd.haigaiapp.cn

#include <iostream>
来源：http://pc.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://st.jianghongdianzi.cn

[S32] C++：字符串
来源：http://ok.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://gx.newstarts.cn

[S33] C++：vector 增删
来源：http://sf.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://my.gzmigu.cn

[S34] C++：遍历 vector
来源：http://vz.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://sf.bjjhwx.cn

[S35] C++：map
来源：http://jn.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mm.shxzskj.cn

[S36] C++：unordered_map
来源：http://kp.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jb.panjiajie.cn

[S37] C++：set
来源：http://vn.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ro.yuntaijiaju.cn

[S38] C++：排序
来源：http://oj.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://ev.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://jg.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vc.521024.cn

[S40] C++：查找元素
来源：http://as.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://of.hahajie.cn

[S41] C++：类与构造函数
来源：http://pl.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rl.9csxet.cn

[S42] C++：继承与虚函数
来源：http://cv.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://wi.nszjky.cn

[S43] C++：智能指针
来源：http://lo.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://bj.newstarts.cn

[S44] C++：引用传参
来源：http://qt.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://mi.colortex.cn

[S45] C++：lambda
来源：http://re.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vh.gzmigu.cn

[S46] C++：函数模板
来源：http://nb.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gp.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://lv.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mv.szsharing.cn

[S48] C++：逐行读文件
来源：http://qd.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xd.szsharing.cn

while (std::getline(in, line)) { }
来源：http://ey.asd995.cn

[S49] C++：写文件
来源：http://hh.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pf.newstarts.cn

[S50] C++：格式化数字
来源：http://qr.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xm.nicolike.cn

[S51] C++：显式类型转换
来源：http://in.huanxung.cn

static_cast<double>(a) / b
来源：http://us.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://vi.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://co.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://to.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://jt.muxihuayi.cn

[S54] C++：异常处理
来源：http://ag.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zl.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://qc.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ft.gzmigu.cn

[S56] C++：optional
来源：http://qa.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wm.nicolike.cn

[S57] C++：编译期常量
来源：http://qg.bjjhwx.cn

constexpr int N = 10;
来源：http://li.huanxung.cn

[S58] C++：命名空间
来源：http://ol.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://bk.shtwfgs.cn

[S59] C++：静态断言
来源：http://eg.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ji.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://uf.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zu.gzmigu.cn

================================================================================
来源：http://rp.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dn.szxytkj.cn

================================================================================
来源：http://ll.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://jh.newstarts.cn

println("Hello")
来源：http://mm.panjiajie.cn

[T02] Kotlin：变量
来源：http://jm.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tx.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://wt.shxzskj.cn

"值: $b"
来源：http://nt.szxytkj.cn

[T04] Kotlin：空安全
来源：http://sk.asd995.cn

val n: String? = null;  n?.length
来源：http://nu.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://sh.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hs.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://vq.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cm.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://pi.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cz.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://xz.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://nb.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://yd.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://lu.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://tz.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ta.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://il.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hv.asd995.cn

[T12] Kotlin：解构声明
来源：http://sx.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://by.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://pf.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://sg.9csxet.cn

[T14] Kotlin：循环
来源：http://eb.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://ig.panjiajie.cn

[T15] Kotlin：接口
来源：http://lb.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://an.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://jz.bjjhwx.cn

print("Hello")
来源：http://zc.gzmigu.cn

[T17] Swift：变量与常量
来源：http://et.panjiajie.cn

var a = 1;  let b = 2
来源：http://mh.hahajie.cn

[T18] Swift：字符串插值
来源：http://mr.muxihuayi.cn

"值: \(b)"
来源：http://fs.shxzskj.cn

[T19] Swift：可选绑定
来源：http://zb.jctech888.com.cn

if let n = opt { print(n) }
来源：http://cw.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://go.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uj.9csxet.cn

[T21] Swift：遍历
来源：http://je.shtwfgs.cn

for x in a { print(x) }
来源：http://cf.nicolike.cn

[T22] Swift：字典
来源：http://jn.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dd.lnxyls.cn

[T23] Swift：函数
来源：http://fk.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uk.huixiangedu.cn

[T24] Swift：闭包
来源：http://yc.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jh.asd995.cn

[T25] Swift：结构体
来源：http://cp.jctech888.com.cn

struct P { var x: Int }
来源：http://cc.yuexingan06.cn

[T26] Swift：类与重写
来源：http://mb.newstarts.cn

class A: Base { override func f() {} }
来源：http://jg.panjiajie.cn

[T27] Swift：错误处理
来源：http://oe.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://ia.chemitech.net.cn

[T28] Swift：枚举
来源：http://ih.nicolike.cn

enum Color { case red, green }
来源：http://sm.asd995.cn

[T29] Swift：guard 提前返回
来源：http://zo.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://tk.nszjky.cn

[T30] Swift：协议
来源：http://lf.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://no.muxihuayi.cn

[T31] Lua：Hello World
来源：http://ef.lnxyls.cn

print("Hello")
来源：http://rm.521024.cn

[T32] Lua：局部变量
来源：http://zw.haigaiapp.cn

local a = 1
来源：http://uq.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://jl.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yf.yuexingan06.cn

[T34] Lua：遍历表
来源：http://ei.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ds.hnjuh.cn

[T35] Lua：字典表
来源：http://up.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://nf.huixiangedu.cn

[T36] Lua：函数
来源：http://zl.huixiangedu.cn

function add(a, b) return a + b end
来源：http://cp.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://oa.yuexingan06.cn

"a" .. "b"
来源：http://hm.hahajie.cn

[T38] Lua：条件
来源：http://do.asd995.cn

if x > 0 then print("正") end
来源：http://cs.gzmigu.cn

[T39] Lua：模式匹配
来源：http://yv.shtwfgs.cn

string.find(s, "%d+")
来源：http://gi.gzmigu.cn

[T40] Lua：元表
来源：http://vt.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://th.szxytkj.cn

[T41] Perl：Hello World
来源：http://uf.huanxung.cn

print "Hello\n";
来源：http://nk.yuexingan06.cn

[T42] Perl：变量类型
来源：http://zv.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mg.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://ew.newstarts.cn

"值: $a"
来源：http://kn.muxihuayi.cn

[T44] Perl：条件
来源：http://yb.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://bs.asd995.cn

[T45] Perl：数组遍历
来源：http://ek.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://er.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://kh.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://et.nicolike.cn


<!-- 参考信息 -->