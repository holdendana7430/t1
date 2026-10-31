代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://aj.szsharing.cn

[R18] 遍历数组
来源：http://hp.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nf.asd995.cn

[R19] 数组长度
来源：http://zc.huixiangedu.cn

echo "${#arr[@]}"
来源：http://ns.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://ew.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gb.521024.cn

[R21] 字符串长度
来源：http://tt.newstarts.cn

echo "${#s}"
来源：http://sp.yuntaijiaju.cn

[R22] 截取子串
来源：http://ts.nszjky.cn

echo "${s:0:5}"
来源：http://hw.9csxet.cn

[R23] 字符串替换
来源：http://rr.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ul.yuntaijiaju.cn

[R24] 大小写转换
来源：http://dd.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cj.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://sa.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://on.chemitech.net.cn

[R26] 命令替换
来源：http://ec.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://ja.shtwfgs.cn

[R27] 算术展开
来源：http://vs.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://jo.bookmarksfly.cn

[R28] 浮点运算
来源：http://wr.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://ja.jianghongdianzi.cn

[R29] 定义函数
来源：http://rx.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xj.muxihuayi.cn

[R30] 函数返回状态码
来源：http://yb.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://qn.yuntaijiaju.cn

[R31] 局部变量
来源：http://wp.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://xh.shxzukj.cn

[R32] 参数个数校验
来源：http://go.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://od.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://co.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yy.521024.cn

[R34] 退出时清理
来源：http://rb.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xq.wgjwhj.cn

[R35] 后台执行并等待
来源：http://fy.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zn.szxytkj.cn

[R36] 并发执行多个任务
来源：http://hc.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cb.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://fk.huixinmuqiang.cn

files=$(ls -1)
来源：http://iz.huanxung.cn

[R38] 管道串联
来源：http://jw.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://eu.colortex.cn

[R39] 重定向标准输出与错误
来源：http://tw.panjiajie.cn

cmd > out.log 2>&1
来源：http://fp.9csxet.cn

[R40] 追加写日志
来源：http://ad.jianghongdianzi.cn

echo "log" >> out.log
来源：http://zs.huanxung.cn

[R41] 丢弃输出
来源：http://pe.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://xi.chemitech.net.cn

[R42] 输入重定向
来源：http://lp.jctech888.com.cn

wc -l < a.txt
来源：http://io.nicolike.cn

[R43] 按名字查找文件
来源：http://te.gzmigu.cn

find . -name "*.log" -type f
来源：http://nw.shtwfgs.cn

[R44] 按修改时间查找
来源：http://xj.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://ge.szxytkj.cn

[R45] 批量删除
来源：http://ip.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://pg.huanxung.cn

[R46] 递归替换文件内容
来源：http://it.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bh.chemitech.net.cn

[R47] sed 单行替换
来源：http://ic.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ru.nszjky.cn

[R48] awk 取指定列
来源：http://uf.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://bd.shxzskj.cn

[R49] awk 带条件
来源：http://jc.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kv.huanxung.cn

[R50] awk 求和
来源：http://pw.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://is.nszjky.cn

[R51] 排序去重取前几
来源：http://cz.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jv.gzmigu.cn

[R52] 统计行数
来源：http://oo.huixiangedu.cn

wc -l a.txt
来源：http://sz.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://ht.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://au.huixiangedu.cn

[R54] 比较两个文件
来源：http://rh.521024.cn

diff a.txt b.txt
来源：http://qv.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://hw.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hm.hnjuh.cn

[R56] 远程拷贝
来源：http://op.lnxyls.cn

scp file user@host:/path/
来源：http://wf.szsharing.cn

[R57] 远程执行命令
来源：http://bx.gzmigu.cn

ssh user@host 'uptime'
来源：http://cw.shtwfgs.cn

[R58] 下载文件
来源：http://bg.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://if.shxzukj.cn

[R59] 发 POST JSON
来源：http://ok.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ty.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://vb.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://al.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://rg.muxihuayi.cn

df -h;  du -sh *
来源：http://xv.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://im.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://hq.shxzukj.cn

[R63] 内存与进程
来源：http://et.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://re.haigaiapp.cn

[R64] 结束进程
来源：http://ej.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://qw.asd995.cn

[R65] 查看端口占用
来源：http://hv.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sx.yuexingan06.cn

[R66] 定时任务
来源：http://zz.asd995.cn

