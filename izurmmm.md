代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://ql.szxytkj.cn

[R32] 参数个数校验
来源：http://hs.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tc.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://uz.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://is.shxzukj.cn

[R34] 退出时清理
来源：http://go.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bz.chemitech.net.cn

[R35] 后台执行并等待
来源：http://vo.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iv.521024.cn

[R36] 并发执行多个任务
来源：http://eu.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jl.newstarts.cn

[R37] 把输出赋给变量
来源：http://ty.asd995.cn

files=$(ls -1)
来源：http://hz.panjiajie.cn

[R38] 管道串联
来源：http://zn.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://xc.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://ub.nszjky.cn

cmd > out.log 2>&1
来源：http://va.huanxung.cn

[R40] 追加写日志
来源：http://ph.muxihuayi.cn

echo "log" >> out.log
来源：http://il.shxzukj.cn

[R41] 丢弃输出
来源：http://ox.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://sg.shxzskj.cn

[R42] 输入重定向
来源：http://jq.muxihuayi.cn

wc -l < a.txt
来源：http://lp.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://pk.9csxet.cn

find . -name "*.log" -type f
来源：http://kd.szsharing.cn

[R44] 按修改时间查找
来源：http://oq.chemitech.net.cn

find . -mtime -7 -type f
来源：http://ow.asd995.cn

[R45] 批量删除
来源：http://hu.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://ya.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://nb.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gb.panjiajie.cn

[R47] sed 单行替换
来源：http://qt.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ov.shtwfgs.cn

[R48] awk 取指定列
来源：http://en.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://ss.hnjuh.cn

[R49] awk 带条件
来源：http://fe.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bb.521024.cn

[R50] awk 求和
来源：http://tj.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://de.haigaiapp.cn

[R51] 排序去重取前几
来源：http://zc.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fp.bjjhwx.cn

[R52] 统计行数
来源：http://cx.newstarts.cn

wc -l a.txt
来源：http://fs.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://oc.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ls.bjjhwx.cn

[R54] 比较两个文件
来源：http://nj.hahajie.cn

diff a.txt b.txt
来源：http://nt.521024.cn

[R55] 压缩与解压
来源：http://iz.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://aa.colortex.cn

[R56] 远程拷贝
来源：http://vu.huanxung.cn

scp file user@host:/path/
来源：http://sb.wgjwhj.cn

[R57] 远程执行命令
来源：http://km.shtwfgs.cn

ssh user@host 'uptime'
来源：http://tm.huixinmuqiang.cn

[R58] 下载文件
来源：http://jf.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://px.jctech888.com.cn

[R59] 发 POST JSON
来源：http://mb.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ba.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://vr.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rt.colortex.cn

[R61] 磁盘占用
来源：http://pw.jianghongdianzi.cn

df -h;  du -sh *
来源：http://jr.521024.cn

[R62] 找最占空间的文件
来源：http://rf.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://xd.chemitech.net.cn

[R63] 内存与进程
来源：http://ef.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://xm.haigaiapp.cn

[R64] 结束进程
来源：http://cx.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://zu.shtwfgs.cn

[R65] 查看端口占用
来源：http://zu.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iv.yuexingan06.cn

[R66] 定时任务
来源：http://ts.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://ff.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://km.panjiajie.cn

openssl rand -hex 16
来源：http://vn.jctech888.com.cn

[R68] 计算文件校验值
来源：http://el.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sk.shxzskj.cn

[R69] 生成随机密码
来源：http://br.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://ff.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://qh.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://ph.hnjuh.cn

[R71] 日期格式化
来源：http://ru.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fg.asd995.cn

[R72] 等待端口就绪
来源：http://xp.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hl.nszjky.cn

[R73] 分割大日志
来源：http://bo.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://cr.lnxyls.cn

[R74] 批量重命名
来源：http://cj.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.bjjhwx.cn

[R75] 导出环境变量
来源：http://ic.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://mi.szxytkj.cn

[R76] 使用临时文件
来源：http://en.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cg.haigaiapp.cn

[R77] 读取用户输入
来源：http://xg.lnxyls.cn

read -rp "请输入: " ans
来源：http://jn.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://zp.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gv.muxihuayi.cn

[R79] 解析命令行选项
来源：http://pj.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mq.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://fy.chemitech.net.cn

