代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cv.hnjuh.cn

[R34] 退出时清理
来源：http://ff.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oi.521024.cn

[R35] 后台执行并等待
来源：http://nk.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://am.huanxung.cn

[R36] 并发执行多个任务
来源：http://cf.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://it.gzmigu.cn

[R37] 把输出赋给变量
来源：http://lo.9csxet.cn

files=$(ls -1)
来源：http://jv.gzmigu.cn

[R38] 管道串联
来源：http://en.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://hm.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://fw.shxzukj.cn

cmd > out.log 2>&1
来源：http://vq.9csxet.cn

[R40] 追加写日志
来源：http://qo.shxzukj.cn

echo "log" >> out.log
来源：http://jl.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://an.nicolike.cn

cmd >/dev/null 2>&1
来源：http://do.huixinmuqiang.cn

[R42] 输入重定向
来源：http://ez.yuntaijiaju.cn

wc -l < a.txt
来源：http://wy.bjjhwx.cn

[R43] 按名字查找文件
来源：http://qs.shxzskj.cn

find . -name "*.log" -type f
来源：http://du.gzmigu.cn

[R44] 按修改时间查找
来源：http://qp.wgjwhj.cn

find . -mtime -7 -type f
来源：http://ty.huixinmuqiang.cn

[R45] 批量删除
来源：http://xk.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://su.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://ty.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wp.9csxet.cn

[R47] sed 单行替换
来源：http://if.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ah.asd995.cn

[R48] awk 取指定列
来源：http://dt.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://ci.lnxyls.cn

[R49] awk 带条件
来源：http://fy.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qy.szxytkj.cn

[R50] awk 求和
来源：http://ax.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tu.colortex.cn

[R51] 排序去重取前几
来源：http://qa.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://op.shtwfgs.cn

[R52] 统计行数
来源：http://jt.nicolike.cn

wc -l a.txt
来源：http://vv.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://te.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fh.shxzukj.cn

[R54] 比较两个文件
来源：http://ap.gzmigu.cn

diff a.txt b.txt
来源：http://yj.nicolike.cn

[R55] 压缩与解压
来源：http://qf.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ys.muxihuayi.cn

[R56] 远程拷贝
来源：http://et.huixinmuqiang.cn

scp file user@host:/path/
来源：http://sl.colortex.cn

[R57] 远程执行命令
来源：http://kq.chemitech.net.cn

ssh user@host 'uptime'
来源：http://tm.haigaiapp.cn

[R58] 下载文件
来源：http://pi.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xg.nicolike.cn

[R59] 发 POST JSON
来源：http://wi.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jb.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://cm.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wq.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://fh.yuexingan06.cn

df -h;  du -sh *
来源：http://lq.huanxung.cn

[R62] 找最占空间的文件
来源：http://yl.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://le.521024.cn

[R63] 内存与进程
来源：http://mh.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://is.hnjuh.cn

[R64] 结束进程
来源：http://lp.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://fw.shxzukj.cn

[R65] 查看端口占用
来源：http://hl.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://le.bookmarksfly.cn

[R66] 定时任务
来源：http://bx.chemitech.net.cn

crontab -e;  crontab -l
来源：http://mx.hahajie.cn

[R67] 生成随机十六进制串
来源：http://ns.bjjhwx.cn

openssl rand -hex 16
来源：http://dv.jctech888.com.cn

[R68] 计算文件校验值
来源：http://tn.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mh.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://kt.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://ax.9csxet.cn

[R70] 时间戳与互转
来源：http://pw.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://gx.colortex.cn

[R71] 日期格式化
来源：http://en.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jl.muxihuayi.cn

[R72] 等待端口就绪
来源：http://tq.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://id.asd995.cn

[R73] 分割大日志
来源：http://cf.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://yz.lnxyls.cn

[R74] 批量重命名
来源：http://wb.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tu.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://px.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ce.huanxung.cn

[R76] 使用临时文件
来源：http://pw.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zk.panjiajie.cn

[R77] 读取用户输入
来源：http://zg.gzmigu.cn

read -rp "请输入: " ans
来源：http://ym.9csxet.cn

[R78] 交互式菜单
来源：http://ez.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uv.colortex.cn

[R79] 解析命令行选项
来源：http://bw.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uv.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://cg.bjjhwx.cn

time ./run.sh
来源：http://xe.szsharing.cn

================================================================================
来源：http://nl.shxzukj.cn

