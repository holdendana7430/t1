代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://xw.hahajie.cn

[R26] 命令替换
来源：http://pa.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://vv.nicolike.cn

[R27] 算术展开
来源：http://lh.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://ej.asd995.cn

[R28] 浮点运算
来源：http://nz.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://so.nszjky.cn

[R29] 定义函数
来源：http://xe.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xd.chemitech.net.cn

[R30] 函数返回状态码
来源：http://gb.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://yw.gzmigu.cn

[R31] 局部变量
来源：http://wv.521024.cn

f() { local x=1; echo "$x"; }
来源：http://ew.szxytkj.cn

[R32] 参数个数校验
来源：http://mr.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ii.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://lz.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qr.jianghongdianzi.cn

[R34] 退出时清理
来源：http://vo.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dp.shxzskj.cn

[R35] 后台执行并等待
来源：http://lq.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bb.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://nn.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eh.shxzukj.cn

[R37] 把输出赋给变量
来源：http://rh.wgjwhj.cn

files=$(ls -1)
来源：http://jw.huixinmuqiang.cn

[R38] 管道串联
来源：http://gn.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://vc.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://gf.szsharing.cn

cmd > out.log 2>&1
来源：http://io.521024.cn

[R40] 追加写日志
来源：http://cm.huixiangedu.cn

echo "log" >> out.log
来源：http://fs.bookmarksfly.cn

[R41] 丢弃输出
来源：http://po.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://fh.wgjwhj.cn

[R42] 输入重定向
来源：http://tw.shxzskj.cn

wc -l < a.txt
来源：http://zk.gzmigu.cn

[R43] 按名字查找文件
来源：http://za.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://jw.yuexingan06.cn

[R44] 按修改时间查找
来源：http://cq.chemitech.net.cn

find . -mtime -7 -type f
来源：http://hd.panjiajie.cn

[R45] 批量删除
来源：http://pb.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://ya.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://qx.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bh.yuexingan06.cn

[R47] sed 单行替换
来源：http://wm.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sm.asd995.cn

[R48] awk 取指定列
来源：http://gr.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://rm.huanxung.cn

[R49] awk 带条件
来源：http://lt.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ut.huixinmuqiang.cn

[R50] awk 求和
来源：http://ru.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hh.szsharing.cn

[R51] 排序去重取前几
来源：http://qc.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sj.szsharing.cn

[R52] 统计行数
来源：http://zu.colortex.cn

wc -l a.txt
来源：http://hr.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://tk.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://br.shtwfgs.cn

[R54] 比较两个文件
来源：http://dx.9csxet.cn

diff a.txt b.txt
来源：http://yx.huanxung.cn

[R55] 压缩与解压
来源：http://fc.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qq.haigaiapp.cn

[R56] 远程拷贝
来源：http://pz.nicolike.cn

scp file user@host:/path/
来源：http://dn.wgjwhj.cn

[R57] 远程执行命令
来源：http://ho.colortex.cn

ssh user@host 'uptime'
来源：http://pc.huanxung.cn

[R58] 下载文件
来源：http://lk.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nb.huixiangedu.cn

[R59] 发 POST JSON
来源：http://np.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sh.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://ws.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rr.yuexingan06.cn

[R61] 磁盘占用
来源：http://zy.bjjhwx.cn

df -h;  du -sh *
来源：http://zr.lnxyls.cn

[R62] 找最占空间的文件
来源：http://dj.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://ap.panjiajie.cn

[R63] 内存与进程
来源：http://hx.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://il.wgjwhj.cn

[R64] 结束进程
来源：http://iy.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://sy.shtwfgs.cn

[R65] 查看端口占用
来源：http://xj.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nx.gzmigu.cn

[R66] 定时任务
来源：http://au.lnxyls.cn

crontab -e;  crontab -l
来源：http://ex.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://pb.szsharing.cn

openssl rand -hex 16
来源：http://mc.muxihuayi.cn

[R68] 计算文件校验值
来源：http://vm.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ro.521024.cn

[R69] 生成随机密码
来源：http://kf.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://qx.gzmigu.cn

[R70] 时间戳与互转
来源：http://nb.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://nj.lnxyls.cn

[R71] 日期格式化
来源：http://fc.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zk.jctech888.com.cn

[R72] 等待端口就绪
来源：http://ll.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nv.szsharing.cn

[R73] 分割大日志
来源：http://gb.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://tn.nicolike.cn