crontab -e;  crontab -l
来源：http://ll.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://vx.wgjwhj.cn

openssl rand -hex 16
来源：http://ag.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://ek.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wu.asd995.cn

[R69] 生成随机密码
来源：http://is.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://ep.jctech888.com.cn

[R70] 时间戳与互转
来源：http://lh.huanxung.cn

date +%s;  date -d @1700000000
来源：http://cr.asd995.cn

[R71] 日期格式化
来源：http://rv.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ao.shtwfgs.cn

[R72] 等待端口就绪
来源：http://rw.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hc.huanxung.cn

[R73] 分割大日志
来源：http://zq.shtwfgs.cn

split -l 1000 big.log part_
来源：http://eo.panjiajie.cn

[R74] 批量重命名
来源：http://ck.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fx.hnjuh.cn

[R75] 导出环境变量
来源：http://il.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://vh.newstarts.cn

[R76] 使用临时文件
来源：http://ie.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mn.lnxyls.cn

[R77] 读取用户输入
来源：http://oi.haigaiapp.cn

read -rp "请输入: " ans
来源：http://br.muxihuayi.cn

[R78] 交互式菜单
来源：http://sr.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mz.shxzskj.cn

[R79] 解析命令行选项
来源：http://nc.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wh.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://mn.bookmarksfly.cn

time ./run.sh
来源：http://az.shtwfgs.cn

================================================================================
来源：http://tj.yuexingan06.cn

S. C / C++ 专题
来源：http://ub.shxzskj.cn

================================================================================
来源：http://ot.muxihuayi.cn

[S01] C：Hello World
来源：http://tn.szsharing.cn

#include <stdio.h>
来源：http://qw.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gg.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://uq.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://jt.lnxyls.cn

[S03] C：读入整数
来源：http://fb.hahajie.cn

int x; scanf("%d", &x);
来源：http://sg.hnjuh.cn

[S04] C：字符串复制
来源：http://ff.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zj.panjiajie.cn

[S05] C：字符串长度
来源：http://wy.panjiajie.cn

strlen(s)
来源：http://xm.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://hr.hahajie.cn

strcmp(a, b) == 0
来源：http://gd.panjiajie.cn

[S07] C：数组遍历求和
来源：http://hr.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kq.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://as.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lj.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://rw.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://am.jctech888.com.cn

[S10] C：指针与解引用
来源：http://ja.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://ya.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://tu.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://vl.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jn.nszjky.cn

fclose(f);
来源：http://qd.hnjuh.cn

[S12] C：写文件
来源：http://im.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bo.panjiajie.cn

[S13] C：宏定义
来源：http://ie.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nu.shtwfgs.cn

[S14] C：枚举
来源：http://hz.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://sm.hahajie.cn

[S15] C：类型转换
来源：http://bx.shxzukj.cn

(double) a / b
来源：http://ja.panjiajie.cn

[S16] C：位操作置位
来源：http://dy.colortex.cn

x |= (1 << 3);
来源：http://ef.asd995.cn

[S17] C：安全拼接字符串
来源：http://ac.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sd.hnjuh.cn

[S18] C：命令行参数
来源：http://jn.szsharing.cn

int main(int argc, char **argv)
来源：http://zo.szsharing.cn

[S19] C：快速排序
来源：http://zf.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xe.huixinmuqiang.cn

[S20] C：二分查找
来源：http://xo.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sm.chemitech.net.cn

[S21] C：字符类别判断
来源：http://el.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://id.huanxung.cn

[S22] C：字符串转数字
来源：http://sc.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kc.yuexingan06.cn

[S23] C：随机数
来源：http://rn.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xl.wgjwhj.cn

[S24] C：获取本地时间
来源：http://nf.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dw.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://jq.9csxet.cn

memcpy(dst, src, n);
来源：http://cy.shxzukj.cn

[S26] C：内存清零
来源：http://kn.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://dx.asd995.cn

[S27] C：定义常量
来源：http://kq.newstarts.cn

const double PI = 3.14159;
来源：http://gx.yuntaijiaju.cn

[S28] C：静态变量
来源：http://ml.shxzskj.cn

static int counter = 0;
来源：http://xp.yuntaijiaju.cn

[S29] C：变参函数
来源：http://yb.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zy.szxytkj.cn

[S30] C：头文件保护
来源：http://cs.shtwfgs.cn

