代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://zv.newstarts.cn

[R32] 参数个数校验
来源：http://wv.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qk.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://hv.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yv.asd995.cn

[R34] 退出时清理
来源：http://wa.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qg.colortex.cn

[R35] 后台执行并等待
来源：http://pb.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mw.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://jd.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fe.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://wj.gzmigu.cn

files=$(ls -1)
来源：http://hk.panjiajie.cn

[R38] 管道串联
来源：http://nl.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://wn.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://qc.muxihuayi.cn

cmd > out.log 2>&1
来源：http://qz.szxytkj.cn

[R40] 追加写日志
来源：http://bf.wgjwhj.cn

echo "log" >> out.log
来源：http://mp.szsharing.cn

[R41] 丢弃输出
来源：http://md.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://hu.szxytkj.cn

[R42] 输入重定向
来源：http://or.szsharing.cn

wc -l < a.txt
来源：http://tp.haigaiapp.cn

[R43] 按名字查找文件
来源：http://gk.nszjky.cn

find . -name "*.log" -type f
来源：http://wc.szxytkj.cn

[R44] 按修改时间查找
来源：http://yp.lnxyls.cn

find . -mtime -7 -type f
来源：http://bg.bjjhwx.cn

[R45] 批量删除
来源：http://vo.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://hi.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://zb.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://id.nicolike.cn

[R47] sed 单行替换
来源：http://vp.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zt.lnxyls.cn

[R48] awk 取指定列
来源：http://jw.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://nx.9csxet.cn

[R49] awk 带条件
来源：http://uy.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ni.hahajie.cn

[R50] awk 求和
来源：http://uf.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hp.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://mp.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pr.shxzukj.cn

[R52] 统计行数
来源：http://vu.hnjuh.cn

wc -l a.txt
来源：http://yc.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://fj.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ad.nszjky.cn

[R54] 比较两个文件
来源：http://wo.9csxet.cn

diff a.txt b.txt
来源：http://lh.szxytkj.cn

[R55] 压缩与解压
来源：http://hn.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ky.nicolike.cn

[R56] 远程拷贝
来源：http://nb.huixinmuqiang.cn

scp file user@host:/path/
来源：http://uc.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://pk.colortex.cn

ssh user@host 'uptime'
来源：http://yx.muxihuayi.cn

[R58] 下载文件
来源：http://zx.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ls.huanxung.cn

[R59] 发 POST JSON
来源：http://uj.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://ja.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ot.bjjhwx.cn

[R61] 磁盘占用
来源：http://gv.asd995.cn

df -h;  du -sh *
来源：http://tp.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://iy.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://lx.szxytkj.cn

[R63] 内存与进程
来源：http://mp.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://ie.hahajie.cn

[R64] 结束进程
来源：http://ia.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://zh.hahajie.cn

[R65] 查看端口占用
来源：http://vp.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://po.lnxyls.cn

[R66] 定时任务
来源：http://qj.wgjwhj.cn

crontab -e;  crontab -l
来源：http://sh.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://gu.huanxung.cn

openssl rand -hex 16
来源：http://sw.panjiajie.cn

[R68] 计算文件校验值
来源：http://mp.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rv.9csxet.cn

[R69] 生成随机密码
来源：http://xx.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://tj.wgjwhj.cn

[R70] 时间戳与互转
来源：http://vf.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://zs.huanxung.cn

[R71] 日期格式化
来源：http://kl.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xy.hnjuh.cn

[R72] 等待端口就绪
来源：http://bu.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ll.521024.cn

[R73] 分割大日志
来源：http://kp.bjjhwx.cn

split -l 1000 big.log part_
来源：http://nz.yuntaijiaju.cn

[R74] 批量重命名
来源：http://uh.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ql.newstarts.cn

[R75] 导出环境变量
来源：http://di.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://eg.muxihuayi.cn

[R76] 使用临时文件
来源：http://gj.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ou.huanxung.cn

[R77] 读取用户输入
来源：http://uy.huanxung.cn

read -rp "请输入: " ans
来源：http://xo.huixiangedu.cn

[R78] 交互式菜单
来源：http://mx.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pc.521024.cn

[R79] 解析命令行选项
来源：http://tc.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yv.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://ju.jianghongdianzi.cn

time ./run.sh
来源：http://yh.wgjwhj.cn

