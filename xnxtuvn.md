代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uc.jctech888.com.cn

[R30] 函数返回状态码
来源：http://hs.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://fc.bookmarksfly.cn

[R31] 局部变量
来源：http://yz.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://uc.szsharing.cn

[R32] 参数个数校验
来源：http://cc.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oq.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://qq.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cz.hahajie.cn

[R34] 退出时清理
来源：http://gw.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dk.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://va.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yq.lnxyls.cn

[R36] 并发执行多个任务
来源：http://he.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gj.521024.cn

[R37] 把输出赋给变量
来源：http://ux.muxihuayi.cn

files=$(ls -1)
来源：http://tu.colortex.cn

[R38] 管道串联
来源：http://rl.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://ix.asd995.cn

[R39] 重定向标准输出与错误
来源：http://jb.shtwfgs.cn

cmd > out.log 2>&1
来源：http://pq.bookmarksfly.cn

[R40] 追加写日志
来源：http://ps.colortex.cn

echo "log" >> out.log
来源：http://be.nicolike.cn

[R41] 丢弃输出
来源：http://gn.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://oe.muxihuayi.cn

[R42] 输入重定向
来源：http://ff.521024.cn

wc -l < a.txt
来源：http://mf.bjjhwx.cn

[R43] 按名字查找文件
来源：http://fn.huixiangedu.cn

find . -name "*.log" -type f
来源：http://tg.shxzukj.cn

[R44] 按修改时间查找
来源：http://ru.jctech888.com.cn

find . -mtime -7 -type f
来源：http://na.521024.cn

[R45] 批量删除
来源：http://ih.9csxet.cn

find . -name "*.tmp" -delete
来源：http://qj.9csxet.cn

[R46] 递归替换文件内容
来源：http://wt.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zd.panjiajie.cn

[R47] sed 单行替换
来源：http://sh.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gf.shxzskj.cn

[R48] awk 取指定列
来源：http://ac.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://vw.hnjuh.cn

[R49] awk 带条件
来源：http://ib.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://up.nicolike.cn

[R50] awk 求和
来源：http://rr.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://po.asd995.cn

[R51] 排序去重取前几
来源：http://jt.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://me.shtwfgs.cn

[R52] 统计行数
来源：http://ba.newstarts.cn

wc -l a.txt
来源：http://gf.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://eo.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cx.jctech888.com.cn

[R54] 比较两个文件
来源：http://kq.shtwfgs.cn

diff a.txt b.txt
来源：http://mz.panjiajie.cn

[R55] 压缩与解压
来源：http://io.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pm.bjjhwx.cn

[R56] 远程拷贝
来源：http://jd.shxzukj.cn

scp file user@host:/path/
来源：http://su.asd995.cn

[R57] 远程执行命令
来源：http://db.shxzukj.cn

ssh user@host 'uptime'
来源：http://zr.lnxyls.cn

[R58] 下载文件
来源：http://vu.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sh.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://ed.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ll.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://fj.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vt.szxytkj.cn

[R61] 磁盘占用
来源：http://qy.newstarts.cn

df -h;  du -sh *
来源：http://hx.shxzskj.cn

[R62] 找最占空间的文件
来源：http://wj.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://pa.yuexingan06.cn

[R63] 内存与进程
来源：http://mc.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://yw.haigaiapp.cn

[R64] 结束进程
来源：http://zb.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://yl.asd995.cn

[R65] 查看端口占用
来源：http://wn.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hv.gzmigu.cn

[R66] 定时任务
来源：http://ss.shtwfgs.cn

crontab -e;  crontab -l
来源：http://cz.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://kk.szxytkj.cn

openssl rand -hex 16
来源：http://bf.521024.cn

[R68] 计算文件校验值
来源：http://ps.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://di.asd995.cn

[R69] 生成随机密码
来源：http://in.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://ya.newstarts.cn

[R70] 时间戳与互转
来源：http://cu.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://bk.shxzskj.cn

[R71] 日期格式化
来源：http://sm.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://iz.lnxyls.cn

[R72] 等待端口就绪
来源：http://qy.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fn.lnxyls.cn

[R73] 分割大日志
来源：http://rj.huanxung.cn

split -l 1000 big.log part_
来源：http://fe.shtwfgs.cn

[R74] 批量重命名
来源：http://oq.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tw.panjiajie.cn

