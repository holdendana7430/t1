代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hi.yuexingan06.cn

[R30] 函数返回状态码
来源：http://pi.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://ts.bookmarksfly.cn

[R31] 局部变量
来源：http://xl.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://ty.shxzukj.cn

[R32] 参数个数校验
来源：http://jr.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mu.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://nh.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zi.hnjuh.cn

[R34] 退出时清理
来源：http://ly.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://td.wgjwhj.cn

[R35] 后台执行并等待
来源：http://yi.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://af.9csxet.cn

[R36] 并发执行多个任务
来源：http://no.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lw.szsharing.cn

[R37] 把输出赋给变量
来源：http://cb.huanxung.cn

files=$(ls -1)
来源：http://qi.nszjky.cn

[R38] 管道串联
来源：http://ua.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://fd.colortex.cn

[R39] 重定向标准输出与错误
来源：http://rq.haigaiapp.cn

cmd > out.log 2>&1
来源：http://go.yuntaijiaju.cn

[R40] 追加写日志
来源：http://qg.szxytkj.cn

echo "log" >> out.log
来源：http://nd.shxzukj.cn

[R41] 丢弃输出
来源：http://vm.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://xl.haigaiapp.cn

[R42] 输入重定向
来源：http://ic.huanxung.cn

wc -l < a.txt
来源：http://ct.muxihuayi.cn

[R43] 按名字查找文件
来源：http://ku.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://ll.chemitech.net.cn

[R44] 按修改时间查找
来源：http://ht.haigaiapp.cn

find . -mtime -7 -type f
来源：http://hm.yuexingan06.cn

[R45] 批量删除
来源：http://xo.nszjky.cn

find . -name "*.tmp" -delete
来源：http://zt.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://yi.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kh.asd995.cn

[R47] sed 单行替换
来源：http://fb.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xr.bookmarksfly.cn

[R48] awk 取指定列
来源：http://gh.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://mh.gzmigu.cn

[R49] awk 带条件
来源：http://ve.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wu.panjiajie.cn

[R50] awk 求和
来源：http://zo.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mt.chemitech.net.cn

[R51] 排序去重取前几
来源：http://om.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ic.haigaiapp.cn

[R52] 统计行数
来源：http://ag.muxihuayi.cn

wc -l a.txt
来源：http://xh.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://nm.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zw.panjiajie.cn

[R54] 比较两个文件
来源：http://ck.nicolike.cn

diff a.txt b.txt
来源：http://xq.521024.cn

[R55] 压缩与解压
来源：http://iw.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ba.szxytkj.cn

[R56] 远程拷贝
来源：http://pe.shxzukj.cn

scp file user@host:/path/
来源：http://pg.wgjwhj.cn

[R57] 远程执行命令
来源：http://zq.jctech888.com.cn

ssh user@host 'uptime'
来源：http://qx.colortex.cn

[R58] 下载文件
来源：http://fy.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://en.shxzskj.cn

[R59] 发 POST JSON
来源：http://lq.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://us.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://kp.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xg.bjjhwx.cn

[R61] 磁盘占用
来源：http://kb.huixiangedu.cn

df -h;  du -sh *
来源：http://py.hahajie.cn

[R62] 找最占空间的文件
来源：http://us.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://bb.szsharing.cn

[R63] 内存与进程
来源：http://ex.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://ru.nicolike.cn

[R64] 结束进程
来源：http://ye.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://ki.panjiajie.cn

[R65] 查看端口占用
来源：http://yk.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tr.huixinmuqiang.cn

[R66] 定时任务
来源：http://ed.szsharing.cn

crontab -e;  crontab -l
来源：http://iz.asd995.cn

[R67] 生成随机十六进制串
来源：http://ya.nszjky.cn

openssl rand -hex 16
来源：http://wn.jctech888.com.cn

[R68] 计算文件校验值
来源：http://al.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fz.jctech888.com.cn

[R69] 生成随机密码
来源：http://vj.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://it.newstarts.cn

[R70] 时间戳与互转
来源：http://li.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://ht.colortex.cn

[R71] 日期格式化
来源：http://we.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pc.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://ya.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zt.huixiangedu.cn

[R73] 分割大日志
来源：http://wq.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://hg.asd995.cn

[R74] 批量重命名
来源：http://yz.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pq.szsharing.cn

[R75] 导出环境变量
来源：http://pm.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://fh.9csxet.cn