time ./run.sh
来源：http://sb.chemitech.net.cn

================================================================================
来源：http://pc.yuexingan06.cn

S. C / C++ 专题
来源：http://du.muxihuayi.cn

================================================================================
来源：http://sr.hnjuh.cn

[S01] C：Hello World
来源：http://vp.szsharing.cn

#include <stdio.h>
来源：http://xe.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uv.nszjky.cn

[S02] C：变量与格式化输出
来源：http://rg.shxzukj.cn

int a = 10; printf("%d\n", a);
来源：http://jv.huixinmuqiang.cn

[S03] C：读入整数
来源：http://oq.lnxyls.cn

int x; scanf("%d", &x);
来源：http://vv.gzmigu.cn

[S04] C：字符串复制
来源：http://xv.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://is.shxzukj.cn

[S05] C：字符串长度
来源：http://bs.nicolike.cn

strlen(s)
来源：http://lr.haigaiapp.cn

[S06] C：字符串比较
来源：http://kj.haigaiapp.cn

strcmp(a, b) == 0
来源：http://wr.nszjky.cn

[S07] C：数组遍历求和
来源：http://zu.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tf.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://ai.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ui.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://nd.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yn.shtwfgs.cn

[S10] C：指针与解引用
来源：http://ys.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://mx.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://zy.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://ek.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bs.yuntaijiaju.cn

fclose(f);
来源：http://jl.nszjky.cn

[S12] C：写文件
来源：http://ad.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jm.gzmigu.cn

[S13] C：宏定义
来源：http://qk.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jq.yuexingan06.cn

[S14] C：枚举
来源：http://ly.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://sq.yuexingan06.cn

[S15] C：类型转换
来源：http://en.bookmarksfly.cn

(double) a / b
来源：http://sm.9csxet.cn

[S16] C：位操作置位
来源：http://az.shxzukj.cn

x |= (1 << 3);
来源：http://hq.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://ah.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ph.nicolike.cn

[S18] C：命令行参数
来源：http://ho.colortex.cn

int main(int argc, char **argv)
来源：http://vc.yuntaijiaju.cn

[S19] C：快速排序
来源：http://ze.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ct.yuexingan06.cn

[S20] C：二分查找
来源：http://pc.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yi.hnjuh.cn

[S21] C：字符类别判断
来源：http://xx.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://is.bjjhwx.cn

[S22] C：字符串转数字
来源：http://bd.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rs.hahajie.cn

[S23] C：随机数
来源：http://xl.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dp.nszjky.cn

[S24] C：获取本地时间
来源：http://kx.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wy.szsharing.cn

[S25] C：内存拷贝
来源：http://zq.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://lt.huixiangedu.cn

[S26] C：内存清零
来源：http://xr.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://or.huanxung.cn

[S27] C：定义常量
来源：http://es.huixiangedu.cn

const double PI = 3.14159;
来源：http://kt.521024.cn

[S28] C：静态变量
来源：http://cv.bookmarksfly.cn

static int counter = 0;
来源：http://rg.shxzskj.cn

[S29] C：变参函数
来源：http://lp.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://et.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://bh.shxzukj.cn

#ifndef X_H
来源：http://ug.nicolike.cn

#define X_H
来源：http://pn.lnxyls.cn

#endif
来源：http://jf.bookmarksfly.cn

[S31] C++：Hello World
来源：http://mu.shtwfgs.cn

#include <iostream>
来源：http://vj.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://vx.huixiangedu.cn

[S32] C++：字符串
来源：http://zc.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://cp.hnjuh.cn

[S33] C++：vector 增删
来源：http://wg.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rb.panjiajie.cn

[S34] C++：遍历 vector
来源：http://rj.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://hj.yuntaijiaju.cn

[S35] C++：map
来源：http://wu.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kr.hahajie.cn

[S36] C++：unordered_map
来源：http://mo.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ay.muxihuayi.cn

[S37] C++：set
来源：http://gx.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ho.szxytkj.cn

[S38] C++：排序
来源：http://wa.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://mk.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://xz.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xe.chemitech.net.cn

[S40] C++：查找元素
来源：http://tz.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zo.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://fd.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aq.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://md.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://lz.huixiangedu.cn

[S43] C++：智能指针
来源：http://ds.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://bk.szxytkj.cn

[S44] C++：引用传参
来源：http://nq.9csxet.cn