[R75] 导出环境变量
来源：http://ez.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://wk.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://jw.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vs.panjiajie.cn

[R77] 读取用户输入
来源：http://fr.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://ve.nicolike.cn

[R78] 交互式菜单
来源：http://oh.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ee.panjiajie.cn

[R79] 解析命令行选项
来源：http://fn.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sk.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://ol.jianghongdianzi.cn

time ./run.sh
来源：http://di.lnxyls.cn

================================================================================
来源：http://qz.bjjhwx.cn

S. C / C++ 专题
来源：http://vx.shxzskj.cn

================================================================================
来源：http://bu.hnjuh.cn

[S01] C：Hello World
来源：http://zy.asd995.cn

#include <stdio.h>
来源：http://ci.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pw.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://sd.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://ex.jianghongdianzi.cn

[S03] C：读入整数
来源：http://wv.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://ov.hahajie.cn

[S04] C：字符串复制
来源：http://et.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yg.szsharing.cn

[S05] C：字符串长度
来源：http://bw.jianghongdianzi.cn

strlen(s)
来源：http://rf.haigaiapp.cn

[S06] C：字符串比较
来源：http://dv.huanxung.cn

strcmp(a, b) == 0
来源：http://mb.szxytkj.cn

[S07] C：数组遍历求和
来源：http://qr.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zt.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://fo.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pq.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://dz.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uc.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://vh.colortex.cn

int *p = &a;  *p = 5;
来源：http://jj.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://tl.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://mo.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hp.9csxet.cn

fclose(f);
来源：http://sy.nszjky.cn

[S12] C：写文件
来源：http://hq.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ls.haigaiapp.cn

[S13] C：宏定义
来源：http://hq.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gk.muxihuayi.cn

[S14] C：枚举
来源：http://sq.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://nl.huanxung.cn

[S15] C：类型转换
来源：http://wi.chemitech.net.cn

(double) a / b
来源：http://mp.lnxyls.cn

[S16] C：位操作置位
来源：http://zt.bjjhwx.cn

x |= (1 << 3);
来源：http://ha.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://zm.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fe.newstarts.cn

[S18] C：命令行参数
来源：http://st.chemitech.net.cn

int main(int argc, char **argv)
来源：http://ot.hnjuh.cn

[S19] C：快速排序
来源：http://lz.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pi.szsharing.cn

[S20] C：二分查找
来源：http://px.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kh.wgjwhj.cn

[S21] C：字符类别判断
来源：http://ly.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tf.panjiajie.cn

[S22] C：字符串转数字
来源：http://tg.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ub.muxihuayi.cn

[S23] C：随机数
来源：http://rz.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gt.521024.cn

[S24] C：获取本地时间
来源：http://gy.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://is.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://in.wgjwhj.cn

memcpy(dst, src, n);
来源：http://as.shtwfgs.cn

[S26] C：内存清零
来源：http://lx.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://np.szxytkj.cn

[S27] C：定义常量
来源：http://mu.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://ur.haigaiapp.cn

[S28] C：静态变量
来源：http://ka.bjjhwx.cn

static int counter = 0;
来源：http://wu.shxzskj.cn

[S29] C：变参函数
来源：http://yq.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tn.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://fv.jctech888.com.cn

#ifndef X_H
来源：http://kg.yuexingan06.cn

#define X_H
来源：http://bq.shtwfgs.cn

#endif
来源：http://ks.nszjky.cn

[S31] C++：Hello World
来源：http://ts.jctech888.com.cn

#include <iostream>
来源：http://aj.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://qx.shxzukj.cn

[S32] C++：字符串
来源：http://le.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://ym.chemitech.net.cn

[S33] C++：vector 增删
来源：http://vf.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xk.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://id.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://xh.shxzskj.cn

[S35] C++：map
来源：http://dw.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mv.hnjuh.cn

[S36] C++：unordered_map
来源：http://sy.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tq.huixinmuqiang.cn

[S37] C++：set
来源：http://kc.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ye.haigaiapp.cn

[S38] C++：排序
来源：http://bq.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://td.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://ke.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://of.huixiangedu.cn

[S40] C++：查找元素
来源：http://zz.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sx.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://zr.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://um.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://ha.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://uq.muxihuayi.cn

[S43] C++：智能指针
来源：http://vu.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://gs.chemitech.net.cn

