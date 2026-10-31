代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://me.szxytkj.cn

[R30] 函数返回状态码
来源：http://ex.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://um.huixiangedu.cn

[R31] 局部变量
来源：http://rs.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://uw.jctech888.com.cn

[R32] 参数个数校验
来源：http://gj.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dn.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://rn.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oh.asd995.cn

[R34] 退出时清理
来源：http://jp.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jm.hnjuh.cn

[R35] 后台执行并等待
来源：http://qe.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ko.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://he.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ev.colortex.cn

[R37] 把输出赋给变量
来源：http://ya.muxihuayi.cn

files=$(ls -1)
来源：http://cn.521024.cn

[R38] 管道串联
来源：http://ly.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://pq.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://lv.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://oz.huixiangedu.cn

[R40] 追加写日志
来源：http://rl.yuntaijiaju.cn

echo "log" >> out.log
来源：http://sj.jctech888.com.cn

[R41] 丢弃输出
来源：http://cn.nicolike.cn

cmd >/dev/null 2>&1
来源：http://mb.szxytkj.cn

[R42] 输入重定向
来源：http://uq.szsharing.cn

wc -l < a.txt
来源：http://jg.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://ll.haigaiapp.cn

find . -name "*.log" -type f
来源：http://zj.muxihuayi.cn

[R44] 按修改时间查找
来源：http://ra.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://gj.9csxet.cn

[R45] 批量删除
来源：http://fq.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://rc.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://hs.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ka.panjiajie.cn

[R47] sed 单行替换
来源：http://er.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ux.colortex.cn

[R48] awk 取指定列
来源：http://ry.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://wd.nicolike.cn

[R49] awk 带条件
来源：http://hz.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vn.muxihuayi.cn

[R50] awk 求和
来源：http://km.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://na.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://kg.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ns.nszjky.cn

[R52] 统计行数
来源：http://kj.huixinmuqiang.cn

wc -l a.txt
来源：http://ze.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://et.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wa.chemitech.net.cn

[R54] 比较两个文件
来源：http://rp.colortex.cn

diff a.txt b.txt
来源：http://vw.wgjwhj.cn

[R55] 压缩与解压
来源：http://gi.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cj.huanxung.cn

[R56] 远程拷贝
来源：http://ru.huixiangedu.cn

scp file user@host:/path/
来源：http://qv.bookmarksfly.cn

[R57] 远程执行命令
来源：http://rs.wgjwhj.cn

ssh user@host 'uptime'
来源：http://ul.huixiangedu.cn

[R58] 下载文件
来源：http://aj.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zz.shxzukj.cn

[R59] 发 POST JSON
来源：http://lx.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rd.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://xf.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://od.shxzukj.cn

[R61] 磁盘占用
来源：http://fn.lnxyls.cn

df -h;  du -sh *
来源：http://xp.shxzskj.cn

[R62] 找最占空间的文件
来源：http://sc.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://qk.nszjky.cn

[R63] 内存与进程
来源：http://cj.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://ow.9csxet.cn

[R64] 结束进程
来源：http://vv.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://bp.bookmarksfly.cn

[R65] 查看端口占用
来源：http://gz.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hw.huixinmuqiang.cn

[R66] 定时任务
来源：http://tz.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://si.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://qq.shxzskj.cn

openssl rand -hex 16
来源：http://ew.chemitech.net.cn

[R68] 计算文件校验值
来源：http://by.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bj.szsharing.cn

[R69] 生成随机密码
来源：http://ed.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://ub.chemitech.net.cn

[R70] 时间戳与互转
来源：http://kr.521024.cn

date +%s;  date -d @1700000000
来源：http://jj.huixinmuqiang.cn

[R71] 日期格式化
来源：http://xu.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://es.huixiangedu.cn

[R72] 等待端口就绪
来源：http://qh.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rv.bjjhwx.cn

[R73] 分割大日志
来源：http://ly.hnjuh.cn

split -l 1000 big.log part_
来源：http://do.shxzukj.cn

[R74] 批量重命名
来源：http://km.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aw.asd995.cn

[R75] 导出环境变量
来源：http://ay.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://wi.panjiajie.cn

[R76] 使用临时文件
来源：http://id.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ds.hahajie.cn

[R77] 读取用户输入
来源：http://co.panjiajie.cn

read -rp "请输入: " ans
来源：http://pb.shtwfgs.cn

