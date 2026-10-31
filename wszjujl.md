代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://za.colortex.cn

[R32] 参数个数校验
来源：http://ps.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zb.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://wd.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nz.szsharing.cn

[R34] 退出时清理
来源：http://xq.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wq.yuexingan06.cn

[R35] 后台执行并等待
来源：http://mf.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ui.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://aw.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qi.huanxung.cn

[R37] 把输出赋给变量
来源：http://qp.asd995.cn

files=$(ls -1)
来源：http://pk.wgjwhj.cn

[R38] 管道串联
来源：http://sl.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://fi.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://ey.muxihuayi.cn

cmd > out.log 2>&1
来源：http://ua.yuntaijiaju.cn

[R40] 追加写日志
来源：http://ko.gzmigu.cn

echo "log" >> out.log
来源：http://we.bookmarksfly.cn

[R41] 丢弃输出
来源：http://tk.nszjky.cn

cmd >/dev/null 2>&1
来源：http://gm.yuntaijiaju.cn

[R42] 输入重定向
来源：http://uj.chemitech.net.cn

wc -l < a.txt
来源：http://hn.yuexingan06.cn

[R43] 按名字查找文件
来源：http://ry.shxzukj.cn

find . -name "*.log" -type f
来源：http://ak.muxihuayi.cn

[R44] 按修改时间查找
来源：http://al.lnxyls.cn

find . -mtime -7 -type f
来源：http://zy.nicolike.cn

[R45] 批量删除
来源：http://ek.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://ge.shxzukj.cn

[R46] 递归替换文件内容
来源：http://tb.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vj.yuexingan06.cn

[R47] sed 单行替换
来源：http://us.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ab.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://al.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://xp.hnjuh.cn

[R49] awk 带条件
来源：http://is.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pb.521024.cn

[R50] awk 求和
来源：http://jx.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ye.colortex.cn

[R51] 排序去重取前几
来源：http://rc.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sc.521024.cn

[R52] 统计行数
来源：http://fg.muxihuayi.cn

wc -l a.txt
来源：http://ll.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://th.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cm.colortex.cn

[R54] 比较两个文件
来源：http://dh.jctech888.com.cn

diff a.txt b.txt
来源：http://zy.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://vu.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tt.chemitech.net.cn

[R56] 远程拷贝
来源：http://ln.hahajie.cn

scp file user@host:/path/
来源：http://sc.chemitech.net.cn

[R57] 远程执行命令
来源：http://kv.huanxung.cn

ssh user@host 'uptime'
来源：http://hg.chemitech.net.cn

[R58] 下载文件
来源：http://rp.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xw.nszjky.cn

[R59] 发 POST JSON
来源：http://wy.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sa.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://dl.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dl.muxihuayi.cn

[R61] 磁盘占用
来源：http://hl.newstarts.cn

df -h;  du -sh *
来源：http://ba.szxytkj.cn

[R62] 找最占空间的文件
来源：http://jz.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://ph.nszjky.cn

[R63] 内存与进程
来源：http://kr.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://gd.9csxet.cn

[R64] 结束进程
来源：http://yu.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://lj.wgjwhj.cn

[R65] 查看端口占用
来源：http://mc.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fm.yuntaijiaju.cn

[R66] 定时任务
来源：http://uv.yuexingan06.cn

crontab -e;  crontab -l
来源：http://aj.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://zk.hnjuh.cn

openssl rand -hex 16
来源：http://kx.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://uw.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ek.panjiajie.cn

[R69] 生成随机密码
来源：http://fq.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://ei.hnjuh.cn

[R70] 时间戳与互转
来源：http://ur.nszjky.cn

date +%s;  date -d @1700000000
来源：http://tr.bjjhwx.cn

[R71] 日期格式化
来源：http://ca.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ev.jctech888.com.cn

[R72] 等待端口就绪
来源：http://lh.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bv.hnjuh.cn

[R73] 分割大日志
来源：http://es.colortex.cn

split -l 1000 big.log part_
来源：http://hu.yuexingan06.cn

[R74] 批量重命名
来源：http://vx.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ye.shxzukj.cn

[R75] 导出环境变量
来源：http://uy.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://jv.haigaiapp.cn

[R76] 使用临时文件
来源：http://sm.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sp.bookmarksfly.cn

[R77] 读取用户输入
来源：http://st.huanxung.cn

read -rp "请输入: " ans
来源：http://uz.asd995.cn

