代发 wailian999

cmd >/dev/null 2>&1
来源：http://vq.chemitech.net.cn

[R42] 输入重定向
来源：http://sc.bjjhwx.cn

wc -l < a.txt
来源：http://xv.hahajie.cn

[R43] 按名字查找文件
来源：http://ts.lnxyls.cn

find . -name "*.log" -type f
来源：http://dl.shxzskj.cn

[R44] 按修改时间查找
来源：http://sd.szxytkj.cn

find . -mtime -7 -type f
来源：http://fb.muxihuayi.cn

[R45] 批量删除
来源：http://qw.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://nj.szsharing.cn

[R46] 递归替换文件内容
来源：http://qn.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://na.shxzukj.cn

[R47] sed 单行替换
来源：http://qq.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vt.panjiajie.cn

[R48] awk 取指定列
来源：http://ep.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://na.panjiajie.cn

[R49] awk 带条件
来源：http://qs.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ki.jctech888.com.cn

[R50] awk 求和
来源：http://iu.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xj.huanxung.cn

[R51] 排序去重取前几
来源：http://ul.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vk.shxzskj.cn

[R52] 统计行数
来源：http://cz.hahajie.cn

wc -l a.txt
来源：http://gn.521024.cn

[R53] 查看文件头与实时尾
来源：http://pr.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yu.yuexingan06.cn

[R54] 比较两个文件
来源：http://vx.haigaiapp.cn

diff a.txt b.txt
来源：http://zb.jctech888.com.cn

[R55] 压缩与解压
来源：http://vd.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://up.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://mh.muxihuayi.cn

scp file user@host:/path/
来源：http://yb.newstarts.cn

[R57] 远程执行命令
来源：http://ml.nszjky.cn

ssh user@host 'uptime'
来源：http://vk.huixiangedu.cn

[R58] 下载文件
来源：http://ps.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://km.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://ay.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qt.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://sn.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://li.chemitech.net.cn

[R61] 磁盘占用
来源：http://ug.jianghongdianzi.cn

df -h;  du -sh *
来源：http://og.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://xz.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://vs.yuntaijiaju.cn

[R63] 内存与进程
来源：http://sj.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://yq.szxytkj.cn

[R64] 结束进程
来源：http://ns.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://hs.hahajie.cn

[R65] 查看端口占用
来源：http://ph.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rt.shxzukj.cn

[R66] 定时任务
来源：http://ol.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://zt.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://vg.gzmigu.cn

openssl rand -hex 16
来源：http://vv.huixiangedu.cn

[R68] 计算文件校验值
来源：http://eg.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ud.hnjuh.cn

[R69] 生成随机密码
来源：http://md.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://mo.huanxung.cn

[R70] 时间戳与互转
来源：http://pc.9csxet.cn

date +%s;  date -d @1700000000
来源：http://od.szxytkj.cn

[R71] 日期格式化
来源：http://bz.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bq.9csxet.cn

[R72] 等待端口就绪
来源：http://tx.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://um.jianghongdianzi.cn

[R73] 分割大日志
来源：http://oz.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://wa.yuexingan06.cn

[R74] 批量重命名
来源：http://su.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aa.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://og.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://fa.wgjwhj.cn

[R76] 使用临时文件
来源：http://os.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gl.lnxyls.cn

[R77] 读取用户输入
来源：http://mr.muxihuayi.cn

read -rp "请输入: " ans
来源：http://qf.9csxet.cn

[R78] 交互式菜单
来源：http://yq.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jc.panjiajie.cn

[R79] 解析命令行选项
来源：http://gq.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sq.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://ur.yuexingan06.cn

time ./run.sh
来源：http://te.bjjhwx.cn

================================================================================
来源：http://dy.bookmarksfly.cn

S. C / C++ 专题
来源：http://tr.haigaiapp.cn

================================================================================
来源：http://gm.newstarts.cn

[S01] C：Hello World
来源：http://ec.bookmarksfly.cn

#include <stdio.h>
来源：http://uw.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qy.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://yb.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://om.nszjky.cn

[S03] C：读入整数
来源：http://ji.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://dl.wgjwhj.cn

[S04] C：字符串复制
来源：http://wo.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rb.huixiangedu.cn

[S05] C：字符串长度
来源：http://kr.bookmarksfly.cn

strlen(s)
来源：http://ci.jctech888.com.cn

[S06] C：字符串比较
来源：http://cv.bjjhwx.cn

