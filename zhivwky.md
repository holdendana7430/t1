代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://zj.muxihuayi.cn

[R26] 命令替换
来源：http://jg.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://ce.yuntaijiaju.cn

[R27] 算术展开
来源：http://bz.colortex.cn

echo $((1 + 2 * 3))
来源：http://hd.yuexingan06.cn

[R28] 浮点运算
来源：http://wr.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://fr.yuexingan06.cn

[R29] 定义函数
来源：http://rm.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nicolike.cn

[R30] 函数返回状态码
来源：http://em.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://rl.nicolike.cn

[R31] 局部变量
来源：http://mw.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://sm.yuexingan06.cn

[R32] 参数个数校验
来源：http://ik.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zh.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://ok.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iv.jianghongdianzi.cn

[R34] 退出时清理
来源：http://qr.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vs.nicolike.cn

[R35] 后台执行并等待
来源：http://xz.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vb.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://zq.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zk.asd995.cn

[R37] 把输出赋给变量
来源：http://lr.szxytkj.cn

files=$(ls -1)
来源：http://xs.huanxung.cn

[R38] 管道串联
来源：http://ti.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://du.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://by.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://zq.huixiangedu.cn

[R40] 追加写日志
来源：http://td.wgjwhj.cn

echo "log" >> out.log
来源：http://yb.colortex.cn

[R41] 丢弃输出
来源：http://re.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://hh.szsharing.cn

[R42] 输入重定向
来源：http://yv.asd995.cn

wc -l < a.txt
来源：http://be.lnxyls.cn

[R43] 按名字查找文件
来源：http://qz.haigaiapp.cn

find . -name "*.log" -type f
来源：http://mv.asd995.cn

[R44] 按修改时间查找
来源：http://se.szxytkj.cn

find . -mtime -7 -type f
来源：http://hz.colortex.cn

[R45] 批量删除
来源：http://vo.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://jj.hahajie.cn

[R46] 递归替换文件内容
来源：http://fm.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fj.9csxet.cn

[R47] sed 单行替换
来源：http://ta.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vs.shxzskj.cn

[R48] awk 取指定列
来源：http://bh.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://pl.panjiajie.cn

[R49] awk 带条件
来源：http://un.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cl.huixiangedu.cn

[R50] awk 求和
来源：http://sc.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xz.gzmigu.cn

[R51] 排序去重取前几
来源：http://mp.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xb.huixinmuqiang.cn

[R52] 统计行数
来源：http://zg.hnjuh.cn

wc -l a.txt
来源：http://td.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://op.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gc.haigaiapp.cn

[R54] 比较两个文件
来源：http://pv.yuntaijiaju.cn

diff a.txt b.txt
来源：http://sh.bjjhwx.cn

[R55] 压缩与解压
来源：http://rs.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wg.muxihuayi.cn

[R56] 远程拷贝
来源：http://hz.szsharing.cn

scp file user@host:/path/
来源：http://sk.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://nn.colortex.cn

ssh user@host 'uptime'
来源：http://fr.muxihuayi.cn

[R58] 下载文件
来源：http://ur.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ul.gzmigu.cn

[R59] 发 POST JSON
来源：http://tw.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://la.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://kl.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lh.bjjhwx.cn

[R61] 磁盘占用
来源：http://ed.nicolike.cn

df -h;  du -sh *
来源：http://od.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://ap.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://lm.huixiangedu.cn

[R63] 内存与进程
来源：http://af.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://fa.jctech888.com.cn

[R64] 结束进程
来源：http://kd.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://oa.521024.cn

[R65] 查看端口占用
来源：http://gs.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gs.yuntaijiaju.cn

[R66] 定时任务
来源：http://sl.shtwfgs.cn

crontab -e;  crontab -l
来源：http://py.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://eb.521024.cn

openssl rand -hex 16
来源：http://kl.panjiajie.cn

[R68] 计算文件校验值
来源：http://cl.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xz.szsharing.cn

[R69] 生成随机密码
来源：http://nt.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://ig.newstarts.cn

[R70] 时间戳与互转
来源：http://qb.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://ki.newstarts.cn

[R71] 日期格式化
来源：http://dc.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xn.nszjky.cn

[R72] 等待端口就绪
来源：http://rr.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ym.chemitech.net.cn

[R73] 分割大日志
来源：http://lq.521024.cn

split -l 1000 big.log part_
来源：http://km.bookmarksfly.cn

