代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://mp.gzmigu.cn

[R18] 遍历数组
来源：http://kq.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gc.gzmigu.cn

[R19] 数组长度
来源：http://ot.newstarts.cn

echo "${#arr[@]}"
来源：http://px.shxzukj.cn

[R20] 关联数组（字典）
来源：http://xh.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gq.szsharing.cn

[R21] 字符串长度
来源：http://ce.lnxyls.cn

echo "${#s}"
来源：http://hr.haigaiapp.cn

[R22] 截取子串
来源：http://iv.521024.cn

echo "${s:0:5}"
来源：http://lm.muxihuayi.cn

[R23] 字符串替换
来源：http://sc.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cf.chemitech.net.cn

[R24] 大小写转换
来源：http://pz.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xe.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://uv.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://od.shxzukj.cn

[R26] 命令替换
来源：http://jl.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://uq.nszjky.cn

[R27] 算术展开
来源：http://jc.colortex.cn

echo $((1 + 2 * 3))
来源：http://mg.huixiangedu.cn

[R28] 浮点运算
来源：http://sx.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://bb.jctech888.com.cn

[R29] 定义函数
来源：http://kk.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pl.gzmigu.cn

[R30] 函数返回状态码
来源：http://of.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://sb.haigaiapp.cn

[R31] 局部变量
来源：http://fa.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://oc.asd995.cn

[R32] 参数个数校验
来源：http://hc.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bs.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://ds.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gw.521024.cn

[R34] 退出时清理
来源：http://fu.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qs.chemitech.net.cn

[R35] 后台执行并等待
来源：http://pw.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wo.nszjky.cn

[R36] 并发执行多个任务
来源：http://tn.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://js.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://ua.jctech888.com.cn

files=$(ls -1)
来源：http://rg.jianghongdianzi.cn

[R38] 管道串联
来源：http://qo.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://tt.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://vc.shxzskj.cn

cmd > out.log 2>&1
来源：http://wm.szsharing.cn

[R40] 追加写日志
来源：http://ps.jctech888.com.cn

echo "log" >> out.log
来源：http://hx.bookmarksfly.cn

[R41] 丢弃输出
来源：http://sk.nicolike.cn

cmd >/dev/null 2>&1
来源：http://zn.nicolike.cn

[R42] 输入重定向
来源：http://bl.9csxet.cn

wc -l < a.txt
来源：http://gd.huixiangedu.cn

[R43] 按名字查找文件
来源：http://ll.jctech888.com.cn

find . -name "*.log" -type f
来源：http://nj.nicolike.cn

[R44] 按修改时间查找
来源：http://xp.colortex.cn

find . -mtime -7 -type f
来源：http://oj.lnxyls.cn

[R45] 批量删除
来源：http://kr.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://ts.huanxung.cn

[R46] 递归替换文件内容
来源：http://zt.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mp.bjjhwx.cn

[R47] sed 单行替换
来源：http://po.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xu.shtwfgs.cn

[R48] awk 取指定列
来源：http://ts.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://rk.shxzskj.cn

[R49] awk 带条件
来源：http://sw.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nf.chemitech.net.cn

[R50] awk 求和
来源：http://vs.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tv.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://xm.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bo.gzmigu.cn

[R52] 统计行数
来源：http://ze.yuexingan06.cn

wc -l a.txt
来源：http://gw.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://wy.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xv.szsharing.cn

[R54] 比较两个文件
来源：http://we.shxzukj.cn

diff a.txt b.txt
来源：http://xk.chemitech.net.cn

[R55] 压缩与解压
来源：http://ep.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qy.wgjwhj.cn

[R56] 远程拷贝
来源：http://xa.yuntaijiaju.cn

scp file user@host:/path/
来源：http://eg.haigaiapp.cn

[R57] 远程执行命令
来源：http://ku.colortex.cn

ssh user@host 'uptime'
来源：http://ob.shtwfgs.cn

[R58] 下载文件
来源：http://ch.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ll.jctech888.com.cn

[R59] 发 POST JSON
来源：http://mt.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://st.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://uy.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fg.asd995.cn

[R61] 磁盘占用
来源：http://um.9csxet.cn

df -h;  du -sh *
来源：http://pp.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://xm.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://ct.nicolike.cn

[R63] 内存与进程
来源：http://hm.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://th.huixiangedu.cn

