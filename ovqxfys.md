代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://yy.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://le.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ca.9csxet.cn

[R37] 把输出赋给变量
来源：http://jd.521024.cn

files=$(ls -1)
来源：http://lk.yuexingan06.cn

[R38] 管道串联
来源：http://ly.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://pg.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://jh.nszjky.cn

cmd > out.log 2>&1
来源：http://xm.bookmarksfly.cn

[R40] 追加写日志
来源：http://bk.521024.cn

echo "log" >> out.log
来源：http://bl.colortex.cn

[R41] 丢弃输出
来源：http://ns.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://rs.haigaiapp.cn

[R42] 输入重定向
来源：http://qj.panjiajie.cn

wc -l < a.txt
来源：http://pc.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://vi.wgjwhj.cn

find . -name "*.log" -type f
来源：http://yp.szsharing.cn

[R44] 按修改时间查找
来源：http://uf.jctech888.com.cn

find . -mtime -7 -type f
来源：http://en.bookmarksfly.cn

[R45] 批量删除
来源：http://om.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://ky.panjiajie.cn

[R46] 递归替换文件内容
来源：http://sb.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eh.bookmarksfly.cn

[R47] sed 单行替换
来源：http://mn.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uh.jctech888.com.cn

[R48] awk 取指定列
来源：http://fr.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://rt.hahajie.cn

[R49] awk 带条件
来源：http://hu.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qb.huanxung.cn

[R50] awk 求和
来源：http://ly.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pg.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://br.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fz.yuexingan06.cn

[R52] 统计行数
来源：http://da.9csxet.cn

wc -l a.txt
来源：http://be.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://yb.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zo.yuexingan06.cn

[R54] 比较两个文件
来源：http://qb.newstarts.cn

diff a.txt b.txt
来源：http://so.yuexingan06.cn

[R55] 压缩与解压
来源：http://yy.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cj.szsharing.cn

[R56] 远程拷贝
来源：http://kh.huixinmuqiang.cn

scp file user@host:/path/
来源：http://yb.wgjwhj.cn

[R57] 远程执行命令
来源：http://wh.jctech888.com.cn

ssh user@host 'uptime'
来源：http://xx.jctech888.com.cn

[R58] 下载文件
来源：http://db.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hh.huanxung.cn

[R59] 发 POST JSON
来源：http://sr.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rp.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://ay.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ms.huixiangedu.cn

[R61] 磁盘占用
来源：http://nf.shtwfgs.cn

df -h;  du -sh *
来源：http://nz.colortex.cn

[R62] 找最占空间的文件
来源：http://ox.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://jd.yuexingan06.cn

[R63] 内存与进程
来源：http://pl.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://fo.wgjwhj.cn

[R64] 结束进程
来源：http://rq.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://sp.jctech888.com.cn

[R65] 查看端口占用
来源：http://vh.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ad.colortex.cn

[R66] 定时任务
来源：http://ka.szsharing.cn

crontab -e;  crontab -l
来源：http://bn.9csxet.cn

[R67] 生成随机十六进制串
来源：http://ki.shxzskj.cn

openssl rand -hex 16
来源：http://fc.hahajie.cn

[R68] 计算文件校验值
来源：http://ii.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qn.haigaiapp.cn

[R69] 生成随机密码
来源：http://zc.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://je.muxihuayi.cn

[R70] 时间戳与互转
来源：http://xa.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://dx.wgjwhj.cn

[R71] 日期格式化
来源：http://xo.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://db.lnxyls.cn

[R72] 等待端口就绪
来源：http://rp.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pm.szsharing.cn

[R73] 分割大日志
来源：http://xq.521024.cn

split -l 1000 big.log part_
来源：http://qs.9csxet.cn

[R74] 批量重命名
来源：http://dy.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tr.haigaiapp.cn

[R75] 导出环境变量
来源：http://lv.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://bh.lnxyls.cn

[R76] 使用临时文件
来源：http://nb.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wj.nszjky.cn

[R77] 读取用户输入
来源：http://rh.shtwfgs.cn

read -rp "请输入: " ans
来源：http://yu.hnjuh.cn

[R78] 交互式菜单
来源：http://vv.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mt.asd995.cn

[R79] 解析命令行选项
来源：http://dr.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lk.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://oj.hnjuh.cn

time ./run.sh
来源：http://zj.yuntaijiaju.cn

================================================================================
来源：http://qb.wgjwhj.cn

S. C / C++ 专题
来源：http://vi.shxzskj.cn