[R78] 交互式菜单
来源：http://xd.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nb.haigaiapp.cn

[R79] 解析命令行选项
来源：http://wg.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://to.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://qw.jctech888.com.cn

time ./run.sh
来源：http://pz.huixinmuqiang.cn

================================================================================
来源：http://ue.newstarts.cn

S. C / C++ 专题
来源：http://zx.huixiangedu.cn

================================================================================
来源：http://zs.shtwfgs.cn

[S01] C：Hello World
来源：http://dt.shxzskj.cn

#include <stdio.h>
来源：http://st.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ib.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://wm.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://gl.gzmigu.cn

[S03] C：读入整数
来源：http://ic.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://eq.shxzskj.cn

[S04] C：字符串复制
来源：http://yb.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bd.hahajie.cn

[S05] C：字符串长度
来源：http://ns.yuexingan06.cn

strlen(s)
来源：http://ws.shxzukj.cn

[S06] C：字符串比较
来源：http://ha.yuexingan06.cn

strcmp(a, b) == 0
来源：http://fx.9csxet.cn

[S07] C：数组遍历求和
来源：http://ck.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xc.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://bw.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zi.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://hq.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vi.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://uh.huanxung.cn

int *p = &a;  *p = 5;
来源：http://fo.huanxung.cn

[S11] C：逐行读文件
来源：http://cc.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://bv.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vy.jctech888.com.cn

fclose(f);
来源：http://fo.yuexingan06.cn

[S12] C：写文件
来源：http://kk.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yw.yuexingan06.cn

[S13] C：宏定义
来源：http://xw.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://un.nszjky.cn

[S14] C：枚举
来源：http://vd.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://fc.bookmarksfly.cn

[S15] C：类型转换
来源：http://lx.shxzskj.cn

(double) a / b
来源：http://ka.nicolike.cn

[S16] C：位操作置位
来源：http://rj.jianghongdianzi.cn

x |= (1 << 3);
来源：http://ty.colortex.cn

[S17] C：安全拼接字符串
来源：http://xo.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qw.shxzukj.cn

[S18] C：命令行参数
来源：http://bg.asd995.cn

int main(int argc, char **argv)
来源：http://lq.szxytkj.cn

[S19] C：快速排序
来源：http://zy.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hv.huanxung.cn

[S20] C：二分查找
来源：http://ng.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xa.newstarts.cn

[S21] C：字符类别判断
来源：http://gd.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hw.9csxet.cn

[S22] C：字符串转数字
来源：http://km.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ye.yuntaijiaju.cn

[S23] C：随机数
来源：http://ls.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tb.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://tn.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bn.521024.cn

[S25] C：内存拷贝
来源：http://yr.szxytkj.cn

memcpy(dst, src, n);
来源：http://tj.bookmarksfly.cn

[S26] C：内存清零
来源：http://pt.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://kv.szxytkj.cn

[S27] C：定义常量
来源：http://sz.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://ew.huixiangedu.cn

[S28] C：静态变量
来源：http://ak.hnjuh.cn

static int counter = 0;
来源：http://mw.huanxung.cn

[S29] C：变参函数
来源：http://oe.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vd.panjiajie.cn

[S30] C：头文件保护
来源：http://rm.9csxet.cn

#ifndef X_H
来源：http://iy.bjjhwx.cn

#define X_H
来源：http://qx.asd995.cn

#endif
来源：http://bs.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://ym.jianghongdianzi.cn

#include <iostream>
来源：http://jx.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://uj.huixiangedu.cn

[S32] C++：字符串
来源：http://yw.asd995.cn

std::string s = "hi";  s += "!";
来源：http://wf.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://ix.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uc.521024.cn

[S34] C++：遍历 vector
来源：http://at.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://ty.wgjwhj.cn

[S35] C++：map
来源：http://nk.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sn.huanxung.cn

[S36] C++：unordered_map
来源：http://ny.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ht.yuexingan06.cn

[S37] C++：set
来源：http://as.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yw.yuexingan06.cn

[S38] C++：排序
来源：http://qh.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://hf.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://co.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jn.hahajie.cn

[S40] C++：查找元素
来源：http://zu.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fu.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://sb.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rn.szsharing.cn

[S42] C++：继承与虚函数
来源：http://wj.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://vq.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://xs.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://xj.huanxung.cn

[S44] C++：引用传参
来源：http://lk.szsharing.cn