strcmp(a, b) == 0
来源：http://cf.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://op.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pm.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://gw.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ah.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://pc.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fc.haigaiapp.cn

[S10] C：指针与解引用
来源：http://ey.9csxet.cn

int *p = &a;  *p = 5;
来源：http://ei.haigaiapp.cn

[S11] C：逐行读文件
来源：http://ea.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://xp.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sb.asd995.cn

fclose(f);
来源：http://hz.szsharing.cn

[S12] C：写文件
来源：http://qa.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sq.chemitech.net.cn

[S13] C：宏定义
来源：http://sy.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yl.asd995.cn

[S14] C：枚举
来源：http://dr.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://le.shtwfgs.cn

[S15] C：类型转换
来源：http://oc.jctech888.com.cn

(double) a / b
来源：http://st.yuexingan06.cn

[S16] C：位操作置位
来源：http://ii.nicolike.cn

x |= (1 << 3);
来源：http://qh.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://rn.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qz.yuexingan06.cn

[S18] C：命令行参数
来源：http://rc.bjjhwx.cn

int main(int argc, char **argv)
来源：http://gy.szsharing.cn

[S19] C：快速排序
来源：http://xj.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iv.shxzukj.cn

[S20] C：二分查找
来源：http://ht.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vw.bjjhwx.cn

[S21] C：字符类别判断
来源：http://tw.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hh.wgjwhj.cn

[S22] C：字符串转数字
来源：http://oa.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rt.shtwfgs.cn

[S23] C：随机数
来源：http://oi.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lw.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://hb.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ut.szsharing.cn

[S25] C：内存拷贝
来源：http://lq.wgjwhj.cn

memcpy(dst, src, n);
来源：http://xu.gzmigu.cn

[S26] C：内存清零
来源：http://jy.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://xl.yuexingan06.cn

[S27] C：定义常量
来源：http://kx.newstarts.cn

const double PI = 3.14159;
来源：http://xp.shxzskj.cn

[S28] C：静态变量
来源：http://pp.shxzskj.cn

static int counter = 0;
来源：http://mq.jctech888.com.cn

[S29] C：变参函数
来源：http://ja.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yo.szsharing.cn

[S30] C：头文件保护
来源：http://iw.hnjuh.cn

#ifndef X_H
来源：http://au.jianghongdianzi.cn

#define X_H
来源：http://rz.huixiangedu.cn

#endif
来源：http://ng.nszjky.cn

[S31] C++：Hello World
来源：http://sg.haigaiapp.cn

#include <iostream>
来源：http://cu.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://sj.muxihuayi.cn

[S32] C++：字符串
来源：http://nh.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://qh.huanxung.cn

[S33] C++：vector 增删
来源：http://yb.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gm.521024.cn

[S34] C++：遍历 vector
来源：http://vq.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://ut.shtwfgs.cn

[S35] C++：map
来源：http://md.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hp.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://dh.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://js.huixinmuqiang.cn

[S37] C++：set
来源：http://br.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kw.newstarts.cn

[S38] C++：排序
来源：http://tq.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://tv.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://xj.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vu.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://gx.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uq.lnxyls.cn

[S41] C++：类与构造函数
来源：http://wn.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bg.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://wr.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://ei.bjjhwx.cn

[S43] C++：智能指针
来源：http://ui.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://qq.bookmarksfly.cn

[S44] C++：引用传参
来源：http://zs.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://ns.wgjwhj.cn

[S45] C++：lambda
来源：http://xh.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://eb.gzmigu.cn

[S46] C++：函数模板
来源：http://tn.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ih.521024.cn

[S47] C++：结构化绑定遍历
来源：http://ol.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dh.shxzskj.cn

[S48] C++：逐行读文件
来源：http://ib.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ms.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://cd.huixiangedu.cn

[S49] C++：写文件
来源：http://nb.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kw.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://tf.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xf.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://vo.jctech888.com.cn

static_cast<double>(a) / b
来源：http://so.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://ev.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://yi.szxytkj.cn

[S53] C++：移动语义
来源：http://un.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://oy.szsharing.cn

[S54] C++：异常处理
来源：http://xf.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gc.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://gk.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ft.huanxung.cn

[S56] C++：optional
来源：http://li.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bz.szxytkj.cn

[S57] C++：编译期常量
来源：http://fb.newstarts.cn

constexpr int N = 10;
来源：http://et.huanxung.cn

