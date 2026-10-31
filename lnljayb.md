代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ja.colortex.cn

[R24] 大小写转换
来源：http://wp.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://go.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://va.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://er.szxytkj.cn

[R26] 命令替换
来源：http://lq.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://bp.hnjuh.cn

[R27] 算术展开
来源：http://gt.szsharing.cn

echo $((1 + 2 * 3))
来源：http://dt.szsharing.cn

[R28] 浮点运算
来源：http://gn.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://nn.yuexingan06.cn

[R29] 定义函数
来源：http://tc.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oz.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://ix.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://jo.haigaiapp.cn

[R31] 局部变量
来源：http://vt.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://ap.9csxet.cn

[R32] 参数个数校验
来源：http://yi.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ay.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://tm.szxytkj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dx.huixiangedu.cn

[R34] 退出时清理
来源：http://yw.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eg.521024.cn

[R35] 后台执行并等待
来源：http://wn.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nf.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://ov.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ju.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://dp.shxzskj.cn

files=$(ls -1)
来源：http://db.asd995.cn

[R38] 管道串联
来源：http://zc.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://hw.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://bq.nicolike.cn

cmd > out.log 2>&1
来源：http://vj.yuntaijiaju.cn

[R40] 追加写日志
来源：http://pq.bookmarksfly.cn

echo "log" >> out.log
来源：http://lk.szxytkj.cn

[R41] 丢弃输出
来源：http://mx.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://tl.szxytkj.cn

[R42] 输入重定向
来源：http://io.szxytkj.cn

wc -l < a.txt
来源：http://cs.bjjhwx.cn

[R43] 按名字查找文件
来源：http://dc.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://hg.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://oo.newstarts.cn

find . -mtime -7 -type f
来源：http://nz.hnjuh.cn

[R45] 批量删除
来源：http://ql.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://sy.colortex.cn

[R46] 递归替换文件内容
来源：http://ng.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wd.asd995.cn

[R47] sed 单行替换
来源：http://zs.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zc.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://fc.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://ub.asd995.cn

[R49] awk 带条件
来源：http://ok.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xh.shtwfgs.cn

[R50] awk 求和
来源：http://pe.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ny.bjjhwx.cn

[R51] 排序去重取前几
来源：http://mu.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rm.gzmigu.cn

[R52] 统计行数
来源：http://nn.jctech888.com.cn

wc -l a.txt
来源：http://kl.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://ej.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://in.yuexingan06.cn

[R54] 比较两个文件
来源：http://nd.jctech888.com.cn

diff a.txt b.txt
来源：http://ps.panjiajie.cn

[R55] 压缩与解压
来源：http://tk.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yd.lnxyls.cn

[R56] 远程拷贝
来源：http://yd.jianghongdianzi.cn

scp file user@host:/path/
来源：http://vo.haigaiapp.cn

[R57] 远程执行命令
来源：http://sr.jctech888.com.cn

ssh user@host 'uptime'
来源：http://xy.chemitech.net.cn

[R58] 下载文件
来源：http://hv.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lq.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://dt.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xy.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://wn.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dn.szxytkj.cn

[R61] 磁盘占用
来源：http://rv.9csxet.cn

df -h;  du -sh *
来源：http://kt.nicolike.cn

[R62] 找最占空间的文件
来源：http://kt.521024.cn

du -ah . | sort -rh | head -10
来源：http://ay.bookmarksfly.cn

[R63] 内存与进程
来源：http://na.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://yq.bookmarksfly.cn

[R64] 结束进程
来源：http://ii.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://pr.hnjuh.cn

[R65] 查看端口占用
来源：http://hx.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vc.asd995.cn

[R66] 定时任务
来源：http://kg.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://pe.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://gc.nszjky.cn

openssl rand -hex 16
来源：http://xs.muxihuayi.cn

[R68] 计算文件校验值
来源：http://lj.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tf.szxytkj.cn

[R69] 生成随机密码
来源：http://fb.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://bz.9csxet.cn

[R70] 时间戳与互转
来源：http://xx.colortex.cn

date +%s;  date -d @1700000000
来源：http://je.hahajie.cn

[R71] 日期格式化
来源：http://kb.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rm.colortex.cn

[R72] 等待端口就绪
来源：http://oc.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nd.szsharing.cn

[R73] 分割大日志
来源：http://rw.asd995.cn