[R74] 批量重命名
来源：http://ym.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ws.muxihuayi.cn

[R75] 导出环境变量
来源：http://mv.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://ra.newstarts.cn

[R76] 使用临时文件
来源：http://rs.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pc.hnjuh.cn

[R77] 读取用户输入
来源：http://ob.lnxyls.cn

read -rp "请输入: " ans
来源：http://cx.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://yp.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rw.bjjhwx.cn

[R79] 解析命令行选项
来源：http://yo.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zp.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://yu.muxihuayi.cn

time ./run.sh
来源：http://cn.huixinmuqiang.cn

================================================================================
来源：http://tm.shtwfgs.cn

S. C / C++ 专题
来源：http://vz.huixinmuqiang.cn

================================================================================
来源：http://cp.szsharing.cn

[S01] C：Hello World
来源：http://qi.nszjky.cn

#include <stdio.h>
来源：http://gv.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nz.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://ij.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://wd.hahajie.cn

[S03] C：读入整数
来源：http://ez.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://nf.gzmigu.cn

[S04] C：字符串复制
来源：http://iz.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yc.bjjhwx.cn

[S05] C：字符串长度
来源：http://be.huixiangedu.cn

strlen(s)
来源：http://rb.panjiajie.cn

[S06] C：字符串比较
来源：http://ki.jctech888.com.cn

strcmp(a, b) == 0
来源：http://dw.szxytkj.cn

[S07] C：数组遍历求和
来源：http://jz.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ke.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://xv.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wl.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://at.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fz.jctech888.com.cn

[S10] C：指针与解引用
来源：http://ds.huanxung.cn

int *p = &a;  *p = 5;
来源：http://zz.shxzukj.cn

[S11] C：逐行读文件
来源：http://ai.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://ni.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hj.yuntaijiaju.cn

fclose(f);
来源：http://qu.chemitech.net.cn

[S12] C：写文件
来源：http://il.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ge.lnxyls.cn

[S13] C：宏定义
来源：http://dv.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://li.szsharing.cn

[S14] C：枚举
来源：http://ay.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://rt.521024.cn

[S15] C：类型转换
来源：http://zd.yuexingan06.cn

(double) a / b
来源：http://ur.hahajie.cn

[S16] C：位操作置位
来源：http://pr.hnjuh.cn

x |= (1 << 3);
来源：http://ly.nszjky.cn

[S17] C：安全拼接字符串
来源：http://ts.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yh.9csxet.cn

[S18] C：命令行参数
来源：http://xq.huanxung.cn

int main(int argc, char **argv)
来源：http://nu.9csxet.cn

[S19] C：快速排序
来源：http://jx.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mp.szxytkj.cn

[S20] C：二分查找
来源：http://kw.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qt.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://dx.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zs.panjiajie.cn

[S22] C：字符串转数字
来源：http://na.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kp.gzmigu.cn

[S23] C：随机数
来源：http://wj.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uq.szxytkj.cn

[S24] C：获取本地时间
来源：http://hy.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://db.haigaiapp.cn

[S25] C：内存拷贝
来源：http://nz.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://ku.panjiajie.cn

[S26] C：内存清零
来源：http://gm.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://kg.huixinmuqiang.cn

[S27] C：定义常量
来源：http://ey.newstarts.cn

const double PI = 3.14159;
来源：http://im.newstarts.cn

[S28] C：静态变量
来源：http://rr.colortex.cn

static int counter = 0;
来源：http://wo.yuexingan06.cn

[S29] C：变参函数
来源：http://jj.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qm.szsharing.cn

[S30] C：头文件保护
来源：http://si.muxihuayi.cn

#ifndef X_H
来源：http://ef.jctech888.com.cn

#define X_H
来源：http://co.huanxung.cn

#endif
来源：http://fl.hahajie.cn

[S31] C++：Hello World
来源：http://oa.shxzukj.cn

#include <iostream>
来源：http://xx.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://rq.nicolike.cn

[S32] C++：字符串
来源：http://xz.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://tt.haigaiapp.cn

[S33] C++：vector 增删
来源：http://hj.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mq.gzmigu.cn

[S34] C++：遍历 vector
来源：http://va.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://bu.szxytkj.cn

[S35] C++：map
来源：http://mi.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ys.shtwfgs.cn

[S36] C++：unordered_map
来源：http://dz.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bk.jianghongdianzi.cn

