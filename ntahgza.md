代发 wailian999

files=$(ls -1)
来源：http://pt.shtwfgs.cn

[R38] 管道串联
来源：http://jf.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://yc.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://as.nszjky.cn

cmd > out.log 2>&1
来源：http://rj.hahajie.cn

[R40] 追加写日志
来源：http://ck.nicolike.cn

echo "log" >> out.log
来源：http://aw.hahajie.cn

[R41] 丢弃输出
来源：http://kz.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://qh.shtwfgs.cn

[R42] 输入重定向
来源：http://or.szsharing.cn

wc -l < a.txt
来源：http://ij.lnxyls.cn

[R43] 按名字查找文件
来源：http://hv.lnxyls.cn

find . -name "*.log" -type f
来源：http://rl.haigaiapp.cn

[R44] 按修改时间查找
来源：http://ih.hnjuh.cn

find . -mtime -7 -type f
来源：http://sd.nicolike.cn

[R45] 批量删除
来源：http://yi.9csxet.cn

find . -name "*.tmp" -delete
来源：http://ca.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://ts.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xu.huixiangedu.cn

[R47] sed 单行替换
来源：http://pm.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lb.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://us.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://fi.asd995.cn

[R49] awk 带条件
来源：http://rc.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://so.muxihuayi.cn

[R50] awk 求和
来源：http://pd.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cz.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://fp.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jf.wgjwhj.cn

[R52] 统计行数
来源：http://es.newstarts.cn

wc -l a.txt
来源：http://mg.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://yi.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://co.nicolike.cn

[R54] 比较两个文件
来源：http://xi.yuexingan06.cn

diff a.txt b.txt
来源：http://os.colortex.cn

[R55] 压缩与解压
来源：http://oz.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hv.huanxung.cn

[R56] 远程拷贝
来源：http://vd.huixiangedu.cn

scp file user@host:/path/
来源：http://ed.bookmarksfly.cn

[R57] 远程执行命令
来源：http://yq.nicolike.cn

ssh user@host 'uptime'
来源：http://ke.asd995.cn

[R58] 下载文件
来源：http://rs.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bl.yuexingan06.cn

[R59] 发 POST JSON
来源：http://tp.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vn.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://ye.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tg.9csxet.cn

[R61] 磁盘占用
来源：http://vn.yuexingan06.cn

df -h;  du -sh *
来源：http://qy.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://xb.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://pe.haigaiapp.cn

[R63] 内存与进程
来源：http://fz.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://et.haigaiapp.cn

[R64] 结束进程
来源：http://oq.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://bh.shxzukj.cn

[R65] 查看端口占用
来源：http://ty.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ue.hnjuh.cn

[R66] 定时任务
来源：http://bq.hahajie.cn

crontab -e;  crontab -l
来源：http://ar.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://rr.shtwfgs.cn

openssl rand -hex 16
来源：http://mi.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://ub.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lo.huixiangedu.cn

[R69] 生成随机密码
来源：http://vx.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://qz.szsharing.cn

[R70] 时间戳与互转
来源：http://ga.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://qt.gzmigu.cn

[R71] 日期格式化
来源：http://ox.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gs.newstarts.cn

[R72] 等待端口就绪
来源：http://gh.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ys.muxihuayi.cn

[R73] 分割大日志
来源：http://mh.lnxyls.cn

split -l 1000 big.log part_
来源：http://fi.yuexingan06.cn

[R74] 批量重命名
来源：http://yy.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://el.shxzskj.cn

[R75] 导出环境变量
来源：http://qb.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://yr.9csxet.cn

[R76] 使用临时文件
来源：http://fk.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fu.muxihuayi.cn

[R77] 读取用户输入
来源：http://cm.haigaiapp.cn

read -rp "请输入: " ans
来源：http://of.colortex.cn

[R78] 交互式菜单
来源：http://ca.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nl.chemitech.net.cn

[R79] 解析命令行选项
来源：http://uv.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fa.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://av.nicolike.cn

time ./run.sh
来源：http://is.chemitech.net.cn

================================================================================
来源：http://gn.nicolike.cn

S. C / C++ 专题
来源：http://mz.huixiangedu.cn

================================================================================
来源：http://rj.bookmarksfly.cn

[S01] C：Hello World
来源：http://ou.huixiangedu.cn

#include <stdio.h>
来源：http://xr.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yo.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://py.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://tr.shxzukj.cn

[S03] C：读入整数
来源：http://cm.szxytkj.cn

int x; scanf("%d", &x);
来源：http://ff.lnxyls.cn

