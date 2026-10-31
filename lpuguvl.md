代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fh.nicolike.cn

[R30] 函数返回状态码
来源：http://pk.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://cv.shxzukj.cn

[R31] 局部变量
来源：http://jj.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://oy.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://er.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qj.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://ni.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zp.newstarts.cn

[R34] 退出时清理
来源：http://ns.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ej.521024.cn

[R35] 后台执行并等待
来源：http://bz.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nc.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://kw.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gg.hnjuh.cn

[R37] 把输出赋给变量
来源：http://pc.gzmigu.cn

files=$(ls -1)
来源：http://rr.bjjhwx.cn

[R38] 管道串联
来源：http://aj.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://pu.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://ad.colortex.cn

cmd > out.log 2>&1
来源：http://rr.huanxung.cn

[R40] 追加写日志
来源：http://ia.panjiajie.cn

echo "log" >> out.log
来源：http://tp.bjjhwx.cn

[R41] 丢弃输出
来源：http://jb.nszjky.cn

cmd >/dev/null 2>&1
来源：http://sw.huixinmuqiang.cn

[R42] 输入重定向
来源：http://mn.shxzukj.cn

wc -l < a.txt
来源：http://lw.9csxet.cn

[R43] 按名字查找文件
来源：http://sp.asd995.cn

find . -name "*.log" -type f
来源：http://rk.gzmigu.cn

[R44] 按修改时间查找
来源：http://lf.nszjky.cn

find . -mtime -7 -type f
来源：http://bf.gzmigu.cn

[R45] 批量删除
来源：http://ps.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://cx.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://gp.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cf.haigaiapp.cn

[R47] sed 单行替换
来源：http://bn.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ht.haigaiapp.cn

[R48] awk 取指定列
来源：http://nz.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://qc.asd995.cn

[R49] awk 带条件
来源：http://us.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sl.lnxyls.cn

[R50] awk 求和
来源：http://fb.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://af.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://bd.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gg.shxzukj.cn

[R52] 统计行数
来源：http://ba.huixinmuqiang.cn

wc -l a.txt
来源：http://qd.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://iv.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kn.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://gf.colortex.cn

diff a.txt b.txt
来源：http://gk.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://tm.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yu.colortex.cn

[R56] 远程拷贝
来源：http://ri.jctech888.com.cn

scp file user@host:/path/
来源：http://ov.szxytkj.cn

[R57] 远程执行命令
来源：http://nv.huanxung.cn

ssh user@host 'uptime'
来源：http://ey.haigaiapp.cn

[R58] 下载文件
来源：http://zl.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ky.colortex.cn

[R59] 发 POST JSON
来源：http://bn.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kl.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://sl.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ox.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://fu.haigaiapp.cn

df -h;  du -sh *
来源：http://yf.szsharing.cn

[R62] 找最占空间的文件
来源：http://sd.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://lz.bjjhwx.cn

[R63] 内存与进程
来源：http://zv.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://ds.jctech888.com.cn

[R64] 结束进程
来源：http://mq.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://ma.yuexingan06.cn

[R65] 查看端口占用
来源：http://xy.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ag.bookmarksfly.cn

[R66] 定时任务
来源：http://xf.huanxung.cn

crontab -e;  crontab -l
来源：http://aa.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://tm.bjjhwx.cn

openssl rand -hex 16
来源：http://qh.nszjky.cn

[R68] 计算文件校验值
来源：http://zc.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nr.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://kv.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://mn.huanxung.cn

[R70] 时间戳与互转
来源：http://ae.nszjky.cn

date +%s;  date -d @1700000000
来源：http://sc.gzmigu.cn

[R71] 日期格式化
来源：http://rc.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rd.shxzukj.cn

[R72] 等待端口就绪
来源：http://ax.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ow.yuexingan06.cn

[R73] 分割大日志
来源：http://ry.bjjhwx.cn

split -l 1000 big.log part_
来源：http://cr.yuexingan06.cn

[R74] 批量重命名
来源：http://ua.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aa.haigaiapp.cn

[R75] 导出环境变量
来源：http://lt.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://bs.gzmigu.cn

[R76] 使用临时文件
来源：http://dj.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qi.jctech888.com.cn

[R77] 读取用户输入
来源：http://hi.hnjuh.cn