================================================================================
来源：http://xj.newstarts.cn

S. C / C++ 专题
来源：http://dq.nicolike.cn

================================================================================
来源：http://uo.nicolike.cn

[S01] C：Hello World
来源：http://bm.chemitech.net.cn

#include <stdio.h>
来源：http://kx.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zi.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://bo.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://sm.colortex.cn

[S03] C：读入整数
来源：http://pn.panjiajie.cn

int x; scanf("%d", &x);
来源：http://qg.szxytkj.cn

[S04] C：字符串复制
来源：http://zx.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yd.newstarts.cn

[S05] C：字符串长度
来源：http://yx.szxytkj.cn

strlen(s)
来源：http://vb.wgjwhj.cn

[S06] C：字符串比较
来源：http://rh.hahajie.cn

strcmp(a, b) == 0
来源：http://bo.lnxyls.cn

[S07] C：数组遍历求和
来源：http://oh.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fn.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://nl.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yq.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://nd.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jn.colortex.cn

[S10] C：指针与解引用
来源：http://mo.nicolike.cn

int *p = &a;  *p = 5;
来源：http://pw.haigaiapp.cn

[S11] C：逐行读文件
来源：http://vi.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://zv.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lh.szsharing.cn

fclose(f);
来源：http://jw.gzmigu.cn

[S12] C：写文件
来源：http://cc.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mf.wgjwhj.cn

[S13] C：宏定义
来源：http://zd.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rj.huixiangedu.cn

[S14] C：枚举
来源：http://rp.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://la.hahajie.cn

[S15] C：类型转换
来源：http://qd.wgjwhj.cn

(double) a / b
来源：http://cx.newstarts.cn

[S16] C：位操作置位
来源：http://as.hnjuh.cn

x |= (1 << 3);
来源：http://hx.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://ok.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://et.nicolike.cn

[S18] C：命令行参数
来源：http://ee.haigaiapp.cn

int main(int argc, char **argv)
来源：http://lz.shtwfgs.cn

[S19] C：快速排序
来源：http://vh.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ew.lnxyls.cn

[S20] C：二分查找
来源：http://nl.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xw.colortex.cn

[S21] C：字符类别判断
来源：http://ez.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cc.shxzukj.cn

[S22] C：字符串转数字
来源：http://or.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xc.muxihuayi.cn

[S23] C：随机数
来源：http://zv.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://om.shxzukj.cn

[S24] C：获取本地时间
来源：http://rv.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ft.nicolike.cn

[S25] C：内存拷贝
来源：http://we.jctech888.com.cn

memcpy(dst, src, n);
来源：http://js.bookmarksfly.cn

[S26] C：内存清零
来源：http://zq.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://pt.chemitech.net.cn

[S27] C：定义常量
来源：http://mi.wgjwhj.cn

const double PI = 3.14159;
来源：http://vl.huixinmuqiang.cn

[S28] C：静态变量
来源：http://ik.colortex.cn

static int counter = 0;
来源：http://tc.huixiangedu.cn

[S29] C：变参函数
来源：http://lk.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nv.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://em.asd995.cn

#ifndef X_H
来源：http://dg.panjiajie.cn

#define X_H
来源：http://sd.nszjky.cn

#endif
来源：http://yl.hahajie.cn

[S31] C++：Hello World
来源：http://oe.gzmigu.cn

#include <iostream>
来源：http://uc.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://ns.huixiangedu.cn

[S32] C++：字符串
来源：http://iv.asd995.cn

std::string s = "hi";  s += "!";
来源：http://jj.bjjhwx.cn

[S33] C++：vector 增删
来源：http://ub.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ez.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://zo.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ns.huanxung.cn

[S35] C++：map
来源：http://jx.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kf.9csxet.cn

[S36] C++：unordered_map
来源：http://ls.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fx.huixiangedu.cn

[S37] C++：set
来源：http://oq.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wy.huixiangedu.cn

[S38] C++：排序
来源：http://pj.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://tv.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://di.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ez.bookmarksfly.cn

[S40] C++：查找元素
来源：http://kj.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iv.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://zy.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iu.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://gg.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://er.wgjwhj.cn

[S43] C++：智能指针
来源：http://vm.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://nj.lnxyls.cn

[S44] C++：引用传参
来源：http://os.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://cq.bjjhwx.cn