[R74] 批量重命名
来源：http://ca.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ab.hnjuh.cn

[R75] 导出环境变量
来源：http://yq.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://kh.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://lv.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ab.hnjuh.cn

[R77] 读取用户输入
来源：http://vz.szsharing.cn

read -rp "请输入: " ans
来源：http://zp.hahajie.cn

[R78] 交互式菜单
来源：http://wi.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ew.shxzukj.cn

[R79] 解析命令行选项
来源：http://tq.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gr.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://xe.haigaiapp.cn

time ./run.sh
来源：http://da.huixinmuqiang.cn

================================================================================
来源：http://we.nszjky.cn

S. C / C++ 专题
来源：http://gx.bjjhwx.cn

================================================================================
来源：http://zn.haigaiapp.cn

[S01] C：Hello World
来源：http://ep.jianghongdianzi.cn

#include <stdio.h>
来源：http://px.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hs.huanxung.cn

[S02] C：变量与格式化输出
来源：http://au.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://hy.9csxet.cn

[S03] C：读入整数
来源：http://vs.panjiajie.cn

int x; scanf("%d", &x);
来源：http://jl.nicolike.cn

[S04] C：字符串复制
来源：http://ce.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pq.bookmarksfly.cn

[S05] C：字符串长度
来源：http://ky.huanxung.cn

strlen(s)
来源：http://br.szsharing.cn

[S06] C：字符串比较
来源：http://nu.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://qj.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://ip.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ew.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://ka.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nx.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://di.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bx.wgjwhj.cn

[S10] C：指针与解引用
来源：http://ck.asd995.cn

int *p = &a;  *p = 5;
来源：http://ub.asd995.cn

[S11] C：逐行读文件
来源：http://hp.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://ae.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xt.9csxet.cn

fclose(f);
来源：http://ue.9csxet.cn

[S12] C：写文件
来源：http://rg.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dj.9csxet.cn

[S13] C：宏定义
来源：http://zn.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://id.jianghongdianzi.cn

[S14] C：枚举
来源：http://rc.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://zt.bjjhwx.cn

[S15] C：类型转换
来源：http://xl.yuexingan06.cn

(double) a / b
来源：http://iy.9csxet.cn

[S16] C：位操作置位
来源：http://eg.asd995.cn

x |= (1 << 3);
来源：http://ut.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://mf.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wj.huanxung.cn

[S18] C：命令行参数
来源：http://jy.wgjwhj.cn

int main(int argc, char **argv)
来源：http://eq.yuexingan06.cn

[S19] C：快速排序
来源：http://ob.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qo.shtwfgs.cn

[S20] C：二分查找
来源：http://hl.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://de.huanxung.cn

[S21] C：字符类别判断
来源：http://nm.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tn.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://ix.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://di.lnxyls.cn

[S23] C：随机数
来源：http://gy.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://st.muxihuayi.cn

[S24] C：获取本地时间
来源：http://hb.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jr.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://wd.shtwfgs.cn

memcpy(dst, src, n);
来源：http://sg.panjiajie.cn

[S26] C：内存清零
来源：http://gb.9csxet.cn

memset(a, 0, sizeof a);
来源：http://fq.huixiangedu.cn

[S27] C：定义常量
来源：http://ll.huanxung.cn

const double PI = 3.14159;
来源：http://ls.shxzskj.cn

[S28] C：静态变量
来源：http://ja.szsharing.cn

static int counter = 0;
来源：http://hb.haigaiapp.cn

[S29] C：变参函数
来源：http://xj.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gn.nszjky.cn

[S30] C：头文件保护
来源：http://zp.shxzskj.cn

#ifndef X_H
来源：http://jx.szxytkj.cn

#define X_H
来源：http://mo.chemitech.net.cn

#endif
来源：http://yp.chemitech.net.cn

[S31] C++：Hello World
来源：http://vj.gzmigu.cn

#include <iostream>
来源：http://lt.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://mw.shtwfgs.cn

[S32] C++：字符串
来源：http://xy.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://ef.newstarts.cn

[S33] C++：vector 增删
来源：http://bx.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sw.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://vp.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://tq.shtwfgs.cn

[S35] C++：map
来源：http://eg.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fs.lnxyls.cn

[S36] C++：unordered_map
来源：http://jj.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nc.huixinmuqiang.cn

[S37] C++：set
来源：http://an.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gy.bookmarksfly.cn

