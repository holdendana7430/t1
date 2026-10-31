代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://vv.bookmarksfly.cn

[R26] 命令替换
来源：http://dx.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://yu.huixinmuqiang.cn

[R27] 算术展开
来源：http://yg.szsharing.cn

echo $((1 + 2 * 3))
来源：http://um.hnjuh.cn

[R28] 浮点运算
来源：http://yc.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://sn.colortex.cn

[R29] 定义函数
来源：http://zi.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ay.haigaiapp.cn

[R30] 函数返回状态码
来源：http://ek.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://on.shtwfgs.cn

[R31] 局部变量
来源：http://hz.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://kq.asd995.cn

[R32] 参数个数校验
来源：http://tz.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rm.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://xh.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fq.chemitech.net.cn

[R34] 退出时清理
来源：http://ik.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jl.chemitech.net.cn

[R35] 后台执行并等待
来源：http://bb.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lq.shxzukj.cn

[R36] 并发执行多个任务
来源：http://jz.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ea.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://py.521024.cn

files=$(ls -1)
来源：http://hg.chemitech.net.cn

[R38] 管道串联
来源：http://fb.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://wz.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://qy.huanxung.cn

cmd > out.log 2>&1
来源：http://lr.9csxet.cn

[R40] 追加写日志
来源：http://gp.521024.cn

echo "log" >> out.log
来源：http://qd.nszjky.cn

[R41] 丢弃输出
来源：http://kv.9csxet.cn

cmd >/dev/null 2>&1
来源：http://pm.huixinmuqiang.cn

[R42] 输入重定向
来源：http://tb.colortex.cn

wc -l < a.txt
来源：http://mf.muxihuayi.cn

[R43] 按名字查找文件
来源：http://ks.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://ux.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://en.hahajie.cn

find . -mtime -7 -type f
来源：http://lh.wgjwhj.cn

[R45] 批量删除
来源：http://ar.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://pl.colortex.cn

[R46] 递归替换文件内容
来源：http://tf.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ed.yuexingan06.cn

[R47] sed 单行替换
来源：http://ad.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ej.huanxung.cn

[R48] awk 取指定列
来源：http://tl.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://oq.nicolike.cn

[R49] awk 带条件
来源：http://dg.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ln.bjjhwx.cn

[R50] awk 求和
来源：http://fx.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dn.hnjuh.cn

[R51] 排序去重取前几
来源：http://ly.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dw.bookmarksfly.cn

[R52] 统计行数
来源：http://vx.nszjky.cn

wc -l a.txt
来源：http://jr.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://fr.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://of.muxihuayi.cn

[R54] 比较两个文件
来源：http://wq.wgjwhj.cn

diff a.txt b.txt
来源：http://up.muxihuayi.cn

[R55] 压缩与解压
来源：http://me.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dr.gzmigu.cn

[R56] 远程拷贝
来源：http://pa.szxytkj.cn

scp file user@host:/path/
来源：http://xp.521024.cn

[R57] 远程执行命令
来源：http://zi.nszjky.cn

ssh user@host 'uptime'
来源：http://an.huanxung.cn

[R58] 下载文件
来源：http://rj.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pe.shxzskj.cn

[R59] 发 POST JSON
来源：http://wc.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jw.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://dy.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rb.nicolike.cn

[R61] 磁盘占用
来源：http://tm.chemitech.net.cn

df -h;  du -sh *
来源：http://hw.szsharing.cn

[R62] 找最占空间的文件
来源：http://zb.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://fc.nicolike.cn

[R63] 内存与进程
来源：http://pt.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://ww.shxzskj.cn

[R64] 结束进程
来源：http://mm.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://jg.huanxung.cn

[R65] 查看端口占用
来源：http://co.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://th.colortex.cn

[R66] 定时任务
来源：http://mc.lnxyls.cn

crontab -e;  crontab -l
来源：http://ru.huanxung.cn

[R67] 生成随机十六进制串
来源：http://vt.lnxyls.cn

openssl rand -hex 16
来源：http://ef.panjiajie.cn

[R68] 计算文件校验值
来源：http://fo.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ce.lnxyls.cn

[R69] 生成随机密码
来源：http://mg.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://da.szxytkj.cn

[R70] 时间戳与互转
来源：http://rt.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://ef.521024.cn