[S58] C++：命名空间
来源：http://zv.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://ak.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://hg.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ta.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://pa.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yx.gzmigu.cn

================================================================================
来源：http://da.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nk.szxytkj.cn

================================================================================
来源：http://vg.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://ub.muxihuayi.cn

println("Hello")
来源：http://ca.bjjhwx.cn

[T02] Kotlin：变量
来源：http://vy.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ix.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://wy.jctech888.com.cn

"值: $b"
来源：http://ny.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://de.asd995.cn

val n: String? = null;  n?.length
来源：http://au.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://dh.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tp.hahajie.cn

[T06] Kotlin：集合映射
来源：http://ez.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jk.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://ru.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zu.szsharing.cn

[T08] Kotlin：数据类
来源：http://lh.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://tn.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://cr.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://jx.asd995.cn

[T10] Kotlin：默认参数
来源：http://sa.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cd.shxzukj.cn

[T11] Kotlin：协程
来源：http://kg.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gm.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://qi.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://kg.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://tc.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://gi.panjiajie.cn

[T14] Kotlin：循环
来源：http://cg.szsharing.cn

for (i in 1..10) println(i)
来源：http://gz.shtwfgs.cn

[T15] Kotlin：接口
来源：http://ff.asd995.cn

interface Shape { fun area(): Double }
来源：http://rs.colortex.cn

[T16] Swift：Hello World
来源：http://ah.szsharing.cn

print("Hello")
来源：http://ji.szsharing.cn

[T17] Swift：变量与常量
来源：http://ka.szsharing.cn

var a = 1;  let b = 2
来源：http://qe.panjiajie.cn

[T18] Swift：字符串插值
来源：http://jh.wgjwhj.cn

"值: \(b)"
来源：http://ou.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://tz.shxzskj.cn

if let n = opt { print(n) }
来源：http://hw.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://gs.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ho.huixiangedu.cn

[T21] Swift：遍历
来源：http://vv.huixiangedu.cn

for x in a { print(x) }
来源：http://pv.shtwfgs.cn

[T22] Swift：字典
来源：http://ux.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uo.lnxyls.cn

[T23] Swift：函数
来源：http://cp.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gm.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://te.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qp.nicolike.cn

[T25] Swift：结构体
来源：http://jm.chemitech.net.cn

struct P { var x: Int }
来源：http://dv.huixiangedu.cn

[T26] Swift：类与重写
来源：http://jl.panjiajie.cn

class A: Base { override func f() {} }
来源：http://aa.panjiajie.cn

[T27] Swift：错误处理
来源：http://qk.nicolike.cn

do { try f() } catch { print(error) }
来源：http://ku.asd995.cn

[T28] Swift：枚举
来源：http://py.shxzskj.cn

enum Color { case red, green }
来源：http://xf.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://di.huixiangedu.cn

guard let x = opt else { return }
来源：http://sr.jianghongdianzi.cn

[T30] Swift：协议
来源：http://qt.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://cx.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://un.shxzukj.cn

print("Hello")
来源：http://bw.nicolike.cn

[T32] Lua：局部变量
来源：http://vk.yuexingan06.cn

local a = 1
来源：http://kj.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://jd.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zr.shxzukj.cn

[T34] Lua：遍历表
来源：http://xp.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hh.colortex.cn

[T35] Lua：字典表
来源：http://al.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://fv.bjjhwx.cn

[T36] Lua：函数
来源：http://qj.wgjwhj.cn

function add(a, b) return a + b end
来源：http://zw.521024.cn

[T37] Lua：字符串拼接
来源：http://xk.shtwfgs.cn

"a" .. "b"
来源：http://zy.jianghongdianzi.cn

[T38] Lua：条件
来源：http://zm.colortex.cn

if x > 0 then print("正") end
来源：http://ka.nszjky.cn

[T39] Lua：模式匹配
来源：http://rv.9csxet.cn

string.find(s, "%d+")
来源：http://ez.bjjhwx.cn

[T40] Lua：元表
来源：http://ix.nicolike.cn

setmetatable({}, { __index = base })
来源：http://ih.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://tb.huanxung.cn

print "Hello\n";
来源：http://ol.szsharing.cn

[T42] Perl：变量类型
来源：http://rk.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kg.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://wn.lnxyls.cn

"值: $a"
来源：http://ez.yuexingan06.cn

[T44] Perl：条件
来源：http://cl.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://ak.jctech888.com.cn


<!-- 参考信息 -->