[S37] C++：set
来源：http://yb.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yc.bjjhwx.cn

[S38] C++：排序
来源：http://sz.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://zw.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://ht.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ut.haigaiapp.cn

[S40] C++：查找元素
来源：http://zo.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yg.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://zr.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ko.hahajie.cn

[S42] C++：继承与虚函数
来源：http://ow.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://ty.521024.cn

[S43] C++：智能指针
来源：http://fh.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://fk.hahajie.cn

[S44] C++：引用传参
来源：http://qr.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://qa.gzmigu.cn

[S45] C++：lambda
来源：http://oq.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iu.shtwfgs.cn

[S46] C++：函数模板
来源：http://xx.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sf.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://dv.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kw.nszjky.cn

[S48] C++：逐行读文件
来源：http://px.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sb.newstarts.cn

while (std::getline(in, line)) { }
来源：http://vw.yuexingan06.cn

[S49] C++：写文件
来源：http://oo.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ww.shtwfgs.cn

[S50] C++：格式化数字
来源：http://km.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oy.szsharing.cn

[S51] C++：显式类型转换
来源：http://mj.colortex.cn

static_cast<double>(a) / b
来源：http://ky.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://wp.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://ts.huanxung.cn

[S53] C++：移动语义
来源：http://ur.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://gn.yuexingan06.cn

[S54] C++：异常处理
来源：http://qr.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bg.nszjky.cn

[S55] C++：结构化绑定
来源：http://wi.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mt.huanxung.cn

[S56] C++：optional
来源：http://ay.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fh.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://ck.huixiangedu.cn

constexpr int N = 10;
来源：http://xy.muxihuayi.cn

[S58] C++：命名空间
来源：http://eb.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://vb.9csxet.cn

[S59] C++：静态断言
来源：http://qg.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mw.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://bm.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xz.huixinmuqiang.cn

================================================================================
来源：http://cv.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sb.chemitech.net.cn

================================================================================
来源：http://zw.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://ie.gzmigu.cn

println("Hello")
来源：http://bf.muxihuayi.cn

[T02] Kotlin：变量
来源：http://pe.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kw.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://gu.hahajie.cn

"值: $b"
来源：http://fr.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://px.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://oi.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://sd.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fi.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://yu.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dm.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://xp.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lo.shxzukj.cn

[T08] Kotlin：数据类
来源：http://rw.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://oq.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://fd.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://kj.nszjky.cn

[T10] Kotlin：默认参数
来源：http://dl.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bp.chemitech.net.cn

[T11] Kotlin：协程
来源：http://lm.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oh.hahajie.cn

[T12] Kotlin：解构声明
来源：http://bj.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://wd.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://zm.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://od.huanxung.cn

[T14] Kotlin：循环
来源：http://la.colortex.cn

for (i in 1..10) println(i)
来源：http://zi.bjjhwx.cn

[T15] Kotlin：接口
来源：http://tc.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://sl.hnjuh.cn

[T16] Swift：Hello World
来源：http://sn.chemitech.net.cn

print("Hello")
来源：http://hn.panjiajie.cn

[T17] Swift：变量与常量
来源：http://qu.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://tf.lnxyls.cn

[T18] Swift：字符串插值
来源：http://fs.nszjky.cn

"值: \(b)"
来源：http://pr.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://yh.huanxung.cn

if let n = opt { print(n) }
来源：http://ik.hnjuh.cn

[T20] Swift：数组操作
来源：http://mn.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://md.szsharing.cn

[T21] Swift：遍历
来源：http://bb.hahajie.cn

for x in a { print(x) }
来源：http://pd.nszjky.cn

[T22] Swift：字典
来源：http://sf.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wu.chemitech.net.cn

[T23] Swift：函数
来源：http://rx.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dz.lnxyls.cn

[T24] Swift：闭包
来源：http://lj.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ix.muxihuayi.cn

[T25] Swift：结构体
来源：http://ty.huixinmuqiang.cn

struct P { var x: Int }
来源：http://ix.521024.cn

[T26] Swift：类与重写
来源：http://xw.szsharing.cn

class A: Base { override func f() {} }
来源：http://pg.panjiajie.cn

[T27] Swift：错误处理
来源：http://io.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://az.9csxet.cn

[T28] Swift：枚举
来源：http://wm.asd995.cn

enum Color { case red, green }
来源：http://ve.huanxung.cn


<!-- 参考信息 -->