[R78] 交互式菜单
来源：http://mx.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yk.9csxet.cn

[R79] 解析命令行选项
来源：http://vy.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://el.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://tw.huixinmuqiang.cn

time ./run.sh
来源：http://om.newstarts.cn

================================================================================
来源：http://kk.bjjhwx.cn

S. C / C++ 专题
来源：http://hq.chemitech.net.cn

================================================================================
来源：http://cw.colortex.cn

[S01] C：Hello World
来源：http://ir.muxihuayi.cn

#include <stdio.h>
来源：http://bm.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://by.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://qa.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://nc.chemitech.net.cn

[S03] C：读入整数
来源：http://mz.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://ow.gzmigu.cn

[S04] C：字符串复制
来源：http://xe.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jp.shxzskj.cn

[S05] C：字符串长度
来源：http://ww.yuexingan06.cn

strlen(s)
来源：http://tl.521024.cn

[S06] C：字符串比较
来源：http://zb.muxihuayi.cn

strcmp(a, b) == 0
来源：http://cd.521024.cn

[S07] C：数组遍历求和
来源：http://cg.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://el.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://wg.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://py.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://yc.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yg.asd995.cn

[S10] C：指针与解引用
来源：http://kw.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://yk.gzmigu.cn

[S11] C：逐行读文件
来源：http://sa.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://hc.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://av.chemitech.net.cn

fclose(f);
来源：http://ro.huixinmuqiang.cn

[S12] C：写文件
来源：http://ai.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wb.shxzukj.cn

[S13] C：宏定义
来源：http://fa.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eh.lnxyls.cn

[S14] C：枚举
来源：http://rq.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://iv.gzmigu.cn

[S15] C：类型转换
来源：http://zr.szxytkj.cn

(double) a / b
来源：http://bs.szsharing.cn

[S16] C：位操作置位
来源：http://st.9csxet.cn

x |= (1 << 3);
来源：http://zt.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://da.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wh.hnjuh.cn

[S18] C：命令行参数
来源：http://sl.hnjuh.cn

int main(int argc, char **argv)
来源：http://qj.bookmarksfly.cn

[S19] C：快速排序
来源：http://zn.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oa.lnxyls.cn

[S20] C：二分查找
来源：http://ab.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zt.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://le.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gy.521024.cn

[S22] C：字符串转数字
来源：http://hb.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lq.jianghongdianzi.cn

[S23] C：随机数
来源：http://vz.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dt.panjiajie.cn

[S24] C：获取本地时间
来源：http://hq.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hg.shxzukj.cn

[S25] C：内存拷贝
来源：http://mo.nicolike.cn

memcpy(dst, src, n);
来源：http://wt.shxzskj.cn

[S26] C：内存清零
来源：http://sz.szsharing.cn

memset(a, 0, sizeof a);
来源：http://io.gzmigu.cn

[S27] C：定义常量
来源：http://cp.bookmarksfly.cn

const double PI = 3.14159;
来源：http://zw.shxzukj.cn

[S28] C：静态变量
来源：http://el.asd995.cn

static int counter = 0;
来源：http://nb.bjjhwx.cn

[S29] C：变参函数
来源：http://wu.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://je.muxihuayi.cn

[S30] C：头文件保护
来源：http://ii.521024.cn

#ifndef X_H
来源：http://ql.bjjhwx.cn

#define X_H
来源：http://rp.bookmarksfly.cn

#endif
来源：http://md.shxzukj.cn

[S31] C++：Hello World
来源：http://tn.szsharing.cn

#include <iostream>
来源：http://of.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://uo.shxzukj.cn

[S32] C++：字符串
来源：http://yv.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://ts.gzmigu.cn

[S33] C++：vector 增删
来源：http://wv.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://da.nszjky.cn

[S34] C++：遍历 vector
来源：http://ym.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://jg.huixiangedu.cn

[S35] C++：map
来源：http://vd.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rj.asd995.cn

[S36] C++：unordered_map
来源：http://do.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lq.haigaiapp.cn

[S37] C++：set
来源：http://if.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ii.jianghongdianzi.cn

[S38] C++：排序
来源：http://kx.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://nk.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://bm.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jy.lnxyls.cn

[S40] C++：查找元素
来源：http://ha.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xp.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://zl.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vc.9csxet.cn

[S42] C++：继承与虚函数
来源：http://ls.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://yv.panjiajie.cn

