代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kb.chemitech.net.cn

[R24] 大小写转换
来源：http://pw.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bt.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://xl.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nt.yuntaijiaju.cn

[R26] 命令替换
来源：http://ir.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://cp.szxytkj.cn

[R27] 算术展开
来源：http://qq.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://ss.wgjwhj.cn

[R28] 浮点运算
来源：http://uz.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://zn.shxzukj.cn

[R29] 定义函数
来源：http://va.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fa.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://hz.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://ih.huanxung.cn

[R31] 局部变量
来源：http://ri.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://la.nszjky.cn

[R32] 参数个数校验
来源：http://fi.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sn.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://bz.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ch.huanxung.cn

[R34] 退出时清理
来源：http://zo.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lt.shxzukj.cn

[R35] 后台执行并等待
来源：http://mh.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://be.gzmigu.cn

[R36] 并发执行多个任务
来源：http://rj.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aa.shxzukj.cn

[R37] 把输出赋给变量
来源：http://ca.muxihuayi.cn

files=$(ls -1)
来源：http://at.haigaiapp.cn

[R38] 管道串联
来源：http://op.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://kj.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://xo.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://rq.hnjuh.cn

[R40] 追加写日志
来源：http://fn.yuntaijiaju.cn

echo "log" >> out.log
来源：http://vn.nicolike.cn

[R41] 丢弃输出
来源：http://sf.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://io.nicolike.cn

[R42] 输入重定向
来源：http://zc.shxzukj.cn

wc -l < a.txt
来源：http://yu.szsharing.cn

[R43] 按名字查找文件
来源：http://gf.szsharing.cn

find . -name "*.log" -type f
来源：http://py.shtwfgs.cn

[R44] 按修改时间查找
来源：http://gw.lnxyls.cn

find . -mtime -7 -type f
来源：http://ih.huanxung.cn

[R45] 批量删除
来源：http://tv.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://pt.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://ye.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ic.panjiajie.cn

[R47] sed 单行替换
来源：http://aw.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yq.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://an.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://et.521024.cn

[R49] awk 带条件
来源：http://hd.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ms.chemitech.net.cn

[R50] awk 求和
来源：http://ns.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xu.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://ca.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kf.shxzskj.cn

[R52] 统计行数
来源：http://qr.yuexingan06.cn

wc -l a.txt
来源：http://sp.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://et.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gc.colortex.cn

[R54] 比较两个文件
来源：http://ai.shxzukj.cn

diff a.txt b.txt
来源：http://mh.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://zq.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ze.wgjwhj.cn

[R56] 远程拷贝
来源：http://eg.shxzskj.cn

scp file user@host:/path/
来源：http://mp.newstarts.cn

[R57] 远程执行命令
来源：http://fz.colortex.cn

ssh user@host 'uptime'
来源：http://dm.wgjwhj.cn

[R58] 下载文件
来源：http://mr.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://od.shxzskj.cn

[R59] 发 POST JSON
来源：http://xi.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tv.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://gc.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ga.colortex.cn

[R61] 磁盘占用
来源：http://zf.lnxyls.cn

df -h;  du -sh *
来源：http://kt.shxzskj.cn

[R62] 找最占空间的文件
来源：http://os.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://os.wgjwhj.cn

[R63] 内存与进程
来源：http://sm.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://zp.panjiajie.cn

[R64] 结束进程
来源：http://gp.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://kq.newstarts.cn

[R65] 查看端口占用
来源：http://pj.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cg.huixiangedu.cn

[R66] 定时任务
来源：http://xq.hahajie.cn

crontab -e;  crontab -l
来源：http://iu.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://xv.9csxet.cn

openssl rand -hex 16
来源：http://nb.shxzukj.cn

[R68] 计算文件校验值
来源：http://hj.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://eq.jctech888.com.cn

[R69] 生成随机密码
来源：http://ho.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://vw.newstarts.cn

[R70] 时间戳与互转
来源：http://fy.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://xc.yuntaijiaju.cn

[R71] 日期格式化
来源：http://qi.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ie.nicolike.cn

[R72] 等待端口就绪
来源：http://vb.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xq.9csxet.cn

