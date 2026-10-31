代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://sw.newstarts.cn

[R26] 命令替换
来源：http://ww.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://wb.yuntaijiaju.cn

[R27] 算术展开
来源：http://hq.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://yh.521024.cn

[R28] 浮点运算
来源：http://us.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://wd.huanxung.cn

[R29] 定义函数
来源：http://af.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mk.lnxyls.cn

[R30] 函数返回状态码
来源：http://jw.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://pp.lnxyls.cn

[R31] 局部变量
来源：http://xb.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://jc.hahajie.cn

[R32] 参数个数校验
来源：http://et.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nq.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://em.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jo.521024.cn

[R34] 退出时清理
来源：http://em.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sk.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://bm.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://or.nicolike.cn

[R36] 并发执行多个任务
来源：http://zx.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nu.szsharing.cn

[R37] 把输出赋给变量
来源：http://lx.newstarts.cn

files=$(ls -1)
来源：http://ne.haigaiapp.cn

[R38] 管道串联
来源：http://zu.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://pl.colortex.cn

[R39] 重定向标准输出与错误
来源：http://zq.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://ew.hnjuh.cn

[R40] 追加写日志
来源：http://bw.colortex.cn

echo "log" >> out.log
来源：http://xh.szxytkj.cn

[R41] 丢弃输出
来源：http://vt.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://ll.shxzskj.cn

[R42] 输入重定向
来源：http://ia.szsharing.cn

wc -l < a.txt
来源：http://eo.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://sn.shxzukj.cn

find . -name "*.log" -type f
来源：http://pb.yuexingan06.cn

[R44] 按修改时间查找
来源：http://pe.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://mu.jianghongdianzi.cn

[R45] 批量删除
来源：http://dn.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://lb.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://dv.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fr.colortex.cn

[R47] sed 单行替换
来源：http://fb.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ek.haigaiapp.cn

[R48] awk 取指定列
来源：http://dj.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://qm.gzmigu.cn

[R49] awk 带条件
来源：http://dv.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pl.bookmarksfly.cn

[R50] awk 求和
来源：http://ci.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ks.lnxyls.cn

[R51] 排序去重取前几
来源：http://yz.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hk.521024.cn

[R52] 统计行数
来源：http://gq.9csxet.cn

wc -l a.txt
来源：http://bn.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://mh.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tq.colortex.cn

[R54] 比较两个文件
来源：http://fu.hnjuh.cn

diff a.txt b.txt
来源：http://zr.shtwfgs.cn

[R55] 压缩与解压
来源：http://rg.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qh.bjjhwx.cn

[R56] 远程拷贝
来源：http://pp.colortex.cn

scp file user@host:/path/
来源：http://ar.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://gy.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://pz.szxytkj.cn

[R58] 下载文件
来源：http://hv.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ve.lnxyls.cn

[R59] 发 POST JSON
来源：http://rq.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gb.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://ot.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tt.jctech888.com.cn

[R61] 磁盘占用
来源：http://rz.asd995.cn

df -h;  du -sh *
来源：http://qh.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://ey.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://vj.bjjhwx.cn

[R63] 内存与进程
来源：http://oa.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://fq.muxihuayi.cn

[R64] 结束进程
来源：http://ie.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://vu.521024.cn

[R65] 查看端口占用
来源：http://lv.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ws.nszjky.cn

[R66] 定时任务
来源：http://qq.shxzskj.cn

crontab -e;  crontab -l
来源：http://ho.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://vd.huixinmuqiang.cn

openssl rand -hex 16
来源：http://np.gzmigu.cn

[R68] 计算文件校验值
来源：http://io.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kw.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://ua.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://rm.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://ce.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://dh.panjiajie.cn

[R71] 日期格式化
来源：http://ab.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sh.bjjhwx.cn

[R72] 等待端口就绪
来源：http://ow.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yj.huanxung.cn

[R73] 分割大日志
来源：http://ei.colortex.cn

split -l 1000 big.log part_
来源：http://uo.shxzukj.cn

[R74] 批量重命名
来源：http://nh.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nf.gzmigu.cn

[R75] 导出环境变量
来源：http://hh.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://dg.gzmigu.cn