[S04] C：字符串复制
来源：http://wl.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nt.nicolike.cn

[S05] C：字符串长度
来源：http://uk.nicolike.cn

strlen(s)
来源：http://qv.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://sj.newstarts.cn

strcmp(a, b) == 0
来源：http://ug.9csxet.cn

[S07] C：数组遍历求和
来源：http://nf.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bh.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://kz.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nl.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://gq.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vb.hahajie.cn

[S10] C：指针与解引用
来源：http://ks.asd995.cn

int *p = &a;  *p = 5;
来源：http://un.hnjuh.cn

[S11] C：逐行读文件
来源：http://mg.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://rs.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ka.hnjuh.cn

fclose(f);
来源：http://qv.muxihuayi.cn

[S12] C：写文件
来源：http://xs.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mi.szxytkj.cn

[S13] C：宏定义
来源：http://dg.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jx.yuntaijiaju.cn

[S14] C：枚举
来源：http://hx.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://sk.haigaiapp.cn

[S15] C：类型转换
来源：http://jj.yuexingan06.cn

(double) a / b
来源：http://ni.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://ga.lnxyls.cn

x |= (1 << 3);
来源：http://kn.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://qd.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rd.panjiajie.cn

[S18] C：命令行参数
来源：http://ul.huixiangedu.cn

int main(int argc, char **argv)
来源：http://uc.nicolike.cn

[S19] C：快速排序
来源：http://jj.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://he.bookmarksfly.cn

[S20] C：二分查找
来源：http://kf.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ku.yuexingan06.cn

[S21] C：字符类别判断
来源：http://xr.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dc.yuexingan06.cn

[S22] C：字符串转数字
来源：http://zg.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wl.shtwfgs.cn

[S23] C：随机数
来源：http://xw.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ci.haigaiapp.cn

[S24] C：获取本地时间
来源：http://ce.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iv.gzmigu.cn

[S25] C：内存拷贝
来源：http://jn.huixiangedu.cn

memcpy(dst, src, n);
来源：http://yn.newstarts.cn

[S26] C：内存清零
来源：http://yz.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://kp.muxihuayi.cn

[S27] C：定义常量
来源：http://xr.huixiangedu.cn

const double PI = 3.14159;
来源：http://ly.asd995.cn

[S28] C：静态变量
来源：http://ai.bookmarksfly.cn

static int counter = 0;
来源：http://lx.shxzukj.cn

[S29] C：变参函数
来源：http://gk.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bi.chemitech.net.cn

[S30] C：头文件保护
来源：http://ah.shxzskj.cn

#ifndef X_H
来源：http://sx.shxzskj.cn

#define X_H
来源：http://mz.panjiajie.cn

#endif
来源：http://lk.9csxet.cn

[S31] C++：Hello World
来源：http://od.asd995.cn

#include <iostream>
来源：http://um.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://ty.521024.cn

[S32] C++：字符串
来源：http://vm.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://se.9csxet.cn

[S33] C++：vector 增删
来源：http://fg.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://da.szsharing.cn

[S34] C++：遍历 vector
来源：http://xq.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://vg.huanxung.cn

[S35] C++：map
来源：http://bt.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ov.shxzskj.cn

[S36] C++：unordered_map
来源：http://ua.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tt.shxzskj.cn

[S37] C++：set
来源：http://xs.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vl.jctech888.com.cn

[S38] C++：排序
来源：http://ey.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://cc.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://by.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://po.newstarts.cn

[S40] C++：查找元素
来源：http://gx.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hv.huanxung.cn

[S41] C++：类与构造函数
来源：http://se.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wj.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://kz.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://ts.huanxung.cn

[S43] C++：智能指针
来源：http://bt.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://sf.gzmigu.cn

[S44] C++：引用传参
来源：http://la.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://uf.hahajie.cn

[S45] C++：lambda
来源：http://ib.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gs.hahajie.cn

[S46] C++：函数模板
来源：http://ly.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qg.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://tc.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fl.newstarts.cn

[S48] C++：逐行读文件
来源：http://qi.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://eg.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://pv.jianghongdianzi.cn

[S49] C++：写文件
来源：http://xg.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mi.hahajie.cn

[S50] C++：格式化数字
来源：http://zi.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ji.huanxung.cn

[S51] C++：显式类型转换
来源：http://sl.nicolike.cn

static_cast<double>(a) / b
来源：http://dy.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://oz.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://ga.yuexingan06.cn

[S53] C++：移动语义
来源：http://ms.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://sb.chemitech.net.cn

