代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ce.jctech888.com.cn

[R24] 大小写转换
来源：http://qe.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iy.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://ui.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rl.wgjwhj.cn

[R26] 命令替换
来源：http://vk.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://el.lnxyls.cn

[R27] 算术展开
来源：http://rg.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://an.wgjwhj.cn

[R28] 浮点运算
来源：http://vv.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://ll.shxzukj.cn

[R29] 定义函数
来源：http://cl.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wo.yuexingan06.cn

[R30] 函数返回状态码
来源：http://rt.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://sv.bjjhwx.cn

[R31] 局部变量
来源：http://uc.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://wm.lnxyls.cn

[R32] 参数个数校验
来源：http://nd.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ea.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://dm.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bz.nicolike.cn

[R34] 退出时清理
来源：http://ku.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jn.hnjuh.cn

[R35] 后台执行并等待
来源：http://tw.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xg.asd995.cn

[R36] 并发执行多个任务
来源：http://kx.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tu.shxzukj.cn

[R37] 把输出赋给变量
来源：http://lu.huixinmuqiang.cn

files=$(ls -1)
来源：http://kq.shxzskj.cn

[R38] 管道串联
来源：http://lq.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://xk.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://na.nszjky.cn

cmd > out.log 2>&1
来源：http://ju.9csxet.cn

[R40] 追加写日志
来源：http://xq.huixiangedu.cn

echo "log" >> out.log
来源：http://gn.chemitech.net.cn

[R41] 丢弃输出
来源：http://ye.9csxet.cn

cmd >/dev/null 2>&1
来源：http://pv.9csxet.cn

[R42] 输入重定向
来源：http://oy.huixiangedu.cn

wc -l < a.txt
来源：http://hu.chemitech.net.cn

[R43] 按名字查找文件
来源：http://uk.lnxyls.cn

find . -name "*.log" -type f
来源：http://zp.jctech888.com.cn

[R44] 按修改时间查找
来源：http://pi.colortex.cn

find . -mtime -7 -type f
来源：http://hv.jianghongdianzi.cn

[R45] 批量删除
来源：http://gw.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://ww.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://lf.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ru.bjjhwx.cn

[R47] sed 单行替换
来源：http://qe.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hk.bjjhwx.cn

[R48] awk 取指定列
来源：http://xv.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://vd.colortex.cn

[R49] awk 带条件
来源：http://sj.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fc.lnxyls.cn

[R50] awk 求和
来源：http://zh.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ie.chemitech.net.cn

[R51] 排序去重取前几
来源：http://bq.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kt.wgjwhj.cn

[R52] 统计行数
来源：http://iy.lnxyls.cn

wc -l a.txt
来源：http://oe.521024.cn

[R53] 查看文件头与实时尾
来源：http://lw.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sv.panjiajie.cn

[R54] 比较两个文件
来源：http://at.jctech888.com.cn

diff a.txt b.txt
来源：http://uh.521024.cn

[R55] 压缩与解压
来源：http://zd.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xt.haigaiapp.cn

[R56] 远程拷贝
来源：http://ei.colortex.cn

scp file user@host:/path/
来源：http://tf.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://ir.lnxyls.cn

ssh user@host 'uptime'
来源：http://yb.yuntaijiaju.cn

[R58] 下载文件
来源：http://yx.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gt.hahajie.cn

[R59] 发 POST JSON
来源：http://op.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hk.521024.cn

[R60] 只看 HTTP 状态码
来源：http://uj.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zt.colortex.cn

[R61] 磁盘占用
来源：http://gi.chemitech.net.cn

df -h;  du -sh *
来源：http://yb.huanxung.cn

[R62] 找最占空间的文件
来源：http://qk.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://ev.huixinmuqiang.cn

[R63] 内存与进程
来源：http://ca.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://pp.huixinmuqiang.cn

[R64] 结束进程
来源：http://mq.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://el.shxzskj.cn

[R65] 查看端口占用
来源：http://hq.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iw.asd995.cn

[R66] 定时任务
来源：http://rc.shtwfgs.cn

crontab -e;  crontab -l
来源：http://cb.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://cv.haigaiapp.cn

openssl rand -hex 16
来源：http://sv.521024.cn

[R68] 计算文件校验值
来源：http://sy.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nn.muxihuayi.cn

[R69] 生成随机密码
来源：http://kc.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://cx.colortex.cn

