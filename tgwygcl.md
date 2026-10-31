代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://li.newstarts.cn

[R24] 大小写转换
来源：http://yo.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://os.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://bu.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zu.shtwfgs.cn

[R26] 命令替换
来源：http://ql.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://ep.hahajie.cn

[R27] 算术展开
来源：http://wo.9csxet.cn

echo $((1 + 2 * 3))
来源：http://yl.huixinmuqiang.cn

[R28] 浮点运算
来源：http://np.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://bt.yuexingan06.cn

[R29] 定义函数
来源：http://az.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yy.huixiangedu.cn

[R30] 函数返回状态码
来源：http://xw.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://qk.newstarts.cn

[R31] 局部变量
来源：http://gl.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://jt.bjjhwx.cn

[R32] 参数个数校验
来源：http://we.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zn.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://fi.bookmarksfly.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zx.colortex.cn

[R34] 退出时清理
来源：http://vn.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ob.newstarts.cn

[R35] 后台执行并等待
来源：http://aj.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wr.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://kq.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://em.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://fq.shxzukj.cn

files=$(ls -1)
来源：http://uy.haigaiapp.cn

[R38] 管道串联
来源：http://tc.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://iu.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://pe.newstarts.cn

cmd > out.log 2>&1
来源：http://ix.newstarts.cn

[R40] 追加写日志
来源：http://fb.gzmigu.cn

echo "log" >> out.log
来源：http://tt.asd995.cn

[R41] 丢弃输出
来源：http://tf.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://fv.colortex.cn

[R42] 输入重定向
来源：http://ku.szsharing.cn

wc -l < a.txt
来源：http://ny.wgjwhj.cn

[R43] 按名字查找文件
来源：http://pm.huanxung.cn

find . -name "*.log" -type f
来源：http://ie.chemitech.net.cn

[R44] 按修改时间查找
来源：http://iq.gzmigu.cn

find . -mtime -7 -type f
来源：http://zq.huixinmuqiang.cn

[R45] 批量删除
来源：http://xs.hahajie.cn

find . -name "*.tmp" -delete
来源：http://gx.szxytkj.cn

[R46] 递归替换文件内容
来源：http://kv.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wg.lnxyls.cn

[R47] sed 单行替换
来源：http://jj.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qh.szxytkj.cn

[R48] awk 取指定列
来源：http://mb.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://iy.gzmigu.cn

[R49] awk 带条件
来源：http://mi.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dw.asd995.cn

[R50] awk 求和
来源：http://qh.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rc.muxihuayi.cn

[R51] 排序去重取前几
来源：http://kc.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tp.huixiangedu.cn

[R52] 统计行数
来源：http://yb.szsharing.cn

wc -l a.txt
来源：http://rp.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://md.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qm.huixiangedu.cn

[R54] 比较两个文件
来源：http://cw.bjjhwx.cn

diff a.txt b.txt
来源：http://wa.shxzskj.cn

[R55] 压缩与解压
来源：http://zl.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://on.newstarts.cn

[R56] 远程拷贝
来源：http://sg.huixinmuqiang.cn

scp file user@host:/path/
来源：http://ul.shxzukj.cn

[R57] 远程执行命令
来源：http://vg.gzmigu.cn

ssh user@host 'uptime'
来源：http://ty.chemitech.net.cn

[R58] 下载文件
来源：http://sp.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dc.huanxung.cn

[R59] 发 POST JSON
来源：http://em.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xy.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://na.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yc.asd995.cn

[R61] 磁盘占用
来源：http://pz.yuexingan06.cn

df -h;  du -sh *
来源：http://zs.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://fj.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://rv.muxihuayi.cn

[R63] 内存与进程
来源：http://as.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://fv.lnxyls.cn

[R64] 结束进程
来源：http://ay.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://ft.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://we.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wa.asd995.cn

[R66] 定时任务
来源：http://jw.9csxet.cn

crontab -e;  crontab -l
来源：http://ou.hahajie.cn

[R67] 生成随机十六进制串
来源：http://rg.bookmarksfly.cn

openssl rand -hex 16
来源：http://mj.huixiangedu.cn

[R68] 计算文件校验值
来源：http://te.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dw.newstarts.cn

[R69] 生成随机密码
来源：http://cl.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://su.lnxyls.cn

[R70] 时间戳与互转
来源：http://xn.nszjky.cn

date +%s;  date -d @1700000000
来源：http://vj.haigaiapp.cn