[R73] 分割大日志
来源：http://sn.nicolike.cn

split -l 1000 big.log part_
来源：http://oz.jctech888.com.cn

[R74] 批量重命名
来源：http://ic.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lp.bjjhwx.cn

[R75] 导出环境变量
来源：http://ez.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://sk.haigaiapp.cn

[R76] 使用临时文件
来源：http://nn.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yj.colortex.cn

[R77] 读取用户输入
来源：http://ep.nicolike.cn

read -rp "请输入: " ans
来源：http://wo.szxytkj.cn

[R78] 交互式菜单
来源：http://kk.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nc.shtwfgs.cn

[R79] 解析命令行选项
来源：http://yp.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jc.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://xn.hnjuh.cn

time ./run.sh
来源：http://jk.szsharing.cn

================================================================================
来源：http://xt.wgjwhj.cn

S. C / C++ 专题
来源：http://wa.yuntaijiaju.cn

================================================================================
来源：http://bk.jianghongdianzi.cn

[S01] C：Hello World
来源：http://fy.huixinmuqiang.cn

#include <stdio.h>
来源：http://do.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tt.nicolike.cn

[S02] C：变量与格式化输出
来源：http://kv.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://nk.lnxyls.cn

[S03] C：读入整数
来源：http://ow.shxzskj.cn

int x; scanf("%d", &x);
来源：http://zs.newstarts.cn

[S04] C：字符串复制
来源：http://sz.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yw.wgjwhj.cn

[S05] C：字符串长度
来源：http://ex.szxytkj.cn

strlen(s)
来源：http://gw.bjjhwx.cn

[S06] C：字符串比较
来源：http://ka.lnxyls.cn

strcmp(a, b) == 0
来源：http://zy.gzmigu.cn

[S07] C：数组遍历求和
来源：http://hm.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ix.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://et.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ff.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://zs.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ld.haigaiapp.cn

[S10] C：指针与解引用
来源：http://wz.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://ow.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://qj.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://rx.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jh.shxzukj.cn

fclose(f);
来源：http://mx.shxzskj.cn

[S12] C：写文件
来源：http://sb.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nn.chemitech.net.cn

[S13] C：宏定义
来源：http://gg.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dj.9csxet.cn

[S14] C：枚举
来源：http://pn.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://bh.newstarts.cn

[S15] C：类型转换
来源：http://cg.haigaiapp.cn

(double) a / b
来源：http://wm.shtwfgs.cn

[S16] C：位操作置位
来源：http://pv.bookmarksfly.cn

x |= (1 << 3);
来源：http://hm.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://gn.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://si.nszjky.cn

[S18] C：命令行参数
来源：http://ml.huixiangedu.cn

int main(int argc, char **argv)
来源：http://ed.szxytkj.cn

[S19] C：快速排序
来源：http://hj.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nd.asd995.cn

[S20] C：二分查找
来源：http://ly.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cv.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://bc.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lo.shxzskj.cn

[S22] C：字符串转数字
来源：http://rp.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ul.nicolike.cn

[S23] C：随机数
来源：http://ca.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lo.hnjuh.cn

[S24] C：获取本地时间
来源：http://od.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nk.shxzukj.cn

[S25] C：内存拷贝
来源：http://as.521024.cn

memcpy(dst, src, n);
来源：http://ur.bjjhwx.cn

[S26] C：内存清零
来源：http://dk.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://qs.chemitech.net.cn

[S27] C：定义常量
来源：http://bi.lnxyls.cn

const double PI = 3.14159;
来源：http://ee.colortex.cn

[S28] C：静态变量
来源：http://dc.9csxet.cn

static int counter = 0;
来源：http://ea.chemitech.net.cn

[S29] C：变参函数
来源：http://ij.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lj.panjiajie.cn

[S30] C：头文件保护
来源：http://cf.bookmarksfly.cn

#ifndef X_H
来源：http://jp.521024.cn

#define X_H
来源：http://ez.bjjhwx.cn

#endif
来源：http://ju.shxzukj.cn

[S31] C++：Hello World
来源：http://lh.szsharing.cn

#include <iostream>
来源：http://sm.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://so.jianghongdianzi.cn

