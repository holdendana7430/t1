代发 wailian999

cmd >/dev/null 2>&1
来源：http://xy.huanxung.cn

[R42] 输入重定向
来源：http://sb.jctech888.com.cn

wc -l < a.txt
来源：http://it.szxytkj.cn

[R43] 按名字查找文件
来源：http://oy.asd995.cn

find . -name "*.log" -type f
来源：http://ab.haigaiapp.cn

[R44] 按修改时间查找
来源：http://dw.lnxyls.cn

find . -mtime -7 -type f
来源：http://yk.jctech888.com.cn

[R45] 批量删除
来源：http://ob.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://fa.panjiajie.cn

[R46] 递归替换文件内容
来源：http://re.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nw.lnxyls.cn

[R47] sed 单行替换
来源：http://yy.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ww.gzmigu.cn

[R48] awk 取指定列
来源：http://xx.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://we.521024.cn

[R49] awk 带条件
来源：http://zh.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ya.huanxung.cn

[R50] awk 求和
来源：http://dl.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xd.hnjuh.cn

[R51] 排序去重取前几
来源：http://uy.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fa.hnjuh.cn

[R52] 统计行数
来源：http://es.shxzukj.cn

wc -l a.txt
来源：http://gs.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://rl.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vs.hahajie.cn

[R54] 比较两个文件
来源：http://ua.huanxung.cn

diff a.txt b.txt
来源：http://bp.bjjhwx.cn

[R55] 压缩与解压
来源：http://nc.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ur.bjjhwx.cn

[R56] 远程拷贝
来源：http://nv.szxytkj.cn

scp file user@host:/path/
来源：http://zw.bookmarksfly.cn

[R57] 远程执行命令
来源：http://fk.panjiajie.cn

ssh user@host 'uptime'
来源：http://yd.hahajie.cn

[R58] 下载文件
来源：http://su.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jk.asd995.cn

[R59] 发 POST JSON
来源：http://tc.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mm.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://xj.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lp.huanxung.cn

[R61] 磁盘占用
来源：http://qg.haigaiapp.cn

df -h;  du -sh *
来源：http://ln.shxzskj.cn

[R62] 找最占空间的文件
来源：http://zj.asd995.cn

du -ah . | sort -rh | head -10
来源：http://ok.shtwfgs.cn

[R63] 内存与进程
来源：http://cj.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://pm.shtwfgs.cn

[R64] 结束进程
来源：http://ke.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://zj.nszjky.cn

[R65] 查看端口占用
来源：http://nc.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tr.shxzskj.cn

[R66] 定时任务
来源：http://ut.shxzskj.cn

crontab -e;  crontab -l
来源：http://av.521024.cn

[R67] 生成随机十六进制串
来源：http://hh.jianghongdianzi.cn

openssl rand -hex 16
来源：http://il.haigaiapp.cn

[R68] 计算文件校验值
来源：http://hl.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ff.wgjwhj.cn

[R69] 生成随机密码
来源：http://ou.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://cq.yuexingan06.cn

[R70] 时间戳与互转
来源：http://dd.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://yq.szxytkj.cn

[R71] 日期格式化
来源：http://wh.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://un.colortex.cn

[R72] 等待端口就绪
来源：http://ce.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rh.hahajie.cn

[R73] 分割大日志
来源：http://ij.panjiajie.cn

split -l 1000 big.log part_
来源：http://gx.huixinmuqiang.cn

[R74] 批量重命名
来源：http://gx.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dn.asd995.cn

[R75] 导出环境变量
来源：http://kv.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://rq.szxytkj.cn

[R76] 使用临时文件
来源：http://cq.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zk.shxzukj.cn

[R77] 读取用户输入
来源：http://oh.yuexingan06.cn

read -rp "请输入: " ans
来源：http://yy.huanxung.cn

[R78] 交互式菜单
来源：http://qy.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fd.shtwfgs.cn

[R79] 解析命令行选项
来源：http://ar.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ju.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://gi.shxzskj.cn

time ./run.sh
来源：http://sl.colortex.cn

================================================================================
来源：http://ei.9csxet.cn

S. C / C++ 专题
来源：http://iv.nicolike.cn

================================================================================
来源：http://kw.jianghongdianzi.cn

[S01] C：Hello World
来源：http://un.wgjwhj.cn

#include <stdio.h>
来源：http://vf.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bd.9csxet.cn

[S02] C：变量与格式化输出
来源：http://vi.521024.cn

int a = 10; printf("%d\n", a);
来源：http://xq.nszjky.cn

[S03] C：读入整数
来源：http://vk.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://dl.lnxyls.cn

