代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gf.panjiajie.cn

[R30] 函数返回状态码
来源：http://jw.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://gi.shxzukj.cn

[R31] 局部变量
来源：http://tl.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://si.panjiajie.cn

[R32] 参数个数校验
来源：http://zr.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fb.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://sm.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vz.szsharing.cn

[R34] 退出时清理
来源：http://pi.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sc.hnjuh.cn

[R35] 后台执行并等待
来源：http://ph.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://up.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://vz.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fw.szxytkj.cn

[R37] 把输出赋给变量
来源：http://ht.521024.cn

files=$(ls -1)
来源：http://cp.newstarts.cn

[R38] 管道串联
来源：http://co.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://sr.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://eu.hnjuh.cn

cmd > out.log 2>&1
来源：http://cn.chemitech.net.cn

[R40] 追加写日志
来源：http://lr.gzmigu.cn

echo "log" >> out.log
来源：http://uy.gzmigu.cn

[R41] 丢弃输出
来源：http://sl.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://zx.nszjky.cn

[R42] 输入重定向
来源：http://fu.newstarts.cn

wc -l < a.txt
来源：http://gm.colortex.cn

[R43] 按名字查找文件
来源：http://lb.jctech888.com.cn

find . -name "*.log" -type f
来源：http://za.521024.cn

[R44] 按修改时间查找
来源：http://xo.jctech888.com.cn

find . -mtime -7 -type f
来源：http://du.huixiangedu.cn

[R45] 批量删除
来源：http://ei.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://jf.gzmigu.cn

[R46] 递归替换文件内容
来源：http://gs.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://it.521024.cn

[R47] sed 单行替换
来源：http://be.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ny.lnxyls.cn

[R48] awk 取指定列
来源：http://wj.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://vd.chemitech.net.cn

[R49] awk 带条件
来源：http://fa.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vn.asd995.cn

[R50] awk 求和
来源：http://jo.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kd.haigaiapp.cn

[R51] 排序去重取前几
来源：http://fx.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lb.shtwfgs.cn

[R52] 统计行数
来源：http://iz.haigaiapp.cn

wc -l a.txt
来源：http://pj.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://rn.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rm.521024.cn

[R54] 比较两个文件
来源：http://cg.chemitech.net.cn

diff a.txt b.txt
来源：http://oz.huixiangedu.cn

[R55] 压缩与解压
来源：http://cr.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://at.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://gs.hahajie.cn

scp file user@host:/path/
来源：http://pq.gzmigu.cn

[R57] 远程执行命令
来源：http://qc.szxytkj.cn

ssh user@host 'uptime'
来源：http://pk.huixinmuqiang.cn

[R58] 下载文件
来源：http://vz.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dr.yuexingan06.cn

[R59] 发 POST JSON
来源：http://kt.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ya.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://re.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fb.huanxung.cn

[R61] 磁盘占用
来源：http://yt.huixinmuqiang.cn

df -h;  du -sh *
来源：http://iw.asd995.cn

[R62] 找最占空间的文件
来源：http://eo.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://ke.yuexingan06.cn

[R63] 内存与进程
来源：http://nf.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://mi.gzmigu.cn

[R64] 结束进程
来源：http://lt.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://fr.muxihuayi.cn

[R65] 查看端口占用
来源：http://sd.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ut.shtwfgs.cn

[R66] 定时任务
来源：http://oh.9csxet.cn

crontab -e;  crontab -l
来源：http://dw.9csxet.cn

[R67] 生成随机十六进制串
来源：http://fw.huanxung.cn

openssl rand -hex 16
来源：http://bp.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://sa.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bc.szxytkj.cn

[R69] 生成随机密码
来源：http://ws.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://xh.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://ye.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://it.hahajie.cn

[R71] 日期格式化
来源：http://ch.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zh.9csxet.cn

[R72] 等待端口就绪
来源：http://ly.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jc.asd995.cn

[R73] 分割大日志
来源：http://tj.hnjuh.cn

split -l 1000 big.log part_
来源：http://yc.newstarts.cn

[R74] 批量重命名
来源：http://gy.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nf.haigaiapp.cn

[R75] 导出环境变量
来源：http://um.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://ak.muxihuayi.cn

[R76] 使用临时文件
来源：http://mm.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://is.nszjky.cn

[R77] 读取用户输入
来源：http://az.gzmigu.cn

