代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://yr.521024.cn

[R18] 遍历数组
来源：http://fb.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lw.gzmigu.cn

[R19] 数组长度
来源：http://im.chemitech.net.cn

echo "${#arr[@]}"
来源：http://lu.nszjky.cn

[R20] 关联数组（字典）
来源：http://kt.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ps.shtwfgs.cn

[R21] 字符串长度
来源：http://ye.colortex.cn

echo "${#s}"
来源：http://tk.colortex.cn

[R22] 截取子串
来源：http://hr.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://om.muxihuayi.cn

[R23] 字符串替换
来源：http://xi.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cw.shxzukj.cn

[R24] 大小写转换
来源：http://lu.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yb.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://kr.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wa.haigaiapp.cn

[R26] 命令替换
来源：http://aa.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://gi.panjiajie.cn

[R27] 算术展开
来源：http://yw.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://mg.colortex.cn

[R28] 浮点运算
来源：http://dk.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://vh.521024.cn

[R29] 定义函数
来源：http://rb.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mr.haigaiapp.cn

[R30] 函数返回状态码
来源：http://ng.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://ah.gzmigu.cn

[R31] 局部变量
来源：http://ls.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://eo.hnjuh.cn

[R32] 参数个数校验
来源：http://iv.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yw.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://ay.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kq.shxzukj.cn

[R34] 退出时清理
来源：http://jk.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cl.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://vi.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cs.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://ud.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pd.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://kv.nszjky.cn

files=$(ls -1)
来源：http://qw.jianghongdianzi.cn

[R38] 管道串联
来源：http://vq.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://ol.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://ke.shxzskj.cn

cmd > out.log 2>&1
来源：http://sx.szsharing.cn

[R40] 追加写日志
来源：http://pk.huanxung.cn

echo "log" >> out.log
来源：http://ti.wgjwhj.cn

[R41] 丢弃输出
来源：http://ep.521024.cn

cmd >/dev/null 2>&1
来源：http://qj.hnjuh.cn

[R42] 输入重定向
来源：http://cb.haigaiapp.cn

wc -l < a.txt
来源：http://ck.chemitech.net.cn

[R43] 按名字查找文件
来源：http://kn.panjiajie.cn

find . -name "*.log" -type f
来源：http://gp.colortex.cn

[R44] 按修改时间查找
来源：http://pw.szsharing.cn

find . -mtime -7 -type f
来源：http://gg.jianghongdianzi.cn

[R45] 批量删除
来源：http://ph.szsharing.cn

find . -name "*.tmp" -delete
来源：http://vh.colortex.cn

[R46] 递归替换文件内容
来源：http://gp.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zx.newstarts.cn

[R47] sed 单行替换
来源：http://sj.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rn.shxzskj.cn

[R48] awk 取指定列
来源：http://da.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://fx.szsharing.cn

[R49] awk 带条件
来源：http://hr.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ur.nicolike.cn

[R50] awk 求和
来源：http://dz.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rz.colortex.cn

[R51] 排序去重取前几
来源：http://wk.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sp.yuntaijiaju.cn

[R52] 统计行数
来源：http://vv.chemitech.net.cn

wc -l a.txt
来源：http://ww.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://nz.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tj.bookmarksfly.cn

[R54] 比较两个文件
来源：http://mx.lnxyls.cn

diff a.txt b.txt
来源：http://xv.haigaiapp.cn

[R55] 压缩与解压
来源：http://cb.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lu.szxytkj.cn

[R56] 远程拷贝
来源：http://ln.szsharing.cn

scp file user@host:/path/
来源：http://zi.wgjwhj.cn

[R57] 远程执行命令
来源：http://rl.lnxyls.cn

ssh user@host 'uptime'
来源：http://ke.lnxyls.cn

[R58] 下载文件
来源：http://op.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jc.521024.cn

[R59] 发 POST JSON
来源：http://bl.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yg.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://js.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ae.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://ve.chemitech.net.cn

df -h;  du -sh *
来源：http://hn.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://xu.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://br.shxzukj.cn

[R63] 内存与进程
来源：http://ah.asd995.cn

free -h;  ps aux | grep nginx
来源：http://sq.shxzskj.cn

[R64] 结束进程
来源：http://sm.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://vy.asd995.cn

[R65] 查看端口占用
来源：http://mz.nicolike.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ii.hnjuh.cn