[R64] 结束进程
来源：http://yb.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://xp.jctech888.com.cn

[R65] 查看端口占用
来源：http://fm.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xw.haigaiapp.cn

[R66] 定时任务
来源：http://ov.colortex.cn

crontab -e;  crontab -l
来源：http://ng.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://gp.jianghongdianzi.cn

openssl rand -hex 16
来源：http://ld.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://tv.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wd.shxzukj.cn

[R69] 生成随机密码
来源：http://qo.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://el.bjjhwx.cn

[R70] 时间戳与互转
来源：http://fv.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://ed.colortex.cn

[R71] 日期格式化
来源：http://qr.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://im.bjjhwx.cn

[R72] 等待端口就绪
来源：http://dw.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fp.szxytkj.cn

[R73] 分割大日志
来源：http://gd.huixiangedu.cn

split -l 1000 big.log part_
来源：http://rt.wgjwhj.cn

[R74] 批量重命名
来源：http://ga.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aw.haigaiapp.cn

[R75] 导出环境变量
来源：http://mo.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://ri.chemitech.net.cn

[R76] 使用临时文件
来源：http://jy.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gk.hnjuh.cn

[R77] 读取用户输入
来源：http://nz.nicolike.cn

read -rp "请输入: " ans
来源：http://bq.wgjwhj.cn

[R78] 交互式菜单
来源：http://sp.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zk.panjiajie.cn

[R79] 解析命令行选项
来源：http://gw.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mo.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://lp.szsharing.cn

time ./run.sh
来源：http://wl.muxihuayi.cn

================================================================================
来源：http://xj.haigaiapp.cn

S. C / C++ 专题
来源：http://jr.bjjhwx.cn

================================================================================
来源：http://mm.wgjwhj.cn

[S01] C：Hello World
来源：http://pa.yuexingan06.cn

#include <stdio.h>
来源：http://br.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bk.521024.cn

[S02] C：变量与格式化输出
来源：http://hg.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://gm.szsharing.cn

[S03] C：读入整数
来源：http://zj.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://mo.gzmigu.cn

[S04] C：字符串复制
来源：http://zx.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ru.shxzukj.cn

[S05] C：字符串长度
来源：http://cj.huixinmuqiang.cn

strlen(s)
来源：http://ex.lnxyls.cn

[S06] C：字符串比较
来源：http://gq.huixiangedu.cn

strcmp(a, b) == 0
来源：http://vc.asd995.cn

[S07] C：数组遍历求和
来源：http://oq.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cm.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://in.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qg.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://tn.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ug.szsharing.cn

[S10] C：指针与解引用
来源：http://sl.szsharing.cn

int *p = &a;  *p = 5;
来源：http://ka.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://sj.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://dy.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ke.huixiangedu.cn

fclose(f);
来源：http://xh.szxytkj.cn

[S12] C：写文件
来源：http://qf.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bg.bookmarksfly.cn

[S13] C：宏定义
来源：http://pp.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eg.9csxet.cn

[S14] C：枚举
来源：http://ni.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://dn.haigaiapp.cn

[S15] C：类型转换
来源：http://sy.huanxung.cn

(double) a / b
来源：http://yi.muxihuayi.cn

[S16] C：位操作置位
来源：http://ez.colortex.cn

x |= (1 << 3);
来源：http://hv.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://nv.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pv.chemitech.net.cn

[S18] C：命令行参数
来源：http://he.chemitech.net.cn

int main(int argc, char **argv)
来源：http://pg.panjiajie.cn

[S19] C：快速排序
来源：http://vb.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zy.huixinmuqiang.cn

[S20] C：二分查找
来源：http://by.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gk.panjiajie.cn

[S21] C：字符类别判断
来源：http://yo.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ar.gzmigu.cn

[S22] C：字符串转数字
来源：http://zi.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rz.huixiangedu.cn

[S23] C：随机数
来源：http://wz.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yc.huanxung.cn

[S24] C：获取本地时间
来源：http://ra.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vr.haigaiapp.cn

[S25] C：内存拷贝
来源：http://cy.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://at.lnxyls.cn

[S26] C：内存清零
来源：http://fx.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://sp.szxytkj.cn

[S27] C：定义常量
来源：http://pi.szxytkj.cn

const double PI = 3.14159;
来源：http://uq.bjjhwx.cn

[S28] C：静态变量
来源：http://lh.jianghongdianzi.cn