[S38] C++：排序
来源：http://pj.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://jm.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://ys.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jn.asd995.cn

[S40] C++：查找元素
来源：http://mg.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gs.asd995.cn

[S41] C++：类与构造函数
来源：http://rv.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zj.nszjky.cn

[S42] C++：继承与虚函数
来源：http://yk.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://mm.huanxung.cn

[S43] C++：智能指针
来源：http://xg.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://gd.asd995.cn

[S44] C++：引用传参
来源：http://an.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://dc.wgjwhj.cn

[S45] C++：lambda
来源：http://zc.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ob.huixiangedu.cn

[S46] C++：函数模板
来源：http://kf.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nd.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://em.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ho.hahajie.cn

[S48] C++：逐行读文件
来源：http://vr.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gy.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://ce.nszjky.cn

[S49] C++：写文件
来源：http://ge.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qn.nszjky.cn

[S50] C++：格式化数字
来源：http://nr.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tt.shxzukj.cn

[S51] C++：显式类型转换
来源：http://fx.wgjwhj.cn

static_cast<double>(a) / b
来源：http://da.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://pu.9csxet.cn

int size() const noexcept { return n_; }
来源：http://ou.yuexingan06.cn

[S53] C++：移动语义
来源：http://sq.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://jz.shtwfgs.cn

[S54] C++：异常处理
来源：http://lq.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ku.nszjky.cn

[S55] C++：结构化绑定
来源：http://ev.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pj.hnjuh.cn

[S56] C++：optional
来源：http://xb.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fn.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://bz.jianghongdianzi.cn

constexpr int N = 10;
来源：http://bc.nszjky.cn

[S58] C++：命名空间
来源：http://ap.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://nt.gzmigu.cn

[S59] C++：静态断言
来源：http://gi.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://on.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://as.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://su.gzmigu.cn

================================================================================
来源：http://sz.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://px.haigaiapp.cn

================================================================================
来源：http://kf.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://ul.huanxung.cn

println("Hello")
来源：http://oa.gzmigu.cn

[T02] Kotlin：变量
来源：http://ez.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zu.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://hv.9csxet.cn

"值: $b"
来源：http://hr.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://vm.shxzskj.cn

val n: String? = null;  n?.length
来源：http://ur.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://qm.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://up.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://uh.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rp.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://va.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pu.521024.cn

[T08] Kotlin：数据类
来源：http://qn.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://jl.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://dg.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://ss.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://gl.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qp.haigaiapp.cn

[T11] Kotlin：协程
来源：http://he.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ug.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://ae.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://hp.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://wf.521024.cn

val m = mapOf("a" to 1)
来源：http://gp.jctech888.com.cn

[T14] Kotlin：循环
来源：http://pk.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://hh.asd995.cn

[T15] Kotlin：接口
来源：http://uh.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://fx.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://vm.chemitech.net.cn

print("Hello")
来源：http://ag.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://ar.nszjky.cn

var a = 1;  let b = 2
来源：http://fm.shxzukj.cn

[T18] Swift：字符串插值
来源：http://gc.nszjky.cn

"值: \(b)"
来源：http://to.shxzukj.cn

[T19] Swift：可选绑定
来源：http://nj.huixiangedu.cn

if let n = opt { print(n) }
来源：http://bg.wgjwhj.cn

[T20] Swift：数组操作
来源：http://gv.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://eu.wgjwhj.cn

[T21] Swift：遍历
来源：http://tn.chemitech.net.cn

for x in a { print(x) }
来源：http://cc.muxihuayi.cn

[T22] Swift：字典
来源：http://zu.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kk.huanxung.cn

[T23] Swift：函数
来源：http://if.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://av.shxzskj.cn

[T24] Swift：闭包
来源：http://rr.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jx.nicolike.cn

[T25] Swift：结构体
来源：http://kb.chemitech.net.cn

struct P { var x: Int }
来源：http://hw.lnxyls.cn

[T26] Swift：类与重写
来源：http://ca.nicolike.cn

class A: Base { override func f() {} }
来源：http://hq.lnxyls.cn

[T27] Swift：错误处理
来源：http://na.huanxung.cn

do { try f() } catch { print(error) }
来源：http://nv.521024.cn

[T28] Swift：枚举
来源：http://mn.yuntaijiaju.cn

enum Color { case red, green }
来源：http://wl.huixinmuqiang.cn


<!-- 参考信息 -->