代发 wailian999

echo $((1 + 2 * 3))
来源：http://wt.9csxet.cn

[R28] 浮点运算
来源：http://xg.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://jn.shxzukj.cn

[R29] 定义函数
来源：http://ly.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yq.shxzskj.cn

[R30] 函数返回状态码
来源：http://dt.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://ie.bjjhwx.cn

[R31] 局部变量
来源：http://ye.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://hw.yuexingan06.cn

[R32] 参数个数校验
来源：http://mc.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dk.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://pl.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qy.chemitech.net.cn

[R34] 退出时清理
来源：http://ox.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tt.szsharing.cn

[R35] 后台执行并等待
来源：http://zo.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qu.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://oi.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wm.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://tl.asd995.cn

files=$(ls -1)
来源：http://ok.521024.cn

[R38] 管道串联
来源：http://sv.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://hl.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://dz.nicolike.cn

cmd > out.log 2>&1
来源：http://ej.szxytkj.cn

[R40] 追加写日志
来源：http://nv.9csxet.cn

echo "log" >> out.log
来源：http://fc.huanxung.cn

[R41] 丢弃输出
来源：http://cm.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://gt.hahajie.cn

[R42] 输入重定向
来源：http://uh.newstarts.cn

wc -l < a.txt
来源：http://rt.shxzukj.cn

[R43] 按名字查找文件
来源：http://ti.asd995.cn

find . -name "*.log" -type f
来源：http://ox.wgjwhj.cn

[R44] 按修改时间查找
来源：http://go.szxytkj.cn

find . -mtime -7 -type f
来源：http://ik.yuntaijiaju.cn

[R45] 批量删除
来源：http://rm.nicolike.cn

find . -name "*.tmp" -delete
来源：http://qc.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://nq.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rp.panjiajie.cn

[R47] sed 单行替换
来源：http://bb.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vb.wgjwhj.cn

[R48] awk 取指定列
来源：http://mr.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://ch.chemitech.net.cn

[R49] awk 带条件
来源：http://ty.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://js.521024.cn

[R50] awk 求和
来源：http://nf.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kn.hnjuh.cn

[R51] 排序去重取前几
来源：http://yu.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pw.huanxung.cn

[R52] 统计行数
来源：http://rz.wgjwhj.cn

wc -l a.txt
来源：http://aj.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://aa.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lt.shxzukj.cn

[R54] 比较两个文件
来源：http://pf.panjiajie.cn

diff a.txt b.txt
来源：http://bc.wgjwhj.cn

[R55] 压缩与解压
来源：http://zk.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bb.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://wf.bookmarksfly.cn

scp file user@host:/path/
来源：http://dk.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://zl.panjiajie.cn

ssh user@host 'uptime'
来源：http://yk.wgjwhj.cn

[R58] 下载文件
来源：http://yu.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eg.colortex.cn

[R59] 发 POST JSON
来源：http://di.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gh.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://ci.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://od.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://zk.nicolike.cn

df -h;  du -sh *
来源：http://sq.shxzukj.cn

[R62] 找最占空间的文件
来源：http://fc.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://uk.nicolike.cn

[R63] 内存与进程
来源：http://yx.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://xl.hnjuh.cn

[R64] 结束进程
来源：http://yh.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://tm.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://bw.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vp.huixinmuqiang.cn

[R66] 定时任务
来源：http://ej.huixiangedu.cn

crontab -e;  crontab -l
来源：http://er.asd995.cn

[R67] 生成随机十六进制串
来源：http://if.shxzukj.cn

openssl rand -hex 16
来源：http://fg.shxzskj.cn

[R68] 计算文件校验值
来源：http://hs.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nt.huixiangedu.cn

[R69] 生成随机密码
来源：http://ul.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://nb.hnjuh.cn

[R70] 时间戳与互转
来源：http://ow.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://yg.chemitech.net.cn

[R71] 日期格式化
来源：http://ww.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jw.9csxet.cn

[R72] 等待端口就绪
来源：http://eh.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sb.newstarts.cn

[R73] 分割大日志
来源：http://bk.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://cv.521024.cn

[R74] 批量重命名
来源：http://pz.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ur.haigaiapp.cn

[R75] 导出环境变量
来源：http://yz.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://xr.szxytkj.cn

[R76] 使用临时文件
来源：http://co.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uj.colortex.cn

