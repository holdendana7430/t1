代发 wailian999

find . -name "*.log" -type f
来源：http://wd.yuexingan06.cn

[R44] 按修改时间查找
来源：http://wq.wgjwhj.cn

find . -mtime -7 -type f
来源：http://nf.9csxet.cn

[R45] 批量删除
来源：http://ur.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://ns.gzmigu.cn

[R46] 递归替换文件内容
来源：http://rv.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://co.szsharing.cn

[R47] sed 单行替换
来源：http://nf.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://iy.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://jh.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://iw.haigaiapp.cn

[R49] awk 带条件
来源：http://am.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bd.hahajie.cn

[R50] awk 求和
来源：http://tb.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hz.asd995.cn

[R51] 排序去重取前几
来源：http://gg.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jh.lnxyls.cn

[R52] 统计行数
来源：http://jr.nszjky.cn

wc -l a.txt
来源：http://lq.colortex.cn

[R53] 查看文件头与实时尾
来源：http://zi.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://na.shtwfgs.cn

[R54] 比较两个文件
来源：http://ln.shtwfgs.cn

diff a.txt b.txt
来源：http://ai.huanxung.cn

[R55] 压缩与解压
来源：http://kp.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://av.bookmarksfly.cn

[R56] 远程拷贝
来源：http://az.jianghongdianzi.cn

scp file user@host:/path/
来源：http://qs.szsharing.cn

[R57] 远程执行命令
来源：http://bd.chemitech.net.cn

ssh user@host 'uptime'
来源：http://ct.haigaiapp.cn

[R58] 下载文件
来源：http://hh.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kx.jctech888.com.cn

[R59] 发 POST JSON
来源：http://ig.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eh.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://kp.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sb.szxytkj.cn

[R61] 磁盘占用
来源：http://yj.panjiajie.cn

df -h;  du -sh *
来源：http://ad.hahajie.cn

[R62] 找最占空间的文件
来源：http://mg.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://py.nszjky.cn

[R63] 内存与进程
来源：http://cc.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://tp.jianghongdianzi.cn

[R64] 结束进程
来源：http://rd.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://ho.lnxyls.cn

[R65] 查看端口占用
来源：http://vp.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pu.asd995.cn

[R66] 定时任务
来源：http://ga.yuexingan06.cn

crontab -e;  crontab -l
来源：http://bk.hahajie.cn

[R67] 生成随机十六进制串
来源：http://kd.huixiangedu.cn

openssl rand -hex 16
来源：http://uo.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://hi.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vq.szxytkj.cn

[R69] 生成随机密码
来源：http://tm.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://sa.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://vg.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://wk.panjiajie.cn

[R71] 日期格式化
来源：http://qx.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yu.newstarts.cn

[R72] 等待端口就绪
来源：http://im.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://px.shxzskj.cn

[R73] 分割大日志
来源：http://qj.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://wh.hahajie.cn

[R74] 批量重命名
来源：http://lj.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cj.shxzukj.cn

[R75] 导出环境变量
来源：http://rh.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://xt.muxihuayi.cn

[R76] 使用临时文件
来源：http://xu.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sf.wgjwhj.cn

[R77] 读取用户输入
来源：http://wd.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://yo.haigaiapp.cn

[R78] 交互式菜单
来源：http://vz.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fa.521024.cn

[R79] 解析命令行选项
来源：http://gk.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hr.colortex.cn

[R80] 查看脚本执行耗时
来源：http://qg.bookmarksfly.cn

time ./run.sh
来源：http://xq.bookmarksfly.cn

================================================================================
来源：http://iw.bookmarksfly.cn

S. C / C++ 专题
来源：http://jn.9csxet.cn

================================================================================
来源：http://wg.jianghongdianzi.cn

[S01] C：Hello World
来源：http://sp.jctech888.com.cn

#include <stdio.h>
来源：http://gp.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vu.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://dk.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://ly.9csxet.cn

[S03] C：读入整数
来源：http://rl.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://ll.asd995.cn

[S04] C：字符串复制
来源：http://km.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uj.nszjky.cn

[S05] C：字符串长度
来源：http://du.521024.cn

strlen(s)
来源：http://jz.haigaiapp.cn

[S06] C：字符串比较
来源：http://fk.bjjhwx.cn

strcmp(a, b) == 0
来源：http://bz.9csxet.cn

[S07] C：数组遍历求和
来源：http://yo.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pb.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://lf.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rc.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://rd.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://um.nszjky.cn

[S10] C：指针与解引用
来源：http://tn.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://ir.nszjky.cn