[R76] 使用临时文件
来源：http://wa.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jl.szxytkj.cn

[R77] 读取用户输入
来源：http://ht.gzmigu.cn

read -rp "请输入: " ans
来源：http://mx.asd995.cn

[R78] 交互式菜单
来源：http://zh.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nm.szxytkj.cn

[R79] 解析命令行选项
来源：http://ph.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aw.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://cx.lnxyls.cn

time ./run.sh
来源：http://ce.huixinmuqiang.cn

================================================================================
来源：http://bp.yuntaijiaju.cn

S. C / C++ 专题
来源：http://ft.chemitech.net.cn

================================================================================
来源：http://fy.wgjwhj.cn

[S01] C：Hello World
来源：http://wf.hnjuh.cn

#include <stdio.h>
来源：http://xl.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bd.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://mh.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://ns.gzmigu.cn

[S03] C：读入整数
来源：http://uw.huanxung.cn

int x; scanf("%d", &x);
来源：http://ih.colortex.cn

[S04] C：字符串复制
来源：http://hr.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eb.hnjuh.cn

[S05] C：字符串长度
来源：http://aq.jctech888.com.cn

strlen(s)
来源：http://xc.szsharing.cn

[S06] C：字符串比较
来源：http://kk.muxihuayi.cn

strcmp(a, b) == 0
来源：http://xd.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://hn.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fp.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://jq.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mj.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://nl.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wd.nszjky.cn

[S10] C：指针与解引用
来源：http://uh.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://ej.shxzukj.cn

[S11] C：逐行读文件
来源：http://le.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://tx.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pk.nszjky.cn

fclose(f);
来源：http://fh.hahajie.cn

[S12] C：写文件
来源：http://ui.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://so.shxzskj.cn

[S13] C：宏定义
来源：http://cj.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mi.gzmigu.cn

[S14] C：枚举
来源：http://uq.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://nl.panjiajie.cn

[S15] C：类型转换
来源：http://an.9csxet.cn

(double) a / b
来源：http://gy.panjiajie.cn

[S16] C：位操作置位
来源：http://cm.bookmarksfly.cn

x |= (1 << 3);
来源：http://my.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://yv.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lc.lnxyls.cn

[S18] C：命令行参数
来源：http://bv.gzmigu.cn

int main(int argc, char **argv)
来源：http://xf.wgjwhj.cn

[S19] C：快速排序
来源：http://ew.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uv.shxzskj.cn

[S20] C：二分查找
来源：http://ru.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bi.szxytkj.cn

[S21] C：字符类别判断
来源：http://dw.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://os.yuexingan06.cn

[S22] C：字符串转数字
来源：http://bs.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cf.shxzukj.cn

[S23] C：随机数
来源：http://ep.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vq.lnxyls.cn

[S24] C：获取本地时间
来源：http://fp.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pf.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://sr.shxzskj.cn

memcpy(dst, src, n);
来源：http://va.newstarts.cn

[S26] C：内存清零
来源：http://sw.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://vb.panjiajie.cn

[S27] C：定义常量
来源：http://sa.nszjky.cn

const double PI = 3.14159;
来源：http://un.panjiajie.cn

[S28] C：静态变量
来源：http://ke.gzmigu.cn

static int counter = 0;
来源：http://sv.yuexingan06.cn

[S29] C：变参函数
来源：http://he.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zu.panjiajie.cn

[S30] C：头文件保护
来源：http://vu.huixiangedu.cn

#ifndef X_H
来源：http://mn.muxihuayi.cn

#define X_H
来源：http://jp.szsharing.cn

#endif
来源：http://am.asd995.cn

[S31] C++：Hello World
来源：http://qg.shtwfgs.cn

#include <iostream>
来源：http://mj.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://gf.szsharing.cn

[S32] C++：字符串
来源：http://or.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://lz.asd995.cn

[S33] C++：vector 增删
来源：http://co.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rb.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://lp.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://en.yuexingan06.cn

[S35] C++：map
来源：http://zv.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://df.nicolike.cn

[S36] C++：unordered_map
来源：http://wl.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wo.hahajie.cn

[S37] C++：set
来源：http://iz.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qg.lnxyls.cn

[S38] C++：排序
来源：http://un.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://eb.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://zb.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://br.521024.cn

[S40] C++：查找元素
来源：http://zh.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sp.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://gf.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://js.newstarts.cn