[S43] C++：智能指针
来源：http://sl.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://jw.newstarts.cn

[S44] C++：引用传参
来源：http://ku.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://en.muxihuayi.cn

[S45] C++：lambda
来源：http://nn.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fm.newstarts.cn

[S46] C++：函数模板
来源：http://qc.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://en.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://dz.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fo.shxzukj.cn

[S48] C++：逐行读文件
来源：http://zv.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jh.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://tj.muxihuayi.cn

[S49] C++：写文件
来源：http://oc.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wv.chemitech.net.cn

[S50] C++：格式化数字
来源：http://kb.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qb.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://rj.9csxet.cn

static_cast<double>(a) / b
来源：http://de.asd995.cn

[S52] C++：const 与 noexcept
来源：http://oz.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://fu.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://tj.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://tw.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://ri.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zt.hnjuh.cn

[S55] C++：结构化绑定
来源：http://ef.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pz.muxihuayi.cn

[S56] C++：optional
来源：http://yj.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ku.gzmigu.cn

[S57] C++：编译期常量
来源：http://nw.521024.cn

constexpr int N = 10;
来源：http://ge.nicolike.cn

[S58] C++：命名空间
来源：http://wq.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://hm.shxzukj.cn

[S59] C++：静态断言
来源：http://zd.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://it.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://vh.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dy.asd995.cn

================================================================================
来源：http://rc.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ov.huanxung.cn

================================================================================
来源：http://ih.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://gr.asd995.cn

println("Hello")
来源：http://sr.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://js.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cl.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://im.nicolike.cn

"值: $b"
来源：http://hu.nicolike.cn

[T04] Kotlin：空安全
来源：http://yd.521024.cn

val n: String? = null;  n?.length
来源：http://gg.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://nb.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fv.colortex.cn

[T06] Kotlin：集合映射
来源：http://jt.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fl.asd995.cn

[T07] Kotlin：集合过滤
来源：http://wn.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://on.colortex.cn

[T08] Kotlin：数据类
来源：http://ud.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://mt.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://pb.colortex.cn

fun String.exclaim() = this + "!"
来源：http://kh.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://kz.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ky.newstarts.cn

[T11] Kotlin：协程
来源：http://xo.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yd.colortex.cn

[T12] Kotlin：解构声明
来源：http://ff.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://yl.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://kh.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://cw.huanxung.cn

[T14] Kotlin：循环
来源：http://mt.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://ja.wgjwhj.cn

[T15] Kotlin：接口
来源：http://kv.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://tv.szxytkj.cn

[T16] Swift：Hello World
来源：http://pm.szxytkj.cn

print("Hello")
来源：http://kz.nicolike.cn

[T17] Swift：变量与常量
来源：http://kg.lnxyls.cn

var a = 1;  let b = 2
来源：http://ic.shxzskj.cn

[T18] Swift：字符串插值
来源：http://tu.jianghongdianzi.cn

"值: \(b)"
来源：http://kd.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://ed.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://jl.panjiajie.cn

[T20] Swift：数组操作
来源：http://ar.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fg.gzmigu.cn

[T21] Swift：遍历
来源：http://be.wgjwhj.cn

for x in a { print(x) }
来源：http://rz.jctech888.com.cn

[T22] Swift：字典
来源：http://ng.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cs.521024.cn

[T23] Swift：函数
来源：http://bw.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://do.jctech888.com.cn

[T24] Swift：闭包
来源：http://vb.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://op.panjiajie.cn

[T25] Swift：结构体
来源：http://mf.muxihuayi.cn

struct P { var x: Int }
来源：http://tn.9csxet.cn

[T26] Swift：类与重写
来源：http://lf.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://xa.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://nf.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://mc.szsharing.cn

[T28] Swift：枚举
来源：http://bw.szxytkj.cn

enum Color { case red, green }
来源：http://oz.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://no.9csxet.cn

guard let x = opt else { return }
来源：http://gw.shtwfgs.cn

[T30] Swift：协议
来源：http://dv.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://rq.nicolike.cn

[T31] Lua：Hello World
来源：http://jl.szxytkj.cn

print("Hello")
来源：http://jz.huixiangedu.cn

[T32] Lua：局部变量
来源：http://ri.muxihuayi.cn

local a = 1
来源：http://av.wgjwhj.cn


<!-- 参考信息 -->