[S11] C：逐行读文件
来源：http://eh.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://rv.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xy.colortex.cn

fclose(f);
来源：http://ec.chemitech.net.cn

[S12] C：写文件
来源：http://do.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://or.hnjuh.cn

[S13] C：宏定义
来源：http://hp.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fu.panjiajie.cn

[S14] C：枚举
来源：http://tm.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://aj.shtwfgs.cn

[S15] C：类型转换
来源：http://yh.huanxung.cn

(double) a / b
来源：http://ay.huanxung.cn

[S16] C：位操作置位
来源：http://ac.521024.cn

x |= (1 << 3);
来源：http://se.nicolike.cn

[S17] C：安全拼接字符串
来源：http://qx.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nn.szxytkj.cn

[S18] C：命令行参数
来源：http://qx.nicolike.cn

int main(int argc, char **argv)
来源：http://ja.jctech888.com.cn

[S19] C：快速排序
来源：http://fz.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ht.lnxyls.cn

[S20] C：二分查找
来源：http://ke.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://du.shxzskj.cn

[S21] C：字符类别判断
来源：http://ur.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rn.huixiangedu.cn

[S22] C：字符串转数字
来源：http://ia.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fg.huixiangedu.cn

[S23] C：随机数
来源：http://og.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jg.hnjuh.cn

[S24] C：获取本地时间
来源：http://ba.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dc.huixiangedu.cn

[S25] C：内存拷贝
来源：http://es.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://jy.gzmigu.cn

[S26] C：内存清零
来源：http://ia.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://kt.chemitech.net.cn

[S27] C：定义常量
来源：http://xf.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://hd.jctech888.com.cn

[S28] C：静态变量
来源：http://en.521024.cn

static int counter = 0;
来源：http://up.haigaiapp.cn

[S29] C：变参函数
来源：http://bv.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vm.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://mg.haigaiapp.cn

#ifndef X_H
来源：http://rn.chemitech.net.cn

#define X_H
来源：http://zx.wgjwhj.cn

#endif
来源：http://xt.huanxung.cn

[S31] C++：Hello World
来源：http://io.jctech888.com.cn

#include <iostream>
来源：http://vs.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://zb.nszjky.cn

[S32] C++：字符串
来源：http://fm.colortex.cn

std::string s = "hi";  s += "!";
来源：http://dz.newstarts.cn

[S33] C++：vector 增删
来源：http://lv.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://in.gzmigu.cn

[S34] C++：遍历 vector
来源：http://ev.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://ju.hahajie.cn

[S35] C++：map
来源：http://gv.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://un.chemitech.net.cn

[S36] C++：unordered_map
来源：http://qq.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uj.colortex.cn

[S37] C++：set
来源：http://rj.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ui.huixiangedu.cn

[S38] C++：排序
来源：http://zt.colortex.cn

std::sort(v.begin(), v.end());
来源：http://ot.asd995.cn

[S39] C++：自定义比较器排序
来源：http://jt.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mx.bookmarksfly.cn

[S40] C++：查找元素
来源：http://av.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xj.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://li.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tf.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://ri.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://of.521024.cn

[S43] C++：智能指针
来源：http://ui.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://yx.szsharing.cn

[S44] C++：引用传参
来源：http://aa.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://cz.bjjhwx.cn

[S45] C++：lambda
来源：http://ik.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://px.newstarts.cn

[S46] C++：函数模板
来源：http://uu.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cl.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://av.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vr.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://kn.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jf.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://ui.shtwfgs.cn

[S49] C++：写文件
来源：http://oq.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mi.asd995.cn

[S50] C++：格式化数字
来源：http://wf.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tw.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://kd.shtwfgs.cn

static_cast<double>(a) / b
来源：http://bd.521024.cn

[S52] C++：const 与 noexcept
来源：http://nj.huanxung.cn

int size() const noexcept { return n_; }
来源：http://zg.haigaiapp.cn

[S53] C++：移动语义
来源：http://ao.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://iy.asd995.cn

[S54] C++：异常处理
来源：http://cy.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jf.521024.cn

[S55] C++：结构化绑定
来源：http://iq.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oq.szxytkj.cn

[S56] C++：optional
来源：http://cs.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mt.panjiajie.cn

[S57] C++：编译期常量
来源：http://kj.huixiangedu.cn

constexpr int N = 10;
来源：http://te.lnxyls.cn

[S58] C++：命名空间
来源：http://pg.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://iy.bookmarksfly.cn