split -l 1000 big.log part_
来源：http://zs.panjiajie.cn

[R74] 批量重命名
来源：http://gd.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gb.jctech888.com.cn

[R75] 导出环境变量
来源：http://pf.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://ef.szxytkj.cn

[R76] 使用临时文件
来源：http://sd.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://en.panjiajie.cn

[R77] 读取用户输入
来源：http://ts.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://ij.shtwfgs.cn

[R78] 交互式菜单
来源：http://um.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dt.9csxet.cn

[R79] 解析命令行选项
来源：http://qq.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ma.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://df.nicolike.cn

time ./run.sh
来源：http://ky.wgjwhj.cn

================================================================================
来源：http://nj.huixiangedu.cn

S. C / C++ 专题
来源：http://rn.huixiangedu.cn

================================================================================
来源：http://bx.lnxyls.cn

[S01] C：Hello World
来源：http://ly.shxzskj.cn

#include <stdio.h>
来源：http://qy.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gv.9csxet.cn

[S02] C：变量与格式化输出
来源：http://yl.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://ve.hahajie.cn

[S03] C：读入整数
来源：http://nx.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://tx.asd995.cn

[S04] C：字符串复制
来源：http://wa.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://iv.szxytkj.cn

[S05] C：字符串长度
来源：http://cm.panjiajie.cn

strlen(s)
来源：http://vi.huixiangedu.cn

[S06] C：字符串比较
来源：http://wx.bjjhwx.cn

strcmp(a, b) == 0
来源：http://cf.shxzskj.cn

[S07] C：数组遍历求和
来源：http://fp.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pa.colortex.cn

[S08] C：动态内存分配与释放
来源：http://fv.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zb.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://bt.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ot.chemitech.net.cn

[S10] C：指针与解引用
来源：http://tv.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://iq.colortex.cn

[S11] C：逐行读文件
来源：http://yw.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://jy.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wc.jianghongdianzi.cn

fclose(f);
来源：http://ay.szxytkj.cn

[S12] C：写文件
来源：http://uj.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ih.9csxet.cn

[S13] C：宏定义
来源：http://um.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ob.muxihuayi.cn

[S14] C：枚举
来源：http://rl.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://my.huixinmuqiang.cn

[S15] C：类型转换
来源：http://sk.huixinmuqiang.cn

(double) a / b
来源：http://nd.szxytkj.cn

[S16] C：位操作置位
来源：http://ua.szxytkj.cn

x |= (1 << 3);
来源：http://ux.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://tr.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cx.shxzukj.cn

[S18] C：命令行参数
来源：http://mg.huixiangedu.cn

int main(int argc, char **argv)
来源：http://kq.shtwfgs.cn

[S19] C：快速排序
来源：http://nn.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bq.szsharing.cn

[S20] C：二分查找
来源：http://qq.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ta.panjiajie.cn

[S21] C：字符类别判断
来源：http://ku.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://li.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://ux.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wq.wgjwhj.cn

[S23] C：随机数
来源：http://ly.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://em.lnxyls.cn

[S24] C：获取本地时间
来源：http://hv.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ej.shxzskj.cn

[S25] C：内存拷贝
来源：http://cg.huanxung.cn

memcpy(dst, src, n);
来源：http://uq.huixinmuqiang.cn

[S26] C：内存清零
来源：http://nc.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://pl.shtwfgs.cn

[S27] C：定义常量
来源：http://nf.9csxet.cn

const double PI = 3.14159;
来源：http://lc.panjiajie.cn

[S28] C：静态变量
来源：http://wj.bjjhwx.cn

static int counter = 0;
来源：http://xj.huanxung.cn

[S29] C：变参函数
来源：http://qu.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qs.panjiajie.cn

[S30] C：头文件保护
来源：http://kt.gzmigu.cn

#ifndef X_H
来源：http://jx.szsharing.cn

#define X_H
来源：http://if.lnxyls.cn

#endif
来源：http://fg.nszjky.cn

[S31] C++：Hello World
来源：http://rr.huixinmuqiang.cn

#include <iostream>
来源：http://au.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://ld.nszjky.cn

[S32] C++：字符串
来源：http://cf.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://dq.panjiajie.cn

[S33] C++：vector 增删
来源：http://fb.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xw.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://os.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://hb.szsharing.cn

[S35] C++：map
来源：http://hs.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cc.jctech888.com.cn

