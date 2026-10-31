代发 wailian999

echo "${#s}"
来源：http://ta.chemitech.net.cn

[R22] 截取子串
来源：http://bx.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://od.panjiajie.cn

[R23] 字符串替换
来源：http://nr.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iq.nszjky.cn

[R24] 大小写转换
来源：http://ex.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yo.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://ex.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wr.hnjuh.cn

[R26] 命令替换
来源：http://sz.haigaiapp.cn

now=$(date +%F); echo "$now"
来源：http://sc.lnxyls.cn

[R27] 算术展开
来源：http://sc.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://jx.szsharing.cn

[R28] 浮点运算
来源：http://mu.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://dd.nicolike.cn

[R29] 定义函数
来源：http://xk.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://en.jctech888.com.cn

[R30] 函数返回状态码
来源：http://vb.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://az.huanxung.cn

[R31] 局部变量
来源：http://uc.nszjky.cn

f() { local x=1; echo "$x"; }
来源：http://vw.huanxung.cn

[R32] 参数个数校验
来源：http://so.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ph.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://tv.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oj.shxzskj.cn

[R34] 退出时清理
来源：http://ba.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bn.chemitech.net.cn

[R35] 后台执行并等待
来源：http://tz.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qx.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://ed.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ms.asd995.cn

[R37] 把输出赋给变量
来源：http://sm.szxytkj.cn

files=$(ls -1)
来源：http://eq.lnxyls.cn

[R38] 管道串联
来源：http://ly.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://tr.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://ki.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://zy.panjiajie.cn

[R40] 追加写日志
来源：http://gc.hnjuh.cn

echo "log" >> out.log
来源：http://ga.gzmigu.cn

[R41] 丢弃输出
来源：http://cc.asd995.cn

cmd >/dev/null 2>&1
来源：http://rd.jctech888.com.cn

[R42] 输入重定向
来源：http://th.chemitech.net.cn

wc -l < a.txt
来源：http://nl.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://sa.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://ll.muxihuayi.cn

[R44] 按修改时间查找
来源：http://sa.shxzukj.cn

find . -mtime -7 -type f
来源：http://zd.asd995.cn

[R45] 批量删除
来源：http://in.huanxung.cn

find . -name "*.tmp" -delete
来源：http://ts.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://fq.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xp.muxihuayi.cn

[R47] sed 单行替换
来源：http://ih.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gp.nicolike.cn

[R48] awk 取指定列
来源：http://wz.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://oo.huixinmuqiang.cn

[R49] awk 带条件
来源：http://ny.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ub.chemitech.net.cn

[R50] awk 求和
来源：http://gc.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rj.521024.cn

[R51] 排序去重取前几
来源：http://rd.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ej.gzmigu.cn

[R52] 统计行数
来源：http://zs.nicolike.cn

wc -l a.txt
来源：http://he.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://vz.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zl.521024.cn

[R54] 比较两个文件
来源：http://df.bjjhwx.cn

diff a.txt b.txt
来源：http://nf.nszjky.cn

[R55] 压缩与解压
来源：http://ka.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kd.hnjuh.cn

[R56] 远程拷贝
来源：http://wn.asd995.cn

scp file user@host:/path/
来源：http://fo.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://rx.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://th.chemitech.net.cn

[R58] 下载文件
来源：http://kw.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ct.bjjhwx.cn

[R59] 发 POST JSON
来源：http://rz.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ci.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://ks.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vg.nicolike.cn

[R61] 磁盘占用
来源：http://jb.muxihuayi.cn

df -h;  du -sh *
来源：http://lv.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://cp.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://qf.yuntaijiaju.cn

[R63] 内存与进程
来源：http://jc.colortex.cn

free -h;  ps aux | grep nginx
来源：http://ia.nszjky.cn

[R64] 结束进程
来源：http://qi.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://gr.yuexingan06.cn

[R65] 查看端口占用
来源：http://nb.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vs.bookmarksfly.cn

[R66] 定时任务
来源：http://ev.haigaiapp.cn

crontab -e;  crontab -l
来源：http://ed.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://dp.huanxung.cn

openssl rand -hex 16
来源：http://su.nszjky.cn

[R68] 计算文件校验值
来源：http://gz.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yf.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://em.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://dx.nicolike.cn

[R70] 时间戳与互转
来源：http://xl.521024.cn

