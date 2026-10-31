代发 wailian999

cmd >/dev/null 2>&1
来源：http://uv.wgjwhj.cn

[R42] 输入重定向
来源：http://hs.nicolike.cn

wc -l < a.txt
来源：http://iy.haigaiapp.cn

[R43] 按名字查找文件
来源：http://fn.521024.cn

find . -name "*.log" -type f
来源：http://ip.shxzukj.cn

[R44] 按修改时间查找
来源：http://fx.lnxyls.cn

find . -mtime -7 -type f
来源：http://zw.wgjwhj.cn

[R45] 批量删除
来源：http://jd.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://ii.nicolike.cn

[R46] 递归替换文件内容
来源：http://uk.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bp.shxzskj.cn

[R47] sed 单行替换
来源：http://lt.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ba.nicolike.cn

[R48] awk 取指定列
来源：http://pr.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://wq.521024.cn

[R49] awk 带条件
来源：http://xx.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ul.bookmarksfly.cn

[R50] awk 求和
来源：http://kg.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dh.shxzukj.cn

[R51] 排序去重取前几
来源：http://lp.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ux.nszjky.cn

[R52] 统计行数
来源：http://lg.yuntaijiaju.cn

wc -l a.txt
来源：http://kx.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://aj.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hf.chemitech.net.cn

[R54] 比较两个文件
来源：http://ez.9csxet.cn

diff a.txt b.txt
来源：http://td.jctech888.com.cn

[R55] 压缩与解压
来源：http://ak.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ga.bjjhwx.cn

[R56] 远程拷贝
来源：http://dp.panjiajie.cn

scp file user@host:/path/
来源：http://pq.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://zp.shtwfgs.cn

ssh user@host 'uptime'
来源：http://ee.lnxyls.cn

[R58] 下载文件
来源：http://xk.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ys.colortex.cn

[R59] 发 POST JSON
来源：http://zi.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nd.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://nz.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://py.lnxyls.cn

[R61] 磁盘占用
来源：http://um.yuntaijiaju.cn

df -h;  du -sh *
来源：http://xh.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://uh.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://pe.szsharing.cn

[R63] 内存与进程
来源：http://bs.521024.cn

free -h;  ps aux | grep nginx
来源：http://ol.huixiangedu.cn

[R64] 结束进程
来源：http://bt.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://qc.szxytkj.cn

[R65] 查看端口占用
来源：http://zi.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sq.szxytkj.cn

[R66] 定时任务
来源：http://gg.chemitech.net.cn

crontab -e;  crontab -l
来源：http://rk.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://yo.bookmarksfly.cn

openssl rand -hex 16
来源：http://zk.shxzukj.cn

[R68] 计算文件校验值
来源：http://vs.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ew.chemitech.net.cn

[R69] 生成随机密码
来源：http://qk.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://mo.shxzukj.cn

[R70] 时间戳与互转
来源：http://tg.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://wh.hnjuh.cn

[R71] 日期格式化
来源：http://zk.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pf.szsharing.cn

[R72] 等待端口就绪
来源：http://io.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dy.huixiangedu.cn

[R73] 分割大日志
来源：http://ug.chemitech.net.cn

split -l 1000 big.log part_
来源：http://qp.chemitech.net.cn

[R74] 批量重命名
来源：http://kq.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://av.chemitech.net.cn

[R75] 导出环境变量
来源：http://hx.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://bp.9csxet.cn

[R76] 使用临时文件
来源：http://wq.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nu.bjjhwx.cn

[R77] 读取用户输入
来源：http://qv.521024.cn

read -rp "请输入: " ans
来源：http://bb.newstarts.cn

[R78] 交互式菜单
来源：http://lu.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xm.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://qt.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pb.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://uy.521024.cn

time ./run.sh
来源：http://pr.gzmigu.cn

================================================================================
来源：http://mf.wgjwhj.cn

S. C / C++ 专题
来源：http://pl.wgjwhj.cn

================================================================================
来源：http://lh.asd995.cn

[S01] C：Hello World
来源：http://ge.shxzukj.cn

#include <stdio.h>
来源：http://pc.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ki.hahajie.cn

[S02] C：变量与格式化输出
来源：http://vn.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://jm.huixinmuqiang.cn

[S03] C：读入整数
来源：http://ui.hnjuh.cn

int x; scanf("%d", &x);
来源：http://cv.521024.cn

[S04] C：字符串复制
来源：http://cc.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rn.hahajie.cn

[S05] C：字符串长度
来源：http://ww.huixinmuqiang.cn

