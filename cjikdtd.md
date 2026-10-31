代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://xf.chemitech.net.cn

[R26] 命令替换
来源：http://ih.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://kd.nszjky.cn

[R27] 算术展开
来源：http://sj.nicolike.cn

echo $((1 + 2 * 3))
来源：http://ts.chemitech.net.cn

[R28] 浮点运算
来源：http://qe.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://op.huanxung.cn

[R29] 定义函数
来源：http://la.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rg.hnjuh.cn

[R30] 函数返回状态码
来源：http://ne.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://tf.newstarts.cn

[R31] 局部变量
来源：http://pb.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://po.yuexingan06.cn

[R32] 参数个数校验
来源：http://oq.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uo.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://sz.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://la.haigaiapp.cn

[R34] 退出时清理
来源：http://rp.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lw.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://ns.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pf.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://zx.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ey.asd995.cn

[R37] 把输出赋给变量
来源：http://sa.yuntaijiaju.cn

files=$(ls -1)
来源：http://nm.wgjwhj.cn

[R38] 管道串联
来源：http://id.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://hg.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://ln.panjiajie.cn

cmd > out.log 2>&1
来源：http://zm.szxytkj.cn

[R40] 追加写日志
来源：http://ga.nicolike.cn

echo "log" >> out.log
来源：http://wo.hahajie.cn

[R41] 丢弃输出
来源：http://ev.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://si.chemitech.net.cn

[R42] 输入重定向
来源：http://va.gzmigu.cn

wc -l < a.txt
来源：http://pw.haigaiapp.cn

[R43] 按名字查找文件
来源：http://zo.hnjuh.cn

find . -name "*.log" -type f
来源：http://xr.chemitech.net.cn

[R44] 按修改时间查找
来源：http://wo.szxytkj.cn

find . -mtime -7 -type f
来源：http://ll.yuexingan06.cn

[R45] 批量删除
来源：http://rj.521024.cn

find . -name "*.tmp" -delete
来源：http://vw.newstarts.cn

[R46] 递归替换文件内容
来源：http://iu.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ck.yuexingan06.cn

[R47] sed 单行替换
来源：http://ih.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gb.shxzskj.cn

[R48] awk 取指定列
来源：http://sp.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://eb.jianghongdianzi.cn

[R49] awk 带条件
来源：http://mo.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jh.panjiajie.cn

[R50] awk 求和
来源：http://ll.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zm.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://sd.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kh.haigaiapp.cn

[R52] 统计行数
来源：http://ms.nicolike.cn

wc -l a.txt
来源：http://qn.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://xw.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fv.hnjuh.cn

[R54] 比较两个文件
来源：http://zh.shtwfgs.cn

diff a.txt b.txt
来源：http://zi.9csxet.cn

[R55] 压缩与解压
来源：http://mu.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gf.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://zm.521024.cn

scp file user@host:/path/
来源：http://ol.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://ry.szxytkj.cn

ssh user@host 'uptime'
来源：http://dj.nicolike.cn

[R58] 下载文件
来源：http://sk.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://od.muxihuayi.cn

[R59] 发 POST JSON
来源：http://hh.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yq.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://pf.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gq.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://sm.huanxung.cn

df -h;  du -sh *
来源：http://pn.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://bv.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://kq.bjjhwx.cn

[R63] 内存与进程
来源：http://os.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://lu.szsharing.cn

[R64] 结束进程
来源：http://ru.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://xm.wgjwhj.cn

[R65] 查看端口占用
来源：http://cc.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dy.huixinmuqiang.cn

[R66] 定时任务
来源：http://ld.szxytkj.cn

crontab -e;  crontab -l
来源：http://ne.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://gt.colortex.cn

openssl rand -hex 16
来源：http://xl.nicolike.cn

[R68] 计算文件校验值
来源：http://vz.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xw.szxytkj.cn

[R69] 生成随机密码
来源：http://ah.521024.cn

head -c 16 /dev/urandom | base64
来源：http://mz.shtwfgs.cn

[R70] 时间戳与互转
来源：http://ui.hahajie.cn

date +%s;  date -d @1700000000
来源：http://fx.huixinmuqiang.cn

[R71] 日期格式化
来源：http://up.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ma.9csxet.cn

[R72] 等待端口就绪
来源：http://lz.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qc.haigaiapp.cn