[R70] 时间戳与互转
来源：http://nj.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://va.huixinmuqiang.cn

[R71] 日期格式化
来源：http://yi.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fh.521024.cn

[R72] 等待端口就绪
来源：http://lz.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qe.shxzskj.cn

[R73] 分割大日志
来源：http://es.huanxung.cn

split -l 1000 big.log part_
来源：http://qs.asd995.cn

[R74] 批量重命名
来源：http://pi.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ub.huanxung.cn

[R75] 导出环境变量
来源：http://ly.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://sr.bookmarksfly.cn

[R76] 使用临时文件
来源：http://ca.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tn.szsharing.cn

[R77] 读取用户输入
来源：http://mb.huixiangedu.cn

read -rp "请输入: " ans
来源：http://ld.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://ba.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ag.yuexingan06.cn

[R79] 解析命令行选项
来源：http://cy.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dy.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://ts.bookmarksfly.cn

time ./run.sh
来源：http://uf.wgjwhj.cn

================================================================================
来源：http://vm.szxytkj.cn

S. C / C++ 专题
来源：http://tv.huanxung.cn

================================================================================
来源：http://nv.shtwfgs.cn

[S01] C：Hello World
来源：http://xq.lnxyls.cn

#include <stdio.h>
来源：http://au.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pi.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://gr.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://ay.wgjwhj.cn

[S03] C：读入整数
来源：http://qo.asd995.cn

int x; scanf("%d", &x);
来源：http://tp.bjjhwx.cn

[S04] C：字符串复制
来源：http://ow.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lo.gzmigu.cn

[S05] C：字符串长度
来源：http://ic.szxytkj.cn

strlen(s)
来源：http://ui.shtwfgs.cn

[S06] C：字符串比较
来源：http://gt.lnxyls.cn

strcmp(a, b) == 0
来源：http://it.9csxet.cn

[S07] C：数组遍历求和
来源：http://xx.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://my.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://wy.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ct.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://ke.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rg.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://na.nicolike.cn

int *p = &a;  *p = 5;
来源：http://ud.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://qy.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://mf.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://if.yuntaijiaju.cn

fclose(f);
来源：http://av.szxytkj.cn

[S12] C：写文件
来源：http://rc.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://df.panjiajie.cn

[S13] C：宏定义
来源：http://pg.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bg.colortex.cn

[S14] C：枚举
来源：http://zc.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://rx.nicolike.cn

[S15] C：类型转换
来源：http://jw.hahajie.cn

(double) a / b
来源：http://rh.yuexingan06.cn

[S16] C：位操作置位
来源：http://xv.gzmigu.cn

x |= (1 << 3);
来源：http://xx.newstarts.cn

[S17] C：安全拼接字符串
来源：http://xw.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dt.nicolike.cn

[S18] C：命令行参数
来源：http://rt.chemitech.net.cn

int main(int argc, char **argv)
来源：http://rt.asd995.cn

[S19] C：快速排序
来源：http://ol.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ar.lnxyls.cn

[S20] C：二分查找
来源：http://dz.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ut.panjiajie.cn

[S21] C：字符类别判断
来源：http://ao.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xo.haigaiapp.cn

[S22] C：字符串转数字
来源：http://lr.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sd.muxihuayi.cn

[S23] C：随机数
来源：http://zg.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qx.asd995.cn

[S24] C：获取本地时间
来源：http://jz.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rp.haigaiapp.cn

[S25] C：内存拷贝
来源：http://dq.shtwfgs.cn

memcpy(dst, src, n);
来源：http://iz.huixiangedu.cn

[S26] C：内存清零
来源：http://eo.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://tk.hahajie.cn

[S27] C：定义常量
来源：http://nc.521024.cn

const double PI = 3.14159;
来源：http://ih.bookmarksfly.cn

[S28] C：静态变量
来源：http://fa.9csxet.cn

static int counter = 0;
来源：http://tt.9csxet.cn

[S29] C：变参函数
来源：http://ge.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xu.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://is.huixiangedu.cn

#ifndef X_H
来源：http://rd.shxzskj.cn

#define X_H
来源：http://xo.gzmigu.cn

#endif
来源：http://fn.panjiajie.cn

[S31] C++：Hello World
来源：http://ky.shxzskj.cn

#include <iostream>
来源：http://tf.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://et.huixiangedu.cn

[S32] C++：字符串
来源：http://fj.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://ke.hnjuh.cn

