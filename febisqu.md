代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oh.lnxyls.cn

[R30] 函数返回状态码
来源：http://ey.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://vv.gzmigu.cn

[R31] 局部变量
来源：http://uc.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://qe.nicolike.cn

[R32] 参数个数校验
来源：http://yj.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yf.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://fb.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jz.szsharing.cn

[R34] 退出时清理
来源：http://py.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gj.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://wk.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://od.newstarts.cn

[R36] 并发执行多个任务
来源：http://sw.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ca.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://ve.9csxet.cn

files=$(ls -1)
来源：http://pm.newstarts.cn

[R38] 管道串联
来源：http://pb.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://jg.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://eo.hnjuh.cn

cmd > out.log 2>&1
来源：http://ku.szxytkj.cn

[R40] 追加写日志
来源：http://um.yuntaijiaju.cn

echo "log" >> out.log
来源：http://ar.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://sa.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://qa.shxzskj.cn

[R42] 输入重定向
来源：http://ku.huixiangedu.cn

wc -l < a.txt
来源：http://cx.lnxyls.cn

[R43] 按名字查找文件
来源：http://ec.shtwfgs.cn

find . -name "*.log" -type f
来源：http://zz.newstarts.cn

[R44] 按修改时间查找
来源：http://jp.colortex.cn

find . -mtime -7 -type f
来源：http://gx.szxytkj.cn

[R45] 批量删除
来源：http://up.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://vz.hnjuh.cn

[R46] 递归替换文件内容
来源：http://hx.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://te.shxzukj.cn

[R47] sed 单行替换
来源：http://kz.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wy.bookmarksfly.cn

[R48] awk 取指定列
来源：http://fh.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://so.hahajie.cn

[R49] awk 带条件
来源：http://sv.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qh.jianghongdianzi.cn

[R50] awk 求和
来源：http://at.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uj.szxytkj.cn

[R51] 排序去重取前几
来源：http://zx.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qa.521024.cn

[R52] 统计行数
来源：http://zy.huixinmuqiang.cn

wc -l a.txt
来源：http://ad.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://oj.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ks.shxzskj.cn

[R54] 比较两个文件
来源：http://uo.newstarts.cn

diff a.txt b.txt
来源：http://dv.yuexingan06.cn

[R55] 压缩与解压
来源：http://yf.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oo.bjjhwx.cn

[R56] 远程拷贝
来源：http://hf.nicolike.cn

scp file user@host:/path/
来源：http://oq.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://rm.colortex.cn

ssh user@host 'uptime'
来源：http://zp.asd995.cn

[R58] 下载文件
来源：http://ao.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hl.521024.cn

[R59] 发 POST JSON
来源：http://ik.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://we.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://kh.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jd.hnjuh.cn

[R61] 磁盘占用
来源：http://ug.huixiangedu.cn

df -h;  du -sh *
来源：http://fk.hahajie.cn

[R62] 找最占空间的文件
来源：http://zx.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://cl.shtwfgs.cn

[R63] 内存与进程
来源：http://ki.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://hs.szsharing.cn

[R64] 结束进程
来源：http://oj.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://ow.nicolike.cn

[R65] 查看端口占用
来源：http://ic.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kw.yuntaijiaju.cn

[R66] 定时任务
来源：http://kh.panjiajie.cn

crontab -e;  crontab -l
来源：http://hu.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://kb.521024.cn

openssl rand -hex 16
来源：http://nj.hnjuh.cn

[R68] 计算文件校验值
来源：http://xc.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xa.asd995.cn

[R69] 生成随机密码
来源：http://wb.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://bq.panjiajie.cn

[R70] 时间戳与互转
来源：http://pm.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://ye.shxzukj.cn

[R71] 日期格式化
来源：http://zc.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mr.wgjwhj.cn

[R72] 等待端口就绪
来源：http://yb.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oy.chemitech.net.cn

[R73] 分割大日志
来源：http://oz.szxytkj.cn

split -l 1000 big.log part_
来源：http://mz.szxytkj.cn

[R74] 批量重命名
来源：http://qp.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cl.yuexingan06.cn

[R75] 导出环境变量
来源：http://yl.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://av.nszjky.cn

[R76] 使用临时文件
来源：http://bq.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sl.wgjwhj.cn

[R77] 读取用户输入
来源：http://tf.muxihuayi.cn

read -rp "请输入: " ans
来源：http://mj.shtwfgs.cn

[R78] 交互式菜单
来源：http://wg.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gt.nszjky.cn