read -rp "请输入: " ans
来源：http://hu.lnxyls.cn

[R78] 交互式菜单
来源：http://zg.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://by.shtwfgs.cn

[R79] 解析命令行选项
来源：http://hk.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gj.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://mv.521024.cn

time ./run.sh
来源：http://bv.jianghongdianzi.cn

================================================================================
来源：http://of.shxzskj.cn

S. C / C++ 专题
来源：http://wq.chemitech.net.cn

================================================================================
来源：http://qn.newstarts.cn

[S01] C：Hello World
来源：http://rl.nicolike.cn

#include <stdio.h>
来源：http://mf.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xb.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://kv.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://zb.yuexingan06.cn

[S03] C：读入整数
来源：http://sq.lnxyls.cn

int x; scanf("%d", &x);
来源：http://ok.panjiajie.cn

[S04] C：字符串复制
来源：http://bc.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ye.huanxung.cn

[S05] C：字符串长度
来源：http://em.9csxet.cn

strlen(s)
来源：http://bl.gzmigu.cn

[S06] C：字符串比较
来源：http://oh.haigaiapp.cn

strcmp(a, b) == 0
来源：http://ed.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://wq.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vb.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://yo.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://up.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://pz.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pi.haigaiapp.cn

[S10] C：指针与解引用
来源：http://zd.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://po.gzmigu.cn

[S11] C：逐行读文件
来源：http://od.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://mz.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gz.bookmarksfly.cn

fclose(f);
来源：http://yq.shxzukj.cn

[S12] C：写文件
来源：http://yh.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pl.bookmarksfly.cn

[S13] C：宏定义
来源：http://sz.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yb.yuexingan06.cn

[S14] C：枚举
来源：http://kw.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://tx.shxzskj.cn

[S15] C：类型转换
来源：http://hm.wgjwhj.cn

(double) a / b
来源：http://np.muxihuayi.cn

[S16] C：位操作置位
来源：http://uk.asd995.cn

x |= (1 << 3);
来源：http://tc.szsharing.cn

[S17] C：安全拼接字符串
来源：http://wn.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wu.9csxet.cn

[S18] C：命令行参数
来源：http://ni.huixiangedu.cn

int main(int argc, char **argv)
来源：http://uz.muxihuayi.cn

[S19] C：快速排序
来源：http://nq.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://js.wgjwhj.cn

[S20] C：二分查找
来源：http://dm.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cn.nicolike.cn

[S21] C：字符类别判断
来源：http://gn.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qk.panjiajie.cn

[S22] C：字符串转数字
来源：http://sk.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tn.hahajie.cn

[S23] C：随机数
来源：http://so.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vv.shxzukj.cn

[S24] C：获取本地时间
来源：http://am.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ak.lnxyls.cn

[S25] C：内存拷贝
来源：http://ha.9csxet.cn

memcpy(dst, src, n);
来源：http://fu.chemitech.net.cn

[S26] C：内存清零
来源：http://kd.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://do.haigaiapp.cn

[S27] C：定义常量
来源：http://kb.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://gq.bjjhwx.cn

[S28] C：静态变量
来源：http://nb.nszjky.cn

static int counter = 0;
来源：http://wd.newstarts.cn

[S29] C：变参函数
来源：http://zt.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kh.gzmigu.cn

[S30] C：头文件保护
来源：http://oj.hnjuh.cn

#ifndef X_H
来源：http://ux.szxytkj.cn

#define X_H
来源：http://hv.newstarts.cn

#endif
来源：http://hs.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://nd.shxzukj.cn

#include <iostream>
来源：http://cf.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://tc.szxytkj.cn

[S32] C++：字符串
来源：http://dn.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://nt.jctech888.com.cn

[S33] C++：vector 增删
来源：http://op.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bh.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://db.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://lv.521024.cn

[S35] C++：map
来源：http://zu.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ic.colortex.cn

[S36] C++：unordered_map
来源：http://lo.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qp.wgjwhj.cn

[S37] C++：set
来源：http://rr.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vi.bookmarksfly.cn

[S38] C++：排序
来源：http://js.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://dn.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://uy.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ub.yuexingan06.cn

[S40] C++：查找元素
来源：http://zu.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sv.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://ft.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ul.521024.cn

[S42] C++：继承与虚函数
来源：http://tf.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://ki.hahajie.cn