[R71] 日期格式化
来源：http://qc.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://am.muxihuayi.cn

[R72] 等待端口就绪
来源：http://df.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ed.haigaiapp.cn

[R73] 分割大日志
来源：http://qr.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://iz.wgjwhj.cn

[R74] 批量重命名
来源：http://un.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gy.wgjwhj.cn

[R75] 导出环境变量
来源：http://an.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://xe.huanxung.cn

[R76] 使用临时文件
来源：http://no.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ki.muxihuayi.cn

[R77] 读取用户输入
来源：http://kh.muxihuayi.cn

read -rp "请输入: " ans
来源：http://af.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://vr.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ni.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://kd.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wj.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://dy.hnjuh.cn

time ./run.sh
来源：http://dt.nicolike.cn

================================================================================
来源：http://bt.yuexingan06.cn

S. C / C++ 专题
来源：http://tw.nicolike.cn

================================================================================
来源：http://js.wgjwhj.cn

[S01] C：Hello World
来源：http://mc.chemitech.net.cn

#include <stdio.h>
来源：http://po.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rd.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://wb.521024.cn

int a = 10; printf("%d\n", a);
来源：http://rg.shtwfgs.cn

[S03] C：读入整数
来源：http://dl.asd995.cn

int x; scanf("%d", &x);
来源：http://wq.nicolike.cn

[S04] C：字符串复制
来源：http://jk.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://or.szsharing.cn

[S05] C：字符串长度
来源：http://mt.wgjwhj.cn

strlen(s)
来源：http://pk.newstarts.cn

[S06] C：字符串比较
来源：http://yo.hnjuh.cn

strcmp(a, b) == 0
来源：http://gz.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://gy.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qq.asd995.cn

[S08] C：动态内存分配与释放
来源：http://ad.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ay.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://ct.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://je.wgjwhj.cn

[S10] C：指针与解引用
来源：http://oo.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://ag.huanxung.cn

[S11] C：逐行读文件
来源：http://hr.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://lf.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uq.szxytkj.cn

fclose(f);
来源：http://yj.hahajie.cn

[S12] C：写文件
来源：http://cu.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dh.bjjhwx.cn

[S13] C：宏定义
来源：http://ol.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sh.521024.cn

[S14] C：枚举
来源：http://ct.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://jd.gzmigu.cn

[S15] C：类型转换
来源：http://kb.gzmigu.cn

(double) a / b
来源：http://rg.asd995.cn

[S16] C：位操作置位
来源：http://qq.huixiangedu.cn

x |= (1 << 3);
来源：http://cp.hahajie.cn

[S17] C：安全拼接字符串
来源：http://zu.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cu.szxytkj.cn

[S18] C：命令行参数
来源：http://js.yuexingan06.cn

int main(int argc, char **argv)
来源：http://sf.hnjuh.cn

[S19] C：快速排序
来源：http://tp.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nb.wgjwhj.cn

[S20] C：二分查找
来源：http://jc.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nn.huixiangedu.cn

[S21] C：字符类别判断
来源：http://dy.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ew.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://sv.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hy.521024.cn

[S23] C：随机数
来源：http://hm.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rc.colortex.cn

[S24] C：获取本地时间
来源：http://re.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uf.hahajie.cn

[S25] C：内存拷贝
来源：http://pg.nszjky.cn

memcpy(dst, src, n);
来源：http://yb.nszjky.cn

[S26] C：内存清零
来源：http://oa.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://fs.hahajie.cn

[S27] C：定义常量
来源：http://jm.asd995.cn

const double PI = 3.14159;
来源：http://pd.haigaiapp.cn

[S28] C：静态变量
来源：http://xv.jianghongdianzi.cn

static int counter = 0;
来源：http://ox.panjiajie.cn

[S29] C：变参函数
来源：http://zv.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dp.hahajie.cn

[S30] C：头文件保护
来源：http://iv.hahajie.cn

#ifndef X_H
来源：http://cp.hahajie.cn

#define X_H
来源：http://iv.huixiangedu.cn

#endif
来源：http://co.szsharing.cn

[S31] C++：Hello World
来源：http://dc.bookmarksfly.cn

#include <iostream>
来源：http://hb.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://cm.bookmarksfly.cn

[S32] C++：字符串
来源：http://ir.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://by.jctech888.com.cn

[S33] C++：vector 增删
来源：http://ey.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hf.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://bk.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://dz.colortex.cn

[S35] C++：map
来源：http://eo.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mf.colortex.cn

