代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jo.szxytkj.cn

[R30] 函数返回状态码
来源：http://mv.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://rq.huixinmuqiang.cn

[R31] 局部变量
来源：http://jm.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://jq.szxytkj.cn

[R32] 参数个数校验
来源：http://qr.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ed.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://yq.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kt.yuntaijiaju.cn

[R34] 退出时清理
来源：http://xe.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pt.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://px.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dy.hahajie.cn

[R36] 并发执行多个任务
来源：http://uw.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ja.hnjuh.cn

[R37] 把输出赋给变量
来源：http://us.shtwfgs.cn

files=$(ls -1)
来源：http://fv.lnxyls.cn

[R38] 管道串联
来源：http://hw.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://gg.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://ls.wgjwhj.cn

cmd > out.log 2>&1
来源：http://aj.muxihuayi.cn

[R40] 追加写日志
来源：http://tj.521024.cn

echo "log" >> out.log
来源：http://cg.asd995.cn

[R41] 丢弃输出
来源：http://ea.nszjky.cn

cmd >/dev/null 2>&1
来源：http://hl.bjjhwx.cn

[R42] 输入重定向
来源：http://zg.jctech888.com.cn

wc -l < a.txt
来源：http://ot.lnxyls.cn

[R43] 按名字查找文件
来源：http://wp.521024.cn

find . -name "*.log" -type f
来源：http://pq.yuexingan06.cn

[R44] 按修改时间查找
来源：http://zn.9csxet.cn

find . -mtime -7 -type f
来源：http://kc.szxytkj.cn

[R45] 批量删除
来源：http://xe.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://vp.asd995.cn

[R46] 递归替换文件内容
来源：http://pe.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mt.521024.cn

[R47] sed 单行替换
来源：http://ip.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ob.huanxung.cn

[R48] awk 取指定列
来源：http://ss.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://pi.newstarts.cn

[R49] awk 带条件
来源：http://wj.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mt.yuntaijiaju.cn

[R50] awk 求和
来源：http://kd.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jr.szsharing.cn

[R51] 排序去重取前几
来源：http://ih.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ee.nszjky.cn

[R52] 统计行数
来源：http://wr.hnjuh.cn

wc -l a.txt
来源：http://br.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://sp.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kd.nicolike.cn

[R54] 比较两个文件
来源：http://tk.shtwfgs.cn

diff a.txt b.txt
来源：http://ma.gzmigu.cn

[R55] 压缩与解压
来源：http://ex.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nv.shxzukj.cn

[R56] 远程拷贝
来源：http://mn.jianghongdianzi.cn

scp file user@host:/path/
来源：http://ys.jctech888.com.cn

[R57] 远程执行命令
来源：http://cc.shxzukj.cn

ssh user@host 'uptime'
来源：http://tq.colortex.cn

[R58] 下载文件
来源：http://gw.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lk.jctech888.com.cn

[R59] 发 POST JSON
来源：http://lt.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dn.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://vq.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ny.bjjhwx.cn

[R61] 磁盘占用
来源：http://bw.jianghongdianzi.cn

df -h;  du -sh *
来源：http://gf.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://bq.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://bc.bjjhwx.cn

[R63] 内存与进程
来源：http://xd.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://ui.wgjwhj.cn

[R64] 结束进程
来源：http://pn.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://yr.bookmarksfly.cn

[R65] 查看端口占用
来源：http://jp.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zw.nszjky.cn

[R66] 定时任务
来源：http://em.huixiangedu.cn

crontab -e;  crontab -l
来源：http://vo.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://dp.yuexingan06.cn

openssl rand -hex 16
来源：http://oq.nicolike.cn

[R68] 计算文件校验值
来源：http://ro.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uu.szxytkj.cn

[R69] 生成随机密码
来源：http://ei.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://tc.huanxung.cn

[R70] 时间戳与互转
来源：http://dd.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://xe.shxzskj.cn

[R71] 日期格式化
来源：http://qh.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hg.hahajie.cn

[R72] 等待端口就绪
来源：http://bs.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://my.newstarts.cn

[R73] 分割大日志
来源：http://gf.panjiajie.cn

split -l 1000 big.log part_
来源：http://us.shxzukj.cn

[R74] 批量重命名
来源：http://kn.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yu.shxzukj.cn

[R75] 导出环境变量
来源：http://ax.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://jo.hahajie.cn

[R76] 使用临时文件
来源：http://hg.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eb.nszjky.cn

[R77] 读取用户输入
来源：http://ck.jctech888.com.cn