[S42] C++：继承与虚函数
来源：http://gj.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://nb.bjjhwx.cn

[S43] C++：智能指针
来源：http://wf.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://sw.yuexingan06.cn

[S44] C++：引用传参
来源：http://ha.nszjky.cn

void inc(int &x) { ++x; }
来源：http://dg.521024.cn

[S45] C++：lambda
来源：http://ns.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hf.huanxung.cn

[S46] C++：函数模板
来源：http://su.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kg.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://dp.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jp.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://ll.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rx.nszjky.cn

while (std::getline(in, line)) { }
来源：http://kv.nszjky.cn

[S49] C++：写文件
来源：http://yj.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gc.521024.cn

[S50] C++：格式化数字
来源：http://fm.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yc.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://an.muxihuayi.cn

static_cast<double>(a) / b
来源：http://md.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://ih.hahajie.cn

int size() const noexcept { return n_; }
来源：http://mf.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://ts.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://xr.muxihuayi.cn

[S54] C++：异常处理
来源：http://gd.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nk.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://bj.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yu.wgjwhj.cn

[S56] C++：optional
来源：http://bc.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ow.yuexingan06.cn

[S57] C++：编译期常量
来源：http://if.szxytkj.cn

constexpr int N = 10;
来源：http://lm.shxzskj.cn

[S58] C++：命名空间
来源：http://ch.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://ee.shxzskj.cn

[S59] C++：静态断言
来源：http://lv.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://we.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://ih.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uw.huanxung.cn

================================================================================
来源：http://jx.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ck.yuntaijiaju.cn

================================================================================
来源：http://cd.nszjky.cn

[T01] Kotlin：Hello World
来源：http://xw.asd995.cn

println("Hello")
来源：http://sj.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://xq.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ee.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://ij.szxytkj.cn

"值: $b"
来源：http://jx.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://tq.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://cg.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://je.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xm.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://rz.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xh.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://tl.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ds.9csxet.cn

[T08] Kotlin：数据类
来源：http://jj.colortex.cn

data class User(val name: String, val age: Int)
来源：http://et.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://ll.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://sf.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://ad.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zy.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://ei.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ql.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://ww.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://ws.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://th.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://yx.bjjhwx.cn

[T14] Kotlin：循环
来源：http://fn.nszjky.cn

for (i in 1..10) println(i)
来源：http://wu.panjiajie.cn

[T15] Kotlin：接口
来源：http://bf.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://dh.szsharing.cn

[T16] Swift：Hello World
来源：http://qt.jctech888.com.cn

print("Hello")
来源：http://kd.panjiajie.cn

[T17] Swift：变量与常量
来源：http://dl.huixiangedu.cn

var a = 1;  let b = 2
来源：http://xx.nszjky.cn

[T18] Swift：字符串插值
来源：http://yb.panjiajie.cn

"值: \(b)"
来源：http://hg.huanxung.cn

[T19] Swift：可选绑定
来源：http://lo.lnxyls.cn

if let n = opt { print(n) }
来源：http://zp.haigaiapp.cn

[T20] Swift：数组操作
来源：http://cn.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uh.huixiangedu.cn

[T21] Swift：遍历
来源：http://zq.hahajie.cn

for x in a { print(x) }
来源：http://jg.szsharing.cn

[T22] Swift：字典
来源：http://pr.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bf.huixiangedu.cn

[T23] Swift：函数
来源：http://jn.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dx.bookmarksfly.cn

[T24] Swift：闭包
来源：http://lz.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zi.9csxet.cn

[T25] Swift：结构体
来源：http://vp.muxihuayi.cn

struct P { var x: Int }
来源：http://cg.jctech888.com.cn

[T26] Swift：类与重写
来源：http://vm.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://kt.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://vp.colortex.cn

do { try f() } catch { print(error) }
来源：http://wc.yuexingan06.cn

[T28] Swift：枚举
来源：http://sc.szsharing.cn

enum Color { case red, green }
来源：http://gl.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://fz.huanxung.cn

guard let x = opt else { return }
来源：http://nz.hahajie.cn

[T30] Swift：协议
来源：http://zv.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://tk.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://mi.bookmarksfly.cn

print("Hello")
来源：http://pg.newstarts.cn

[T32] Lua：局部变量
来源：http://qe.nszjky.cn

local a = 1
来源：http://gn.bookmarksfly.cn


<!-- 参考信息 -->