[S45] C++：lambda
来源：http://dw.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lq.lnxyls.cn

[S46] C++：函数模板
来源：http://zw.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jy.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://qz.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vt.9csxet.cn

[S48] C++：逐行读文件
来源：http://tu.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vg.9csxet.cn

while (std::getline(in, line)) { }
来源：http://yg.nicolike.cn

[S49] C++：写文件
来源：http://jv.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dc.wgjwhj.cn

[S50] C++：格式化数字
来源：http://uq.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wa.hnjuh.cn

[S51] C++：显式类型转换
来源：http://wu.panjiajie.cn

static_cast<double>(a) / b
来源：http://be.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://xb.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://tp.asd995.cn

[S53] C++：移动语义
来源：http://wx.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://dq.chemitech.net.cn

[S54] C++：异常处理
来源：http://pw.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lp.nicolike.cn

[S55] C++：结构化绑定
来源：http://nd.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sh.panjiajie.cn

[S56] C++：optional
来源：http://an.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ap.lnxyls.cn

[S57] C++：编译期常量
来源：http://id.panjiajie.cn

constexpr int N = 10;
来源：http://ip.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://ky.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://vr.nicolike.cn

[S59] C++：静态断言
来源：http://on.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ga.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://gf.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zq.hahajie.cn

================================================================================
来源：http://hq.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nk.9csxet.cn

================================================================================
来源：http://dd.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://md.colortex.cn

println("Hello")
来源：http://hq.shxzukj.cn

[T02] Kotlin：变量
来源：http://zk.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bb.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://xy.hnjuh.cn

"值: $b"
来源：http://ez.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://tv.521024.cn

val n: String? = null;  n?.length
来源：http://cr.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://lw.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gs.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://ux.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://do.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://bp.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iv.panjiajie.cn

[T08] Kotlin：数据类
来源：http://qf.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://ub.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://dj.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://xz.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://is.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yq.shtwfgs.cn

[T11] Kotlin：协程
来源：http://hd.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yq.huanxung.cn

[T12] Kotlin：解构声明
来源：http://cs.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://gn.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://al.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://pw.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://uy.nicolike.cn

for (i in 1..10) println(i)
来源：http://tt.szxytkj.cn

[T15] Kotlin：接口
来源：http://vz.nszjky.cn

interface Shape { fun area(): Double }
来源：http://qh.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://mw.lnxyls.cn

print("Hello")
来源：http://bo.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://nc.lnxyls.cn

var a = 1;  let b = 2
来源：http://gz.gzmigu.cn

[T18] Swift：字符串插值
来源：http://ci.shxzukj.cn

"值: \(b)"
来源：http://sd.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://lr.chemitech.net.cn

if let n = opt { print(n) }
来源：http://qo.colortex.cn

[T20] Swift：数组操作
来源：http://of.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://to.gzmigu.cn

[T21] Swift：遍历
来源：http://zq.jctech888.com.cn

for x in a { print(x) }
来源：http://xi.hnjuh.cn

[T22] Swift：字典
来源：http://jb.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vu.bookmarksfly.cn

[T23] Swift：函数
来源：http://sq.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uy.lnxyls.cn

[T24] Swift：闭包
来源：http://qn.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lt.yuexingan06.cn

[T25] Swift：结构体
来源：http://kf.gzmigu.cn

struct P { var x: Int }
来源：http://yq.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://wh.hahajie.cn

class A: Base { override func f() {} }
来源：http://qo.huixiangedu.cn

[T27] Swift：错误处理
来源：http://wi.szsharing.cn

do { try f() } catch { print(error) }
来源：http://gk.shxzukj.cn

[T28] Swift：枚举
来源：http://lu.szxytkj.cn

enum Color { case red, green }
来源：http://tq.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://ud.colortex.cn

guard let x = opt else { return }
来源：http://mr.panjiajie.cn

[T30] Swift：协议
来源：http://pm.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://an.panjiajie.cn

[T31] Lua：Hello World
来源：http://yi.nicolike.cn

print("Hello")
来源：http://ql.bjjhwx.cn

[T32] Lua：局部变量
来源：http://ar.shxzukj.cn

local a = 1
来源：http://qd.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://ba.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hu.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://ef.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yd.huixiangedu.cn


<!-- 参考信息 -->