read -rp "请输入: " ans
来源：http://uo.szxytkj.cn

[R78] 交互式菜单
来源：http://se.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pr.shxzukj.cn

[R79] 解析命令行选项
来源：http://jb.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rx.asd995.cn

[R80] 查看脚本执行耗时
来源：http://bk.colortex.cn

time ./run.sh
来源：http://jy.szxytkj.cn

================================================================================
来源：http://ko.huixinmuqiang.cn

S. C / C++ 专题
来源：http://ko.wgjwhj.cn

================================================================================
来源：http://pe.jianghongdianzi.cn

[S01] C：Hello World
来源：http://wd.shxzskj.cn

#include <stdio.h>
来源：http://ca.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wd.nszjky.cn

[S02] C：变量与格式化输出
来源：http://ps.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://zd.lnxyls.cn

[S03] C：读入整数
来源：http://cq.gzmigu.cn

int x; scanf("%d", &x);
来源：http://fc.hahajie.cn

[S04] C：字符串复制
来源：http://vp.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fv.bjjhwx.cn

[S05] C：字符串长度
来源：http://xh.shxzukj.cn

strlen(s)
来源：http://jm.panjiajie.cn

[S06] C：字符串比较
来源：http://nh.hnjuh.cn

strcmp(a, b) == 0
来源：http://gl.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://vw.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ft.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://dl.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bu.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://rr.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iw.hnjuh.cn

[S10] C：指针与解引用
来源：http://uj.asd995.cn

int *p = &a;  *p = 5;
来源：http://yy.shxzukj.cn

[S11] C：逐行读文件
来源：http://uh.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://xo.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iz.panjiajie.cn

fclose(f);
来源：http://qf.yuexingan06.cn

[S12] C：写文件
来源：http://il.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ik.bjjhwx.cn

[S13] C：宏定义
来源：http://sl.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kx.shxzskj.cn

[S14] C：枚举
来源：http://hq.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://tb.newstarts.cn

[S15] C：类型转换
来源：http://ae.yuexingan06.cn

(double) a / b
来源：http://kr.bookmarksfly.cn

[S16] C：位操作置位
来源：http://nm.chemitech.net.cn

x |= (1 << 3);
来源：http://ba.nszjky.cn

[S17] C：安全拼接字符串
来源：http://dp.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://za.huanxung.cn

[S18] C：命令行参数
来源：http://bb.9csxet.cn

int main(int argc, char **argv)
来源：http://hv.asd995.cn

[S19] C：快速排序
来源：http://ev.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cj.shxzukj.cn

[S20] C：二分查找
来源：http://cc.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://at.hahajie.cn

[S21] C：字符类别判断
来源：http://ox.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ax.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://we.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fv.gzmigu.cn

[S23] C：随机数
来源：http://fo.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ul.nszjky.cn

[S24] C：获取本地时间
来源：http://rx.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hp.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://fn.9csxet.cn

memcpy(dst, src, n);
来源：http://ib.colortex.cn

[S26] C：内存清零
来源：http://dh.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://ar.chemitech.net.cn

[S27] C：定义常量
来源：http://rw.asd995.cn

const double PI = 3.14159;
来源：http://wa.szxytkj.cn

[S28] C：静态变量
来源：http://et.yuntaijiaju.cn

static int counter = 0;
来源：http://mx.shtwfgs.cn

[S29] C：变参函数
来源：http://hp.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xz.shxzukj.cn

[S30] C：头文件保护
来源：http://fk.jianghongdianzi.cn

#ifndef X_H
来源：http://di.gzmigu.cn

#define X_H
来源：http://bp.huixiangedu.cn

#endif
来源：http://or.yuexingan06.cn

[S31] C++：Hello World
来源：http://wr.haigaiapp.cn

#include <iostream>
来源：http://ol.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://fw.huixiangedu.cn

[S32] C++：字符串
来源：http://np.colortex.cn

std::string s = "hi";  s += "!";
来源：http://jg.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://vt.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rd.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://dy.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://um.yuntaijiaju.cn

[S35] C++：map
来源：http://ya.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ya.bjjhwx.cn

[S36] C++：unordered_map
来源：http://na.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://le.szsharing.cn

[S37] C++：set
来源：http://qi.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oz.muxihuayi.cn

[S38] C++：排序
来源：http://as.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://je.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://fe.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ao.jctech888.com.cn

[S40] C++：查找元素
来源：http://td.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iv.521024.cn

[S41] C++：类与构造函数
来源：http://gf.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oc.9csxet.cn