read -rp "请输入: " ans
来源：http://wl.lnxyls.cn

[R78] 交互式菜单
来源：http://jo.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kc.9csxet.cn

[R79] 解析命令行选项
来源：http://gj.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qn.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://vb.hnjuh.cn

time ./run.sh
来源：http://sp.huixiangedu.cn

================================================================================
来源：http://ib.huixiangedu.cn

S. C / C++ 专题
来源：http://qv.bjjhwx.cn

================================================================================
来源：http://yj.hnjuh.cn

[S01] C：Hello World
来源：http://ti.521024.cn

#include <stdio.h>
来源：http://rr.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iu.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://zc.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://wx.asd995.cn

[S03] C：读入整数
来源：http://cl.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://dk.521024.cn

[S04] C：字符串复制
来源：http://jb.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gs.muxihuayi.cn

[S05] C：字符串长度
来源：http://ya.wgjwhj.cn

strlen(s)
来源：http://wr.521024.cn

[S06] C：字符串比较
来源：http://ir.9csxet.cn

strcmp(a, b) == 0
来源：http://ms.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://sv.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ci.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://gl.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://io.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://ec.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hc.huanxung.cn

[S10] C：指针与解引用
来源：http://ou.asd995.cn

int *p = &a;  *p = 5;
来源：http://on.shxzskj.cn

[S11] C：逐行读文件
来源：http://sj.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://lh.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://by.szsharing.cn

fclose(f);
来源：http://vw.szsharing.cn

[S12] C：写文件
来源：http://hl.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uz.colortex.cn

[S13] C：宏定义
来源：http://yl.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kn.chemitech.net.cn

[S14] C：枚举
来源：http://sw.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://hs.hnjuh.cn

[S15] C：类型转换
来源：http://em.jctech888.com.cn

(double) a / b
来源：http://ya.nicolike.cn

[S16] C：位操作置位
来源：http://nw.panjiajie.cn

x |= (1 << 3);
来源：http://he.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://zi.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lg.huixiangedu.cn

[S18] C：命令行参数
来源：http://gn.asd995.cn

int main(int argc, char **argv)
来源：http://iy.newstarts.cn

[S19] C：快速排序
来源：http://ap.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://am.haigaiapp.cn

[S20] C：二分查找
来源：http://dy.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sa.gzmigu.cn

[S21] C：字符类别判断
来源：http://mm.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hs.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://vd.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qj.chemitech.net.cn

[S23] C：随机数
来源：http://kn.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oj.colortex.cn

[S24] C：获取本地时间
来源：http://go.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ad.hnjuh.cn

[S25] C：内存拷贝
来源：http://ec.lnxyls.cn

memcpy(dst, src, n);
来源：http://ph.szxytkj.cn

[S26] C：内存清零
来源：http://tw.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://nb.yuntaijiaju.cn

[S27] C：定义常量
来源：http://ti.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://th.nicolike.cn

[S28] C：静态变量
来源：http://dp.521024.cn

static int counter = 0;
来源：http://ii.hahajie.cn

[S29] C：变参函数
来源：http://nj.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ha.haigaiapp.cn

[S30] C：头文件保护
来源：http://tp.panjiajie.cn

#ifndef X_H
来源：http://ar.muxihuayi.cn

#define X_H
来源：http://xw.shxzukj.cn

#endif
来源：http://xz.yuexingan06.cn

[S31] C++：Hello World
来源：http://iq.nicolike.cn

#include <iostream>
来源：http://mn.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://fs.gzmigu.cn

[S32] C++：字符串
来源：http://ff.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://xx.bjjhwx.cn

[S33] C++：vector 增删
来源：http://ck.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ym.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://ba.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://pn.muxihuayi.cn

[S35] C++：map
来源：http://yn.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ta.muxihuayi.cn

[S36] C++：unordered_map
来源：http://ph.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ev.gzmigu.cn

[S37] C++：set
来源：http://jh.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uo.wgjwhj.cn

[S38] C++：排序
来源：http://jw.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://ih.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://lt.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://my.bjjhwx.cn

[S40] C++：查找元素
来源：http://jd.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kh.asd995.cn

[S41] C++：类与构造函数
来源：http://ie.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tx.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://rn.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://wa.muxihuayi.cn