S. C / C++ 专题
来源：http://qg.huixinmuqiang.cn

================================================================================
来源：http://nc.hahajie.cn

[S01] C：Hello World
来源：http://lv.huixinmuqiang.cn

#include <stdio.h>
来源：http://ub.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rn.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://jw.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://ye.asd995.cn

[S03] C：读入整数
来源：http://fx.hahajie.cn

int x; scanf("%d", &x);
来源：http://id.colortex.cn

[S04] C：字符串复制
来源：http://zd.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gz.asd995.cn

[S05] C：字符串长度
来源：http://pl.hnjuh.cn

strlen(s)
来源：http://ge.panjiajie.cn

[S06] C：字符串比较
来源：http://pb.colortex.cn

strcmp(a, b) == 0
来源：http://ke.nicolike.cn

[S07] C：数组遍历求和
来源：http://ou.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xb.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://pk.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bl.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://cq.jianghongdianzi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://of.shxzskj.cn

[S10] C：指针与解引用
来源：http://vz.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://oe.gzmigu.cn

[S11] C：逐行读文件
来源：http://hm.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://fc.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zd.wgjwhj.cn

fclose(f);
来源：http://pt.huixiangedu.cn

[S12] C：写文件
来源：http://wx.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hb.9csxet.cn

[S13] C：宏定义
来源：http://fk.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://at.gzmigu.cn

[S14] C：枚举
来源：http://vo.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://sn.panjiajie.cn

[S15] C：类型转换
来源：http://di.muxihuayi.cn

(double) a / b
来源：http://ja.asd995.cn

[S16] C：位操作置位
来源：http://lk.nszjky.cn

x |= (1 << 3);
来源：http://tn.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://du.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hw.hahajie.cn

[S18] C：命令行参数
来源：http://jw.wgjwhj.cn

int main(int argc, char **argv)
来源：http://yq.szxytkj.cn

[S19] C：快速排序
来源：http://tt.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lr.hnjuh.cn

[S20] C：二分查找
来源：http://mw.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yr.colortex.cn

[S21] C：字符类别判断
来源：http://yp.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lx.szxytkj.cn

[S22] C：字符串转数字
来源：http://zo.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gu.yuexingan06.cn

[S23] C：随机数
来源：http://gx.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uk.nszjky.cn

[S24] C：获取本地时间
来源：http://eu.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xc.newstarts.cn

[S25] C：内存拷贝
来源：http://sy.521024.cn

memcpy(dst, src, n);
来源：http://ql.huixiangedu.cn

[S26] C：内存清零
来源：http://tl.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://um.jctech888.com.cn

[S27] C：定义常量
来源：http://zk.panjiajie.cn

const double PI = 3.14159;
来源：http://fz.colortex.cn

[S28] C：静态变量
来源：http://ri.shxzskj.cn

static int counter = 0;
来源：http://av.szxytkj.cn

[S29] C：变参函数
来源：http://yu.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://is.shxzskj.cn

[S30] C：头文件保护
来源：http://sd.lnxyls.cn

#ifndef X_H
来源：http://pa.huixiangedu.cn

#define X_H
来源：http://fy.colortex.cn

#endif
来源：http://cl.huanxung.cn

[S31] C++：Hello World
来源：http://bt.huixiangedu.cn

#include <iostream>
来源：http://il.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://lb.9csxet.cn

[S32] C++：字符串
来源：http://fw.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://ug.gzmigu.cn

[S33] C++：vector 增删
来源：http://fm.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pv.521024.cn

[S34] C++：遍历 vector
来源：http://bk.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://vp.hahajie.cn

[S35] C++：map
来源：http://gk.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ma.yuexingan06.cn

[S36] C++：unordered_map
来源：http://yp.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nb.yuexingan06.cn

[S37] C++：set
来源：http://rh.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hi.wgjwhj.cn

[S38] C++：排序
来源：http://kq.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://px.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://db.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zl.szxytkj.cn

[S40] C++：查找元素
来源：http://mg.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rp.shxzukj.cn

[S41] C++：类与构造函数
来源：http://up.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ht.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://fc.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://tm.nszjky.cn

[S43] C++：智能指针
来源：http://mp.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://sl.nicolike.cn

[S44] C++：引用传参
来源：http://vh.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://yd.shxzskj.cn

[S45] C++：lambda
来源：http://pv.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yc.wgjwhj.cn