[S42] C++：继承与虚函数
来源：http://dj.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://ud.9csxet.cn

[S43] C++：智能指针
来源：http://qw.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://df.bjjhwx.cn

[S44] C++：引用传参
来源：http://ps.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://tx.yuexingan06.cn

[S45] C++：lambda
来源：http://jw.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hc.521024.cn

[S46] C++：函数模板
来源：http://eo.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ly.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://je.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pw.nicolike.cn

[S48] C++：逐行读文件
来源：http://rp.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hi.colortex.cn

while (std::getline(in, line)) { }
来源：http://nl.bookmarksfly.cn

[S49] C++：写文件
来源：http://oy.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://os.hnjuh.cn

[S50] C++：格式化数字
来源：http://bj.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://df.9csxet.cn

[S51] C++：显式类型转换
来源：http://io.szsharing.cn

static_cast<double>(a) / b
来源：http://mv.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://zs.9csxet.cn

int size() const noexcept { return n_; }
来源：http://by.bookmarksfly.cn

[S53] C++：移动语义
来源：http://vn.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://og.chemitech.net.cn

[S54] C++：异常处理
来源：http://qz.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fw.hahajie.cn

[S55] C++：结构化绑定
来源：http://tz.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tn.bookmarksfly.cn

[S56] C++：optional
来源：http://ui.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ey.shxzskj.cn

[S57] C++：编译期常量
来源：http://kb.hnjuh.cn

constexpr int N = 10;
来源：http://xu.asd995.cn

[S58] C++：命名空间
来源：http://hh.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://aa.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://mg.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eg.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://xm.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ep.haigaiapp.cn

================================================================================
来源：http://mt.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uj.hahajie.cn

================================================================================
来源：http://jk.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://el.nicolike.cn

println("Hello")
来源：http://pa.chemitech.net.cn

[T02] Kotlin：变量
来源：http://os.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bq.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://ic.jianghongdianzi.cn

"值: $b"
来源：http://la.colortex.cn

[T04] Kotlin：空安全
来源：http://hi.lnxyls.cn

val n: String? = null;  n?.length
来源：http://ux.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://oi.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jc.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://qc.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yf.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://qd.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://my.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://gg.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://pi.colortex.cn

[T09] Kotlin：扩展函数
来源：http://ji.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://ls.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://ga.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zw.bjjhwx.cn

[T11] Kotlin：协程
来源：http://ht.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ue.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://bt.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://bl.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://wk.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://xo.hnjuh.cn

[T14] Kotlin：循环
来源：http://ry.huanxung.cn

for (i in 1..10) println(i)
来源：http://za.shxzukj.cn

[T15] Kotlin：接口
来源：http://iq.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://lz.hnjuh.cn

[T16] Swift：Hello World
来源：http://io.nicolike.cn

print("Hello")
来源：http://gb.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://kv.nszjky.cn

var a = 1;  let b = 2
来源：http://cr.newstarts.cn

[T18] Swift：字符串插值
来源：http://xo.bookmarksfly.cn

"值: \(b)"
来源：http://nb.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://ie.colortex.cn

if let n = opt { print(n) }
来源：http://wf.hahajie.cn

[T20] Swift：数组操作
来源：http://vn.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fn.shxzukj.cn

[T21] Swift：遍历
来源：http://uz.shtwfgs.cn

for x in a { print(x) }
来源：http://uy.panjiajie.cn

[T22] Swift：字典
来源：http://lc.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ty.9csxet.cn

[T23] Swift：函数
来源：http://kf.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nm.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://ls.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ak.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://oc.nicolike.cn

struct P { var x: Int }
来源：http://sf.huanxung.cn

[T26] Swift：类与重写
来源：http://gu.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://th.gzmigu.cn

[T27] Swift：错误处理
来源：http://it.nicolike.cn

do { try f() } catch { print(error) }
来源：http://pw.jctech888.com.cn

[T28] Swift：枚举
来源：http://de.hahajie.cn

enum Color { case red, green }
来源：http://ri.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://ll.szsharing.cn

guard let x = opt else { return }
来源：http://uw.newstarts.cn

[T30] Swift：协议
来源：http://cv.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://ou.newstarts.cn

[T31] Lua：Hello World
来源：http://wb.shxzskj.cn

print("Hello")
来源：http://sv.muxihuayi.cn

[T32] Lua：局部变量
来源：http://sr.lnxyls.cn

local a = 1
来源：http://gh.shxzskj.cn


<!-- 参考信息 -->