[S04] C：字符串复制
来源：http://hy.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hw.szxytkj.cn

[S05] C：字符串长度
来源：http://ha.haigaiapp.cn

strlen(s)
来源：http://ue.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://ms.szsharing.cn

strcmp(a, b) == 0
来源：http://he.colortex.cn

[S07] C：数组遍历求和
来源：http://az.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ql.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://uy.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xe.521024.cn

[S09] C：结构体定义与初始化
来源：http://pg.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qe.lnxyls.cn

[S10] C：指针与解引用
来源：http://tt.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://ei.lnxyls.cn

[S11] C：逐行读文件
来源：http://oz.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://kv.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://po.yuexingan06.cn

fclose(f);
来源：http://pd.9csxet.cn

[S12] C：写文件
来源：http://tb.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qv.szsharing.cn

[S13] C：宏定义
来源：http://rg.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nj.panjiajie.cn

[S14] C：枚举
来源：http://qi.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://iz.bjjhwx.cn

[S15] C：类型转换
来源：http://ph.haigaiapp.cn

(double) a / b
来源：http://sr.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://yj.chemitech.net.cn

x |= (1 << 3);
来源：http://yn.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://wk.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oz.wgjwhj.cn

[S18] C：命令行参数
来源：http://zy.gzmigu.cn

int main(int argc, char **argv)
来源：http://ik.szxytkj.cn

[S19] C：快速排序
来源：http://af.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vy.lnxyls.cn

[S20] C：二分查找
来源：http://jn.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ld.szsharing.cn

[S21] C：字符类别判断
来源：http://fm.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fm.hnjuh.cn

[S22] C：字符串转数字
来源：http://qo.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tx.panjiajie.cn

[S23] C：随机数
来源：http://sh.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://in.shxzskj.cn

[S24] C：获取本地时间
来源：http://mj.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yu.521024.cn

[S25] C：内存拷贝
来源：http://lo.shxzskj.cn

memcpy(dst, src, n);
来源：http://uh.asd995.cn

[S26] C：内存清零
来源：http://dd.nicolike.cn

memset(a, 0, sizeof a);
来源：http://ye.wgjwhj.cn

[S27] C：定义常量
来源：http://nb.yuexingan06.cn

const double PI = 3.14159;
来源：http://sb.bjjhwx.cn

[S28] C：静态变量
来源：http://ju.jianghongdianzi.cn

static int counter = 0;
来源：http://ok.521024.cn

[S29] C：变参函数
来源：http://xm.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shtwfgs.cn

[S30] C：头文件保护
来源：http://jj.bjjhwx.cn

#ifndef X_H
来源：http://kz.lnxyls.cn

#define X_H
来源：http://kh.panjiajie.cn

#endif
来源：http://lb.hahajie.cn

[S31] C++：Hello World
来源：http://wl.bjjhwx.cn

#include <iostream>
来源：http://dz.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://xm.chemitech.net.cn

[S32] C++：字符串
来源：http://dg.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://if.jctech888.com.cn

[S33] C++：vector 增删
来源：http://kn.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mm.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://fi.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://ge.jctech888.com.cn

[S35] C++：map
来源：http://cf.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cx.panjiajie.cn

[S36] C++：unordered_map
来源：http://fj.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ce.shxzukj.cn

[S37] C++：set
来源：http://wk.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uj.lnxyls.cn

[S38] C++：排序
来源：http://rd.521024.cn

std::sort(v.begin(), v.end());
来源：http://zd.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://nk.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://io.bjjhwx.cn

[S40] C++：查找元素
来源：http://ix.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mk.shxzskj.cn

[S41] C++：类与构造函数
来源：http://uz.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zr.colortex.cn

[S42] C++：继承与虚函数
来源：http://ca.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://sj.muxihuayi.cn

[S43] C++：智能指针
来源：http://ar.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://ht.shxzukj.cn

[S44] C++：引用传参
来源：http://se.nszjky.cn

void inc(int &x) { ++x; }
来源：http://jm.9csxet.cn

[S45] C++：lambda
来源：http://wy.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nc.panjiajie.cn

[S46] C++：函数模板
来源：http://nn.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nk.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://yc.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ff.asd995.cn

[S48] C++：逐行读文件
来源：http://ie.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pi.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://ee.nszjky.cn

[S49] C++：写文件
来源：http://db.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lu.9csxet.cn

[S50] C++：格式化数字
来源：http://mk.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://am.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://ba.chemitech.net.cn

static_cast<double>(a) / b
来源：http://ug.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://lf.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://iu.gzmigu.cn

[S53] C++：移动语义
来源：http://gv.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://kq.lnxyls.cn