[R76] 使用临时文件
来源：http://vg.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tw.szsharing.cn

[R77] 读取用户输入
来源：http://zk.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://ak.szxytkj.cn

[R78] 交互式菜单
来源：http://vc.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mt.9csxet.cn

[R79] 解析命令行选项
来源：http://kw.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ih.colortex.cn

[R80] 查看脚本执行耗时
来源：http://te.asd995.cn

time ./run.sh
来源：http://ll.colortex.cn

================================================================================
来源：http://mn.szsharing.cn

S. C / C++ 专题
来源：http://zk.shtwfgs.cn

================================================================================
来源：http://xl.szxytkj.cn

[S01] C：Hello World
来源：http://rn.bjjhwx.cn

#include <stdio.h>
来源：http://be.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vd.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://pl.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://cf.jctech888.com.cn

[S03] C：读入整数
来源：http://aq.521024.cn

int x; scanf("%d", &x);
来源：http://zq.bjjhwx.cn

[S04] C：字符串复制
来源：http://nw.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mf.szxytkj.cn

[S05] C：字符串长度
来源：http://hg.hahajie.cn

strlen(s)
来源：http://kn.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://jg.colortex.cn

strcmp(a, b) == 0
来源：http://xv.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://uf.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kt.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://rh.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jf.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://pe.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lj.hahajie.cn

[S10] C：指针与解引用
来源：http://gn.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://hz.gzmigu.cn

[S11] C：逐行读文件
来源：http://ge.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://pu.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bf.hnjuh.cn

fclose(f);
来源：http://fd.nicolike.cn

[S12] C：写文件
来源：http://yq.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://st.szxytkj.cn

[S13] C：宏定义
来源：http://yc.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sy.szsharing.cn

[S14] C：枚举
来源：http://dc.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://sa.yuntaijiaju.cn

[S15] C：类型转换
来源：http://cw.shxzukj.cn

(double) a / b
来源：http://cg.szxytkj.cn

[S16] C：位操作置位
来源：http://ez.shxzskj.cn

x |= (1 << 3);
来源：http://vb.9csxet.cn

[S17] C：安全拼接字符串
来源：http://cf.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fd.yuexingan06.cn

[S18] C：命令行参数
来源：http://gp.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://ld.newstarts.cn

[S19] C：快速排序
来源：http://kr.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iz.nicolike.cn

[S20] C：二分查找
来源：http://mb.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sv.haigaiapp.cn

[S21] C：字符类别判断
来源：http://uo.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hs.yuexingan06.cn

[S22] C：字符串转数字
来源：http://lu.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oh.hnjuh.cn

[S23] C：随机数
来源：http://mn.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xi.wgjwhj.cn

[S24] C：获取本地时间
来源：http://gk.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fz.bjjhwx.cn

[S25] C：内存拷贝
来源：http://vh.chemitech.net.cn

memcpy(dst, src, n);
来源：http://el.jctech888.com.cn

[S26] C：内存清零
来源：http://ie.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://be.nszjky.cn

[S27] C：定义常量
来源：http://gs.lnxyls.cn

const double PI = 3.14159;
来源：http://et.szxytkj.cn

[S28] C：静态变量
来源：http://im.bjjhwx.cn

static int counter = 0;
来源：http://bl.huanxung.cn

[S29] C：变参函数
来源：http://rs.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ai.bookmarksfly.cn

[S30] C：头文件保护
来源：http://np.shtwfgs.cn

#ifndef X_H
来源：http://ey.szxytkj.cn

#define X_H
来源：http://ox.wgjwhj.cn

#endif
来源：http://ri.jctech888.com.cn

[S31] C++：Hello World
来源：http://jp.jctech888.com.cn

#include <iostream>
来源：http://we.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://ya.panjiajie.cn

[S32] C++：字符串
来源：http://mc.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://ar.yuexingan06.cn

[S33] C++：vector 增删
来源：http://zg.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xq.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://jo.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://jt.hnjuh.cn

[S35] C++：map
来源：http://fg.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gp.gzmigu.cn

[S36] C++：unordered_map
来源：http://wp.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nv.newstarts.cn

[S37] C++：set
来源：http://rp.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vl.521024.cn