strlen(s)
来源：http://di.gzmigu.cn

[S06] C：字符串比较
来源：http://gm.521024.cn

strcmp(a, b) == 0
来源：http://vw.newstarts.cn

[S07] C：数组遍历求和
来源：http://iu.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ey.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://iy.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qq.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://wr.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sa.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://xx.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://fu.huixiangedu.cn

[S11] C：逐行读文件
来源：http://yv.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://vy.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wz.chemitech.net.cn

fclose(f);
来源：http://cu.panjiajie.cn

[S12] C：写文件
来源：http://fm.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sx.newstarts.cn

[S13] C：宏定义
来源：http://pt.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uh.yuntaijiaju.cn

[S14] C：枚举
来源：http://ok.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://ok.huanxung.cn

[S15] C：类型转换
来源：http://qc.wgjwhj.cn

(double) a / b
来源：http://zs.haigaiapp.cn

[S16] C：位操作置位
来源：http://yi.shxzskj.cn

x |= (1 << 3);
来源：http://mo.521024.cn

[S17] C：安全拼接字符串
来源：http://jr.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kn.colortex.cn

[S18] C：命令行参数
来源：http://cs.nicolike.cn

int main(int argc, char **argv)
来源：http://fq.wgjwhj.cn

[S19] C：快速排序
来源：http://re.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oa.nszjky.cn

[S20] C：二分查找
来源：http://gn.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://np.newstarts.cn

[S21] C：字符类别判断
来源：http://zq.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tx.wgjwhj.cn

[S22] C：字符串转数字
来源：http://kx.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nr.asd995.cn

[S23] C：随机数
来源：http://ug.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://km.huixiangedu.cn

[S24] C：获取本地时间
来源：http://jz.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eg.521024.cn

[S25] C：内存拷贝
来源：http://cc.wgjwhj.cn

memcpy(dst, src, n);
来源：http://rm.shtwfgs.cn

[S26] C：内存清零
来源：http://bs.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://uo.hnjuh.cn

[S27] C：定义常量
来源：http://es.wgjwhj.cn

const double PI = 3.14159;
来源：http://bw.lnxyls.cn

[S28] C：静态变量
来源：http://kg.colortex.cn

static int counter = 0;
来源：http://qh.asd995.cn

[S29] C：变参函数
来源：http://mt.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cc.shtwfgs.cn

[S30] C：头文件保护
来源：http://cc.szsharing.cn

#ifndef X_H
来源：http://no.gzmigu.cn

#define X_H
来源：http://he.521024.cn

#endif
来源：http://va.panjiajie.cn

[S31] C++：Hello World
来源：http://rk.shtwfgs.cn

#include <iostream>
来源：http://mn.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://my.yuexingan06.cn

[S32] C++：字符串
来源：http://tp.asd995.cn

std::string s = "hi";  s += "!";
来源：http://aa.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://xp.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ar.panjiajie.cn

[S34] C++：遍历 vector
来源：http://gp.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://ge.bookmarksfly.cn

[S35] C++：map
来源：http://ry.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ek.jctech888.com.cn

[S36] C++：unordered_map
来源：http://pr.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bv.szxytkj.cn

[S37] C++：set
来源：http://rv.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ag.521024.cn

[S38] C++：排序
来源：http://cm.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://us.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://su.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qd.nicolike.cn

[S40] C++：查找元素
来源：http://bi.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bg.shxzukj.cn

[S41] C++：类与构造函数
来源：http://ag.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://so.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://kk.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://gx.newstarts.cn

[S43] C++：智能指针
来源：http://mk.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://jf.lnxyls.cn

[S44] C++：引用传参
来源：http://lj.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://ie.colortex.cn

[S45] C++：lambda
来源：http://fz.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://du.muxihuayi.cn

[S46] C++：函数模板
来源：http://oz.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qt.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://pd.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uq.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://oo.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ln.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://qx.huanxung.cn

[S49] C++：写文件
来源：http://ca.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ly.shxzukj.cn

[S50] C++：格式化数字
来源：http://ng.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lr.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://fj.newstarts.cn

static_cast<double>(a) / b
来源：http://ec.asd995.cn

[S52] C++：const 与 noexcept
来源：http://ot.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://dl.521024.cn

[S53] C++：移动语义
来源：http://gl.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://qt.wgjwhj.cn

[S54] C++：异常处理
来源：http://nt.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zk.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://yf.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zr.nszjky.cn

[S56] C++：optional
来源：http://er.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kb.shxzukj.cn

[S57] C++：编译期常量
来源：http://mu.huixinmuqiang.cn