date +%s;  date -d @1700000000
来源：http://zd.asd995.cn

[R71] 日期格式化
来源：http://fw.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gl.haigaiapp.cn

[R72] 等待端口就绪
来源：http://au.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pq.bjjhwx.cn

[R73] 分割大日志
来源：http://ik.wgjwhj.cn

split -l 1000 big.log part_
来源：http://oa.bjjhwx.cn

[R74] 批量重命名
来源：http://jj.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fx.lnxyls.cn

[R75] 导出环境变量
来源：http://sv.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://eo.shxzukj.cn

[R76] 使用临时文件
来源：http://as.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wv.muxihuayi.cn

[R77] 读取用户输入
来源：http://lp.bjjhwx.cn

read -rp "请输入: " ans
来源：http://wf.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://ah.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rp.haigaiapp.cn

[R79] 解析命令行选项
来源：http://ck.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sf.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://ce.521024.cn

time ./run.sh
来源：http://hb.nicolike.cn

================================================================================
来源：http://hw.newstarts.cn

S. C / C++ 专题
来源：http://ni.wgjwhj.cn

================================================================================
来源：http://ii.huanxung.cn

[S01] C：Hello World
来源：http://oh.szsharing.cn

#include <stdio.h>
来源：http://mi.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://so.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://hf.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://jv.lnxyls.cn

[S03] C：读入整数
来源：http://tz.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://nj.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://zl.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vw.jctech888.com.cn

[S05] C：字符串长度
来源：http://vg.521024.cn

strlen(s)
来源：http://ns.bookmarksfly.cn

[S06] C：字符串比较
来源：http://du.shxzukj.cn

strcmp(a, b) == 0
来源：http://zo.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://mb.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://am.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://gn.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cu.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://ve.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://os.wgjwhj.cn

[S10] C：指针与解引用
来源：http://gj.newstarts.cn

int *p = &a;  *p = 5;
来源：http://vl.hahajie.cn

[S11] C：逐行读文件
来源：http://zo.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://eu.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ph.bookmarksfly.cn

fclose(f);
来源：http://us.lnxyls.cn

[S12] C：写文件
来源：http://hn.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oa.hahajie.cn

[S13] C：宏定义
来源：http://vr.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tp.szsharing.cn

[S14] C：枚举
来源：http://vc.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://xc.9csxet.cn

[S15] C：类型转换
来源：http://lz.jianghongdianzi.cn

(double) a / b
来源：http://xv.nszjky.cn

[S16] C：位操作置位
来源：http://se.huanxung.cn

x |= (1 << 3);
来源：http://qx.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://ln.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sp.huixiangedu.cn

[S18] C：命令行参数
来源：http://jt.haigaiapp.cn

int main(int argc, char **argv)
来源：http://kd.bookmarksfly.cn

[S19] C：快速排序
来源：http://do.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yw.yuexingan06.cn

[S20] C：二分查找
来源：http://vi.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eq.bjjhwx.cn

[S21] C：字符类别判断
来源：http://ii.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vg.chemitech.net.cn

[S22] C：字符串转数字
来源：http://of.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ol.hnjuh.cn

[S23] C：随机数
来源：http://dj.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ep.huixiangedu.cn

[S24] C：获取本地时间
来源：http://rw.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vw.szsharing.cn

[S25] C：内存拷贝
来源：http://ai.shxzskj.cn

memcpy(dst, src, n);
来源：http://ec.yuexingan06.cn

[S26] C：内存清零
来源：http://iq.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://oc.gzmigu.cn

[S27] C：定义常量
来源：http://oq.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://lr.chemitech.net.cn

[S28] C：静态变量
来源：http://bz.muxihuayi.cn

static int counter = 0;
来源：http://uz.panjiajie.cn

[S29] C：变参函数
来源：http://ql.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mv.szxytkj.cn

[S30] C：头文件保护
来源：http://fk.jctech888.com.cn

#ifndef X_H
来源：http://lh.bookmarksfly.cn

#define X_H
来源：http://iv.newstarts.cn

#endif
来源：http://ot.panjiajie.cn

[S31] C++：Hello World
来源：http://wm.chemitech.net.cn

#include <iostream>
来源：http://xe.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://vg.huanxung.cn

[S32] C++：字符串
来源：http://ng.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://el.521024.cn

[S33] C++：vector 增删
来源：http://lo.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cg.szsharing.cn