void inc(int &x) { ++x; }
来源：http://qa.jianghongdianzi.cn

[S45] C++：lambda
来源：http://hp.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pk.bjjhwx.cn

[S46] C++：函数模板
来源：http://hl.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ct.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://er.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iu.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://gp.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uv.szsharing.cn

while (std::getline(in, line)) { }
来源：http://wn.huixinmuqiang.cn

[S49] C++：写文件
来源：http://eq.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aj.haigaiapp.cn

[S50] C++：格式化数字
来源：http://ll.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://av.shxzukj.cn

[S51] C++：显式类型转换
来源：http://ek.hnjuh.cn

static_cast<double>(a) / b
来源：http://ld.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://zh.huanxung.cn

int size() const noexcept { return n_; }
来源：http://xk.lnxyls.cn

[S53] C++：移动语义
来源：http://gk.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://gs.yuexingan06.cn

[S54] C++：异常处理
来源：http://ry.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gs.hahajie.cn

[S55] C++：结构化绑定
来源：http://cj.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bd.nszjky.cn

[S56] C++：optional
来源：http://wx.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gh.haigaiapp.cn

[S57] C++：编译期常量
来源：http://yj.panjiajie.cn

constexpr int N = 10;
来源：http://oj.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://ct.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://xo.hahajie.cn

[S59] C++：静态断言
来源：http://yo.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kg.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://dx.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ty.nszjky.cn

================================================================================
来源：http://za.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gm.jctech888.com.cn

================================================================================
来源：http://kr.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://ev.muxihuayi.cn

println("Hello")
来源：http://wa.colortex.cn

[T02] Kotlin：变量
来源：http://ye.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bs.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://uh.bjjhwx.cn

"值: $b"
来源：http://ox.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://rw.colortex.cn

val n: String? = null;  n?.length
来源：http://ni.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://mr.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://si.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://jl.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xh.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://zr.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rw.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://xm.asd995.cn

data class User(val name: String, val age: Int)
来源：http://yn.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://lv.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://bg.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://op.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rz.shxzskj.cn

[T11] Kotlin：协程
来源：http://cm.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nq.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://ig.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://lk.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://mn.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://hi.521024.cn

[T14] Kotlin：循环
来源：http://hk.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://ba.muxihuayi.cn

[T15] Kotlin：接口
来源：http://ej.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://et.huanxung.cn

[T16] Swift：Hello World
来源：http://fc.szxytkj.cn

print("Hello")
来源：http://la.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://gu.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://tg.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://bo.hnjuh.cn

"值: \(b)"
来源：http://iq.521024.cn

[T19] Swift：可选绑定
来源：http://us.colortex.cn

if let n = opt { print(n) }
来源：http://mp.chemitech.net.cn

[T20] Swift：数组操作
来源：http://zf.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vm.shxzukj.cn

[T21] Swift：遍历
来源：http://ei.yuntaijiaju.cn

for x in a { print(x) }
来源：http://va.jctech888.com.cn

[T22] Swift：字典
来源：http://dt.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ej.huixiangedu.cn

[T23] Swift：函数
来源：http://kw.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uh.bookmarksfly.cn

[T24] Swift：闭包
来源：http://rs.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ag.shtwfgs.cn

[T25] Swift：结构体
来源：http://cj.shxzskj.cn

struct P { var x: Int }
来源：http://sl.nszjky.cn

[T26] Swift：类与重写
来源：http://vu.huanxung.cn

class A: Base { override func f() {} }
来源：http://le.asd995.cn

[T27] Swift：错误处理
来源：http://dt.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://au.hnjuh.cn

[T28] Swift：枚举
来源：http://at.haigaiapp.cn

enum Color { case red, green }
来源：http://ef.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://ae.521024.cn

guard let x = opt else { return }
来源：http://ni.bookmarksfly.cn

[T30] Swift：协议
来源：http://dc.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://jo.9csxet.cn

[T31] Lua：Hello World
来源：http://zc.521024.cn

print("Hello")
来源：http://ix.lnxyls.cn

[T32] Lua：局部变量
来源：http://cn.haigaiapp.cn

local a = 1
来源：http://ty.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://xz.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qh.gzmigu.cn

[T34] Lua：遍历表
来源：http://pp.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ie.shxzskj.cn


<!-- 参考信息 -->