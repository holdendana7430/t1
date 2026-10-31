代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sr.bjjhwx.cn

[R30] 函数返回状态码
来源：http://bj.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://gc.bookmarksfly.cn

[R31] 局部变量
来源：http://pb.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://ql.nicolike.cn

[R32] 参数个数校验
来源：http://ev.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ne.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://gu.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rd.huixiangedu.cn

[R34] 退出时清理
来源：http://et.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://to.panjiajie.cn

[R35] 后台执行并等待
来源：http://av.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rz.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://xj.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ko.panjiajie.cn

[R37] 把输出赋给变量
来源：http://fi.yuntaijiaju.cn

files=$(ls -1)
来源：http://tn.shxzskj.cn

[R38] 管道串联
来源：http://rb.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://qb.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://zi.jctech888.com.cn

cmd > out.log 2>&1
来源：http://kc.muxihuayi.cn

[R40] 追加写日志
来源：http://ey.yuntaijiaju.cn

echo "log" >> out.log
来源：http://yp.jctech888.com.cn

[R41] 丢弃输出
来源：http://nm.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://xl.bookmarksfly.cn

[R42] 输入重定向
来源：http://qe.shxzskj.cn

wc -l < a.txt
来源：http://ly.521024.cn

[R43] 按名字查找文件
来源：http://el.szsharing.cn

find . -name "*.log" -type f
来源：http://ib.nszjky.cn

[R44] 按修改时间查找
来源：http://ve.hahajie.cn

find . -mtime -7 -type f
来源：http://hx.haigaiapp.cn

[R45] 批量删除
来源：http://ye.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://am.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://qg.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aj.521024.cn

[R47] sed 单行替换
来源：http://ds.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qg.szsharing.cn

[R48] awk 取指定列
来源：http://ab.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://sq.huixinmuqiang.cn

[R49] awk 带条件
来源：http://qs.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dc.nszjky.cn

[R50] awk 求和
来源：http://pn.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mo.szxytkj.cn

[R51] 排序去重取前几
来源：http://sz.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jt.lnxyls.cn

[R52] 统计行数
来源：http://yu.bookmarksfly.cn

wc -l a.txt
来源：http://ix.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://ai.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zs.huanxung.cn

[R54] 比较两个文件
来源：http://al.chemitech.net.cn

diff a.txt b.txt
来源：http://ap.gzmigu.cn

[R55] 压缩与解压
来源：http://ob.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cz.colortex.cn

[R56] 远程拷贝
来源：http://ek.hnjuh.cn

scp file user@host:/path/
来源：http://px.shxzukj.cn

[R57] 远程执行命令
来源：http://ob.nszjky.cn

ssh user@host 'uptime'
来源：http://jz.szsharing.cn

[R58] 下载文件
来源：http://jd.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pk.shxzskj.cn

[R59] 发 POST JSON
来源：http://yw.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cw.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://zs.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ha.hnjuh.cn

[R61] 磁盘占用
来源：http://ch.bjjhwx.cn

df -h;  du -sh *
来源：http://nv.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://bp.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://de.gzmigu.cn

[R63] 内存与进程
来源：http://zs.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://ly.lnxyls.cn

[R64] 结束进程
来源：http://vs.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://gd.nicolike.cn

[R65] 查看端口占用
来源：http://dn.shtwfgs.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ze.huanxung.cn

[R66] 定时任务
来源：http://vj.shxzukj.cn

crontab -e;  crontab -l
来源：http://xj.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://xd.huanxung.cn

openssl rand -hex 16
来源：http://st.huixiangedu.cn

[R68] 计算文件校验值
来源：http://es.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bo.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://gq.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://ln.newstarts.cn

[R70] 时间戳与互转
来源：http://zq.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://mj.huanxung.cn

[R71] 日期格式化
来源：http://xn.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rg.panjiajie.cn

[R72] 等待端口就绪
来源：http://ig.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://at.shxzukj.cn

[R73] 分割大日志
来源：http://ep.panjiajie.cn

split -l 1000 big.log part_
来源：http://qb.nszjky.cn

[R74] 批量重命名
来源：http://zh.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tb.shxzskj.cn

[R75] 导出环境变量
来源：http://vb.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://pc.huixiangedu.cn

[R76] 使用临时文件
来源：http://im.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://db.colortex.cn

[R77] 读取用户输入
来源：http://ed.shtwfgs.cn

