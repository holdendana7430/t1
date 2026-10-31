代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rd.asd995.cn

[R34] 退出时清理
来源：http://ai.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pl.colortex.cn

[R35] 后台执行并等待
来源：http://uo.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://od.lnxyls.cn

[R36] 并发执行多个任务
来源：http://bx.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ov.shxzskj.cn

[R37] 把输出赋给变量
来源：http://yx.wgjwhj.cn

files=$(ls -1)
来源：http://qd.chemitech.net.cn

[R38] 管道串联
来源：http://wm.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://uh.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://ks.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://ct.newstarts.cn

[R40] 追加写日志
来源：http://zs.jianghongdianzi.cn

echo "log" >> out.log
来源：http://du.lnxyls.cn

[R41] 丢弃输出
来源：http://su.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://sg.jctech888.com.cn

[R42] 输入重定向
来源：http://gx.szsharing.cn

wc -l < a.txt
来源：http://af.521024.cn

[R43] 按名字查找文件
来源：http://ke.yuexingan06.cn

find . -name "*.log" -type f
来源：http://cc.shtwfgs.cn

[R44] 按修改时间查找
来源：http://ca.bjjhwx.cn

find . -mtime -7 -type f
来源：http://lt.nicolike.cn

[R45] 批量删除
来源：http://ka.huanxung.cn

find . -name "*.tmp" -delete
来源：http://lw.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://qy.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uc.chemitech.net.cn

[R47] sed 单行替换
来源：http://ra.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yx.shtwfgs.cn

[R48] awk 取指定列
来源：http://pn.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://er.szxytkj.cn

[R49] awk 带条件
来源：http://gj.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oy.yuntaijiaju.cn

[R50] awk 求和
来源：http://qe.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ay.szsharing.cn

[R51] 排序去重取前几
来源：http://py.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ek.chemitech.net.cn

[R52] 统计行数
来源：http://gp.nszjky.cn

wc -l a.txt
来源：http://tm.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://ef.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cv.szsharing.cn

[R54] 比较两个文件
来源：http://mb.newstarts.cn

diff a.txt b.txt
来源：http://fo.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://fv.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jp.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://xl.newstarts.cn

scp file user@host:/path/
来源：http://oq.hahajie.cn

[R57] 远程执行命令
来源：http://fo.bjjhwx.cn

ssh user@host 'uptime'
来源：http://wr.asd995.cn

[R58] 下载文件
来源：http://wx.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dx.gzmigu.cn

[R59] 发 POST JSON
来源：http://cn.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ab.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://vt.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rw.haigaiapp.cn

[R61] 磁盘占用
来源：http://ub.newstarts.cn

df -h;  du -sh *
来源：http://jv.nszjky.cn

[R62] 找最占空间的文件
来源：http://fq.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://ma.huanxung.cn

[R63] 内存与进程
来源：http://bd.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://mh.huixiangedu.cn

[R64] 结束进程
来源：http://bi.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://gx.gzmigu.cn

[R65] 查看端口占用
来源：http://wt.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ok.panjiajie.cn

[R66] 定时任务
来源：http://jr.hnjuh.cn

crontab -e;  crontab -l
来源：http://bd.nicolike.cn

[R67] 生成随机十六进制串
来源：http://xt.asd995.cn

openssl rand -hex 16
来源：http://sh.nszjky.cn

[R68] 计算文件校验值
来源：http://zv.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oz.panjiajie.cn

[R69] 生成随机密码
来源：http://ut.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://so.jctech888.com.cn

[R70] 时间戳与互转
来源：http://jq.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://rk.colortex.cn

[R71] 日期格式化
来源：http://kv.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fx.szxytkj.cn

[R72] 等待端口就绪
来源：http://od.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fb.nszjky.cn

[R73] 分割大日志
来源：http://fl.521024.cn

split -l 1000 big.log part_
来源：http://qs.huixiangedu.cn

[R74] 批量重命名
来源：http://qu.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://at.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://cu.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://gd.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://us.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gb.hahajie.cn

[R77] 读取用户输入
来源：http://ff.shxzukj.cn

read -rp "请输入: " ans
来源：http://or.huanxung.cn

[R78] 交互式菜单
来源：http://ns.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pm.panjiajie.cn

[R79] 解析命令行选项
来源：http://ks.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://df.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://ss.newstarts.cn