================================================================================
来源：http://do.hnjuh.cn

[S01] C：Hello World
来源：http://nl.nszjky.cn

#include <stdio.h>
来源：http://io.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ok.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://tx.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://ma.szxytkj.cn

[S03] C：读入整数
来源：http://xh.9csxet.cn

int x; scanf("%d", &x);
来源：http://bz.jctech888.com.cn

[S04] C：字符串复制
来源：http://mi.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lk.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://xz.huanxung.cn

strlen(s)
来源：http://so.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://tw.chemitech.net.cn

strcmp(a, b) == 0
来源：http://zr.nszjky.cn

[S07] C：数组遍历求和
来源：http://ew.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nq.asd995.cn

[S08] C：动态内存分配与释放
来源：http://gy.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nd.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://nh.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bx.9csxet.cn

[S10] C：指针与解引用
来源：http://gn.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://hc.szxytkj.cn

[S11] C：逐行读文件
来源：http://yc.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://bw.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jo.nszjky.cn

fclose(f);
来源：http://yu.colortex.cn

[S12] C：写文件
来源：http://ab.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xo.521024.cn

[S13] C：宏定义
来源：http://zg.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ln.wgjwhj.cn

[S14] C：枚举
来源：http://xm.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://jt.lnxyls.cn

[S15] C：类型转换
来源：http://qi.haigaiapp.cn

(double) a / b
来源：http://yc.colortex.cn

[S16] C：位操作置位
来源：http://fa.nszjky.cn

x |= (1 << 3);
来源：http://ob.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://od.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hd.bjjhwx.cn

[S18] C：命令行参数
来源：http://fq.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://dx.yuntaijiaju.cn

[S19] C：快速排序
来源：http://fc.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://df.9csxet.cn

[S20] C：二分查找
来源：http://oi.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uk.jctech888.com.cn

[S21] C：字符类别判断
来源：http://gi.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://az.hnjuh.cn

[S22] C：字符串转数字
来源：http://vt.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bw.shxzukj.cn

[S23] C：随机数
来源：http://ab.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rf.9csxet.cn

[S24] C：获取本地时间
来源：http://cm.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bi.wgjwhj.cn

[S25] C：内存拷贝
来源：http://cq.asd995.cn

memcpy(dst, src, n);
来源：http://qw.9csxet.cn

[S26] C：内存清零
来源：http://nf.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://yu.asd995.cn

[S27] C：定义常量
来源：http://xb.gzmigu.cn

const double PI = 3.14159;
来源：http://sp.gzmigu.cn

[S28] C：静态变量
来源：http://ep.huixinmuqiang.cn

static int counter = 0;
来源：http://oy.muxihuayi.cn

[S29] C：变参函数
来源：http://ao.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bw.newstarts.cn

[S30] C：头文件保护
来源：http://oo.521024.cn

#ifndef X_H
来源：http://bd.haigaiapp.cn

#define X_H
来源：http://st.newstarts.cn

#endif
来源：http://ec.szxytkj.cn

[S31] C++：Hello World
来源：http://jc.shtwfgs.cn

#include <iostream>
来源：http://jk.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://mu.szxytkj.cn

[S32] C++：字符串
来源：http://kc.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://lp.bjjhwx.cn

[S33] C++：vector 增删
来源：http://eg.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yq.hnjuh.cn

[S34] C++：遍历 vector
来源：http://pp.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://iq.lnxyls.cn

[S35] C++：map
来源：http://ga.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gw.haigaiapp.cn

[S36] C++：unordered_map
来源：http://vw.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jo.haigaiapp.cn

[S37] C++：set
来源：http://po.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mc.szxytkj.cn

[S38] C++：排序
来源：http://br.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://cy.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://bn.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mm.gzmigu.cn

[S40] C++：查找元素
来源：http://ae.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zm.shxzskj.cn

[S41] C++：类与构造函数
来源：http://jt.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://py.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://bv.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://dl.521024.cn

[S43] C++：智能指针
来源：http://pa.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://cd.wgjwhj.cn

[S44] C++：引用传参
来源：http://uo.newstarts.cn

void inc(int &x) { ++x; }
来源：http://xj.shxzskj.cn

[S45] C++：lambda
来源：http://aa.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ow.gzmigu.cn

[S46] C++：函数模板
来源：http://hq.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zy.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://cz.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mw.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://lq.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pm.nicolike.cn

while (std::getline(in, line)) { }
来源：http://rt.shxzskj.cn