[R66] 定时任务
来源：http://xz.wgjwhj.cn

crontab -e;  crontab -l
来源：http://ml.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://tw.yuntaijiaju.cn

openssl rand -hex 16
来源：http://cb.yuexingan06.cn

[R68] 计算文件校验值
来源：http://mh.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tx.bookmarksfly.cn

[R69] 生成随机密码
来源：http://rb.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://ve.asd995.cn

[R70] 时间戳与互转
来源：http://lt.szsharing.cn

date +%s;  date -d @1700000000
来源：http://su.hnjuh.cn

[R71] 日期格式化
来源：http://lp.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://np.haigaiapp.cn

[R72] 等待端口就绪
来源：http://fn.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bx.szsharing.cn

[R73] 分割大日志
来源：http://lt.jctech888.com.cn

split -l 1000 big.log part_
来源：http://vm.9csxet.cn

[R74] 批量重命名
来源：http://xh.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dn.nszjky.cn

[R75] 导出环境变量
来源：http://fl.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://ux.szsharing.cn

[R76] 使用临时文件
来源：http://xx.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wu.newstarts.cn

[R77] 读取用户输入
来源：http://my.shtwfgs.cn

read -rp "请输入: " ans
来源：http://ib.szxytkj.cn

[R78] 交互式菜单
来源：http://ia.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nu.521024.cn

[R79] 解析命令行选项
来源：http://cu.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uj.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://pd.hnjuh.cn

time ./run.sh
来源：http://ab.newstarts.cn

================================================================================
来源：http://jb.shxzukj.cn

S. C / C++ 专题
来源：http://sm.gzmigu.cn

================================================================================
来源：http://bo.wgjwhj.cn

[S01] C：Hello World
来源：http://yk.jianghongdianzi.cn

#include <stdio.h>
来源：http://hq.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cs.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://ci.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://wd.gzmigu.cn

[S03] C：读入整数
来源：http://fo.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://hd.bjjhwx.cn

[S04] C：字符串复制
来源：http://uh.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jn.shxzukj.cn

[S05] C：字符串长度
来源：http://ex.newstarts.cn

strlen(s)
来源：http://rt.asd995.cn

[S06] C：字符串比较
来源：http://mj.nszjky.cn

strcmp(a, b) == 0
来源：http://bl.nicolike.cn

[S07] C：数组遍历求和
来源：http://zy.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qj.colortex.cn

[S08] C：动态内存分配与释放
来源：http://wz.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fq.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://ya.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://go.muxihuayi.cn

[S10] C：指针与解引用
来源：http://lw.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://zh.bjjhwx.cn

[S11] C：逐行读文件
来源：http://xf.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://rd.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rt.asd995.cn

fclose(f);
来源：http://sv.wgjwhj.cn

[S12] C：写文件
来源：http://sz.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qa.yuexingan06.cn

[S13] C：宏定义
来源：http://oe.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lp.bookmarksfly.cn

[S14] C：枚举
来源：http://wg.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://uf.szsharing.cn

[S15] C：类型转换
来源：http://vx.yuntaijiaju.cn

(double) a / b
来源：http://hm.521024.cn

[S16] C：位操作置位
来源：http://ja.gzmigu.cn

x |= (1 << 3);
来源：http://cz.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://vj.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vo.szxytkj.cn

[S18] C：命令行参数
来源：http://vd.muxihuayi.cn

int main(int argc, char **argv)
来源：http://ye.muxihuayi.cn

[S19] C：快速排序
来源：http://tn.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://aa.lnxyls.cn

[S20] C：二分查找
来源：http://rw.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tm.gzmigu.cn

[S21] C：字符类别判断
来源：http://su.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zt.shxzskj.cn

[S22] C：字符串转数字
来源：http://cz.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wy.shtwfgs.cn

[S23] C：随机数
来源：http://pb.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vr.panjiajie.cn

[S24] C：获取本地时间
来源：http://yk.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ff.nszjky.cn

[S25] C：内存拷贝
来源：http://iv.chemitech.net.cn

memcpy(dst, src, n);
来源：http://ul.yuntaijiaju.cn

[S26] C：内存清零
来源：http://kg.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://cz.bjjhwx.cn

[S27] C：定义常量
来源：http://mf.panjiajie.cn

const double PI = 3.14159;
来源：http://yq.newstarts.cn

[S28] C：静态变量
来源：http://hj.bjjhwx.cn

