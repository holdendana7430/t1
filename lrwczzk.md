代发 wailian999

find . -name "*.log" -type f
来源：http://pv.muxihuayi.cn

[R44] 按修改时间查找
来源：http://hp.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://lu.szsharing.cn

[R45] 批量删除
来源：http://qn.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://ru.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://mt.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dv.9csxet.cn

[R47] sed 单行替换
来源：http://ws.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://du.nszjky.cn

[R48] awk 取指定列
来源：http://bi.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://fm.huixiangedu.cn

[R49] awk 带条件
来源：http://vz.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tu.yuntaijiaju.cn

[R50] awk 求和
来源：http://ca.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tw.521024.cn

[R51] 排序去重取前几
来源：http://sr.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oz.szxytkj.cn

[R52] 统计行数
来源：http://pg.newstarts.cn

wc -l a.txt
来源：http://zf.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://ci.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uo.bookmarksfly.cn

[R54] 比较两个文件
来源：http://yy.huixiangedu.cn

diff a.txt b.txt
来源：http://xu.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://zr.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://og.shtwfgs.cn

[R56] 远程拷贝
来源：http://gd.9csxet.cn

scp file user@host:/path/
来源：http://sn.newstarts.cn

[R57] 远程执行命令
来源：http://pg.nszjky.cn

ssh user@host 'uptime'
来源：http://pa.shxzukj.cn

[R58] 下载文件
来源：http://oi.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yf.nicolike.cn

[R59] 发 POST JSON
来源：http://kj.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pz.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://eg.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hk.asd995.cn

[R61] 磁盘占用
来源：http://im.haigaiapp.cn

df -h;  du -sh *
来源：http://hf.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://pm.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://tj.haigaiapp.cn

[R63] 内存与进程
来源：http://jv.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://fv.jianghongdianzi.cn

[R64] 结束进程
来源：http://sp.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://mo.panjiajie.cn

[R65] 查看端口占用
来源：http://vw.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mi.9csxet.cn

[R66] 定时任务
来源：http://dc.nszjky.cn

crontab -e;  crontab -l
来源：http://zc.newstarts.cn

[R67] 生成随机十六进制串
来源：http://mw.szsharing.cn

openssl rand -hex 16
来源：http://er.hnjuh.cn

[R68] 计算文件校验值
来源：http://pq.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hm.szxytkj.cn

[R69] 生成随机密码
来源：http://qy.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://xs.lnxyls.cn

[R70] 时间戳与互转
来源：http://fa.9csxet.cn

date +%s;  date -d @1700000000
来源：http://ub.shtwfgs.cn

[R71] 日期格式化
来源：http://ge.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hw.hahajie.cn

[R72] 等待端口就绪
来源：http://uf.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ea.huixiangedu.cn

[R73] 分割大日志
来源：http://gh.nszjky.cn

split -l 1000 big.log part_
来源：http://su.colortex.cn

[R74] 批量重命名
来源：http://mw.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zx.bjjhwx.cn

[R75] 导出环境变量
来源：http://at.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://jl.521024.cn

[R76] 使用临时文件
来源：http://pr.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yz.hahajie.cn

[R77] 读取用户输入
来源：http://ok.9csxet.cn

read -rp "请输入: " ans
来源：http://cj.nicolike.cn

[R78] 交互式菜单
来源：http://ym.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nm.jctech888.com.cn

[R79] 解析命令行选项
来源：http://qo.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lf.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://lk.shxzukj.cn

time ./run.sh
来源：http://tb.bjjhwx.cn

================================================================================
来源：http://bf.hnjuh.cn

S. C / C++ 专题
来源：http://cu.muxihuayi.cn

================================================================================
来源：http://au.wgjwhj.cn

[S01] C：Hello World
来源：http://fl.szxytkj.cn

#include <stdio.h>
来源：http://wh.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ur.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://ke.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://uj.haigaiapp.cn

[S03] C：读入整数
来源：http://qj.panjiajie.cn

int x; scanf("%d", &x);
来源：http://rj.haigaiapp.cn

[S04] C：字符串复制
来源：http://kc.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://al.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://tp.yuntaijiaju.cn

strlen(s)
来源：http://ep.huixiangedu.cn

[S06] C：字符串比较
来源：http://vp.chemitech.net.cn

strcmp(a, b) == 0
来源：http://cr.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://if.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nx.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://nw.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lt.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://kk.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zn.chemitech.net.cn