[S36] C++：unordered_map
来源：http://hp.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ex.szxytkj.cn

[S37] C++：set
来源：http://bt.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yn.yuexingan06.cn

[S38] C++：排序
来源：http://qw.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://nm.asd995.cn

[S39] C++：自定义比较器排序
来源：http://rj.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rt.shxzskj.cn

[S40] C++：查找元素
来源：http://dt.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sz.hahajie.cn

[S41] C++：类与构造函数
来源：http://wf.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wf.521024.cn

[S42] C++：继承与虚函数
来源：http://jy.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://cc.panjiajie.cn

[S43] C++：智能指针
来源：http://xv.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://ya.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://ai.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://gw.gzmigu.cn

[S45] C++：lambda
来源：http://kr.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dt.yuexingan06.cn

[S46] C++：函数模板
来源：http://ak.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pd.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://in.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tf.gzmigu.cn

[S48] C++：逐行读文件
来源：http://wx.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nf.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://lg.yuexingan06.cn

[S49] C++：写文件
来源：http://rk.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wt.521024.cn

[S50] C++：格式化数字
来源：http://re.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kr.asd995.cn

[S51] C++：显式类型转换
来源：http://zi.shtwfgs.cn

static_cast<double>(a) / b
来源：http://gb.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://uq.9csxet.cn

int size() const noexcept { return n_; }
来源：http://hu.szxytkj.cn

[S53] C++：移动语义
来源：http://be.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://rz.shxzukj.cn

[S54] C++：异常处理
来源：http://nl.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jb.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://jo.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://be.jctech888.com.cn

[S56] C++：optional
来源：http://ro.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ea.hahajie.cn

[S57] C++：编译期常量
来源：http://xx.wgjwhj.cn

constexpr int N = 10;
来源：http://sb.bjjhwx.cn

[S58] C++：命名空间
来源：http://ze.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://ng.shxzskj.cn

[S59] C++：静态断言
来源：http://ky.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kx.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://nb.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sf.lnxyls.cn

================================================================================
来源：http://iv.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ou.colortex.cn

================================================================================
来源：http://xc.asd995.cn

[T01] Kotlin：Hello World
来源：http://py.shtwfgs.cn

println("Hello")
来源：http://lr.nszjky.cn

[T02] Kotlin：变量
来源：http://wr.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://th.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://xb.huanxung.cn

"值: $b"
来源：http://vq.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://cr.hahajie.cn

val n: String? = null;  n?.length
来源：http://ge.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://cx.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gm.huanxung.cn

[T06] Kotlin：集合映射
来源：http://yp.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sm.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://fo.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qy.9csxet.cn

[T08] Kotlin：数据类
来源：http://xf.521024.cn

data class User(val name: String, val age: Int)
来源：http://jz.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://cn.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://en.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://an.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bw.muxihuayi.cn

[T11] Kotlin：协程
来源：http://tm.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ry.newstarts.cn

[T12] Kotlin：解构声明
来源：http://av.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://hu.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://cl.newstarts.cn

val m = mapOf("a" to 1)
来源：http://jg.szxytkj.cn

[T14] Kotlin：循环
来源：http://lx.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://fa.521024.cn

[T15] Kotlin：接口
来源：http://gd.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://vm.asd995.cn

[T16] Swift：Hello World
来源：http://hw.huixinmuqiang.cn

print("Hello")
来源：http://rs.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://io.huixiangedu.cn

var a = 1;  let b = 2
来源：http://mq.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://is.szxytkj.cn

"值: \(b)"
来源：http://yc.huanxung.cn

[T19] Swift：可选绑定
来源：http://rr.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://go.szxytkj.cn

[T20] Swift：数组操作
来源：http://ay.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fh.nszjky.cn

[T21] Swift：遍历
来源：http://nq.yuexingan06.cn

for x in a { print(x) }
来源：http://ct.nszjky.cn

[T22] Swift：字典
来源：http://qx.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ie.szxytkj.cn

[T23] Swift：函数
来源：http://cf.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://su.huixiangedu.cn

[T24] Swift：闭包
来源：http://ty.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://no.haigaiapp.cn

[T25] Swift：结构体
来源：http://al.jctech888.com.cn

struct P { var x: Int }
来源：http://hv.shxzukj.cn

[T26] Swift：类与重写
来源：http://eq.9csxet.cn

class A: Base { override func f() {} }
来源：http://hk.huixinmuqiang.cn


<!-- 参考信息 -->