[S54] C++：异常处理
来源：http://gc.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nb.panjiajie.cn

[S55] C++：结构化绑定
来源：http://eq.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ug.muxihuayi.cn

[S56] C++：optional
来源：http://gl.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gu.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://eo.yuntaijiaju.cn

constexpr int N = 10;
来源：http://md.gzmigu.cn

[S58] C++：命名空间
来源：http://fb.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://ml.asd995.cn

[S59] C++：静态断言
来源：http://jb.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qp.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://sl.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ev.colortex.cn

================================================================================
来源：http://ci.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bd.huixinmuqiang.cn

================================================================================
来源：http://or.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://rw.huixinmuqiang.cn

println("Hello")
来源：http://tl.hahajie.cn

[T02] Kotlin：变量
来源：http://si.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rq.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://yz.szxytkj.cn

"值: $b"
来源：http://qv.lnxyls.cn

[T04] Kotlin：空安全
来源：http://kn.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://md.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://hr.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xh.521024.cn

[T06] Kotlin：集合映射
来源：http://vd.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://en.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://uu.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://de.shxzukj.cn

[T08] Kotlin：数据类
来源：http://wh.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://bq.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://fo.colortex.cn

fun String.exclaim() = this + "!"
来源：http://oc.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://uu.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://id.panjiajie.cn

[T11] Kotlin：协程
来源：http://au.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ur.nicolike.cn

[T12] Kotlin：解构声明
来源：http://jn.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://iq.colortex.cn

[T13] Kotlin：只读 Map
来源：http://vq.nicolike.cn

val m = mapOf("a" to 1)
来源：http://qz.colortex.cn

[T14] Kotlin：循环
来源：http://ao.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://kl.hahajie.cn

[T15] Kotlin：接口
来源：http://po.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://vv.newstarts.cn

[T16] Swift：Hello World
来源：http://gd.yuexingan06.cn

print("Hello")
来源：http://ti.9csxet.cn

[T17] Swift：变量与常量
来源：http://wb.hnjuh.cn

var a = 1;  let b = 2
来源：http://ie.huanxung.cn

[T18] Swift：字符串插值
来源：http://mc.muxihuayi.cn

"值: \(b)"
来源：http://zv.shxzukj.cn

[T19] Swift：可选绑定
来源：http://ji.lnxyls.cn

if let n = opt { print(n) }
来源：http://jd.huanxung.cn

[T20] Swift：数组操作
来源：http://da.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tg.jctech888.com.cn

[T21] Swift：遍历
来源：http://fq.panjiajie.cn

for x in a { print(x) }
来源：http://mu.shxzukj.cn

[T22] Swift：字典
来源：http://ro.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cd.hnjuh.cn

[T23] Swift：函数
来源：http://ac.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://au.muxihuayi.cn

[T24] Swift：闭包
来源：http://bw.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ol.nicolike.cn

[T25] Swift：结构体
来源：http://tt.newstarts.cn

struct P { var x: Int }
来源：http://ym.jctech888.com.cn

[T26] Swift：类与重写
来源：http://ip.hahajie.cn

class A: Base { override func f() {} }
来源：http://qe.huanxung.cn

[T27] Swift：错误处理
来源：http://rd.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://ii.szxytkj.cn

[T28] Swift：枚举
来源：http://wq.colortex.cn

enum Color { case red, green }
来源：http://uc.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://gg.haigaiapp.cn

guard let x = opt else { return }
来源：http://wf.colortex.cn

[T30] Swift：协议
来源：http://iw.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://mf.9csxet.cn

[T31] Lua：Hello World
来源：http://pc.9csxet.cn

print("Hello")
来源：http://um.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://rc.bookmarksfly.cn

local a = 1
来源：http://ya.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://bu.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jj.szsharing.cn

[T34] Lua：遍历表
来源：http://ko.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://km.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://qf.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://sr.nicolike.cn

[T36] Lua：函数
来源：http://hn.huixiangedu.cn

function add(a, b) return a + b end
来源：http://ra.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://aa.szxytkj.cn

"a" .. "b"
来源：http://fa.521024.cn

[T38] Lua：条件
来源：http://oe.haigaiapp.cn

if x > 0 then print("正") end
来源：http://vf.asd995.cn

[T39] Lua：模式匹配
来源：http://zt.asd995.cn

string.find(s, "%d+")
来源：http://tc.gzmigu.cn

[T40] Lua：元表
来源：http://ru.nszjky.cn

setmetatable({}, { __index = base })
来源：http://qm.huixinmuqiang.cn


<!-- 参考信息 -->