[S33] C++：vector 增删
来源：http://sm.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aw.szsharing.cn

[S34] C++：遍历 vector
来源：http://pk.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://gb.huixiangedu.cn

[S35] C++：map
来源：http://op.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qd.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://xw.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eo.haigaiapp.cn

[S37] C++：set
来源：http://rw.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://id.chemitech.net.cn

[S38] C++：排序
来源：http://gm.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://aq.colortex.cn

[S39] C++：自定义比较器排序
来源：http://uo.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nf.colortex.cn

[S40] C++：查找元素
来源：http://er.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xh.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://ff.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wm.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://ek.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://mu.bookmarksfly.cn

[S43] C++：智能指针
来源：http://ph.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://nz.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://gg.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://so.nszjky.cn

[S45] C++：lambda
来源：http://de.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xj.haigaiapp.cn

[S46] C++：函数模板
来源：http://qd.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qd.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://fc.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rx.521024.cn

[S48] C++：逐行读文件
来源：http://pn.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://av.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://oy.gzmigu.cn

[S49] C++：写文件
来源：http://zv.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sc.gzmigu.cn

[S50] C++：格式化数字
来源：http://ie.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mr.huanxung.cn

[S51] C++：显式类型转换
来源：http://aw.gzmigu.cn

static_cast<double>(a) / b
来源：http://mn.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://ld.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://ft.shtwfgs.cn

[S53] C++：移动语义
来源：http://du.521024.cn

std::vector<int> w = std::move(v);
来源：http://gi.hnjuh.cn

[S54] C++：异常处理
来源：http://dm.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rs.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://ck.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mz.gzmigu.cn

[S56] C++：optional
来源：http://bf.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ls.shxzskj.cn

[S57] C++：编译期常量
来源：http://gr.521024.cn

constexpr int N = 10;
来源：http://ym.huanxung.cn

[S58] C++：命名空间
来源：http://xd.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://is.panjiajie.cn

[S59] C++：静态断言
来源：http://zh.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fr.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://mf.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://st.9csxet.cn

================================================================================
来源：http://sp.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qp.huixiangedu.cn

================================================================================
来源：http://es.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://kj.huixiangedu.cn

println("Hello")
来源：http://lv.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://wc.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zp.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://no.nszjky.cn

"值: $b"
来源：http://bz.nicolike.cn

[T04] Kotlin：空安全
来源：http://io.newstarts.cn

val n: String? = null;  n?.length
来源：http://ra.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://qq.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xi.nicolike.cn

[T06] Kotlin：集合映射
来源：http://gf.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bq.colortex.cn

[T07] Kotlin：集合过滤
来源：http://jz.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yp.shxzukj.cn

[T08] Kotlin：数据类
来源：http://od.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://rj.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://id.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://ua.asd995.cn

[T10] Kotlin：默认参数
来源：http://pc.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kt.muxihuayi.cn

[T11] Kotlin：协程
来源：http://xf.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ci.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://hw.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://ob.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://rq.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://ea.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://tf.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://sm.lnxyls.cn

[T15] Kotlin：接口
来源：http://yg.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://pf.huanxung.cn

[T16] Swift：Hello World
来源：http://ac.nszjky.cn

print("Hello")
来源：http://po.9csxet.cn

[T17] Swift：变量与常量
来源：http://pw.lnxyls.cn

var a = 1;  let b = 2
来源：http://ft.shxzskj.cn

[T18] Swift：字符串插值
来源：http://qu.yuexingan06.cn

"值: \(b)"
来源：http://md.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://zf.yuexingan06.cn

if let n = opt { print(n) }
来源：http://wn.asd995.cn

[T20] Swift：数组操作
来源：http://ll.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iz.jctech888.com.cn

[T21] Swift：遍历
来源：http://yk.shtwfgs.cn

for x in a { print(x) }
来源：http://kv.shxzskj.cn

[T22] Swift：字典
来源：http://ri.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mg.bookmarksfly.cn

[T23] Swift：函数
来源：http://qa.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yz.yuexingan06.cn

[T24] Swift：闭包
来源：http://ts.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ul.huanxung.cn

[T25] Swift：结构体
来源：http://hv.szsharing.cn

struct P { var x: Int }
来源：http://pv.lnxyls.cn

[T26] Swift：类与重写
来源：http://ba.szxytkj.cn

class A: Base { override func f() {} }
来源：http://ba.jctech888.com.cn


<!-- 参考信息 -->