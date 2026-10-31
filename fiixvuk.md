代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://jw.asd995.cn

[R36] 并发执行多个任务
来源：http://ri.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://da.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://bo.bookmarksfly.cn

files=$(ls -1)
来源：http://pk.huanxung.cn

[R38] 管道串联
来源：http://td.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://cs.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://mr.bjjhwx.cn

cmd > out.log 2>&1
来源：http://ct.huixinmuqiang.cn

[R40] 追加写日志
来源：http://dt.huixinmuqiang.cn

echo "log" >> out.log
来源：http://ta.521024.cn

[R41] 丢弃输出
来源：http://iv.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://sx.hahajie.cn

[R42] 输入重定向
来源：http://nk.jianghongdianzi.cn

wc -l < a.txt
来源：http://te.hahajie.cn

[R43] 按名字查找文件
来源：http://lc.panjiajie.cn

find . -name "*.log" -type f
来源：http://zs.nicolike.cn

[R44] 按修改时间查找
来源：http://gn.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://mq.haigaiapp.cn

[R45] 批量删除
来源：http://uh.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://zt.huanxung.cn

[R46] 递归替换文件内容
来源：http://pg.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bz.nszjky.cn

[R47] sed 单行替换
来源：http://fy.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yh.asd995.cn

[R48] awk 取指定列
来源：http://vl.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://js.shxzskj.cn

[R49] awk 带条件
来源：http://kf.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://is.muxihuayi.cn

[R50] awk 求和
来源：http://gu.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ad.lnxyls.cn

[R51] 排序去重取前几
来源：http://ev.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://be.bookmarksfly.cn

[R52] 统计行数
来源：http://bq.chemitech.net.cn

wc -l a.txt
来源：http://ou.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://ry.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lr.szsharing.cn

[R54] 比较两个文件
来源：http://yc.nicolike.cn

diff a.txt b.txt
来源：http://eo.shtwfgs.cn

[R55] 压缩与解压
来源：http://xc.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://od.wgjwhj.cn

[R56] 远程拷贝
来源：http://bt.shxzukj.cn

scp file user@host:/path/
来源：http://pe.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://ap.jctech888.com.cn

ssh user@host 'uptime'
来源：http://lo.yuntaijiaju.cn

[R58] 下载文件
来源：http://jl.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vv.haigaiapp.cn

[R59] 发 POST JSON
来源：http://la.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://du.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://ne.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fz.newstarts.cn

[R61] 磁盘占用
来源：http://dl.yuntaijiaju.cn

df -h;  du -sh *
来源：http://kw.nszjky.cn

[R62] 找最占空间的文件
来源：http://dj.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://lr.521024.cn

[R63] 内存与进程
来源：http://sf.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://el.muxihuayi.cn

[R64] 结束进程
来源：http://qr.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://tc.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://lw.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zb.yuntaijiaju.cn

[R66] 定时任务
来源：http://jb.shtwfgs.cn

crontab -e;  crontab -l
来源：http://iw.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://va.9csxet.cn

openssl rand -hex 16
来源：http://fd.hnjuh.cn

[R68] 计算文件校验值
来源：http://xf.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nv.asd995.cn

[R69] 生成随机密码
来源：http://yx.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://ij.521024.cn

[R70] 时间戳与互转
来源：http://lj.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://he.yuexingan06.cn

[R71] 日期格式化
来源：http://va.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mf.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://rl.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qi.hnjuh.cn

[R73] 分割大日志
来源：http://ad.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://ss.huixinmuqiang.cn

[R74] 批量重命名
来源：http://om.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zg.jianghongdianzi.cn

[R75] 导出环境变量
来源：http://kt.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://be.colortex.cn

[R76] 使用临时文件
来源：http://uk.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qz.chemitech.net.cn

[R77] 读取用户输入
来源：http://ea.huixiangedu.cn

read -rp "请输入: " ans
来源：http://qm.wgjwhj.cn

[R78] 交互式菜单
来源：http://fk.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fa.gzmigu.cn

[R79] 解析命令行选项
来源：http://rm.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xm.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://rn.shxzukj.cn

time ./run.sh
来源：http://wk.lnxyls.cn

================================================================================
来源：http://tn.huixiangedu.cn

S. C / C++ 专题
来源：http://eq.szxytkj.cn

================================================================================
来源：http://hl.szxytkj.cn

[S01] C：Hello World
来源：http://es.jianghongdianzi.cn

#include <stdio.h>
来源：http://uc.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ix.huanxung.cn