[R79] 解析命令行选项
来源：http://bu.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nq.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://ok.shtwfgs.cn

time ./run.sh
来源：http://ex.shxzukj.cn

================================================================================
来源：http://yf.newstarts.cn

S. C / C++ 专题
来源：http://cp.muxihuayi.cn

================================================================================
来源：http://qy.jctech888.com.cn

[S01] C：Hello World
来源：http://cb.shtwfgs.cn

#include <stdio.h>
来源：http://ca.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rq.huanxung.cn

[S02] C：变量与格式化输出
来源：http://zg.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://ih.chemitech.net.cn

[S03] C：读入整数
来源：http://sm.nicolike.cn

int x; scanf("%d", &x);
来源：http://le.jctech888.com.cn

[S04] C：字符串复制
来源：http://hn.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pq.521024.cn

[S05] C：字符串长度
来源：http://qd.colortex.cn

strlen(s)
来源：http://dy.hahajie.cn

[S06] C：字符串比较
来源：http://rq.huixiangedu.cn

strcmp(a, b) == 0
来源：http://bc.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://ih.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jy.asd995.cn

[S08] C：动态内存分配与释放
来源：http://ug.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ys.colortex.cn

[S09] C：结构体定义与初始化
来源：http://id.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://if.asd995.cn

[S10] C：指针与解引用
来源：http://vu.colortex.cn

int *p = &a;  *p = 5;
来源：http://tq.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://cx.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://bi.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mf.shxzukj.cn

fclose(f);
来源：http://vx.huixiangedu.cn

[S12] C：写文件
来源：http://qp.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bb.muxihuayi.cn

[S13] C：宏定义
来源：http://uh.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vx.shxzukj.cn

[S14] C：枚举
来源：http://zd.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://bn.bjjhwx.cn

[S15] C：类型转换
来源：http://fp.yuexingan06.cn

(double) a / b
来源：http://dw.bookmarksfly.cn

[S16] C：位操作置位
来源：http://gk.yuntaijiaju.cn

x |= (1 << 3);
来源：http://nx.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://xx.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yo.nicolike.cn

[S18] C：命令行参数
来源：http://mw.newstarts.cn

int main(int argc, char **argv)
来源：http://hu.panjiajie.cn

[S19] C：快速排序
来源：http://ur.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kh.szxytkj.cn

[S20] C：二分查找
来源：http://pm.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://az.muxihuayi.cn

[S21] C：字符类别判断
来源：http://ru.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ff.nszjky.cn

[S22] C：字符串转数字
来源：http://sc.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cx.lnxyls.cn

[S23] C：随机数
来源：http://um.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oh.nszjky.cn

[S24] C：获取本地时间
来源：http://ui.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ny.gzmigu.cn

[S25] C：内存拷贝
来源：http://ll.nszjky.cn

memcpy(dst, src, n);
来源：http://yp.nszjky.cn

[S26] C：内存清零
来源：http://em.hahajie.cn

memset(a, 0, sizeof a);
来源：http://dn.jianghongdianzi.cn

[S27] C：定义常量
来源：http://ji.521024.cn

const double PI = 3.14159;
来源：http://cc.521024.cn

[S28] C：静态变量
来源：http://if.panjiajie.cn

static int counter = 0;
来源：http://sj.colortex.cn

[S29] C：变参函数
来源：http://ak.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wx.szsharing.cn

[S30] C：头文件保护
来源：http://pl.huanxung.cn

#ifndef X_H
来源：http://br.shxzskj.cn

#define X_H
来源：http://zg.nszjky.cn

#endif
来源：http://wu.shtwfgs.cn

[S31] C++：Hello World
来源：http://zw.huixiangedu.cn

#include <iostream>
来源：http://sv.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://wj.nicolike.cn

[S32] C++：字符串
来源：http://zu.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://xu.haigaiapp.cn

[S33] C++：vector 增删
来源：http://nr.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://is.hahajie.cn

[S34] C++：遍历 vector
来源：http://ix.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://ht.newstarts.cn

[S35] C++：map
来源：http://ao.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xw.bjjhwx.cn

[S36] C++：unordered_map
来源：http://pr.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zo.yuntaijiaju.cn

[S37] C++：set
来源：http://mg.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pe.shxzukj.cn

[S38] C++：排序
来源：http://sx.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://kn.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://ff.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qx.gzmigu.cn

[S40] C++：查找元素
来源：http://gg.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dd.panjiajie.cn

[S41] C++：类与构造函数
来源：http://og.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sh.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://yh.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://zr.521024.cn