[R77] 读取用户输入
来源：http://qj.hahajie.cn

read -rp "请输入: " ans
来源：http://zn.huanxung.cn

[R78] 交互式菜单
来源：http://me.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fq.panjiajie.cn

[R79] 解析命令行选项
来源：http://ki.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ef.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://od.muxihuayi.cn

time ./run.sh
来源：http://rd.gzmigu.cn

================================================================================
来源：http://mr.huanxung.cn

S. C / C++ 专题
来源：http://yf.asd995.cn

================================================================================
来源：http://wh.bookmarksfly.cn

[S01] C：Hello World
来源：http://wm.jctech888.com.cn

#include <stdio.h>
来源：http://gn.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ml.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://mv.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://te.nicolike.cn

[S03] C：读入整数
来源：http://su.gzmigu.cn

int x; scanf("%d", &x);
来源：http://wj.huixiangedu.cn

[S04] C：字符串复制
来源：http://eo.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lm.nszjky.cn

[S05] C：字符串长度
来源：http://hh.nszjky.cn

strlen(s)
来源：http://ts.asd995.cn

[S06] C：字符串比较
来源：http://gl.newstarts.cn

strcmp(a, b) == 0
来源：http://xy.521024.cn

[S07] C：数组遍历求和
来源：http://ce.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dd.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://zi.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cl.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://ak.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vi.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://ea.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://ob.gzmigu.cn

[S11] C：逐行读文件
来源：http://qy.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://mv.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ks.gzmigu.cn

fclose(f);
来源：http://pq.shtwfgs.cn

[S12] C：写文件
来源：http://xq.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rr.asd995.cn

[S13] C：宏定义
来源：http://pi.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vr.muxihuayi.cn

[S14] C：枚举
来源：http://we.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ge.nszjky.cn

[S15] C：类型转换
来源：http://af.521024.cn

(double) a / b
来源：http://fc.bookmarksfly.cn

[S16] C：位操作置位
来源：http://sz.nicolike.cn

x |= (1 << 3);
来源：http://mb.asd995.cn

[S17] C：安全拼接字符串
来源：http://gj.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xg.huixiangedu.cn

[S18] C：命令行参数
来源：http://ok.newstarts.cn

int main(int argc, char **argv)
来源：http://qg.bookmarksfly.cn

[S19] C：快速排序
来源：http://zj.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bn.9csxet.cn

[S20] C：二分查找
来源：http://jn.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ra.shxzukj.cn

[S21] C：字符类别判断
来源：http://tw.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://la.szxytkj.cn

[S22] C：字符串转数字
来源：http://pa.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://py.huixinmuqiang.cn

[S23] C：随机数
来源：http://of.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qa.hahajie.cn

[S24] C：获取本地时间
来源：http://qa.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jb.colortex.cn

[S25] C：内存拷贝
来源：http://yz.szxytkj.cn

memcpy(dst, src, n);
来源：http://yb.newstarts.cn

[S26] C：内存清零
来源：http://ei.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://rm.muxihuayi.cn

[S27] C：定义常量
来源：http://ef.szxytkj.cn

const double PI = 3.14159;
来源：http://st.shxzskj.cn

[S28] C：静态变量
来源：http://au.hahajie.cn

static int counter = 0;
来源：http://iz.hahajie.cn

[S29] C：变参函数
来源：http://pg.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://je.szsharing.cn

[S30] C：头文件保护
来源：http://mj.wgjwhj.cn

#ifndef X_H
来源：http://mb.9csxet.cn

#define X_H
来源：http://jc.jctech888.com.cn

#endif
来源：http://mm.nszjky.cn

[S31] C++：Hello World
来源：http://jb.panjiajie.cn

#include <iostream>
来源：http://xw.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://ss.jctech888.com.cn

[S32] C++：字符串
来源：http://dp.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://lj.chemitech.net.cn

[S33] C++：vector 增删
来源：http://uc.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zw.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://el.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://rd.nicolike.cn

[S35] C++：map
来源：http://yr.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ul.521024.cn

[S36] C++：unordered_map
来源：http://bs.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ek.yuexingan06.cn

[S37] C++：set
来源：http://ik.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ht.lnxyls.cn

[S38] C++：排序
来源：http://mi.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://po.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://vl.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ez.wgjwhj.cn

[S40] C++：查找元素
来源：http://ek.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zi.521024.cn