[S10] C：指针与解引用
来源：http://gz.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://ns.hahajie.cn

[S11] C：逐行读文件
来源：http://cc.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://wl.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ao.muxihuayi.cn

fclose(f);
来源：http://pq.szsharing.cn

[S12] C：写文件
来源：http://iy.szxytkj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vf.muxihuayi.cn

[S13] C：宏定义
来源：http://zr.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://un.huanxung.cn

[S14] C：枚举
来源：http://zm.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://ve.nicolike.cn

[S15] C：类型转换
来源：http://ng.szxytkj.cn

(double) a / b
来源：http://bc.yuexingan06.cn

[S16] C：位操作置位
来源：http://zt.hnjuh.cn

x |= (1 << 3);
来源：http://yg.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://co.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xh.shxzukj.cn

[S18] C：命令行参数
来源：http://ue.521024.cn

int main(int argc, char **argv)
来源：http://dv.huixiangedu.cn

[S19] C：快速排序
来源：http://bw.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zl.szxytkj.cn

[S20] C：二分查找
来源：http://ya.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fh.shtwfgs.cn

[S21] C：字符类别判断
来源：http://kg.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ga.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://gz.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gi.chemitech.net.cn

[S23] C：随机数
来源：http://dg.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pl.wgjwhj.cn

[S24] C：获取本地时间
来源：http://xg.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sn.shxzskj.cn

[S25] C：内存拷贝
来源：http://qx.hnjuh.cn

memcpy(dst, src, n);
来源：http://pc.jianghongdianzi.cn

[S26] C：内存清零
来源：http://nw.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://sv.asd995.cn

[S27] C：定义常量
来源：http://qk.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://qi.bookmarksfly.cn

[S28] C：静态变量
来源：http://qq.muxihuayi.cn

static int counter = 0;
来源：http://fz.colortex.cn

[S29] C：变参函数
来源：http://zo.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uk.nicolike.cn

[S30] C：头文件保护
来源：http://yq.bookmarksfly.cn

#ifndef X_H
来源：http://ft.9csxet.cn

#define X_H
来源：http://av.huanxung.cn

#endif
来源：http://ng.huixiangedu.cn

[S31] C++：Hello World
来源：http://vw.shxzukj.cn

#include <iostream>
来源：http://go.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://mq.newstarts.cn

[S32] C++：字符串
来源：http://fj.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://hh.shtwfgs.cn

[S33] C++：vector 增删
来源：http://lt.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gy.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://er.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://ha.wgjwhj.cn

[S35] C++：map
来源：http://pr.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mf.bjjhwx.cn

[S36] C++：unordered_map
来源：http://iu.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://io.szxytkj.cn

[S37] C++：set
来源：http://ru.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pe.colortex.cn

[S38] C++：排序
来源：http://ko.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://le.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://zz.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cn.gzmigu.cn

[S40] C++：查找元素
来源：http://ep.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xm.huanxung.cn

[S41] C++：类与构造函数
来源：http://pa.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qx.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://bo.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://th.shxzskj.cn

[S43] C++：智能指针
来源：http://re.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://hy.shtwfgs.cn

[S44] C++：引用传参
来源：http://ve.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://un.nicolike.cn

[S45] C++：lambda
来源：http://yx.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xq.shxzskj.cn

[S46] C++：函数模板
来源：http://cx.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ww.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://wl.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lm.521024.cn

[S48] C++：逐行读文件
来源：http://un.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zh.nszjky.cn

while (std::getline(in, line)) { }
来源：http://mp.panjiajie.cn

[S49] C++：写文件
来源：http://gi.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cx.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://ec.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ab.hnjuh.cn

[S51] C++：显式类型转换
来源：http://qc.wgjwhj.cn

static_cast<double>(a) / b
来源：http://kv.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://ge.521024.cn

int size() const noexcept { return n_; }
来源：http://qf.szsharing.cn

[S53] C++：移动语义
来源：http://ho.colortex.cn

std::vector<int> w = std::move(v);
来源：http://rl.hnjuh.cn

[S54] C++：异常处理
来源：http://dn.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oy.shxzukj.cn

[S55] C++：结构化绑定
来源：http://gd.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mr.nicolike.cn

[S56] C++：optional
来源：http://qg.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zc.panjiajie.cn

[S57] C++：编译期常量
来源：http://ix.jctech888.com.cn

constexpr int N = 10;
来源：http://fu.panjiajie.cn