[S43] C++：智能指针
来源：http://ue.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://mm.chemitech.net.cn

[S44] C++：引用传参
来源：http://zf.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://na.bjjhwx.cn

[S45] C++：lambda
来源：http://nq.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ir.yuexingan06.cn

[S46] C++：函数模板
来源：http://lu.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ni.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://cc.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ib.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://st.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hx.szsharing.cn

while (std::getline(in, line)) { }
来源：http://qs.shtwfgs.cn

[S49] C++：写文件
来源：http://ru.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qi.asd995.cn

[S50] C++：格式化数字
来源：http://oe.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ng.asd995.cn

[S51] C++：显式类型转换
来源：http://ig.asd995.cn

static_cast<double>(a) / b
来源：http://wy.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://ob.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://ph.wgjwhj.cn

[S53] C++：移动语义
来源：http://og.asd995.cn

std::vector<int> w = std::move(v);
来源：http://yh.colortex.cn

[S54] C++：异常处理
来源：http://su.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wm.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://lt.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uy.yuntaijiaju.cn

[S56] C++：optional
来源：http://br.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://am.hahajie.cn

[S57] C++：编译期常量
来源：http://nz.hnjuh.cn

constexpr int N = 10;
来源：http://nx.szsharing.cn

[S58] C++：命名空间
来源：http://py.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://qc.nicolike.cn

[S59] C++：静态断言
来源：http://mf.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kb.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://xo.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mk.yuexingan06.cn

================================================================================
来源：http://xv.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xk.hnjuh.cn

================================================================================
来源：http://qb.asd995.cn

[T01] Kotlin：Hello World
来源：http://aq.jctech888.com.cn

println("Hello")
来源：http://qd.shxzskj.cn

[T02] Kotlin：变量
来源：http://tm.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fy.asd995.cn

[T03] Kotlin：字符串模板
来源：http://rj.wgjwhj.cn

"值: $b"
来源：http://xn.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://cs.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://mj.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://jk.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hl.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://cx.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lq.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://ru.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://re.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://wi.asd995.cn

data class User(val name: String, val age: Int)
来源：http://tw.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://un.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://ko.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://xn.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wp.huanxung.cn

[T11] Kotlin：协程
来源：http://es.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iw.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://fj.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://hr.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://qf.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://cp.panjiajie.cn

[T14] Kotlin：循环
来源：http://sp.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://ys.panjiajie.cn

[T15] Kotlin：接口
来源：http://fz.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://qw.nszjky.cn

[T16] Swift：Hello World
来源：http://au.hahajie.cn

print("Hello")
来源：http://ql.hahajie.cn

[T17] Swift：变量与常量
来源：http://dz.muxihuayi.cn

var a = 1;  let b = 2
来源：http://my.shxzskj.cn

[T18] Swift：字符串插值
来源：http://mb.asd995.cn

"值: \(b)"
来源：http://kq.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://gq.shxzskj.cn

if let n = opt { print(n) }
来源：http://ct.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://ej.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dg.huanxung.cn

[T21] Swift：遍历
来源：http://yg.panjiajie.cn

for x in a { print(x) }
来源：http://jf.huixinmuqiang.cn

[T22] Swift：字典
来源：http://hw.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://be.asd995.cn

[T23] Swift：函数
来源：http://lp.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nx.shxzskj.cn

[T24] Swift：闭包
来源：http://iv.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tr.shxzskj.cn

[T25] Swift：结构体
来源：http://ic.wgjwhj.cn

struct P { var x: Int }
来源：http://sv.chemitech.net.cn

[T26] Swift：类与重写
来源：http://zn.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://if.gzmigu.cn

[T27] Swift：错误处理
来源：http://bj.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://ml.asd995.cn

[T28] Swift：枚举
来源：http://ur.9csxet.cn

enum Color { case red, green }
来源：http://tg.asd995.cn

[T29] Swift：guard 提前返回
来源：http://qb.shtwfgs.cn

guard let x = opt else { return }
来源：http://km.shxzukj.cn

[T30] Swift：协议
来源：http://pj.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://ii.lnxyls.cn

[T31] Lua：Hello World
来源：http://sg.yuntaijiaju.cn

print("Hello")
来源：http://pt.asd995.cn

[T32] Lua：局部变量
来源：http://vh.gzmigu.cn

local a = 1
来源：http://bb.haigaiapp.cn


<!-- 参考信息 -->