read -rp "请输入: " ans
来源：http://ot.gzmigu.cn

[R78] 交互式菜单
来源：http://tv.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://th.huanxung.cn

[R79] 解析命令行选项
来源：http://nw.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dp.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://xe.newstarts.cn

time ./run.sh
来源：http://kt.bookmarksfly.cn

================================================================================
来源：http://vy.hnjuh.cn

S. C / C++ 专题
来源：http://ww.szxytkj.cn

================================================================================
来源：http://rb.wgjwhj.cn

[S01] C：Hello World
来源：http://oj.wgjwhj.cn

#include <stdio.h>
来源：http://ze.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dk.newstarts.cn

[S02] C：变量与格式化输出
来源：http://ib.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://rg.newstarts.cn

[S03] C：读入整数
来源：http://wp.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://vt.9csxet.cn

[S04] C：字符串复制
来源：http://cw.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jb.asd995.cn

[S05] C：字符串长度
来源：http://hr.huixinmuqiang.cn

strlen(s)
来源：http://dy.shxzukj.cn

[S06] C：字符串比较
来源：http://sq.gzmigu.cn

strcmp(a, b) == 0
来源：http://iw.nszjky.cn

[S07] C：数组遍历求和
来源：http://xd.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vz.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://ja.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ww.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://jm.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ve.shxzskj.cn

[S10] C：指针与解引用
来源：http://cv.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://za.nszjky.cn

[S11] C：逐行读文件
来源：http://lt.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://mn.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cn.szxytkj.cn

fclose(f);
来源：http://sc.newstarts.cn

[S12] C：写文件
来源：http://su.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aa.muxihuayi.cn

[S13] C：宏定义
来源：http://ie.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bi.shtwfgs.cn

[S14] C：枚举
来源：http://bc.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://fd.chemitech.net.cn

[S15] C：类型转换
来源：http://dk.shtwfgs.cn

(double) a / b
来源：http://np.hnjuh.cn

[S16] C：位操作置位
来源：http://ie.nszjky.cn

x |= (1 << 3);
来源：http://dr.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://zh.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pq.lnxyls.cn

[S18] C：命令行参数
来源：http://ym.521024.cn

int main(int argc, char **argv)
来源：http://rh.shxzukj.cn

[S19] C：快速排序
来源：http://ys.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vb.gzmigu.cn

[S20] C：二分查找
来源：http://qd.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zj.shtwfgs.cn

[S21] C：字符类别判断
来源：http://eh.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bd.9csxet.cn

[S22] C：字符串转数字
来源：http://ak.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rm.asd995.cn

[S23] C：随机数
来源：http://xl.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qu.yuexingan06.cn

[S24] C：获取本地时间
来源：http://da.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bb.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://bd.hnjuh.cn

memcpy(dst, src, n);
来源：http://xg.chemitech.net.cn

[S26] C：内存清零
来源：http://dq.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://ts.9csxet.cn

[S27] C：定义常量
来源：http://vd.huanxung.cn

const double PI = 3.14159;
来源：http://ty.huixiangedu.cn

[S28] C：静态变量
来源：http://vb.szsharing.cn

static int counter = 0;
来源：http://ir.szsharing.cn

[S29] C：变参函数
来源：http://dj.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tw.bookmarksfly.cn

[S30] C：头文件保护
来源：http://gn.chemitech.net.cn

#ifndef X_H
来源：http://ht.haigaiapp.cn

#define X_H
来源：http://vf.chemitech.net.cn

#endif
来源：http://mu.yuexingan06.cn

[S31] C++：Hello World
来源：http://gd.lnxyls.cn

#include <iostream>
来源：http://me.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://jr.panjiajie.cn

[S32] C++：字符串
来源：http://om.asd995.cn

std::string s = "hi";  s += "!";
来源：http://oc.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://qy.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://en.shxzukj.cn

[S34] C++：遍历 vector
来源：http://vm.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://lo.huanxung.cn

[S35] C++：map
来源：http://ve.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nd.nszjky.cn

[S36] C++：unordered_map
来源：http://dp.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gp.newstarts.cn

[S37] C++：set
来源：http://eg.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://di.521024.cn

[S38] C++：排序
来源：http://ch.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://ac.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://ya.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://le.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://tu.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nt.szxytkj.cn

[S41] C++：类与构造函数
来源：http://eu.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mq.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://pl.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://cj.gzmigu.cn