[S49] C++：写文件
来源：http://es.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vt.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://ec.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://et.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://vy.lnxyls.cn

static_cast<double>(a) / b
来源：http://vm.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://bq.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://di.szxytkj.cn

[S53] C++：移动语义
来源：http://lx.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://jb.shxzukj.cn

[S54] C++：异常处理
来源：http://ha.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ql.nicolike.cn

[S55] C++：结构化绑定
来源：http://lv.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sb.haigaiapp.cn

[S56] C++：optional
来源：http://fe.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mf.bjjhwx.cn

[S57] C++：编译期常量
来源：http://dc.muxihuayi.cn

constexpr int N = 10;
来源：http://uf.nicolike.cn

[S58] C++：命名空间
来源：http://dd.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://xn.nicolike.cn

[S59] C++：静态断言
来源：http://ro.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ft.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://et.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://to.gzmigu.cn

================================================================================
来源：http://xa.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fo.szsharing.cn

================================================================================
来源：http://ps.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://hf.jianghongdianzi.cn

println("Hello")
来源：http://bp.lnxyls.cn

[T02] Kotlin：变量
来源：http://cp.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cx.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://gl.shxzskj.cn

"值: $b"
来源：http://hr.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://gu.colortex.cn

val n: String? = null;  n?.length
来源：http://xg.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://md.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://to.huanxung.cn

[T06] Kotlin：集合映射
来源：http://jz.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tx.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://bs.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qx.panjiajie.cn

[T08] Kotlin：数据类
来源：http://so.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://vs.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://ai.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://li.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://hb.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zd.colortex.cn

[T11] Kotlin：协程
来源：http://ip.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tk.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://dk.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://vj.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://ux.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://mn.newstarts.cn

[T14] Kotlin：循环
来源：http://lz.shxzukj.cn

for (i in 1..10) println(i)
来源：http://vo.9csxet.cn

[T15] Kotlin：接口
来源：http://gi.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://sz.hnjuh.cn

[T16] Swift：Hello World
来源：http://mj.wgjwhj.cn

print("Hello")
来源：http://fx.shxzskj.cn

[T17] Swift：变量与常量
来源：http://pn.panjiajie.cn

var a = 1;  let b = 2
来源：http://mz.hahajie.cn

[T18] Swift：字符串插值
来源：http://wa.shxzskj.cn

"值: \(b)"
来源：http://nm.hnjuh.cn

[T19] Swift：可选绑定
来源：http://sa.muxihuayi.cn

if let n = opt { print(n) }
来源：http://rk.nszjky.cn

[T20] Swift：数组操作
来源：http://ft.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kc.chemitech.net.cn

[T21] Swift：遍历
来源：http://nd.huixiangedu.cn

for x in a { print(x) }
来源：http://cw.hnjuh.cn

[T22] Swift：字典
来源：http://nv.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ss.jianghongdianzi.cn

[T23] Swift：函数
来源：http://ur.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ym.muxihuayi.cn

[T24] Swift：闭包
来源：http://yx.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vk.shxzskj.cn

[T25] Swift：结构体
来源：http://wv.huanxung.cn

struct P { var x: Int }
来源：http://ne.shxzskj.cn

[T26] Swift：类与重写
来源：http://xp.lnxyls.cn

class A: Base { override func f() {} }
来源：http://wo.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://sr.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://is.9csxet.cn

[T28] Swift：枚举
来源：http://eg.szxytkj.cn

enum Color { case red, green }
来源：http://ha.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://ky.huixiangedu.cn

guard let x = opt else { return }
来源：http://fm.lnxyls.cn

[T30] Swift：协议
来源：http://uv.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://my.9csxet.cn

[T31] Lua：Hello World
来源：http://ee.panjiajie.cn

print("Hello")
来源：http://xp.szsharing.cn

[T32] Lua：局部变量
来源：http://jk.szxytkj.cn

local a = 1
来源：http://zn.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://ec.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ju.shxzukj.cn

[T34] Lua：遍历表
来源：http://bq.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yo.newstarts.cn

[T35] Lua：字典表
来源：http://fb.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://dq.shxzskj.cn

[T36] Lua：函数
来源：http://bt.hnjuh.cn

function add(a, b) return a + b end
来源：http://mc.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://ax.bookmarksfly.cn

"a" .. "b"
来源：http://zf.asd995.cn

[T38] Lua：条件
来源：http://ei.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://fs.hahajie.cn


<!-- 参考信息 -->