[S54] C++：异常处理
来源：http://of.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ai.9csxet.cn

[S55] C++：结构化绑定
来源：http://ch.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fx.lnxyls.cn

[S56] C++：optional
来源：http://pc.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yb.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://fc.yuntaijiaju.cn

constexpr int N = 10;
来源：http://th.shxzskj.cn

[S58] C++：命名空间
来源：http://do.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://xc.colortex.cn

[S59] C++：静态断言
来源：http://es.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ez.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://gj.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zs.asd995.cn

================================================================================
来源：http://wu.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ly.szxytkj.cn

================================================================================
来源：http://dr.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://hs.shtwfgs.cn

println("Hello")
来源：http://xd.yuexingan06.cn

[T02] Kotlin：变量
来源：http://jv.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mb.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://sh.newstarts.cn

"值: $b"
来源：http://jn.shxzskj.cn

[T04] Kotlin：空安全
来源：http://lv.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://xk.colortex.cn

[T05] Kotlin：when 表达式
来源：http://fw.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sy.asd995.cn

[T06] Kotlin：集合映射
来源：http://nf.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nv.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://nh.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://de.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://fz.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://tk.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://fu.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://ih.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://vp.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ot.jctech888.com.cn

[T11] Kotlin：协程
来源：http://ep.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jd.colortex.cn

[T12] Kotlin：解构声明
来源：http://fi.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://ox.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://ke.nszjky.cn

val m = mapOf("a" to 1)
来源：http://ay.nicolike.cn

[T14] Kotlin：循环
来源：http://qc.huanxung.cn

for (i in 1..10) println(i)
来源：http://ti.asd995.cn

[T15] Kotlin：接口
来源：http://hl.newstarts.cn

interface Shape { fun area(): Double }
来源：http://hc.hahajie.cn

[T16] Swift：Hello World
来源：http://mm.lnxyls.cn

print("Hello")
来源：http://mf.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://kw.szsharing.cn

var a = 1;  let b = 2
来源：http://js.newstarts.cn

[T18] Swift：字符串插值
来源：http://mh.huixiangedu.cn

"值: \(b)"
来源：http://zw.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://js.hahajie.cn

if let n = opt { print(n) }
来源：http://wk.haigaiapp.cn

[T20] Swift：数组操作
来源：http://yu.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://os.shxzukj.cn

[T21] Swift：遍历
来源：http://mi.szxytkj.cn

for x in a { print(x) }
来源：http://gg.colortex.cn

[T22] Swift：字典
来源：http://zv.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sd.asd995.cn

[T23] Swift：函数
来源：http://aw.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vr.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://in.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qt.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://cz.szxytkj.cn

struct P { var x: Int }
来源：http://gn.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://ng.shxzukj.cn

class A: Base { override func f() {} }
来源：http://nb.haigaiapp.cn

[T27] Swift：错误处理
来源：http://ea.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://eb.shtwfgs.cn

[T28] Swift：枚举
来源：http://yy.gzmigu.cn

enum Color { case red, green }
来源：http://vc.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://pv.521024.cn

guard let x = opt else { return }
来源：http://ea.hahajie.cn

[T30] Swift：协议
来源：http://xa.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://uc.hnjuh.cn

[T31] Lua：Hello World
来源：http://ql.lnxyls.cn

print("Hello")
来源：http://tf.shxzukj.cn

[T32] Lua：局部变量
来源：http://ds.shxzskj.cn

local a = 1
来源：http://bh.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://lp.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fz.521024.cn

[T34] Lua：遍历表
来源：http://lr.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lq.9csxet.cn

[T35] Lua：字典表
来源：http://iv.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://ya.9csxet.cn

[T36] Lua：函数
来源：http://vh.gzmigu.cn

function add(a, b) return a + b end
来源：http://cd.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://bb.jianghongdianzi.cn

"a" .. "b"
来源：http://nc.jctech888.com.cn

[T38] Lua：条件
来源：http://ed.hahajie.cn

if x > 0 then print("正") end
来源：http://vc.9csxet.cn

[T39] Lua：模式匹配
来源：http://me.nszjky.cn

string.find(s, "%d+")
来源：http://mt.jctech888.com.cn

[T40] Lua：元表
来源：http://zp.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://yt.hnjuh.cn

[T41] Perl：Hello World
来源：http://or.bookmarksfly.cn

print "Hello\n";
来源：http://xk.shtwfgs.cn

[T42] Perl：变量类型
来源：http://si.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zg.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://mv.hahajie.cn

"值: $a"
来源：http://md.wgjwhj.cn

[T44] Perl：条件
来源：http://tp.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://cv.hnjuh.cn


<!-- 参考信息 -->