[S41] C++：类与构造函数
来源：http://tc.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rj.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://lt.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://qz.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://nx.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://qm.hahajie.cn

[S44] C++：引用传参
来源：http://uu.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://xv.521024.cn

[S45] C++：lambda
来源：http://gb.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oz.huixiangedu.cn

[S46] C++：函数模板
来源：http://cc.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ag.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://cz.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yu.9csxet.cn

[S48] C++：逐行读文件
来源：http://qu.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mz.newstarts.cn

while (std::getline(in, line)) { }
来源：http://zy.nicolike.cn

[S49] C++：写文件
来源：http://yl.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hi.gzmigu.cn

[S50] C++：格式化数字
来源：http://fp.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lo.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://mq.wgjwhj.cn

static_cast<double>(a) / b
来源：http://di.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://qj.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://hz.shxzskj.cn

[S53] C++：移动语义
来源：http://ne.521024.cn

std::vector<int> w = std::move(v);
来源：http://zx.colortex.cn

[S54] C++：异常处理
来源：http://be.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tg.9csxet.cn

[S55] C++：结构化绑定
来源：http://no.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fi.szsharing.cn

[S56] C++：optional
来源：http://tf.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mg.wgjwhj.cn

[S57] C++：编译期常量
来源：http://sl.jianghongdianzi.cn

constexpr int N = 10;
来源：http://qs.haigaiapp.cn

[S58] C++：命名空间
来源：http://ww.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://jh.nicolike.cn

[S59] C++：静态断言
来源：http://cs.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ph.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://mm.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gn.szsharing.cn

================================================================================
来源：http://cf.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iw.bjjhwx.cn

================================================================================
来源：http://nx.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://ho.yuexingan06.cn

println("Hello")
来源：http://bi.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://xm.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jq.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://pu.wgjwhj.cn

"值: $b"
来源：http://lm.shxzskj.cn

[T04] Kotlin：空安全
来源：http://kc.newstarts.cn

val n: String? = null;  n?.length
来源：http://gz.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://jt.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gm.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://ef.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tm.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://ik.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gg.521024.cn

[T08] Kotlin：数据类
来源：http://zs.521024.cn

data class User(val name: String, val age: Int)
来源：http://ad.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://ai.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://oa.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://hr.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jy.shtwfgs.cn

[T11] Kotlin：协程
来源：http://jg.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yx.newstarts.cn

[T12] Kotlin：解构声明
来源：http://jg.521024.cn

val (a, b) = Pair(1, 2)
来源：http://zg.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://ml.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://ia.9csxet.cn

[T14] Kotlin：循环
来源：http://uv.9csxet.cn

for (i in 1..10) println(i)
来源：http://mu.hahajie.cn

[T15] Kotlin：接口
来源：http://ib.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://tx.panjiajie.cn

[T16] Swift：Hello World
来源：http://ix.shxzukj.cn

print("Hello")
来源：http://yu.521024.cn

[T17] Swift：变量与常量
来源：http://dx.jctech888.com.cn

var a = 1;  let b = 2
来源：http://uz.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://mo.chemitech.net.cn

"值: \(b)"
来源：http://qb.shxzskj.cn

[T19] Swift：可选绑定
来源：http://lp.haigaiapp.cn

if let n = opt { print(n) }
来源：http://is.bjjhwx.cn

[T20] Swift：数组操作
来源：http://jb.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ra.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://we.szsharing.cn

for x in a { print(x) }
来源：http://ru.shxzukj.cn

[T22] Swift：字典
来源：http://mo.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lq.huixinmuqiang.cn

[T23] Swift：函数
来源：http://hs.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wj.asd995.cn

[T24] Swift：闭包
来源：http://ss.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ez.wgjwhj.cn

[T25] Swift：结构体
来源：http://hb.yuntaijiaju.cn

struct P { var x: Int }
来源：http://ep.shxzukj.cn

[T26] Swift：类与重写
来源：http://pr.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://op.panjiajie.cn

[T27] Swift：错误处理
来源：http://sv.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://nr.huixiangedu.cn

[T28] Swift：枚举
来源：http://um.nszjky.cn

enum Color { case red, green }
来源：http://rp.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://ij.muxihuayi.cn

guard let x = opt else { return }
来源：http://rl.newstarts.cn

[T30] Swift：协议
来源：http://tv.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://ud.jctech888.com.cn


<!-- 参考信息 -->