#ifndef X_H
来源：http://qx.yuntaijiaju.cn

#define X_H
来源：http://lm.shxzskj.cn

#endif
来源：http://hc.haigaiapp.cn

[S31] C++：Hello World
来源：http://ws.haigaiapp.cn

#include <iostream>
来源：http://sp.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://qp.yuntaijiaju.cn

[S32] C++：字符串
来源：http://xo.colortex.cn

std::string s = "hi";  s += "!";
来源：http://ei.muxihuayi.cn

[S33] C++：vector 增删
来源：http://bo.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ny.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://ai.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://is.hahajie.cn

[S35] C++：map
来源：http://xu.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hn.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://am.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cb.newstarts.cn

[S37] C++：set
来源：http://sw.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://js.bookmarksfly.cn

[S38] C++：排序
来源：http://ou.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://sb.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://kq.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yb.521024.cn

[S40] C++：查找元素
来源：http://gq.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mp.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://ou.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fn.asd995.cn

[S42] C++：继承与虚函数
来源：http://xi.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://kz.huixiangedu.cn

[S43] C++：智能指针
来源：http://xj.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://ys.panjiajie.cn

[S44] C++：引用传参
来源：http://cm.asd995.cn

void inc(int &x) { ++x; }
来源：http://mz.huixiangedu.cn

[S45] C++：lambda
来源：http://ux.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pr.bjjhwx.cn

[S46] C++：函数模板
来源：http://qg.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fr.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://bs.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rp.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://og.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://er.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://nv.asd995.cn

[S49] C++：写文件
来源：http://jb.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bh.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://ri.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wl.gzmigu.cn

[S51] C++：显式类型转换
来源：http://bs.jctech888.com.cn

static_cast<double>(a) / b
来源：http://xb.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://uk.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://cx.colortex.cn

[S53] C++：移动语义
来源：http://ai.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://vm.jctech888.com.cn

[S54] C++：异常处理
来源：http://hp.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hd.huanxung.cn

[S55] C++：结构化绑定
来源：http://nb.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cf.colortex.cn

[S56] C++：optional
来源：http://uh.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oc.muxihuayi.cn

[S57] C++：编译期常量
来源：http://eb.szxytkj.cn

constexpr int N = 10;
来源：http://nl.bookmarksfly.cn

[S58] C++：命名空间
来源：http://kz.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://ea.yuntaijiaju.cn

[S59] C++：静态断言
来源：http://nh.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ws.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://xu.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ui.hahajie.cn

================================================================================
来源：http://zt.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kk.yuexingan06.cn

================================================================================
来源：http://ks.huanxung.cn

[T01] Kotlin：Hello World
来源：http://dn.yuexingan06.cn

println("Hello")
来源：http://vp.huanxung.cn

[T02] Kotlin：变量
来源：http://au.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rb.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://py.panjiajie.cn

"值: $b"
来源：http://zu.lnxyls.cn

[T04] Kotlin：空安全
来源：http://vw.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://dp.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://fo.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://by.huanxung.cn

[T06] Kotlin：集合映射
来源：http://zu.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cd.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://zh.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ul.huanxung.cn

[T08] Kotlin：数据类
来源：http://sb.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://qi.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://mk.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://dm.asd995.cn

[T10] Kotlin：默认参数
来源：http://qe.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gq.asd995.cn

[T11] Kotlin：协程
来源：http://rj.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ny.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://oi.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://jp.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://yk.asd995.cn

val m = mapOf("a" to 1)
来源：http://zw.gzmigu.cn

[T14] Kotlin：循环
来源：http://ed.nicolike.cn

for (i in 1..10) println(i)
来源：http://th.shxzskj.cn

[T15] Kotlin：接口
来源：http://gc.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://zo.haigaiapp.cn

[T16] Swift：Hello World
来源：http://pi.wgjwhj.cn

print("Hello")
来源：http://uu.lnxyls.cn

[T17] Swift：变量与常量
来源：http://pb.szsharing.cn

var a = 1;  let b = 2
来源：http://wl.panjiajie.cn

[T18] Swift：字符串插值
来源：http://ck.bookmarksfly.cn

"值: \(b)"
来源：http://dk.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://yu.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://av.nszjky.cn

[T20] Swift：数组操作
来源：http://th.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nv.shxzskj.cn


<!-- 参考信息 -->