[S43] C++：智能指针
来源：http://om.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://vz.gzmigu.cn

[S44] C++：引用传参
来源：http://qs.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://pn.shtwfgs.cn

[S45] C++：lambda
来源：http://li.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ie.yuexingan06.cn

[S46] C++：函数模板
来源：http://qo.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zo.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://ga.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sx.shxzukj.cn

[S48] C++：逐行读文件
来源：http://tq.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xl.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://hi.colortex.cn

[S49] C++：写文件
来源：http://xb.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jp.lnxyls.cn

[S50] C++：格式化数字
来源：http://su.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gl.nicolike.cn

[S51] C++：显式类型转换
来源：http://tc.muxihuayi.cn

static_cast<double>(a) / b
来源：http://jx.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://vc.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://aw.nszjky.cn

[S53] C++：移动语义
来源：http://gu.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://os.szsharing.cn

[S54] C++：异常处理
来源：http://zf.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://em.9csxet.cn

[S55] C++：结构化绑定
来源：http://cy.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bw.nicolike.cn

[S56] C++：optional
来源：http://zt.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bn.hahajie.cn

[S57] C++：编译期常量
来源：http://be.yuntaijiaju.cn

constexpr int N = 10;
来源：http://kn.shxzukj.cn

[S58] C++：命名空间
来源：http://bs.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://xc.wgjwhj.cn

[S59] C++：静态断言
来源：http://pv.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bm.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://tc.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pq.huanxung.cn

================================================================================
来源：http://wl.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yc.panjiajie.cn

================================================================================
来源：http://cs.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://hd.newstarts.cn

println("Hello")
来源：http://kq.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://ur.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jc.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://ar.bookmarksfly.cn

"值: $b"
来源：http://uf.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://pb.szsharing.cn

val n: String? = null;  n?.length
来源：http://on.colortex.cn

[T05] Kotlin：when 表达式
来源：http://kw.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dq.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://he.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vm.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://ua.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dc.panjiajie.cn

[T08] Kotlin：数据类
来源：http://rm.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://yi.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://yf.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://ii.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://aa.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ej.yuexingan06.cn

[T11] Kotlin：协程
来源：http://eg.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jd.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://sr.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://js.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://uf.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://lp.hahajie.cn

[T14] Kotlin：循环
来源：http://kw.szsharing.cn

for (i in 1..10) println(i)
来源：http://vm.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://mc.hahajie.cn

interface Shape { fun area(): Double }
来源：http://it.shxzskj.cn

[T16] Swift：Hello World
来源：http://rs.shxzukj.cn

print("Hello")
来源：http://vw.lnxyls.cn

[T17] Swift：变量与常量
来源：http://rp.hnjuh.cn

var a = 1;  let b = 2
来源：http://ke.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://mw.shtwfgs.cn

"值: \(b)"
来源：http://wn.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://qb.shtwfgs.cn

if let n = opt { print(n) }
来源：http://ko.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://ht.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bd.szxytkj.cn

[T21] Swift：遍历
来源：http://ri.hahajie.cn

for x in a { print(x) }
来源：http://fj.521024.cn

[T22] Swift：字典
来源：http://mx.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zv.haigaiapp.cn

[T23] Swift：函数
来源：http://dr.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ki.hnjuh.cn

[T24] Swift：闭包
来源：http://ti.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://el.shtwfgs.cn

[T25] Swift：结构体
来源：http://qc.521024.cn

struct P { var x: Int }
来源：http://nv.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://fo.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://yx.nszjky.cn

[T27] Swift：错误处理
来源：http://lm.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://ie.jctech888.com.cn

[T28] Swift：枚举
来源：http://od.yuntaijiaju.cn

enum Color { case red, green }
来源：http://hy.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://wn.panjiajie.cn

guard let x = opt else { return }
来源：http://dt.gzmigu.cn

[T30] Swift：协议
来源：http://fh.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://wx.nszjky.cn

[T31] Lua：Hello World
来源：http://ni.yuexingan06.cn

print("Hello")
来源：http://bm.lnxyls.cn

[T32] Lua：局部变量
来源：http://xh.hahajie.cn

local a = 1
来源：http://rw.yuntaijiaju.cn


<!-- 参考信息 -->