[R73] 分割大日志
来源：http://lz.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://ee.jctech888.com.cn

[R74] 批量重命名
来源：http://wc.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://od.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://fw.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://ma.asd995.cn

[R76] 使用临时文件
来源：http://xz.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ci.wgjwhj.cn

[R77] 读取用户输入
来源：http://sf.521024.cn

read -rp "请输入: " ans
来源：http://nm.nicolike.cn

[R78] 交互式菜单
来源：http://fi.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dd.newstarts.cn

[R79] 解析命令行选项
来源：http://eh.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ql.asd995.cn

[R80] 查看脚本执行耗时
来源：http://kv.bjjhwx.cn

time ./run.sh
来源：http://gp.nszjky.cn

================================================================================
来源：http://ln.yuntaijiaju.cn

S. C / C++ 专题
来源：http://by.huixiangedu.cn

================================================================================
来源：http://cq.lnxyls.cn

[S01] C：Hello World
来源：http://li.shxzskj.cn

#include <stdio.h>
来源：http://hq.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xp.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://ao.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://tx.huanxung.cn

[S03] C：读入整数
来源：http://iv.gzmigu.cn

int x; scanf("%d", &x);
来源：http://fk.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://wq.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ig.nszjky.cn

[S05] C：字符串长度
来源：http://kc.bjjhwx.cn

strlen(s)
来源：http://ai.wgjwhj.cn

[S06] C：字符串比较
来源：http://vs.colortex.cn

strcmp(a, b) == 0
来源：http://qv.nicolike.cn

[S07] C：数组遍历求和
来源：http://qx.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sx.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://jk.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tg.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://hk.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ud.szxytkj.cn

[S10] C：指针与解引用
来源：http://df.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://nl.521024.cn

[S11] C：逐行读文件
来源：http://fq.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://mc.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oo.asd995.cn

fclose(f);
来源：http://tf.bookmarksfly.cn

[S12] C：写文件
来源：http://lr.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hu.panjiajie.cn

[S13] C：宏定义
来源：http://bx.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jc.jianghongdianzi.cn

[S14] C：枚举
来源：http://sc.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://eu.newstarts.cn

[S15] C：类型转换
来源：http://yb.jianghongdianzi.cn

(double) a / b
来源：http://lq.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://fg.gzmigu.cn

x |= (1 << 3);
来源：http://tm.9csxet.cn

[S17] C：安全拼接字符串
来源：http://mp.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ns.gzmigu.cn

[S18] C：命令行参数
来源：http://xc.nicolike.cn

int main(int argc, char **argv)
来源：http://xg.szsharing.cn

[S19] C：快速排序
来源：http://oy.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sc.521024.cn

[S20] C：二分查找
来源：http://sa.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sw.jctech888.com.cn

[S21] C：字符类别判断
来源：http://mj.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lh.shxzskj.cn

[S22] C：字符串转数字
来源：http://jv.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cu.panjiajie.cn

[S23] C：随机数
来源：http://ku.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ct.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://hf.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rk.huanxung.cn

[S25] C：内存拷贝
来源：http://iu.jctech888.com.cn

memcpy(dst, src, n);
来源：http://ou.asd995.cn

[S26] C：内存清零
来源：http://fs.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://zh.9csxet.cn

[S27] C：定义常量
来源：http://gp.newstarts.cn

const double PI = 3.14159;
来源：http://xs.jianghongdianzi.cn

[S28] C：静态变量
来源：http://ul.huanxung.cn

static int counter = 0;
来源：http://qe.yuexingan06.cn

[S29] C：变参函数
来源：http://sg.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vw.newstarts.cn

[S30] C：头文件保护
来源：http://ri.shxzukj.cn

#ifndef X_H
来源：http://fr.yuntaijiaju.cn

#define X_H
来源：http://oj.hahajie.cn

#endif
来源：http://rl.shxzskj.cn

[S31] C++：Hello World
来源：http://zv.521024.cn

#include <iostream>
来源：http://pl.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://ez.asd995.cn

[S32] C++：字符串
来源：http://zl.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://zv.colortex.cn

[S33] C++：vector 增删
来源：http://ca.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tn.szxytkj.cn

[S34] C++：遍历 vector
来源：http://mr.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://iw.newstarts.cn

[S35] C++：map
来源：http://hy.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ub.newstarts.cn

[S36] C++：unordered_map
来源：http://zn.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lh.asd995.cn