[S44] C++：引用传参
来源：http://ty.newstarts.cn

void inc(int &x) { ++x; }
来源：http://zz.huixiangedu.cn

[S45] C++：lambda
来源：http://we.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dd.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://ee.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gy.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://ss.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ve.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://sd.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vi.nicolike.cn

while (std::getline(in, line)) { }
来源：http://zk.nszjky.cn

[S49] C++：写文件
来源：http://dd.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qo.colortex.cn

[S50] C++：格式化数字
来源：http://is.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rw.szsharing.cn

[S51] C++：显式类型转换
来源：http://dv.hnjuh.cn

static_cast<double>(a) / b
来源：http://if.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://cl.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://pv.huanxung.cn

[S53] C++：移动语义
来源：http://bz.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://ji.521024.cn

[S54] C++：异常处理
来源：http://jq.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://od.nicolike.cn

[S55] C++：结构化绑定
来源：http://qa.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cu.shxzukj.cn

[S56] C++：optional
来源：http://nk.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fi.yuexingan06.cn

[S57] C++：编译期常量
来源：http://vy.gzmigu.cn

constexpr int N = 10;
来源：http://vj.huanxung.cn

[S58] C++：命名空间
来源：http://yw.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://xl.asd995.cn

[S59] C++：静态断言
来源：http://xn.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eq.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://au.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uk.huixinmuqiang.cn

================================================================================
来源：http://ti.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ht.wgjwhj.cn

================================================================================
来源：http://xb.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://fr.bookmarksfly.cn

println("Hello")
来源：http://ga.lnxyls.cn

[T02] Kotlin：变量
来源：http://qg.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ew.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://yb.huixinmuqiang.cn

"值: $b"
来源：http://ot.szxytkj.cn

[T04] Kotlin：空安全
来源：http://ib.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://mc.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://xj.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cx.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://fn.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://az.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://zk.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cf.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://tx.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://kx.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://wu.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://ep.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://eu.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nd.nszjky.cn

[T11] Kotlin：协程
来源：http://ce.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qu.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://no.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://ao.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://sm.nszjky.cn

val m = mapOf("a" to 1)
来源：http://xg.gzmigu.cn

[T14] Kotlin：循环
来源：http://is.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://eo.asd995.cn

[T15] Kotlin：接口
来源：http://to.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://go.yuexingan06.cn

[T16] Swift：Hello World
来源：http://hh.nszjky.cn

print("Hello")
来源：http://gq.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://ud.szsharing.cn

var a = 1;  let b = 2
来源：http://ph.asd995.cn

[T18] Swift：字符串插值
来源：http://yq.panjiajie.cn

"值: \(b)"
来源：http://xw.szxytkj.cn

[T19] Swift：可选绑定
来源：http://sr.chemitech.net.cn

if let n = opt { print(n) }
来源：http://ji.shtwfgs.cn

[T20] Swift：数组操作
来源：http://kg.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://td.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://hj.9csxet.cn

for x in a { print(x) }
来源：http://ui.panjiajie.cn

[T22] Swift：字典
来源：http://so.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ws.asd995.cn

[T23] Swift：函数
来源：http://ry.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mi.colortex.cn

[T24] Swift：闭包
来源：http://uu.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ga.szxytkj.cn

[T25] Swift：结构体
来源：http://ct.yuexingan06.cn

struct P { var x: Int }
来源：http://fp.asd995.cn

[T26] Swift：类与重写
来源：http://ea.gzmigu.cn

class A: Base { override func f() {} }
来源：http://pd.panjiajie.cn

[T27] Swift：错误处理
来源：http://lk.nszjky.cn

do { try f() } catch { print(error) }
来源：http://wu.shxzukj.cn

[T28] Swift：枚举
来源：http://yv.521024.cn

enum Color { case red, green }
来源：http://zr.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://hs.haigaiapp.cn

guard let x = opt else { return }
来源：http://cj.panjiajie.cn

[T30] Swift：协议
来源：http://sx.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://rw.panjiajie.cn

[T31] Lua：Hello World
来源：http://yn.hnjuh.cn

print("Hello")
来源：http://et.hahajie.cn

[T32] Lua：局部变量
来源：http://xv.jianghongdianzi.cn

local a = 1
来源：http://oi.haigaiapp.cn


<!-- 参考信息 -->