[R71] 日期格式化
来源：http://pe.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sh.haigaiapp.cn

[R72] 等待端口就绪
来源：http://rq.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vt.huanxung.cn

[R73] 分割大日志
来源：http://tm.9csxet.cn

split -l 1000 big.log part_
来源：http://ls.szxytkj.cn

[R74] 批量重命名
来源：http://uo.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pm.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://su.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://qi.wgjwhj.cn

[R76] 使用临时文件
来源：http://ci.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cv.asd995.cn

[R77] 读取用户输入
来源：http://fz.shtwfgs.cn

read -rp "请输入: " ans
来源：http://df.szsharing.cn

[R78] 交互式菜单
来源：http://ov.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ku.hnjuh.cn

[R79] 解析命令行选项
来源：http://ut.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mo.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://te.panjiajie.cn

time ./run.sh
来源：http://ls.bookmarksfly.cn

================================================================================
来源：http://ut.panjiajie.cn

S. C / C++ 专题
来源：http://ot.shtwfgs.cn

================================================================================
来源：http://qr.huanxung.cn

[S01] C：Hello World
来源：http://qu.jctech888.com.cn

#include <stdio.h>
来源：http://cy.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://np.szsharing.cn

[S02] C：变量与格式化输出
来源：http://re.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://bh.9csxet.cn

[S03] C：读入整数
来源：http://ur.9csxet.cn

int x; scanf("%d", &x);
来源：http://mz.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://mb.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://so.chemitech.net.cn

[S05] C：字符串长度
来源：http://cm.panjiajie.cn

strlen(s)
来源：http://yj.asd995.cn

[S06] C：字符串比较
来源：http://fp.haigaiapp.cn

strcmp(a, b) == 0
来源：http://fz.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://cu.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xq.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://hr.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cp.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://qj.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eo.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://sq.newstarts.cn

int *p = &a;  *p = 5;
来源：http://rg.szxytkj.cn

[S11] C：逐行读文件
来源：http://ez.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://qv.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yr.huixiangedu.cn

fclose(f);
来源：http://hs.huixiangedu.cn

[S12] C：写文件
来源：http://fb.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xq.gzmigu.cn

[S13] C：宏定义
来源：http://cj.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://du.9csxet.cn

[S14] C：枚举
来源：http://bj.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://ri.bjjhwx.cn

[S15] C：类型转换
来源：http://vj.yuexingan06.cn

(double) a / b
来源：http://if.bjjhwx.cn

[S16] C：位操作置位
来源：http://cg.haigaiapp.cn

x |= (1 << 3);
来源：http://em.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://dm.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zi.shxzukj.cn

[S18] C：命令行参数
来源：http://zz.panjiajie.cn

int main(int argc, char **argv)
来源：http://xx.jianghongdianzi.cn

[S19] C：快速排序
来源：http://zt.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lk.panjiajie.cn

[S20] C：二分查找
来源：http://md.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qi.newstarts.cn

[S21] C：字符类别判断
来源：http://bo.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bw.wgjwhj.cn

[S22] C：字符串转数字
来源：http://sh.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xx.szxytkj.cn

[S23] C：随机数
来源：http://aa.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xg.hnjuh.cn

[S24] C：获取本地时间
来源：http://fz.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://py.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://zx.szxytkj.cn

memcpy(dst, src, n);
来源：http://di.nszjky.cn

[S26] C：内存清零
来源：http://ef.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://up.bjjhwx.cn

[S27] C：定义常量
来源：http://pj.shtwfgs.cn

const double PI = 3.14159;
来源：http://sv.muxihuayi.cn

[S28] C：静态变量
来源：http://lq.colortex.cn

static int counter = 0;
来源：http://ay.nszjky.cn

[S29] C：变参函数
来源：http://am.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gj.hnjuh.cn

[S30] C：头文件保护
来源：http://kn.nszjky.cn

#ifndef X_H
来源：http://hw.yuntaijiaju.cn

#define X_H
来源：http://qy.huixiangedu.cn

#endif
来源：http://ni.szsharing.cn

[S31] C++：Hello World
来源：http://wu.shxzskj.cn

#include <iostream>
来源：http://rj.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://wx.shxzukj.cn

[S32] C++：字符串
来源：http://qo.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://kz.muxihuayi.cn

[S33] C++：vector 增删
来源：http://hn.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ct.asd995.cn

