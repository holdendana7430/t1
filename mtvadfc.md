代发 wailian999

find . -name "*.log" -type f
来源：http://db.hnjuh.cn

[R44] 按修改时间查找
来源：http://zb.shxzukj.cn

find . -mtime -7 -type f
来源：http://eu.hahajie.cn

[R45] 批量删除
来源：http://cb.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://va.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://tf.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cj.huanxung.cn

[R47] sed 单行替换
来源：http://tu.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ux.hahajie.cn

[R48] awk 取指定列
来源：http://rm.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://sy.hnjuh.cn

[R49] awk 带条件
来源：http://np.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dj.szxytkj.cn

[R50] awk 求和
来源：http://lc.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lw.gzmigu.cn

[R51] 排序去重取前几
来源：http://oj.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bm.szxytkj.cn

[R52] 统计行数
来源：http://ql.asd995.cn

wc -l a.txt
来源：http://vz.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://tk.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xy.yuexingan06.cn

[R54] 比较两个文件
来源：http://uk.yuexingan06.cn

diff a.txt b.txt
来源：http://sc.haigaiapp.cn

[R55] 压缩与解压
来源：http://xz.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vz.shxzukj.cn

[R56] 远程拷贝
来源：http://ga.hnjuh.cn

scp file user@host:/path/
来源：http://xe.bookmarksfly.cn

[R57] 远程执行命令
来源：http://qm.newstarts.cn

ssh user@host 'uptime'
来源：http://lm.panjiajie.cn

[R58] 下载文件
来源：http://xv.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qk.szsharing.cn

[R59] 发 POST JSON
来源：http://jn.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mn.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://wp.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ax.wgjwhj.cn

[R61] 磁盘占用
来源：http://dy.shxzskj.cn

df -h;  du -sh *
来源：http://yt.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://ax.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://ht.asd995.cn

[R63] 内存与进程
来源：http://wv.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://hs.chemitech.net.cn

[R64] 结束进程
来源：http://tn.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://lo.newstarts.cn

[R65] 查看端口占用
来源：http://rj.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kv.yuexingan06.cn

[R66] 定时任务
来源：http://tt.wgjwhj.cn

crontab -e;  crontab -l
来源：http://wd.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://yj.jianghongdianzi.cn

openssl rand -hex 16
来源：http://sm.hnjuh.cn

[R68] 计算文件校验值
来源：http://wi.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ra.bjjhwx.cn

[R69] 生成随机密码
来源：http://yt.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://du.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://up.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://ay.bjjhwx.cn

[R71] 日期格式化
来源：http://ah.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mn.chemitech.net.cn

[R72] 等待端口就绪
来源：http://bq.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ju.huanxung.cn

[R73] 分割大日志
来源：http://bj.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://xp.shtwfgs.cn

[R74] 批量重命名
来源：http://jy.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kz.9csxet.cn

[R75] 导出环境变量
来源：http://dh.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://jf.nicolike.cn

[R76] 使用临时文件
来源：http://qg.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uv.nicolike.cn

[R77] 读取用户输入
来源：http://av.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://vr.shxzukj.cn

[R78] 交互式菜单
来源：http://ua.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uu.bjjhwx.cn

[R79] 解析命令行选项
来源：http://jp.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cj.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://ft.nszjky.cn

time ./run.sh
来源：http://lr.lnxyls.cn

================================================================================
来源：http://py.9csxet.cn

S. C / C++ 专题
来源：http://ma.huanxung.cn

================================================================================
来源：http://bp.hahajie.cn

[S01] C：Hello World
来源：http://eq.9csxet.cn

#include <stdio.h>
来源：http://me.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mc.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://rg.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://hp.nicolike.cn

[S03] C：读入整数
来源：http://xl.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://af.521024.cn

[S04] C：字符串复制
来源：http://ax.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://en.bookmarksfly.cn

[S05] C：字符串长度
来源：http://vo.yuntaijiaju.cn

strlen(s)
来源：http://ia.szsharing.cn

[S06] C：字符串比较
来源：http://ph.shxzskj.cn

strcmp(a, b) == 0
来源：http://xf.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://ep.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uk.asd995.cn

[S08] C：动态内存分配与释放
来源：http://md.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hw.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://ms.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hb.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://ge.nszjky.cn

int *p = &a;  *p = 5;
来源：http://tb.huixiangedu.cn

[S11] C：逐行读文件
来源：http://eg.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://jr.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lj.yuexingan06.cn

fclose(f);
来源：http://xk.yuntaijiaju.cn