[S34] C++：遍历 vector
来源：http://hd.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://xe.huanxung.cn

[S35] C++：map
来源：http://xs.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yy.chemitech.net.cn

[S36] C++：unordered_map
来源：http://yj.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eq.wgjwhj.cn

[S37] C++：set
来源：http://fe.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rw.hnjuh.cn

[S38] C++：排序
来源：http://oa.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://yh.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://vt.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ja.colortex.cn

[S40] C++：查找元素
来源：http://ji.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dt.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://zm.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.szsharing.cn

[S42] C++：继承与虚函数
来源：http://nx.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://lu.hnjuh.cn

[S43] C++：智能指针
来源：http://go.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://vn.szsharing.cn

[S44] C++：引用传参
来源：http://ni.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://uq.szsharing.cn

[S45] C++：lambda
来源：http://zx.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tf.haigaiapp.cn

[S46] C++：函数模板
来源：http://wz.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sw.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://in.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://db.shxzukj.cn

[S48] C++：逐行读文件
来源：http://se.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dx.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://kk.yuexingan06.cn

[S49] C++：写文件
来源：http://eu.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qc.shxzskj.cn

[S50] C++：格式化数字
来源：http://yj.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xs.shxzskj.cn

[S51] C++：显式类型转换
来源：http://xl.521024.cn

static_cast<double>(a) / b
来源：http://he.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://wu.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://ch.9csxet.cn

[S53] C++：移动语义
来源：http://mv.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://bf.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://ao.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ck.hahajie.cn

[S55] C++：结构化绑定
来源：http://tp.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ti.haigaiapp.cn

[S56] C++：optional
来源：http://ip.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jv.newstarts.cn

[S57] C++：编译期常量
来源：http://ny.shtwfgs.cn

constexpr int N = 10;
来源：http://ql.gzmigu.cn

[S58] C++：命名空间
来源：http://lp.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://ce.gzmigu.cn

[S59] C++：静态断言
来源：http://vf.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qt.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://wy.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ko.jctech888.com.cn

================================================================================
来源：http://nn.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xm.bookmarksfly.cn

================================================================================
来源：http://xe.colortex.cn

[T01] Kotlin：Hello World
来源：http://fe.jctech888.com.cn

println("Hello")
来源：http://eg.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://wo.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kw.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://ik.haigaiapp.cn

"值: $b"
来源：http://gu.nicolike.cn

[T04] Kotlin：空安全
来源：http://it.nicolike.cn

val n: String? = null;  n?.length
来源：http://hf.colortex.cn

[T05] Kotlin：when 表达式
来源：http://qs.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uo.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://lh.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jq.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://bg.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fq.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://cx.asd995.cn

data class User(val name: String, val age: Int)
来源：http://pq.colortex.cn

[T09] Kotlin：扩展函数
来源：http://ml.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://ui.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://xa.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lf.panjiajie.cn

[T11] Kotlin：协程
来源：http://ri.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mo.521024.cn

[T12] Kotlin：解构声明
来源：http://xo.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://ne.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://mb.colortex.cn

val m = mapOf("a" to 1)
来源：http://bs.lnxyls.cn

[T14] Kotlin：循环
来源：http://nn.colortex.cn

for (i in 1..10) println(i)
来源：http://yc.szsharing.cn

[T15] Kotlin：接口
来源：http://tg.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://kt.yuexingan06.cn

[T16] Swift：Hello World
来源：http://is.wgjwhj.cn

print("Hello")
来源：http://al.szsharing.cn

[T17] Swift：变量与常量
来源：http://vs.nicolike.cn

var a = 1;  let b = 2
来源：http://mb.szxytkj.cn

[T18] Swift：字符串插值
来源：http://fk.panjiajie.cn

"值: \(b)"
来源：http://lm.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://ru.nszjky.cn

if let n = opt { print(n) }
来源：http://ub.bjjhwx.cn

[T20] Swift：数组操作
来源：http://pr.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gi.jctech888.com.cn

[T21] Swift：遍历
来源：http://yy.huixiangedu.cn

for x in a { print(x) }
来源：http://az.panjiajie.cn

[T22] Swift：字典
来源：http://qp.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gb.chemitech.net.cn

[T23] Swift：函数
来源：http://eg.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hj.shxzskj.cn

[T24] Swift：闭包
来源：http://ly.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ig.shxzukj.cn


<!-- 参考信息 -->