static int counter = 0;
来源：http://tt.shtwfgs.cn

[S29] C：变参函数
来源：http://xg.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ju.bjjhwx.cn

[S30] C：头文件保护
来源：http://td.haigaiapp.cn

#ifndef X_H
来源：http://vh.jctech888.com.cn

#define X_H
来源：http://ol.jctech888.com.cn

#endif
来源：http://lm.lnxyls.cn

[S31] C++：Hello World
来源：http://aj.nszjky.cn

#include <iostream>
来源：http://uf.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://pp.yuexingan06.cn

[S32] C++：字符串
来源：http://ag.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://db.9csxet.cn

[S33] C++：vector 增删
来源：http://wp.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dc.hnjuh.cn

[S34] C++：遍历 vector
来源：http://df.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://pq.wgjwhj.cn

[S35] C++：map
来源：http://pk.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ox.jctech888.com.cn

[S36] C++：unordered_map
来源：http://su.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jm.panjiajie.cn

[S37] C++：set
来源：http://qx.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zm.shxzskj.cn

[S38] C++：排序
来源：http://fy.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://rc.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://rp.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://az.shxzskj.cn

[S40] C++：查找元素
来源：http://gz.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xu.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://kd.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vo.nszjky.cn

[S42] C++：继承与虚函数
来源：http://rl.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://ap.newstarts.cn

[S43] C++：智能指针
来源：http://qy.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://re.9csxet.cn

[S44] C++：引用传参
来源：http://dh.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://wb.bjjhwx.cn

[S45] C++：lambda
来源：http://ov.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://si.chemitech.net.cn

[S46] C++：函数模板
来源：http://qq.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lh.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://rs.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sa.nicolike.cn

[S48] C++：逐行读文件
来源：http://xo.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dd.huanxung.cn

while (std::getline(in, line)) { }
来源：http://he.yuntaijiaju.cn

[S49] C++：写文件
来源：http://qw.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sx.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://tp.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mr.9csxet.cn

[S51] C++：显式类型转换
来源：http://xg.wgjwhj.cn

static_cast<double>(a) / b
来源：http://mg.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://ol.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://zf.shtwfgs.cn

[S53] C++：移动语义
来源：http://pr.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://ed.haigaiapp.cn

[S54] C++：异常处理
来源：http://fc.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ww.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://rr.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gf.jianghongdianzi.cn

[S56] C++：optional
来源：http://qa.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pf.nicolike.cn

[S57] C++：编译期常量
来源：http://eq.9csxet.cn

constexpr int N = 10;
来源：http://rf.colortex.cn

[S58] C++：命名空间
来源：http://ts.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://sv.shxzukj.cn

[S59] C++：静态断言
来源：http://jb.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fz.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://tw.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tt.bjjhwx.cn

================================================================================
来源：http://by.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mh.wgjwhj.cn

================================================================================
来源：http://sb.nicolike.cn

[T01] Kotlin：Hello World
来源：http://sb.huixinmuqiang.cn

println("Hello")
来源：http://zv.szsharing.cn

[T02] Kotlin：变量
来源：http://mi.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vu.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://gr.bookmarksfly.cn

"值: $b"
来源：http://vu.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://tz.hahajie.cn

val n: String? = null;  n?.length
来源：http://bv.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://hw.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yu.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://nt.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lv.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://pi.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fc.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://qu.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://md.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://ie.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://ag.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://rx.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sk.newstarts.cn

[T11] Kotlin：协程
来源：http://wk.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nt.asd995.cn

[T12] Kotlin：解构声明
来源：http://ro.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://dv.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://ow.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://hl.asd995.cn

[T14] Kotlin：循环
来源：http://xf.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://qw.lnxyls.cn

[T15] Kotlin：接口
来源：http://wr.asd995.cn

interface Shape { fun area(): Double }
来源：http://um.panjiajie.cn

[T16] Swift：Hello World
来源：http://qh.huanxung.cn

print("Hello")
来源：http://lm.colortex.cn

[T17] Swift：变量与常量
来源：http://ar.521024.cn

var a = 1;  let b = 2
来源：http://cf.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://cb.huixiangedu.cn

"值: \(b)"
来源：http://sm.szsharing.cn

[T19] Swift：可选绑定
来源：http://kf.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://kl.huanxung.cn

[T20] Swift：数组操作
来源：http://fj.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hz.asd995.cn


<!-- 参考信息 -->