[S12] C：写文件
来源：http://sq.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ks.muxihuayi.cn

[S13] C：宏定义
来源：http://um.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://so.haigaiapp.cn

[S14] C：枚举
来源：http://cd.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://ke.nszjky.cn

[S15] C：类型转换
来源：http://ye.shtwfgs.cn

(double) a / b
来源：http://ey.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://si.szsharing.cn

x |= (1 << 3);
来源：http://bz.nszjky.cn

[S17] C：安全拼接字符串
来源：http://kj.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dj.szsharing.cn

[S18] C：命令行参数
来源：http://zp.muxihuayi.cn

int main(int argc, char **argv)
来源：http://tj.muxihuayi.cn

[S19] C：快速排序
来源：http://vf.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ff.colortex.cn

[S20] C：二分查找
来源：http://xs.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xo.newstarts.cn

[S21] C：字符类别判断
来源：http://oo.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vl.szsharing.cn

[S22] C：字符串转数字
来源：http://fu.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cs.gzmigu.cn

[S23] C：随机数
来源：http://ag.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sj.haigaiapp.cn

[S24] C：获取本地时间
来源：http://qv.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kf.panjiajie.cn

[S25] C：内存拷贝
来源：http://bo.hnjuh.cn

memcpy(dst, src, n);
来源：http://iq.hnjuh.cn

[S26] C：内存清零
来源：http://xs.colortex.cn

memset(a, 0, sizeof a);
来源：http://ai.szxytkj.cn

[S27] C：定义常量
来源：http://aw.yuexingan06.cn

const double PI = 3.14159;
来源：http://iy.gzmigu.cn

[S28] C：静态变量
来源：http://df.shtwfgs.cn

static int counter = 0;
来源：http://ou.jianghongdianzi.cn

[S29] C：变参函数
来源：http://xn.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zx.9csxet.cn

[S30] C：头文件保护
来源：http://bl.colortex.cn

#ifndef X_H
来源：http://ju.huanxung.cn

#define X_H
来源：http://lz.9csxet.cn

#endif
来源：http://dq.jctech888.com.cn

[S31] C++：Hello World
来源：http://yp.colortex.cn

#include <iostream>
来源：http://go.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://hg.bookmarksfly.cn

[S32] C++：字符串
来源：http://lt.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://jn.szxytkj.cn

[S33] C++：vector 增删
来源：http://bf.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qp.hahajie.cn

[S34] C++：遍历 vector
来源：http://dn.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://hy.chemitech.net.cn

[S35] C++：map
来源：http://zz.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yy.asd995.cn

[S36] C++：unordered_map
来源：http://we.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bn.huixiangedu.cn

[S37] C++：set
来源：http://tc.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vq.shxzukj.cn

[S38] C++：排序
来源：http://qi.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://pj.521024.cn

[S39] C++：自定义比较器排序
来源：http://bb.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eo.huixiangedu.cn

[S40] C++：查找元素
来源：http://ug.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xf.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://pm.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://op.nszjky.cn

[S42] C++：继承与虚函数
来源：http://tq.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://zx.shxzukj.cn

[S43] C++：智能指针
来源：http://xu.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://cz.wgjwhj.cn

[S44] C++：引用传参
来源：http://ol.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://rn.yuexingan06.cn

[S45] C++：lambda
来源：http://zh.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://or.haigaiapp.cn

[S46] C++：函数模板
来源：http://la.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://is.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://to.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ee.shxzukj.cn

[S48] C++：逐行读文件
来源：http://gc.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kz.szsharing.cn

while (std::getline(in, line)) { }
来源：http://mz.521024.cn

[S49] C++：写文件
来源：http://hn.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bl.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://tr.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pf.panjiajie.cn

[S51] C++：显式类型转换
来源：http://kz.newstarts.cn

static_cast<double>(a) / b
来源：http://xi.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://uy.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://jn.nicolike.cn

[S53] C++：移动语义
来源：http://xp.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://ym.haigaiapp.cn

[S54] C++：异常处理
来源：http://ck.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ua.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://pv.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ae.yuntaijiaju.cn

[S56] C++：optional
来源：http://fh.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pz.colortex.cn

[S57] C++：编译期常量
来源：http://nc.yuntaijiaju.cn

constexpr int N = 10;
来源：http://qe.szsharing.cn

[S58] C++：命名空间
来源：http://hr.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://xi.szsharing.cn

[S59] C++：静态断言
来源：http://aw.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fq.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://sa.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://me.huanxung.cn

================================================================================
来源：http://dy.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yb.521024.cn