constexpr int N = 10;
来源：http://na.asd995.cn

[S58] C++：命名空间
来源：http://uf.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://bm.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://ih.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ar.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://mx.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wd.shxzskj.cn

================================================================================
来源：http://lb.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://li.521024.cn

================================================================================
来源：http://zk.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://zy.jianghongdianzi.cn

println("Hello")
来源：http://uj.hahajie.cn

[T02] Kotlin：变量
来源：http://uj.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oi.colortex.cn

[T03] Kotlin：字符串模板
来源：http://az.muxihuayi.cn

"值: $b"
来源：http://do.hahajie.cn

[T04] Kotlin：空安全
来源：http://go.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://qz.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://in.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mq.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://kt.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://di.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://gm.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xj.shxzskj.cn

[T08] Kotlin：数据类
来源：http://qf.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://ri.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://ux.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://ve.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://cx.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rm.shtwfgs.cn

[T11] Kotlin：协程
来源：http://nx.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xy.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://pg.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://vg.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://cb.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://rs.9csxet.cn

[T14] Kotlin：循环
来源：http://rn.colortex.cn

for (i in 1..10) println(i)
来源：http://ef.9csxet.cn

[T15] Kotlin：接口
来源：http://ge.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://fe.nicolike.cn

[T16] Swift：Hello World
来源：http://lb.shtwfgs.cn

print("Hello")
来源：http://tf.lnxyls.cn

[T17] Swift：变量与常量
来源：http://oi.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://mo.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://qb.panjiajie.cn

"值: \(b)"
来源：http://rs.szsharing.cn

[T19] Swift：可选绑定
来源：http://ug.panjiajie.cn

if let n = opt { print(n) }
来源：http://cp.szsharing.cn

[T20] Swift：数组操作
来源：http://ir.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ku.asd995.cn

[T21] Swift：遍历
来源：http://mf.chemitech.net.cn

for x in a { print(x) }
来源：http://lv.shxzskj.cn

[T22] Swift：字典
来源：http://gj.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://al.haigaiapp.cn

[T23] Swift：函数
来源：http://gy.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ji.gzmigu.cn

[T24] Swift：闭包
来源：http://cc.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sn.asd995.cn

[T25] Swift：结构体
来源：http://ou.yuntaijiaju.cn

struct P { var x: Int }
来源：http://yj.yuexingan06.cn

[T26] Swift：类与重写
来源：http://xi.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://jh.nicolike.cn

[T27] Swift：错误处理
来源：http://av.colortex.cn

do { try f() } catch { print(error) }
来源：http://zt.chemitech.net.cn

[T28] Swift：枚举
来源：http://ce.521024.cn

enum Color { case red, green }
来源：http://hj.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://lg.bjjhwx.cn

guard let x = opt else { return }
来源：http://cp.haigaiapp.cn

[T30] Swift：协议
来源：http://tn.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://fd.nicolike.cn

[T31] Lua：Hello World
来源：http://np.shtwfgs.cn

print("Hello")
来源：http://hx.shxzukj.cn

[T32] Lua：局部变量
来源：http://uo.yuntaijiaju.cn

local a = 1
来源：http://vw.nszjky.cn

[T33] Lua：表（数组）
来源：http://yt.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sa.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://gi.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ul.muxihuayi.cn

[T35] Lua：字典表
来源：http://zs.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://bb.nszjky.cn

[T36] Lua：函数
来源：http://wb.jctech888.com.cn

function add(a, b) return a + b end
来源：http://oc.colortex.cn

[T37] Lua：字符串拼接
来源：http://zu.muxihuayi.cn

"a" .. "b"
来源：http://ki.panjiajie.cn

[T38] Lua：条件
来源：http://cl.nicolike.cn

if x > 0 then print("正") end
来源：http://fr.shxzukj.cn

[T39] Lua：模式匹配
来源：http://gs.colortex.cn

string.find(s, "%d+")
来源：http://qm.szxytkj.cn

[T40] Lua：元表
来源：http://qg.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://ut.bjjhwx.cn

[T41] Perl：Hello World
来源：http://jg.newstarts.cn

print "Hello\n";
来源：http://ib.chemitech.net.cn

[T42] Perl：变量类型
来源：http://qi.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kq.hnjuh.cn

[T43] Perl：字符串插值
来源：http://fm.wgjwhj.cn

"值: $a"
来源：http://ye.szsharing.cn

[T44] Perl：条件
来源：http://do.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://tu.wgjwhj.cn


<!-- 参考信息 -->