[S02] C：变量与格式化输出
来源：http://if.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://gq.asd995.cn

[S03] C：读入整数
来源：http://sq.9csxet.cn

int x; scanf("%d", &x);
来源：http://uf.hnjuh.cn

[S04] C：字符串复制
来源：http://yg.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://me.521024.cn

[S05] C：字符串长度
来源：http://jn.gzmigu.cn

strlen(s)
来源：http://gp.shtwfgs.cn

[S06] C：字符串比较
来源：http://qj.jctech888.com.cn

strcmp(a, b) == 0
来源：http://mw.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://dl.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zm.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://rh.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nv.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://ea.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://um.hnjuh.cn

[S10] C：指针与解引用
来源：http://kc.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://ky.nicolike.cn

[S11] C：逐行读文件
来源：http://pf.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://zu.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://so.szxytkj.cn

fclose(f);
来源：http://ar.hnjuh.cn

[S12] C：写文件
来源：http://ge.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://np.wgjwhj.cn

[S13] C：宏定义
来源：http://jx.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kt.bookmarksfly.cn

[S14] C：枚举
来源：http://kn.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://qt.huixiangedu.cn

[S15] C：类型转换
来源：http://db.huixinmuqiang.cn

(double) a / b
来源：http://uw.9csxet.cn

[S16] C：位操作置位
来源：http://fy.szsharing.cn

x |= (1 << 3);
来源：http://cj.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://zp.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cm.hnjuh.cn

[S18] C：命令行参数
来源：http://qb.huanxung.cn

int main(int argc, char **argv)
来源：http://zj.gzmigu.cn

[S19] C：快速排序
来源：http://es.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mz.jianghongdianzi.cn

[S20] C：二分查找
来源：http://hi.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fj.9csxet.cn

[S21] C：字符类别判断
来源：http://ax.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cr.hnjuh.cn

[S22] C：字符串转数字
来源：http://rb.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tt.gzmigu.cn

[S23] C：随机数
来源：http://kk.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ep.shxzskj.cn

[S24] C：获取本地时间
来源：http://mi.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pj.colortex.cn

[S25] C：内存拷贝
来源：http://sa.shxzskj.cn

memcpy(dst, src, n);
来源：http://wj.muxihuayi.cn

[S26] C：内存清零
来源：http://ah.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://hg.shxzukj.cn

[S27] C：定义常量
来源：http://bw.haigaiapp.cn

const double PI = 3.14159;
来源：http://yd.newstarts.cn

[S28] C：静态变量
来源：http://js.bookmarksfly.cn

static int counter = 0;
来源：http://xu.bjjhwx.cn

[S29] C：变参函数
来源：http://eb.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uh.yuexingan06.cn

[S30] C：头文件保护
来源：http://bt.chemitech.net.cn

#ifndef X_H
来源：http://mx.lnxyls.cn

#define X_H
来源：http://zx.jianghongdianzi.cn

#endif
来源：http://gc.bookmarksfly.cn

[S31] C++：Hello World
来源：http://rz.panjiajie.cn

#include <iostream>
来源：http://pl.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://jr.lnxyls.cn

[S32] C++：字符串
来源：http://zo.521024.cn

std::string s = "hi";  s += "!";
来源：http://db.wgjwhj.cn

[S33] C++：vector 增删
来源：http://zw.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rd.lnxyls.cn

[S34] C++：遍历 vector
来源：http://um.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://kr.lnxyls.cn

[S35] C++：map
来源：http://xn.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gt.hnjuh.cn

[S36] C++：unordered_map
来源：http://yi.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ob.9csxet.cn

[S37] C++：set
来源：http://th.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hj.hahajie.cn

[S38] C++：排序
来源：http://et.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://bc.asd995.cn

[S39] C++：自定义比较器排序
来源：http://lu.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yh.521024.cn

[S40] C++：查找元素
来源：http://ss.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bb.huanxung.cn

[S41] C++：类与构造函数
来源：http://es.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dc.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://dg.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://el.521024.cn

[S43] C++：智能指针
来源：http://uj.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://bk.bjjhwx.cn

[S44] C++：引用传参
来源：http://xp.hahajie.cn

void inc(int &x) { ++x; }
来源：http://pr.chemitech.net.cn

[S45] C++：lambda
来源：http://mx.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fy.haigaiapp.cn

[S46] C++：函数模板
来源：http://zh.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xj.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://ap.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jg.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://ql.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iv.9csxet.cn

while (std::getline(in, line)) { }
来源：http://zo.shtwfgs.cn