================================================================================
来源：http://ky.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://hl.newstarts.cn

println("Hello")
来源：http://qp.nszjky.cn

[T02] Kotlin：变量
来源：http://qb.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kn.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://it.jianghongdianzi.cn

"值: $b"
来源：http://ag.nszjky.cn

[T04] Kotlin：空安全
来源：http://px.gzmigu.cn

val n: String? = null;  n?.length
来源：http://qv.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://hd.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ik.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://jk.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cf.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://yj.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ir.szxytkj.cn

[T08] Kotlin：数据类
来源：http://po.asd995.cn

data class User(val name: String, val age: Int)
来源：http://xr.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://vm.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://sj.521024.cn

[T10] Kotlin：默认参数
来源：http://cn.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qh.gzmigu.cn

[T11] Kotlin：协程
来源：http://ua.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hv.521024.cn

[T12] Kotlin：解构声明
来源：http://do.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://nz.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://rh.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://ft.huanxung.cn

[T14] Kotlin：循环
来源：http://rm.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://zn.nszjky.cn

[T15] Kotlin：接口
来源：http://jr.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://az.gzmigu.cn

[T16] Swift：Hello World
来源：http://dz.yuexingan06.cn

print("Hello")
来源：http://ch.shxzskj.cn

[T17] Swift：变量与常量
来源：http://vs.colortex.cn

var a = 1;  let b = 2
来源：http://nq.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://pq.521024.cn

"值: \(b)"
来源：http://hg.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://bp.lnxyls.cn

if let n = opt { print(n) }
来源：http://ur.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://ru.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gy.bjjhwx.cn

[T21] Swift：遍历
来源：http://br.shxzskj.cn

for x in a { print(x) }
来源：http://wf.521024.cn

[T22] Swift：字典
来源：http://zz.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://za.szsharing.cn

[T23] Swift：函数
来源：http://lu.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nq.muxihuayi.cn

[T24] Swift：闭包
来源：http://gz.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nl.shxzukj.cn

[T25] Swift：结构体
来源：http://gs.lnxyls.cn

struct P { var x: Int }
来源：http://tq.szxytkj.cn

[T26] Swift：类与重写
来源：http://qk.nszjky.cn

class A: Base { override func f() {} }
来源：http://mv.9csxet.cn

[T27] Swift：错误处理
来源：http://sf.521024.cn

do { try f() } catch { print(error) }
来源：http://el.nicolike.cn

[T28] Swift：枚举
来源：http://co.haigaiapp.cn

enum Color { case red, green }
来源：http://nu.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://zw.9csxet.cn

guard let x = opt else { return }
来源：http://om.shtwfgs.cn

[T30] Swift：协议
来源：http://pg.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://ac.bjjhwx.cn

[T31] Lua：Hello World
来源：http://tu.yuntaijiaju.cn

print("Hello")
来源：http://dk.huanxung.cn

[T32] Lua：局部变量
来源：http://fs.szxytkj.cn

local a = 1
来源：http://pa.nszjky.cn

[T33] Lua：表（数组）
来源：http://jr.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lt.wgjwhj.cn

[T34] Lua：遍历表
来源：http://sz.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://me.muxihuayi.cn

[T35] Lua：字典表
来源：http://zp.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://vi.9csxet.cn

[T36] Lua：函数
来源：http://az.jctech888.com.cn

function add(a, b) return a + b end
来源：http://wa.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://rs.huixiangedu.cn

"a" .. "b"
来源：http://iq.huixiangedu.cn

[T38] Lua：条件
来源：http://am.shxzukj.cn

if x > 0 then print("正") end
来源：http://ab.huanxung.cn

[T39] Lua：模式匹配
来源：http://us.asd995.cn

string.find(s, "%d+")
来源：http://wk.9csxet.cn

[T40] Lua：元表
来源：http://ql.asd995.cn

setmetatable({}, { __index = base })
来源：http://vh.newstarts.cn

[T41] Perl：Hello World
来源：http://vs.nszjky.cn

print "Hello\n";
来源：http://sd.huixiangedu.cn

[T42] Perl：变量类型
来源：http://vx.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cf.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://vi.haigaiapp.cn

"值: $a"
来源：http://to.chemitech.net.cn

[T44] Perl：条件
来源：http://yl.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://hu.521024.cn

[T45] Perl：数组遍历
来源：http://jj.colortex.cn

for my $x (@arr) { print $x; }
来源：http://bd.szsharing.cn

[T46] Perl：哈希操作
来源：http://gm.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zh.hahajie.cn


<!-- 参考信息 -->