time ./run.sh
来源：http://zs.nicolike.cn

================================================================================
来源：http://pl.bookmarksfly.cn

S. C / C++ 专题
来源：http://fu.jianghongdianzi.cn

================================================================================
来源：http://gd.shxzukj.cn

[S01] C：Hello World
来源：http://gt.szsharing.cn

#include <stdio.h>
来源：http://ge.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xq.nszjky.cn

[S02] C：变量与格式化输出
来源：http://wi.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://dk.muxihuayi.cn

[S03] C：读入整数
来源：http://ox.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://fb.chemitech.net.cn

[S04] C：字符串复制
来源：http://ka.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wk.asd995.cn

[S05] C：字符串长度
来源：http://ic.nszjky.cn

strlen(s)
来源：http://nf.nicolike.cn

[S06] C：字符串比较
来源：http://lm.hahajie.cn

strcmp(a, b) == 0
来源：http://sf.hnjuh.cn

[S07] C：数组遍历求和
来源：http://si.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wm.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://nd.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://si.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://rg.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nr.panjiajie.cn

[S10] C：指针与解引用
来源：http://uu.asd995.cn

int *p = &a;  *p = 5;
来源：http://no.newstarts.cn

[S11] C：逐行读文件
来源：http://fh.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://xc.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sf.nszjky.cn

fclose(f);
来源：http://pd.panjiajie.cn

[S12] C：写文件
来源：http://os.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mf.newstarts.cn

[S13] C：宏定义
来源：http://en.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jn.gzmigu.cn

[S14] C：枚举
来源：http://lt.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://og.huanxung.cn

[S15] C：类型转换
来源：http://aa.bookmarksfly.cn

(double) a / b
来源：http://lr.shxzskj.cn

[S16] C：位操作置位
来源：http://mf.jctech888.com.cn

x |= (1 << 3);
来源：http://ky.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://uo.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nc.chemitech.net.cn

[S18] C：命令行参数
来源：http://uc.hnjuh.cn

int main(int argc, char **argv)
来源：http://pn.shxzukj.cn

[S19] C：快速排序
来源：http://nn.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yu.nszjky.cn

[S20] C：二分查找
来源：http://vq.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qw.panjiajie.cn

[S21] C：字符类别判断
来源：http://tt.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hr.muxihuayi.cn

[S22] C：字符串转数字
来源：http://rn.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gi.chemitech.net.cn

[S23] C：随机数
来源：http://lj.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://em.wgjwhj.cn

[S24] C：获取本地时间
来源：http://wm.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kg.colortex.cn

[S25] C：内存拷贝
来源：http://cg.haigaiapp.cn

memcpy(dst, src, n);
来源：http://ii.szsharing.cn

[S26] C：内存清零
来源：http://ar.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://wa.szxytkj.cn

[S27] C：定义常量
来源：http://vq.szsharing.cn

const double PI = 3.14159;
来源：http://gx.huixiangedu.cn

[S28] C：静态变量
来源：http://ak.9csxet.cn

static int counter = 0;
来源：http://tg.yuntaijiaju.cn

[S29] C：变参函数
来源：http://mq.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ox.yuexingan06.cn

[S30] C：头文件保护
来源：http://pb.521024.cn

#ifndef X_H
来源：http://zt.szsharing.cn

#define X_H
来源：http://cy.521024.cn

#endif
来源：http://tw.nszjky.cn

[S31] C++：Hello World
来源：http://lp.muxihuayi.cn

#include <iostream>
来源：http://yy.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://wc.nszjky.cn

[S32] C++：字符串
来源：http://th.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://kb.muxihuayi.cn

[S33] C++：vector 增删
来源：http://nb.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ct.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://zw.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://lc.bjjhwx.cn

[S35] C++：map
来源：http://nc.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pz.shtwfgs.cn

[S36] C++：unordered_map
来源：http://dv.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lw.huixiangedu.cn

[S37] C++：set
来源：http://nr.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ax.asd995.cn

[S38] C++：排序
来源：http://eg.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://xx.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://wq.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gy.gzmigu.cn

[S40] C++：查找元素
来源：http://fw.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rw.shxzskj.cn

[S41] C++：类与构造函数
来源：http://ht.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hw.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://pd.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://tj.hahajie.cn