[S43] C++：智能指针
来源：http://by.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://cy.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://zb.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://fi.muxihuayi.cn

[S45] C++：lambda
来源：http://at.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zf.hnjuh.cn

[S46] C++：函数模板
来源：http://qk.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mc.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://ri.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qi.szsharing.cn

[S48] C++：逐行读文件
来源：http://lw.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ct.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://bb.gzmigu.cn

[S49] C++：写文件
来源：http://zs.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vq.gzmigu.cn

[S50] C++：格式化数字
来源：http://kv.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ok.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://di.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://pl.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://zg.nszjky.cn

int size() const noexcept { return n_; }
来源：http://qc.hahajie.cn

[S53] C++：移动语义
来源：http://jc.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://js.colortex.cn

[S54] C++：异常处理
来源：http://pq.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uh.gzmigu.cn

[S55] C++：结构化绑定
来源：http://gk.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ls.panjiajie.cn

[S56] C++：optional
来源：http://yq.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uh.haigaiapp.cn

[S57] C++：编译期常量
来源：http://ys.colortex.cn

constexpr int N = 10;
来源：http://ia.nszjky.cn

[S58] C++：命名空间
来源：http://eo.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://kv.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://nj.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jt.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://by.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nj.yuntaijiaju.cn

================================================================================
来源：http://la.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gq.521024.cn

================================================================================
来源：http://xb.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://fw.yuexingan06.cn

println("Hello")
来源：http://ee.colortex.cn

[T02] Kotlin：变量
来源：http://yf.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ws.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://br.huanxung.cn

"值: $b"
来源：http://kh.asd995.cn

[T04] Kotlin：空安全
来源：http://rt.521024.cn

val n: String? = null;  n?.length
来源：http://ts.colortex.cn

[T05] Kotlin：when 表达式
来源：http://yd.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oe.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://gf.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ak.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://es.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ni.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://wl.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://fl.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://xg.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://lq.nicolike.cn

[T10] Kotlin：默认参数
来源：http://ru.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qn.panjiajie.cn

[T11] Kotlin：协程
来源：http://pq.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hh.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://wq.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://yj.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://tb.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://ga.bjjhwx.cn

[T14] Kotlin：循环
来源：http://gh.newstarts.cn

for (i in 1..10) println(i)
来源：http://qs.szsharing.cn

[T15] Kotlin：接口
来源：http://eo.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://lx.huixiangedu.cn

[T16] Swift：Hello World
来源：http://lh.bookmarksfly.cn

print("Hello")
来源：http://qx.shxzukj.cn

[T17] Swift：变量与常量
来源：http://ki.muxihuayi.cn

var a = 1;  let b = 2
来源：http://ie.nszjky.cn

[T18] Swift：字符串插值
来源：http://kx.hahajie.cn

"值: \(b)"
来源：http://cl.hnjuh.cn

[T19] Swift：可选绑定
来源：http://er.lnxyls.cn

if let n = opt { print(n) }
来源：http://nr.szxytkj.cn

[T20] Swift：数组操作
来源：http://pg.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://om.521024.cn

[T21] Swift：遍历
来源：http://in.hnjuh.cn

for x in a { print(x) }
来源：http://vv.shtwfgs.cn

[T22] Swift：字典
来源：http://nd.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://po.colortex.cn

[T23] Swift：函数
来源：http://fq.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wg.yuexingan06.cn

[T24] Swift：闭包
来源：http://ax.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://or.asd995.cn

[T25] Swift：结构体
来源：http://il.nszjky.cn

struct P { var x: Int }
来源：http://en.shtwfgs.cn

[T26] Swift：类与重写
来源：http://jb.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://rn.huanxung.cn

[T27] Swift：错误处理
来源：http://lb.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://dk.hahajie.cn

[T28] Swift：枚举
来源：http://dq.haigaiapp.cn

enum Color { case red, green }
来源：http://er.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://ap.521024.cn

guard let x = opt else { return }
来源：http://wi.chemitech.net.cn

[T30] Swift：协议
来源：http://dk.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://kz.shxzukj.cn

[T31] Lua：Hello World
来源：http://ky.panjiajie.cn

print("Hello")
来源：http://ux.lnxyls.cn

[T32] Lua：局部变量
来源：http://sv.bjjhwx.cn

local a = 1
来源：http://qu.shxzskj.cn


<!-- 参考信息 -->