[S46] C++：函数模板
来源：http://vj.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bl.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://fq.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hk.shxzukj.cn

[S48] C++：逐行读文件
来源：http://qs.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zo.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://ry.chemitech.net.cn

[S49] C++：写文件
来源：http://vc.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fm.yuexingan06.cn

[S50] C++：格式化数字
来源：http://kx.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://je.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://qv.9csxet.cn

static_cast<double>(a) / b
来源：http://fe.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://op.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://ye.huanxung.cn

[S53] C++：移动语义
来源：http://dd.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://kf.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://af.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vo.shxzukj.cn

[S55] C++：结构化绑定
来源：http://sm.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bf.yuexingan06.cn

[S56] C++：optional
来源：http://oi.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lm.szsharing.cn

[S57] C++：编译期常量
来源：http://ut.521024.cn

constexpr int N = 10;
来源：http://fa.lnxyls.cn

[S58] C++：命名空间
来源：http://oq.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://px.muxihuayi.cn

[S59] C++：静态断言
来源：http://yg.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cq.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://cf.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rz.yuntaijiaju.cn

================================================================================
来源：http://gw.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kl.jctech888.com.cn

================================================================================
来源：http://eh.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://wj.szsharing.cn

println("Hello")
来源：http://wa.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://fl.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iu.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://qd.hnjuh.cn

"值: $b"
来源：http://gp.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://ye.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://ot.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://is.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://or.asd995.cn

[T06] Kotlin：集合映射
来源：http://wb.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://px.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://fm.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ba.shxzukj.cn

[T08] Kotlin：数据类
来源：http://bb.521024.cn

data class User(val name: String, val age: Int)
来源：http://oi.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://xt.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://vw.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://qq.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ij.wgjwhj.cn

[T11] Kotlin：协程
来源：http://oo.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://to.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://bp.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://vy.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://nc.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://bq.huanxung.cn

[T14] Kotlin：循环
来源：http://yl.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://dr.panjiajie.cn

[T15] Kotlin：接口
来源：http://gd.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://hr.huixiangedu.cn

[T16] Swift：Hello World
来源：http://ks.colortex.cn

print("Hello")
来源：http://im.panjiajie.cn

[T17] Swift：变量与常量
来源：http://dx.szsharing.cn

var a = 1;  let b = 2
来源：http://wz.521024.cn

[T18] Swift：字符串插值
来源：http://af.chemitech.net.cn

"值: \(b)"
来源：http://sb.huanxung.cn

[T19] Swift：可选绑定
来源：http://hm.jctech888.com.cn

if let n = opt { print(n) }
来源：http://un.huixiangedu.cn

[T20] Swift：数组操作
来源：http://nl.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ji.newstarts.cn

[T21] Swift：遍历
来源：http://ur.jctech888.com.cn

for x in a { print(x) }
来源：http://vl.jianghongdianzi.cn

[T22] Swift：字典
来源：http://pa.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mm.shtwfgs.cn

[T23] Swift：函数
来源：http://js.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bh.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://db.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gf.bookmarksfly.cn

[T25] Swift：结构体
来源：http://sh.hahajie.cn

struct P { var x: Int }
来源：http://wb.shxzskj.cn

[T26] Swift：类与重写
来源：http://nf.shxzskj.cn

class A: Base { override func f() {} }
来源：http://af.521024.cn

[T27] Swift：错误处理
来源：http://pt.colortex.cn

do { try f() } catch { print(error) }
来源：http://iz.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://ho.szxytkj.cn

enum Color { case red, green }
来源：http://wh.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://dx.muxihuayi.cn

guard let x = opt else { return }
来源：http://ek.lnxyls.cn

[T30] Swift：协议
来源：http://ic.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://kr.hahajie.cn

[T31] Lua：Hello World
来源：http://ki.yuexingan06.cn

print("Hello")
来源：http://rs.colortex.cn

[T32] Lua：局部变量
来源：http://as.nszjky.cn

local a = 1
来源：http://ng.9csxet.cn

[T33] Lua：表（数组）
来源：http://fn.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rf.yuexingan06.cn

[T34] Lua：遍历表
来源：http://jf.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cx.haigaiapp.cn

[T35] Lua：字典表
来源：http://gh.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://wv.haigaiapp.cn

[T36] Lua：函数
来源：http://zl.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://ze.yuexingan06.cn


<!-- 参考信息 -->