[S59] C++：静态断言
来源：http://rh.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qw.colortex.cn

[S60] C++：遍历并删除元素
来源：http://xd.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://te.newstarts.cn

================================================================================
来源：http://xc.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ds.9csxet.cn

================================================================================
来源：http://eb.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://lj.szxytkj.cn

println("Hello")
来源：http://ee.asd995.cn

[T02] Kotlin：变量
来源：http://tz.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cd.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://vi.chemitech.net.cn

"值: $b"
来源：http://vu.hnjuh.cn

[T04] Kotlin：空安全
来源：http://aw.shxzskj.cn

val n: String? = null;  n?.length
来源：http://mn.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://wo.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zj.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://fd.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oo.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://lt.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ac.521024.cn

[T08] Kotlin：数据类
来源：http://mx.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://oy.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://er.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://hh.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://eo.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://se.szxytkj.cn

[T11] Kotlin：协程
来源：http://wp.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://db.nicolike.cn

[T12] Kotlin：解构声明
来源：http://ox.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://oj.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://sr.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://gs.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://tj.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://hl.nicolike.cn

[T15] Kotlin：接口
来源：http://op.asd995.cn

interface Shape { fun area(): Double }
来源：http://xf.9csxet.cn

[T16] Swift：Hello World
来源：http://az.shxzskj.cn

print("Hello")
来源：http://xv.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://hg.yuexingan06.cn

var a = 1;  let b = 2
来源：http://mo.hnjuh.cn

[T18] Swift：字符串插值
来源：http://dp.jctech888.com.cn

"值: \(b)"
来源：http://xj.hahajie.cn

[T19] Swift：可选绑定
来源：http://lj.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://ky.hahajie.cn

[T20] Swift：数组操作
来源：http://jp.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://el.nicolike.cn

[T21] Swift：遍历
来源：http://dw.szxytkj.cn

for x in a { print(x) }
来源：http://dq.yuntaijiaju.cn

[T22] Swift：字典
来源：http://mf.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uv.shxzskj.cn

[T23] Swift：函数
来源：http://hj.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ke.hahajie.cn

[T24] Swift：闭包
来源：http://zb.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gp.szsharing.cn

[T25] Swift：结构体
来源：http://xc.gzmigu.cn

struct P { var x: Int }
来源：http://nf.huanxung.cn

[T26] Swift：类与重写
来源：http://rt.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://wv.hnjuh.cn

[T27] Swift：错误处理
来源：http://ah.huanxung.cn

do { try f() } catch { print(error) }
来源：http://ds.bookmarksfly.cn

[T28] Swift：枚举
来源：http://yf.shxzskj.cn

enum Color { case red, green }
来源：http://sf.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://sc.newstarts.cn

guard let x = opt else { return }
来源：http://yv.jctech888.com.cn

[T30] Swift：协议
来源：http://jj.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://ys.panjiajie.cn

[T31] Lua：Hello World
来源：http://rh.nszjky.cn

print("Hello")
来源：http://jf.lnxyls.cn

[T32] Lua：局部变量
来源：http://dc.gzmigu.cn

local a = 1
来源：http://hx.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://be.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bt.szsharing.cn

[T34] Lua：遍历表
来源：http://vw.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ui.wgjwhj.cn

[T35] Lua：字典表
来源：http://ts.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://oy.huixinmuqiang.cn

[T36] Lua：函数
来源：http://le.521024.cn

function add(a, b) return a + b end
来源：http://pp.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://yy.asd995.cn

"a" .. "b"
来源：http://vy.gzmigu.cn

[T38] Lua：条件
来源：http://he.wgjwhj.cn

if x > 0 then print("正") end
来源：http://ps.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://up.9csxet.cn

string.find(s, "%d+")
来源：http://oh.shxzukj.cn

[T40] Lua：元表
来源：http://oh.colortex.cn

setmetatable({}, { __index = base })
来源：http://jj.muxihuayi.cn

[T41] Perl：Hello World
来源：http://bk.huixiangedu.cn

print "Hello\n";
来源：http://mj.bjjhwx.cn

[T42] Perl：变量类型
来源：http://ua.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ne.521024.cn

[T43] Perl：字符串插值
来源：http://qw.haigaiapp.cn

"值: $a"
来源：http://us.colortex.cn

[T44] Perl：条件
来源：http://gj.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://tb.huanxung.cn

[T45] Perl：数组遍历
来源：http://ys.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://iy.szsharing.cn

[T46] Perl：哈希操作
来源：http://fk.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bp.lnxyls.cn


<!-- 参考信息 -->