[S34] C++：遍历 vector
来源：http://wh.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://yn.panjiajie.cn

[S35] C++：map
来源：http://yg.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bc.jctech888.com.cn

[S36] C++：unordered_map
来源：http://yg.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ik.huixinmuqiang.cn

[S37] C++：set
来源：http://le.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lh.huanxung.cn

[S38] C++：排序
来源：http://lg.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://it.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://de.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oh.hnjuh.cn

[S40] C++：查找元素
来源：http://sc.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ye.hnjuh.cn

[S41] C++：类与构造函数
来源：http://zx.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cu.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://wr.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://dh.huanxung.cn

[S43] C++：智能指针
来源：http://hp.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://of.huanxung.cn

[S44] C++：引用传参
来源：http://jn.newstarts.cn

void inc(int &x) { ++x; }
来源：http://eb.gzmigu.cn

[S45] C++：lambda
来源：http://qw.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ol.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://bg.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ve.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://bx.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dv.szxytkj.cn

[S48] C++：逐行读文件
来源：http://kn.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qm.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://py.haigaiapp.cn

[S49] C++：写文件
来源：http://xf.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jh.panjiajie.cn

[S50] C++：格式化数字
来源：http://hf.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hl.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://lh.huanxung.cn

static_cast<double>(a) / b
来源：http://zj.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://dt.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://zf.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://if.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://gv.nszjky.cn

[S54] C++：异常处理
来源：http://ot.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://za.asd995.cn

[S55] C++：结构化绑定
来源：http://oq.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lr.nszjky.cn

[S56] C++：optional
来源：http://tn.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fg.shxzskj.cn

[S57] C++：编译期常量
来源：http://ei.jctech888.com.cn

constexpr int N = 10;
来源：http://pt.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://ke.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://ef.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://zj.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sw.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://mm.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oa.gzmigu.cn

================================================================================
来源：http://ge.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ac.asd995.cn

================================================================================
来源：http://pa.newstarts.cn

[T01] Kotlin：Hello World
来源：http://jr.hnjuh.cn

println("Hello")
来源：http://mn.szxytkj.cn

[T02] Kotlin：变量
来源：http://bp.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fo.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://ju.huixinmuqiang.cn

"值: $b"
来源：http://nz.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://lq.hahajie.cn

val n: String? = null;  n?.length
来源：http://yt.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://th.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yk.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://cm.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dq.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://sa.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cy.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://pw.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://le.asd995.cn

[T09] Kotlin：扩展函数
来源：http://pa.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://lx.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://ih.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mm.gzmigu.cn

[T11] Kotlin：协程
来源：http://bm.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ym.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://pj.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://dc.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://gj.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://ps.asd995.cn

[T14] Kotlin：循环
来源：http://hz.szsharing.cn

for (i in 1..10) println(i)
来源：http://od.yuexingan06.cn

[T15] Kotlin：接口
来源：http://nr.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://nh.gzmigu.cn

[T16] Swift：Hello World
来源：http://qk.colortex.cn

print("Hello")
来源：http://ow.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://vp.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://bg.9csxet.cn

[T18] Swift：字符串插值
来源：http://qo.szxytkj.cn

"值: \(b)"
来源：http://cs.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://bk.shxzukj.cn

if let n = opt { print(n) }
来源：http://lt.newstarts.cn

[T20] Swift：数组操作
来源：http://tx.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gb.shtwfgs.cn

[T21] Swift：遍历
来源：http://sh.haigaiapp.cn

for x in a { print(x) }
来源：http://qy.colortex.cn

[T22] Swift：字典
来源：http://bg.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rd.asd995.cn

[T23] Swift：函数
来源：http://mi.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pc.hahajie.cn

[T24] Swift：闭包
来源：http://xc.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fy.bjjhwx.cn

[T25] Swift：结构体
来源：http://rw.szxytkj.cn

struct P { var x: Int }
来源：http://gz.nicolike.cn

[T26] Swift：类与重写
来源：http://lw.huanxung.cn

class A: Base { override func f() {} }
来源：http://ck.panjiajie.cn

[T27] Swift：错误处理
来源：http://qd.521024.cn

do { try f() } catch { print(error) }
来源：http://vo.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://wt.yuntaijiaju.cn

enum Color { case red, green }
来源：http://bu.lnxyls.cn


<!-- 参考信息 -->