[S32] C++：字符串
来源：http://ym.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://cv.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://mz.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dh.newstarts.cn

[S34] C++：遍历 vector
来源：http://fa.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://em.hahajie.cn

[S35] C++：map
来源：http://gs.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aw.shtwfgs.cn

[S36] C++：unordered_map
来源：http://xb.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dt.asd995.cn

[S37] C++：set
来源：http://tr.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vc.hahajie.cn

[S38] C++：排序
来源：http://lz.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://gs.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://mb.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xe.szsharing.cn

[S40] C++：查找元素
来源：http://os.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ik.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://qs.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xx.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://ch.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://er.muxihuayi.cn

[S43] C++：智能指针
来源：http://lk.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://ki.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://py.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://ud.shxzukj.cn

[S45] C++：lambda
来源：http://wh.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ru.hahajie.cn

[S46] C++：函数模板
来源：http://qz.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ao.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://ay.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fg.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://nk.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rx.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://ez.shxzukj.cn

[S49] C++：写文件
来源：http://cl.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uz.szxytkj.cn

[S50] C++：格式化数字
来源：http://tl.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xs.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://uf.gzmigu.cn

static_cast<double>(a) / b
来源：http://cj.colortex.cn

[S52] C++：const 与 noexcept
来源：http://pi.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://dw.muxihuayi.cn

[S53] C++：移动语义
来源：http://os.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://by.muxihuayi.cn

[S54] C++：异常处理
来源：http://vl.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ig.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://fb.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ge.521024.cn

[S56] C++：optional
来源：http://br.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aw.newstarts.cn

[S57] C++：编译期常量
来源：http://gn.shxzskj.cn

constexpr int N = 10;
来源：http://kq.yuexingan06.cn

[S58] C++：命名空间
来源：http://xy.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://us.nszjky.cn

[S59] C++：静态断言
来源：http://ct.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sf.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://tz.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qk.colortex.cn

================================================================================
来源：http://hp.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lj.chemitech.net.cn

================================================================================
来源：http://wf.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://os.shtwfgs.cn

println("Hello")
来源：http://vn.gzmigu.cn

[T02] Kotlin：变量
来源：http://kz.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hh.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://lc.haigaiapp.cn

"值: $b"
来源：http://nd.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://iv.nicolike.cn

val n: String? = null;  n?.length
来源：http://my.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://fw.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bs.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://dr.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://et.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://eq.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sc.panjiajie.cn

[T08] Kotlin：数据类
来源：http://rt.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://fd.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://uj.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://ax.asd995.cn

[T10] Kotlin：默认参数
来源：http://pt.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gu.hnjuh.cn

[T11] Kotlin：协程
来源：http://ds.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pp.521024.cn

[T12] Kotlin：解构声明
来源：http://gw.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://qz.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://sh.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://vy.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://bx.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://bo.nicolike.cn

[T15] Kotlin：接口
来源：http://mr.hahajie.cn

interface Shape { fun area(): Double }
来源：http://mz.szxytkj.cn

[T16] Swift：Hello World
来源：http://si.jctech888.com.cn

print("Hello")
来源：http://bc.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://vz.wgjwhj.cn

var a = 1;  let b = 2
来源：http://dj.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://ut.521024.cn

"值: \(b)"
来源：http://tc.hnjuh.cn

[T19] Swift：可选绑定
来源：http://nm.muxihuayi.cn

if let n = opt { print(n) }
来源：http://wv.9csxet.cn

[T20] Swift：数组操作
来源：http://uv.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xg.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://ck.asd995.cn

for x in a { print(x) }
来源：http://xy.521024.cn

[T22] Swift：字典
来源：http://dp.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fh.panjiajie.cn

[T23] Swift：函数
来源：http://vc.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ws.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://vm.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ed.szsharing.cn

[T25] Swift：结构体
来源：http://jp.hnjuh.cn

struct P { var x: Int }
来源：http://md.muxihuayi.cn

[T26] Swift：类与重写
来源：http://iy.nicolike.cn

class A: Base { override func f() {} }
来源：http://ky.nszjky.cn


<!-- 参考信息 -->