[S58] C++：命名空间
来源：http://ps.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://fk.9csxet.cn

[S59] C++：静态断言
来源：http://sv.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ye.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://xv.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ik.bjjhwx.cn

================================================================================
来源：http://xl.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sz.nicolike.cn

================================================================================
来源：http://tz.hahajie.cn

[T01] Kotlin：Hello World
来源：http://ox.shxzukj.cn

println("Hello")
来源：http://bl.shtwfgs.cn

[T02] Kotlin：变量
来源：http://wd.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ui.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://kn.jctech888.com.cn

"值: $b"
来源：http://ts.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://ng.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://ut.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://ey.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jk.9csxet.cn

[T06] Kotlin：集合映射
来源：http://ha.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fx.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://tn.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kr.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://ii.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://kn.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://vr.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://qb.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://ot.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nf.asd995.cn

[T11] Kotlin：协程
来源：http://rs.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://an.hahajie.cn

[T12] Kotlin：解构声明
来源：http://ck.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://tm.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://ai.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://rb.gzmigu.cn

[T14] Kotlin：循环
来源：http://ha.nszjky.cn

for (i in 1..10) println(i)
来源：http://tt.bjjhwx.cn

[T15] Kotlin：接口
来源：http://qq.szsharing.cn

interface Shape { fun area(): Double }
来源：http://eg.lnxyls.cn

[T16] Swift：Hello World
来源：http://yy.jctech888.com.cn

print("Hello")
来源：http://gt.hnjuh.cn

[T17] Swift：变量与常量
来源：http://gm.shtwfgs.cn

var a = 1;  let b = 2
来源：http://vj.shxzukj.cn

[T18] Swift：字符串插值
来源：http://ft.panjiajie.cn

"值: \(b)"
来源：http://ff.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://lb.gzmigu.cn

if let n = opt { print(n) }
来源：http://yt.jctech888.com.cn

[T20] Swift：数组操作
来源：http://bd.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ft.huixiangedu.cn

[T21] Swift：遍历
来源：http://al.yuexingan06.cn

for x in a { print(x) }
来源：http://ij.huanxung.cn

[T22] Swift：字典
来源：http://tn.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ew.lnxyls.cn

[T23] Swift：函数
来源：http://gv.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rl.gzmigu.cn

[T24] Swift：闭包
来源：http://ul.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ss.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://bq.chemitech.net.cn

struct P { var x: Int }
来源：http://wi.hnjuh.cn

[T26] Swift：类与重写
来源：http://sf.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://pb.shxzskj.cn

[T27] Swift：错误处理
来源：http://rr.nszjky.cn

do { try f() } catch { print(error) }
来源：http://jm.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://po.9csxet.cn

enum Color { case red, green }
来源：http://vd.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://km.colortex.cn

guard let x = opt else { return }
来源：http://li.colortex.cn

[T30] Swift：协议
来源：http://nl.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://yf.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://ax.jctech888.com.cn

print("Hello")
来源：http://or.szxytkj.cn

[T32] Lua：局部变量
来源：http://ks.shxzskj.cn

local a = 1
来源：http://jj.huanxung.cn

[T33] Lua：表（数组）
来源：http://zx.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://br.bjjhwx.cn

[T34] Lua：遍历表
来源：http://yt.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jj.lnxyls.cn

[T35] Lua：字典表
来源：http://fj.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://jh.shxzskj.cn

[T36] Lua：函数
来源：http://tr.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://zl.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://aj.szxytkj.cn

"a" .. "b"
来源：http://qz.wgjwhj.cn

[T38] Lua：条件
来源：http://fy.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://bk.szsharing.cn

[T39] Lua：模式匹配
来源：http://nl.colortex.cn

string.find(s, "%d+")
来源：http://qa.huixiangedu.cn

[T40] Lua：元表
来源：http://al.nszjky.cn

setmetatable({}, { __index = base })
来源：http://rr.colortex.cn

[T41] Perl：Hello World
来源：http://zf.nszjky.cn

print "Hello\n";
来源：http://ea.shtwfgs.cn

[T42] Perl：变量类型
来源：http://fn.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hr.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://zu.shxzskj.cn

"值: $a"
来源：http://el.lnxyls.cn

[T44] Perl：条件
来源：http://ou.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://it.9csxet.cn

[T45] Perl：数组遍历
来源：http://zd.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://iy.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://qb.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zz.gzmigu.cn


<!-- 参考信息 -->