[S43] C++：智能指针
来源：http://ce.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://im.szxytkj.cn

[S44] C++：引用传参
来源：http://ub.colortex.cn

void inc(int &x) { ++x; }
来源：http://ch.newstarts.cn

[S45] C++：lambda
来源：http://yn.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ph.bookmarksfly.cn

[S46] C++：函数模板
来源：http://am.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jc.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://mk.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://by.huanxung.cn

[S48] C++：逐行读文件
来源：http://vx.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yc.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://wq.haigaiapp.cn

[S49] C++：写文件
来源：http://ge.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xt.huixiangedu.cn

[S50] C++：格式化数字
来源：http://fy.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oc.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://eg.nicolike.cn

static_cast<double>(a) / b
来源：http://dm.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://jf.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://fq.shtwfgs.cn

[S53] C++：移动语义
来源：http://kj.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://wl.newstarts.cn

[S54] C++：异常处理
来源：http://ex.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cd.521024.cn

[S55] C++：结构化绑定
来源：http://ah.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ux.hnjuh.cn

[S56] C++：optional
来源：http://tq.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ha.9csxet.cn

[S57] C++：编译期常量
来源：http://vt.haigaiapp.cn

constexpr int N = 10;
来源：http://as.nicolike.cn

[S58] C++：命名空间
来源：http://nc.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://ve.colortex.cn

[S59] C++：静态断言
来源：http://ne.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pb.521024.cn

[S60] C++：遍历并删除元素
来源：http://pl.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vz.nszjky.cn

================================================================================
来源：http://jl.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ha.huixiangedu.cn

================================================================================
来源：http://hu.huanxung.cn

[T01] Kotlin：Hello World
来源：http://gp.huanxung.cn

println("Hello")
来源：http://zn.huixiangedu.cn

[T02] Kotlin：变量
来源：http://ja.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://du.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://an.hahajie.cn

"值: $b"
来源：http://mk.lnxyls.cn

[T04] Kotlin：空安全
来源：http://om.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://qm.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://br.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zn.szsharing.cn

[T06] Kotlin：集合映射
来源：http://dl.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gb.521024.cn

[T07] Kotlin：集合过滤
来源：http://jc.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pc.521024.cn

[T08] Kotlin：数据类
来源：http://gr.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://sd.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://wo.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://ki.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://ln.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ms.newstarts.cn

[T11] Kotlin：协程
来源：http://tk.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ai.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://he.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://gh.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://yk.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://vt.lnxyls.cn

[T14] Kotlin：循环
来源：http://du.lnxyls.cn

for (i in 1..10) println(i)
来源：http://eq.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://js.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://ff.chemitech.net.cn

[T16] Swift：Hello World
来源：http://yp.521024.cn

print("Hello")
来源：http://is.asd995.cn

[T17] Swift：变量与常量
来源：http://mq.hahajie.cn

var a = 1;  let b = 2
来源：http://gs.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://ry.panjiajie.cn

"值: \(b)"
来源：http://bk.shxzukj.cn

[T19] Swift：可选绑定
来源：http://pd.newstarts.cn

if let n = opt { print(n) }
来源：http://im.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://or.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bn.asd995.cn

[T21] Swift：遍历
来源：http://rr.hahajie.cn

for x in a { print(x) }
来源：http://wy.wgjwhj.cn

[T22] Swift：字典
来源：http://yf.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tj.jianghongdianzi.cn

[T23] Swift：函数
来源：http://kt.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nc.huanxung.cn

[T24] Swift：闭包
来源：http://lh.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cq.yuexingan06.cn

[T25] Swift：结构体
来源：http://dn.lnxyls.cn

struct P { var x: Int }
来源：http://qr.lnxyls.cn

[T26] Swift：类与重写
来源：http://ml.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://fb.wgjwhj.cn

[T27] Swift：错误处理
来源：http://su.newstarts.cn

do { try f() } catch { print(error) }
来源：http://ul.jctech888.com.cn

[T28] Swift：枚举
来源：http://pl.nszjky.cn

enum Color { case red, green }
来源：http://un.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://fk.hahajie.cn

guard let x = opt else { return }
来源：http://ld.lnxyls.cn

[T30] Swift：协议
来源：http://si.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://tr.521024.cn

[T31] Lua：Hello World
来源：http://wy.gzmigu.cn

print("Hello")
来源：http://wk.newstarts.cn

[T32] Lua：局部变量
来源：http://tc.szxytkj.cn

local a = 1
来源：http://vn.bjjhwx.cn


<!-- 参考信息 -->