[S38] C++：排序
来源：http://fa.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://rc.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://ca.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nb.huixiangedu.cn

[S40] C++：查找元素
来源：http://ig.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ib.nszjky.cn

[S41] C++：类与构造函数
来源：http://jd.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tf.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://tl.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://ao.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://fw.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://cv.newstarts.cn

[S44] C++：引用传参
来源：http://bj.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://sv.jianghongdianzi.cn

[S45] C++：lambda
来源：http://or.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yw.panjiajie.cn

[S46] C++：函数模板
来源：http://ki.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ku.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://uf.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pj.panjiajie.cn

[S48] C++：逐行读文件
来源：http://tl.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://js.9csxet.cn

while (std::getline(in, line)) { }
来源：http://cx.jianghongdianzi.cn

[S49] C++：写文件
来源：http://fk.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ff.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://av.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://te.nicolike.cn

[S51] C++：显式类型转换
来源：http://ze.shxzukj.cn

static_cast<double>(a) / b
来源：http://cz.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://fg.9csxet.cn

int size() const noexcept { return n_; }
来源：http://oc.asd995.cn

[S53] C++：移动语义
来源：http://je.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://qj.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://dc.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://un.colortex.cn

[S55] C++：结构化绑定
来源：http://ti.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tv.shxzukj.cn

[S56] C++：optional
来源：http://to.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ja.hahajie.cn

[S57] C++：编译期常量
来源：http://cu.chemitech.net.cn

constexpr int N = 10;
来源：http://pz.asd995.cn

[S58] C++：命名空间
来源：http://pg.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://pw.bjjhwx.cn

[S59] C++：静态断言
来源：http://fk.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vl.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://we.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://we.gzmigu.cn

================================================================================
来源：http://uo.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zo.asd995.cn

================================================================================
来源：http://ee.szsharing.cn

[T01] Kotlin：Hello World
来源：http://hy.521024.cn

println("Hello")
来源：http://cc.hahajie.cn

[T02] Kotlin：变量
来源：http://kf.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mv.521024.cn

[T03] Kotlin：字符串模板
来源：http://wp.bjjhwx.cn

"值: $b"
来源：http://zv.521024.cn

[T04] Kotlin：空安全
来源：http://to.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://fw.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://ge.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eq.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://hp.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ek.asd995.cn

[T07] Kotlin：集合过滤
来源：http://rb.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ca.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://fl.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://xn.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://cp.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://fl.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://zk.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ig.bjjhwx.cn

[T11] Kotlin：协程
来源：http://uq.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cm.huanxung.cn

[T12] Kotlin：解构声明
来源：http://pv.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://oc.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://tw.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://pc.newstarts.cn

[T14] Kotlin：循环
来源：http://ky.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://wk.lnxyls.cn

[T15] Kotlin：接口
来源：http://ly.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://ar.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://ox.huanxung.cn

print("Hello")
来源：http://nh.newstarts.cn

[T17] Swift：变量与常量
来源：http://hw.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://zf.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://lb.shxzukj.cn

"值: \(b)"
来源：http://eu.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://ba.panjiajie.cn

if let n = opt { print(n) }
来源：http://nl.shxzskj.cn

[T20] Swift：数组操作
来源：http://rb.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://my.newstarts.cn

[T21] Swift：遍历
来源：http://pc.shxzskj.cn

for x in a { print(x) }
来源：http://oq.szxytkj.cn

[T22] Swift：字典
来源：http://pl.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://de.521024.cn

[T23] Swift：函数
来源：http://jo.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rl.chemitech.net.cn

[T24] Swift：闭包
来源：http://dg.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ak.szsharing.cn

[T25] Swift：结构体
来源：http://tq.huixiangedu.cn

struct P { var x: Int }
来源：http://ce.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://fd.hnjuh.cn

class A: Base { override func f() {} }
来源：http://lm.panjiajie.cn

[T27] Swift：错误处理
来源：http://vj.521024.cn

do { try f() } catch { print(error) }
来源：http://no.lnxyls.cn

[T28] Swift：枚举
来源：http://qn.hahajie.cn

enum Color { case red, green }
来源：http://os.yuexingan06.cn


<!-- 参考信息 -->