[S36] C++：unordered_map
来源：http://if.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sp.colortex.cn

[S37] C++：set
来源：http://ni.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xw.shxzskj.cn

[S38] C++：排序
来源：http://as.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://zv.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://cy.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ky.9csxet.cn

[S40] C++：查找元素
来源：http://vq.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uu.9csxet.cn

[S41] C++：类与构造函数
来源：http://gw.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tx.9csxet.cn

[S42] C++：继承与虚函数
来源：http://zq.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://bj.shxzukj.cn

[S43] C++：智能指针
来源：http://mu.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://hv.yuexingan06.cn

[S44] C++：引用传参
来源：http://le.521024.cn

void inc(int &x) { ++x; }
来源：http://db.panjiajie.cn

[S45] C++：lambda
来源：http://mf.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ri.bookmarksfly.cn

[S46] C++：函数模板
来源：http://lw.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://je.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://qy.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cf.colortex.cn

[S48] C++：逐行读文件
来源：http://fy.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zl.newstarts.cn

while (std::getline(in, line)) { }
来源：http://ki.nicolike.cn

[S49] C++：写文件
来源：http://vj.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aj.hnjuh.cn

[S50] C++：格式化数字
来源：http://zr.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wm.szxytkj.cn

[S51] C++：显式类型转换
来源：http://ct.huanxung.cn

static_cast<double>(a) / b
来源：http://wf.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://og.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://je.hahajie.cn

[S53] C++：移动语义
来源：http://wo.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://ky.hahajie.cn

[S54] C++：异常处理
来源：http://tl.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vr.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://yu.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dz.shxzukj.cn

[S56] C++：optional
来源：http://ct.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ck.asd995.cn

[S57] C++：编译期常量
来源：http://ef.shtwfgs.cn

constexpr int N = 10;
来源：http://yt.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://vk.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://wr.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://by.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mf.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://eh.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zm.shxzukj.cn

================================================================================
来源：http://jg.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wb.huanxung.cn

================================================================================
来源：http://os.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://mq.panjiajie.cn

println("Hello")
来源：http://ee.bjjhwx.cn

[T02] Kotlin：变量
来源：http://jn.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zv.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://wp.huanxung.cn

"值: $b"
来源：http://fz.lnxyls.cn

[T04] Kotlin：空安全
来源：http://kd.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://sx.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://qu.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ra.huanxung.cn

[T06] Kotlin：集合映射
来源：http://by.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fz.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://ot.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dm.nicolike.cn

[T08] Kotlin：数据类
来源：http://hy.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://vm.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://ml.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://vk.nicolike.cn

[T10] Kotlin：默认参数
来源：http://oa.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://os.newstarts.cn

[T11] Kotlin：协程
来源：http://li.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ye.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://fi.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://bb.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://hi.9csxet.cn

val m = mapOf("a" to 1)
来源：http://bg.bjjhwx.cn

[T14] Kotlin：循环
来源：http://cb.huanxung.cn

for (i in 1..10) println(i)
来源：http://tp.nszjky.cn

[T15] Kotlin：接口
来源：http://sh.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://et.gzmigu.cn

[T16] Swift：Hello World
来源：http://qc.shxzskj.cn

print("Hello")
来源：http://fo.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://fl.gzmigu.cn

var a = 1;  let b = 2
来源：http://nu.hnjuh.cn

[T18] Swift：字符串插值
来源：http://pd.bjjhwx.cn

"值: \(b)"
来源：http://og.shxzukj.cn

[T19] Swift：可选绑定
来源：http://ez.muxihuayi.cn

if let n = opt { print(n) }
来源：http://ao.haigaiapp.cn

[T20] Swift：数组操作
来源：http://sq.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yk.nszjky.cn

[T21] Swift：遍历
来源：http://bz.wgjwhj.cn

for x in a { print(x) }
来源：http://rq.9csxet.cn

[T22] Swift：字典
来源：http://ct.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://td.bjjhwx.cn

[T23] Swift：函数
来源：http://be.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ac.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://ex.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://je.huixiangedu.cn

[T25] Swift：结构体
来源：http://gz.nszjky.cn

struct P { var x: Int }
来源：http://hr.chemitech.net.cn

[T26] Swift：类与重写
来源：http://xf.521024.cn

class A: Base { override func f() {} }
来源：http://an.newstarts.cn


<!-- 参考信息 -->