static int counter = 0;
来源：http://ie.chemitech.net.cn

[S29] C：变参函数
来源：http://ra.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://to.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://qi.wgjwhj.cn

#ifndef X_H
来源：http://ik.newstarts.cn

#define X_H
来源：http://bu.lnxyls.cn

#endif
来源：http://vr.shtwfgs.cn

[S31] C++：Hello World
来源：http://ph.shtwfgs.cn

#include <iostream>
来源：http://vm.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://jf.9csxet.cn

[S32] C++：字符串
来源：http://nc.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://oz.muxihuayi.cn

[S33] C++：vector 增删
来源：http://mx.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bs.hnjuh.cn

[S34] C++：遍历 vector
来源：http://qg.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://od.panjiajie.cn

[S35] C++：map
来源：http://xz.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uy.muxihuayi.cn

[S36] C++：unordered_map
来源：http://nj.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dv.newstarts.cn

[S37] C++：set
来源：http://yn.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ln.bookmarksfly.cn

[S38] C++：排序
来源：http://cb.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://lc.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://bs.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pa.shtwfgs.cn

[S40] C++：查找元素
来源：http://fd.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tl.colortex.cn

[S41] C++：类与构造函数
来源：http://xt.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pm.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://mv.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://te.colortex.cn

[S43] C++：智能指针
来源：http://fd.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://uy.lnxyls.cn

[S44] C++：引用传参
来源：http://ze.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://as.shtwfgs.cn

[S45] C++：lambda
来源：http://uf.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ln.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://qu.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sw.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://tu.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://og.shxzskj.cn

[S48] C++：逐行读文件
来源：http://eq.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nu.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://sk.lnxyls.cn

[S49] C++：写文件
来源：http://lh.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hp.nszjky.cn

[S50] C++：格式化数字
来源：http://ez.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dz.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://yg.bjjhwx.cn

static_cast<double>(a) / b
来源：http://hv.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://zy.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://ul.shtwfgs.cn

[S53] C++：移动语义
来源：http://zd.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://qi.shxzskj.cn

[S54] C++：异常处理
来源：http://hp.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yo.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://pc.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ey.bjjhwx.cn

[S56] C++：optional
来源：http://oq.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nt.gzmigu.cn

[S57] C++：编译期常量
来源：http://dy.szsharing.cn

constexpr int N = 10;
来源：http://vc.bookmarksfly.cn

[S58] C++：命名空间
来源：http://rt.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://fe.haigaiapp.cn

[S59] C++：静态断言
来源：http://qv.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xg.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://jn.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cy.lnxyls.cn

================================================================================
来源：http://rp.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xl.wgjwhj.cn

================================================================================
来源：http://ci.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://aa.jianghongdianzi.cn

println("Hello")
来源：http://jz.huanxung.cn

[T02] Kotlin：变量
来源：http://xb.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ip.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://ub.asd995.cn

"值: $b"
来源：http://wp.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://fg.huanxung.cn

val n: String? = null;  n?.length
来源：http://jj.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://ie.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hl.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://jf.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://de.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://vk.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zz.nicolike.cn

[T08] Kotlin：数据类
来源：http://ui.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://cz.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://pw.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://vi.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://wj.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ki.gzmigu.cn

[T11] Kotlin：协程
来源：http://rd.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nc.9csxet.cn

[T12] Kotlin：解构声明
来源：http://ok.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://hm.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://nb.521024.cn

val m = mapOf("a" to 1)
来源：http://ak.shxzukj.cn

[T14] Kotlin：循环
来源：http://gx.nicolike.cn

for (i in 1..10) println(i)
来源：http://kd.hnjuh.cn

[T15] Kotlin：接口
来源：http://yr.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://rd.haigaiapp.cn

[T16] Swift：Hello World
来源：http://ub.9csxet.cn

print("Hello")
来源：http://qh.521024.cn

[T17] Swift：变量与常量
来源：http://qg.asd995.cn

var a = 1;  let b = 2
来源：http://ad.panjiajie.cn

[T18] Swift：字符串插值
来源：http://mf.yuexingan06.cn

"值: \(b)"
来源：http://fd.huanxung.cn

[T19] Swift：可选绑定
来源：http://du.haigaiapp.cn

if let n = opt { print(n) }
来源：http://xc.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://fw.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hg.muxihuayi.cn


<!-- 参考信息 -->