void inc(int &x) { ++x; }
来源：http://tc.bjjhwx.cn

[S45] C++：lambda
来源：http://fm.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gn.haigaiapp.cn

[S46] C++：函数模板
来源：http://pr.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lg.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://sk.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://av.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://xg.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://av.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://sa.hahajie.cn

[S49] C++：写文件
来源：http://ko.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hn.wgjwhj.cn

[S50] C++：格式化数字
来源：http://mv.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hm.asd995.cn

[S51] C++：显式类型转换
来源：http://uj.newstarts.cn

static_cast<double>(a) / b
来源：http://qt.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://qj.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://yb.bookmarksfly.cn

[S53] C++：移动语义
来源：http://cm.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://ur.colortex.cn

[S54] C++：异常处理
来源：http://xv.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wb.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://dt.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zn.bookmarksfly.cn

[S56] C++：optional
来源：http://ek.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://si.shxzukj.cn

[S57] C++：编译期常量
来源：http://yq.shxzskj.cn

constexpr int N = 10;
来源：http://sg.szsharing.cn

[S58] C++：命名空间
来源：http://cq.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://cb.gzmigu.cn

[S59] C++：静态断言
来源：http://be.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pv.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://nu.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qd.yuexingan06.cn

================================================================================
来源：http://xj.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ht.nszjky.cn

================================================================================
来源：http://wt.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://aq.jctech888.com.cn

println("Hello")
来源：http://tt.bjjhwx.cn

[T02] Kotlin：变量
来源：http://cs.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bg.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://bn.newstarts.cn

"值: $b"
来源：http://ei.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://gd.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://qt.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://bw.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zl.colortex.cn

[T06] Kotlin：集合映射
来源：http://vh.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xu.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://cc.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ul.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://iz.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://mo.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://gl.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://sg.asd995.cn

[T10] Kotlin：默认参数
来源：http://wz.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tg.huixiangedu.cn

[T11] Kotlin：协程
来源：http://ra.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nb.huanxung.cn

[T12] Kotlin：解构声明
来源：http://if.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://et.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://zw.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://wh.nicolike.cn

[T14] Kotlin：循环
来源：http://qg.shxzskj.cn

for (i in 1..10) println(i)
来源：http://uf.huixiangedu.cn

[T15] Kotlin：接口
来源：http://mt.nszjky.cn

interface Shape { fun area(): Double }
来源：http://mz.yuexingan06.cn

[T16] Swift：Hello World
来源：http://rs.szxytkj.cn

print("Hello")
来源：http://kf.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://zu.szsharing.cn

var a = 1;  let b = 2
来源：http://eq.gzmigu.cn

[T18] Swift：字符串插值
来源：http://je.bjjhwx.cn

"值: \(b)"
来源：http://ei.shxzskj.cn

[T19] Swift：可选绑定
来源：http://ey.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://jn.muxihuayi.cn

[T20] Swift：数组操作
来源：http://iz.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ll.bookmarksfly.cn

[T21] Swift：遍历
来源：http://gu.szxytkj.cn

for x in a { print(x) }
来源：http://fd.huanxung.cn

[T22] Swift：字典
来源：http://ai.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uj.colortex.cn

[T23] Swift：函数
来源：http://oo.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ux.nicolike.cn

[T24] Swift：闭包
来源：http://ii.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ds.shxzukj.cn

[T25] Swift：结构体
来源：http://ep.panjiajie.cn

struct P { var x: Int }
来源：http://mc.newstarts.cn

[T26] Swift：类与重写
来源：http://ma.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://dz.asd995.cn

[T27] Swift：错误处理
来源：http://kq.nszjky.cn

do { try f() } catch { print(error) }
来源：http://go.nszjky.cn

[T28] Swift：枚举
来源：http://je.lnxyls.cn

enum Color { case red, green }
来源：http://qt.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://ds.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://sb.colortex.cn

[T30] Swift：协议
来源：http://ea.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://jz.shtwfgs.cn

[T31] Lua：Hello World
来源：http://mc.hahajie.cn

print("Hello")
来源：http://dl.gzmigu.cn

[T32] Lua：局部变量
来源：http://xf.bookmarksfly.cn

local a = 1
来源：http://td.hahajie.cn

[T33] Lua：表（数组）
来源：http://ii.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wp.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://my.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://za.huixinmuqiang.cn


<!-- 参考信息 -->