[S43] C++：智能指针
来源：http://jw.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://or.nszjky.cn

[S44] C++：引用传参
来源：http://uz.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://vx.shxzskj.cn

[S45] C++：lambda
来源：http://dq.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ph.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://bx.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ru.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://aa.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cp.asd995.cn

[S48] C++：逐行读文件
来源：http://tr.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://no.nszjky.cn

while (std::getline(in, line)) { }
来源：http://ef.yuexingan06.cn

[S49] C++：写文件
来源：http://xw.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ms.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://fv.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://js.szxytkj.cn

[S51] C++：显式类型转换
来源：http://hf.huixiangedu.cn

static_cast<double>(a) / b
来源：http://gx.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://mt.huanxung.cn

int size() const noexcept { return n_; }
来源：http://am.huanxung.cn

[S53] C++：移动语义
来源：http://bu.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://hk.chemitech.net.cn

[S54] C++：异常处理
来源：http://mw.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eu.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://zm.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kj.wgjwhj.cn

[S56] C++：optional
来源：http://ic.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wm.newstarts.cn

[S57] C++：编译期常量
来源：http://ng.hnjuh.cn

constexpr int N = 10;
来源：http://vq.newstarts.cn

[S58] C++：命名空间
来源：http://fw.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://jz.szsharing.cn

[S59] C++：静态断言
来源：http://rw.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qx.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://kx.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wb.bookmarksfly.cn

================================================================================
来源：http://yj.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dp.huanxung.cn

================================================================================
来源：http://ps.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://cz.jctech888.com.cn

println("Hello")
来源：http://tf.hnjuh.cn

[T02] Kotlin：变量
来源：http://nj.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sn.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://uq.gzmigu.cn

"值: $b"
来源：http://pc.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://so.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://di.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://lz.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dj.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://hj.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kw.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://bo.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hs.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://rf.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://nd.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://at.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://sh.huanxung.cn

[T10] Kotlin：默认参数
来源：http://wh.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yb.haigaiapp.cn

[T11] Kotlin：协程
来源：http://co.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ci.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://nw.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://zb.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://il.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://ny.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://uv.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://fh.bjjhwx.cn

[T15] Kotlin：接口
来源：http://ld.nicolike.cn

interface Shape { fun area(): Double }
来源：http://dv.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://lp.newstarts.cn

print("Hello")
来源：http://dv.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://ux.nszjky.cn

var a = 1;  let b = 2
来源：http://vo.521024.cn

[T18] Swift：字符串插值
来源：http://se.jctech888.com.cn

"值: \(b)"
来源：http://hy.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://ge.newstarts.cn

if let n = opt { print(n) }
来源：http://vp.huixiangedu.cn

[T20] Swift：数组操作
来源：http://od.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://up.colortex.cn

[T21] Swift：遍历
来源：http://vm.shxzukj.cn

for x in a { print(x) }
来源：http://nn.huanxung.cn

[T22] Swift：字典
来源：http://jn.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kt.9csxet.cn

[T23] Swift：函数
来源：http://qm.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gr.huixiangedu.cn

[T24] Swift：闭包
来源：http://ck.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hu.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://vu.shxzukj.cn

struct P { var x: Int }
来源：http://uw.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://dk.szxytkj.cn

class A: Base { override func f() {} }
来源：http://sr.bjjhwx.cn

[T27] Swift：错误处理
来源：http://tx.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://aa.chemitech.net.cn

[T28] Swift：枚举
来源：http://xt.haigaiapp.cn

enum Color { case red, green }
来源：http://bo.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://cy.nicolike.cn

guard let x = opt else { return }
来源：http://jm.asd995.cn

[T30] Swift：协议
来源：http://yl.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://ry.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://mr.521024.cn

print("Hello")
来源：http://gc.shtwfgs.cn

[T32] Lua：局部变量
来源：http://pn.newstarts.cn

local a = 1
来源：http://pc.szxytkj.cn

[T33] Lua：表（数组）
来源：http://gj.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ms.nszjky.cn

[T34] Lua：遍历表
来源：http://zf.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nj.huixiangedu.cn

[T35] Lua：字典表
来源：http://za.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://tg.nicolike.cn

[T36] Lua：函数
来源：http://ys.yuexingan06.cn

function add(a, b) return a + b end
来源：http://so.haigaiapp.cn


<!-- 参考信息 -->