[S37] C++：set
来源：http://by.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gz.hahajie.cn

[S38] C++：排序
来源：http://gq.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://no.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://js.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qs.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://ck.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hi.shxzskj.cn

[S41] C++：类与构造函数
来源：http://if.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sc.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://xs.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://nl.hnjuh.cn

[S43] C++：智能指针
来源：http://nj.521024.cn

auto p = std::make_unique<int>(5);
来源：http://vd.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://fk.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://dj.newstarts.cn

[S45] C++：lambda
来源：http://gs.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xv.nicolike.cn

[S46] C++：函数模板
来源：http://gi.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eu.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://de.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ho.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://cl.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pm.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://ba.muxihuayi.cn

[S49] C++：写文件
来源：http://ol.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zv.newstarts.cn

[S50] C++：格式化数字
来源：http://mb.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gp.nszjky.cn

[S51] C++：显式类型转换
来源：http://pd.wgjwhj.cn

static_cast<double>(a) / b
来源：http://xz.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://gv.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://yl.huixiangedu.cn

[S53] C++：移动语义
来源：http://ww.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://we.nszjky.cn

[S54] C++：异常处理
来源：http://pk.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yj.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://za.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dl.lnxyls.cn

[S56] C++：optional
来源：http://tf.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cf.colortex.cn

[S57] C++：编译期常量
来源：http://ek.shxzukj.cn

constexpr int N = 10;
来源：http://hv.9csxet.cn

[S58] C++：命名空间
来源：http://lh.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://lo.lnxyls.cn

[S59] C++：静态断言
来源：http://sc.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ab.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://hb.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vi.wgjwhj.cn

================================================================================
来源：http://ta.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sy.wgjwhj.cn

================================================================================
来源：http://cb.szsharing.cn

[T01] Kotlin：Hello World
来源：http://ss.asd995.cn

println("Hello")
来源：http://qv.jctech888.com.cn

[T02] Kotlin：变量
来源：http://cf.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ni.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://zr.huanxung.cn

"值: $b"
来源：http://jw.asd995.cn

[T04] Kotlin：空安全
来源：http://dx.hnjuh.cn

val n: String? = null;  n?.length
来源：http://ug.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://vi.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uu.colortex.cn

[T06] Kotlin：集合映射
来源：http://lo.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rg.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://ot.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://px.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://os.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://bu.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://ze.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://jr.nszjky.cn

[T10] Kotlin：默认参数
来源：http://mv.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rc.hnjuh.cn

[T11] Kotlin：协程
来源：http://cb.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fh.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://ts.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://sz.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://jz.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://uo.szxytkj.cn

[T14] Kotlin：循环
来源：http://cg.shxzskj.cn

for (i in 1..10) println(i)
来源：http://ae.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://ya.521024.cn

interface Shape { fun area(): Double }
来源：http://vr.panjiajie.cn

[T16] Swift：Hello World
来源：http://cn.wgjwhj.cn

print("Hello")
来源：http://oe.shxzskj.cn

[T17] Swift：变量与常量
来源：http://as.bjjhwx.cn

var a = 1;  let b = 2
来源：http://yj.newstarts.cn

[T18] Swift：字符串插值
来源：http://vw.nszjky.cn

"值: \(b)"
来源：http://xh.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://rb.szsharing.cn

if let n = opt { print(n) }
来源：http://qe.haigaiapp.cn

[T20] Swift：数组操作
来源：http://ux.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dk.lnxyls.cn

[T21] Swift：遍历
来源：http://ft.521024.cn

for x in a { print(x) }
来源：http://nr.shxzskj.cn

[T22] Swift：字典
来源：http://gg.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ny.shxzskj.cn

[T23] Swift：函数
来源：http://qt.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://re.lnxyls.cn

[T24] Swift：闭包
来源：http://bz.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nh.shtwfgs.cn

[T25] Swift：结构体
来源：http://ns.muxihuayi.cn

struct P { var x: Int }
来源：http://rt.shxzskj.cn

[T26] Swift：类与重写
来源：http://kc.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://ea.jctech888.com.cn

[T27] Swift：错误处理
来源：http://jz.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://fe.colortex.cn

[T28] Swift：枚举
来源：http://ml.521024.cn

enum Color { case red, green }
来源：http://wf.nicolike.cn


<!-- 参考信息 -->