[S49] C++：写文件
来源：http://nw.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ji.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://pu.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://du.szxytkj.cn

[S51] C++：显式类型转换
来源：http://rp.521024.cn

static_cast<double>(a) / b
来源：http://vn.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://yt.nicolike.cn

int size() const noexcept { return n_; }
来源：http://pj.szsharing.cn

[S53] C++：移动语义
来源：http://ik.asd995.cn

std::vector<int> w = std::move(v);
来源：http://tu.shxzukj.cn

[S54] C++：异常处理
来源：http://ax.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uy.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://hv.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hx.colortex.cn

[S56] C++：optional
来源：http://rh.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ps.colortex.cn

[S57] C++：编译期常量
来源：http://sy.hahajie.cn

constexpr int N = 10;
来源：http://wi.szxytkj.cn

[S58] C++：命名空间
来源：http://yy.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://oj.nicolike.cn

[S59] C++：静态断言
来源：http://el.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ru.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://zf.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oh.hnjuh.cn

================================================================================
来源：http://fb.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oh.haigaiapp.cn

================================================================================
来源：http://yu.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://md.9csxet.cn

println("Hello")
来源：http://cy.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://yd.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gk.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://kn.nszjky.cn

"值: $b"
来源：http://po.gzmigu.cn

[T04] Kotlin：空安全
来源：http://pi.szxytkj.cn

val n: String? = null;  n?.length
来源：http://fp.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://qw.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bl.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://zh.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sd.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://oz.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mj.asd995.cn

[T08] Kotlin：数据类
来源：http://rq.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://oy.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://ad.asd995.cn

fun String.exclaim() = this + "!"
来源：http://pk.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://kz.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dh.9csxet.cn

[T11] Kotlin：协程
来源：http://jg.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jq.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://oz.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://nh.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://hi.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://hg.panjiajie.cn

[T14] Kotlin：循环
来源：http://wm.asd995.cn

for (i in 1..10) println(i)
来源：http://xv.bjjhwx.cn

[T15] Kotlin：接口
来源：http://sd.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://jo.nicolike.cn

[T16] Swift：Hello World
来源：http://na.gzmigu.cn

print("Hello")
来源：http://dm.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://hf.521024.cn

var a = 1;  let b = 2
来源：http://ml.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://nl.wgjwhj.cn

"值: \(b)"
来源：http://pb.shxzskj.cn

[T19] Swift：可选绑定
来源：http://td.chemitech.net.cn

if let n = opt { print(n) }
来源：http://sh.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://zp.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://il.shxzukj.cn

[T21] Swift：遍历
来源：http://qo.panjiajie.cn

for x in a { print(x) }
来源：http://kq.jianghongdianzi.cn

[T22] Swift：字典
来源：http://rx.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://id.hnjuh.cn

[T23] Swift：函数
来源：http://mr.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qh.szxytkj.cn

[T24] Swift：闭包
来源：http://dr.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ao.lnxyls.cn

[T25] Swift：结构体
来源：http://kw.huixiangedu.cn

struct P { var x: Int }
来源：http://pz.szxytkj.cn

[T26] Swift：类与重写
来源：http://xz.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://fm.shtwfgs.cn

[T27] Swift：错误处理
来源：http://ws.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://dz.asd995.cn

[T28] Swift：枚举
来源：http://sl.haigaiapp.cn

enum Color { case red, green }
来源：http://cp.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://cg.asd995.cn

guard let x = opt else { return }
来源：http://zj.huixinmuqiang.cn

[T30] Swift：协议
来源：http://qx.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://tn.haigaiapp.cn

[T31] Lua：Hello World
来源：http://nj.jctech888.com.cn

print("Hello")
来源：http://nf.jctech888.com.cn

[T32] Lua：局部变量
来源：http://fw.shtwfgs.cn

local a = 1
来源：http://mk.shxzskj.cn

[T33] Lua：表（数组）
来源：http://jj.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ns.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://ml.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jn.huanxung.cn

[T35] Lua：字典表
来源：http://rt.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://qj.yuntaijiaju.cn

[T36] Lua：函数
来源：http://mw.huanxung.cn

function add(a, b) return a + b end
来源：http://ou.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://fi.bookmarksfly.cn

"a" .. "b"
来源：http://ll.yuntaijiaju.cn

[T38] Lua：条件
来源：http://jf.huixiangedu.cn

if x > 0 then print("正") end
来源：http://ai.yuntaijiaju.cn


<!-- 参考信息 -->