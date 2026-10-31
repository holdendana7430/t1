代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oa.huixiangedu.cn

[R30] 函数返回状态码
来源：http://ja.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://mg.jianghongdianzi.cn

[R31] 局部变量
来源：http://fn.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://nv.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://pl.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jr.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://sy.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kk.hahajie.cn

[R34] 退出时清理
来源：http://pd.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lz.521024.cn

[R35] 后台执行并等待
来源：http://km.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rs.newstarts.cn

[R36] 并发执行多个任务
来源：http://ku.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lo.hnjuh.cn

[R37] 把输出赋给变量
来源：http://rc.wgjwhj.cn

files=$(ls -1)
来源：http://md.shxzukj.cn

[R38] 管道串联
来源：http://sm.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://dl.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://fw.colortex.cn

cmd > out.log 2>&1
来源：http://tj.hnjuh.cn

[R40] 追加写日志
来源：http://iu.shxzukj.cn

echo "log" >> out.log
来源：http://tu.lnxyls.cn

[R41] 丢弃输出
来源：http://qu.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://bw.lnxyls.cn

[R42] 输入重定向
来源：http://rx.huanxung.cn

wc -l < a.txt
来源：http://oa.chemitech.net.cn

[R43] 按名字查找文件
来源：http://pi.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://tw.521024.cn

[R44] 按修改时间查找
来源：http://ni.newstarts.cn

find . -mtime -7 -type f
来源：http://vk.shxzukj.cn

[R45] 批量删除
来源：http://er.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://re.hnjuh.cn

[R46] 递归替换文件内容
来源：http://wo.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cz.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://iz.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ju.jctech888.com.cn

[R48] awk 取指定列
来源：http://uu.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://dn.bjjhwx.cn

[R49] awk 带条件
来源：http://ab.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cp.asd995.cn

[R50] awk 求和
来源：http://jd.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fo.gzmigu.cn

[R51] 排序去重取前几
来源：http://uo.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gt.colortex.cn

[R52] 统计行数
来源：http://eg.shxzukj.cn

wc -l a.txt
来源：http://qx.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://jx.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pa.nszjky.cn

[R54] 比较两个文件
来源：http://nm.asd995.cn

diff a.txt b.txt
来源：http://za.wgjwhj.cn

[R55] 压缩与解压
来源：http://rz.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rr.521024.cn

[R56] 远程拷贝
来源：http://wy.colortex.cn

scp file user@host:/path/
来源：http://nz.521024.cn

[R57] 远程执行命令
来源：http://rd.jctech888.com.cn

ssh user@host 'uptime'
来源：http://sb.shxzukj.cn

[R58] 下载文件
来源：http://px.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tf.gzmigu.cn

[R59] 发 POST JSON
来源：http://cj.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://us.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://cy.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ra.szsharing.cn

[R61] 磁盘占用
来源：http://be.szsharing.cn

df -h;  du -sh *
来源：http://aw.panjiajie.cn

[R62] 找最占空间的文件
来源：http://ln.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://wn.jctech888.com.cn

[R63] 内存与进程
来源：http://xp.521024.cn

free -h;  ps aux | grep nginx
来源：http://if.bjjhwx.cn

[R64] 结束进程
来源：http://uz.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://hy.panjiajie.cn

[R65] 查看端口占用
来源：http://zd.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vw.lnxyls.cn

[R66] 定时任务
来源：http://ws.huixiangedu.cn

crontab -e;  crontab -l
来源：http://lz.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://wb.521024.cn

openssl rand -hex 16
来源：http://fs.newstarts.cn

[R68] 计算文件校验值
来源：http://pk.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yp.huixiangedu.cn

[R69] 生成随机密码
来源：http://zl.521024.cn

head -c 16 /dev/urandom | base64
来源：http://ml.shxzskj.cn

[R70] 时间戳与互转
来源：http://fx.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://jc.lnxyls.cn

[R71] 日期格式化
来源：http://el.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://il.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://gs.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jianghongdianzi.cn

[R73] 分割大日志
来源：http://om.chemitech.net.cn

split -l 1000 big.log part_
来源：http://tf.shxzskj.cn

[R74] 批量重命名
来源：http://yv.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ho.yuexingan06.cn

[R75] 导出环境变量
来源：http://uu.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://xt.chemitech.net.cn

[R76] 使用临时文件
来源：http://gk.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vx.yuexingan06.cn

[R77] 读取用户输入
来源：http://ut.asd995.cn

read -rp "请输入: " ans
来源：http://gf.nszjky.cn

[R78] 交互式菜单
来源：http://bb.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gn.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://oh.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oq.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://ga.lnxyls.cn

time ./run.sh
来源：http://ja.chemitech.net.cn

================================================================================
来源：http://pr.chemitech.net.cn

S. C / C++ 专题
来源：http://cb.jctech888.com.cn

================================================================================
来源：http://pa.muxihuayi.cn

[S01] C：Hello World
来源：http://ly.shxzskj.cn

#include <stdio.h>
来源：http://mi.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vg.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://xb.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://vs.hahajie.cn

[S03] C：读入整数
来源：http://um.nicolike.cn

int x; scanf("%d", &x);
来源：http://pi.asd995.cn

[S04] C：字符串复制
来源：http://ax.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zs.shxzukj.cn

[S05] C：字符串长度
来源：http://ao.panjiajie.cn

strlen(s)
来源：http://fv.panjiajie.cn

[S06] C：字符串比较
来源：http://wq.gzmigu.cn

strcmp(a, b) == 0
来源：http://jq.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://nz.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fe.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://ug.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yq.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://im.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rw.newstarts.cn

[S10] C：指针与解引用
来源：http://gj.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://ua.panjiajie.cn

[S11] C：逐行读文件
来源：http://np.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://ze.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xs.shtwfgs.cn

fclose(f);
来源：http://hs.nszjky.cn

[S12] C：写文件
来源：http://yu.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wx.shxzskj.cn

[S13] C：宏定义
来源：http://nb.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lq.yuexingan06.cn

[S14] C：枚举
来源：http://bp.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://bi.shxzukj.cn

[S15] C：类型转换
来源：http://jt.yuntaijiaju.cn

(double) a / b
来源：http://ie.panjiajie.cn

[S16] C：位操作置位
来源：http://qn.muxihuayi.cn

x |= (1 << 3);
来源：http://ko.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://ye.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ao.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://kc.colortex.cn

int main(int argc, char **argv)
来源：http://hi.521024.cn

[S19] C：快速排序
来源：http://sx.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fd.szxytkj.cn

[S20] C：二分查找
来源：http://jj.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wx.9csxet.cn

[S21] C：字符类别判断
来源：http://ng.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gr.yuexingan06.cn

[S22] C：字符串转数字
来源：http://yu.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fo.lnxyls.cn

[S23] C：随机数
来源：http://be.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gy.521024.cn

[S24] C：获取本地时间
来源：http://un.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ca.haigaiapp.cn

[S25] C：内存拷贝
来源：http://hc.colortex.cn

memcpy(dst, src, n);
来源：http://iy.bjjhwx.cn

[S26] C：内存清零
来源：http://rd.nszjky.cn

memset(a, 0, sizeof a);
来源：http://nq.9csxet.cn

[S27] C：定义常量
来源：http://lb.shxzskj.cn

const double PI = 3.14159;
来源：http://vf.colortex.cn

[S28] C：静态变量
来源：http://jv.huixiangedu.cn

static int counter = 0;
来源：http://cj.szxytkj.cn

[S29] C：变参函数
来源：http://sy.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://if.nicolike.cn

[S30] C：头文件保护
来源：http://rh.nszjky.cn

#ifndef X_H
来源：http://xe.asd995.cn

#define X_H
来源：http://nd.bjjhwx.cn

#endif
来源：http://mc.wgjwhj.cn

[S31] C++：Hello World
来源：http://ud.shtwfgs.cn

#include <iostream>
来源：http://bb.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://hb.jctech888.com.cn

[S32] C++：字符串
来源：http://tz.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://is.lnxyls.cn

[S33] C++：vector 增删
来源：http://ht.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://su.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://lc.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://mn.huixiangedu.cn

[S35] C++：map
来源：http://fc.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yk.nicolike.cn

[S36] C++：unordered_map
来源：http://wc.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hahajie.cn

[S37] C++：set
来源：http://pb.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wg.nszjky.cn

[S38] C++：排序
来源：http://sb.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://gm.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://rp.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://md.9csxet.cn

[S40] C++：查找元素
来源：http://ue.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yf.gzmigu.cn

[S41] C++：类与构造函数
来源：http://dh.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hx.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://sj.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://jn.shxzskj.cn

[S43] C++：智能指针
来源：http://wb.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://so.chemitech.net.cn

[S44] C++：引用传参
来源：http://zw.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://iq.nicolike.cn

[S45] C++：lambda
来源：http://ht.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qy.muxihuayi.cn

[S46] C++：函数模板
来源：http://ve.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vi.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://gt.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wa.gzmigu.cn

[S48] C++：逐行读文件
来源：http://fe.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jc.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://nx.jctech888.com.cn

[S49] C++：写文件
来源：http://el.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kd.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://qm.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wq.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://ii.bjjhwx.cn

static_cast<double>(a) / b
来源：http://or.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://ae.szsharing.cn

int size() const noexcept { return n_; }
来源：http://ot.bookmarksfly.cn

[S53] C++：移动语义
来源：http://yd.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://no.panjiajie.cn

[S54] C++：异常处理
来源：http://gh.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pw.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://qh.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tf.panjiajie.cn

[S56] C++：optional
来源：http://zm.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zs.nicolike.cn

[S57] C++：编译期常量
来源：http://sm.yuexingan06.cn

constexpr int N = 10;
来源：http://oy.hnjuh.cn

[S58] C++：命名空间
来源：http://uu.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://cq.9csxet.cn

[S59] C++：静态断言
来源：http://el.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pd.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://qp.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://od.hnjuh.cn

================================================================================
来源：http://pa.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ad.haigaiapp.cn

================================================================================
来源：http://ug.szsharing.cn

[T01] Kotlin：Hello World
来源：http://us.asd995.cn

println("Hello")
来源：http://cp.yuexingan06.cn

[T02] Kotlin：变量
来源：http://iv.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zx.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://pl.szsharing.cn

"值: $b"
来源：http://jo.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://av.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://jc.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://pp.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dn.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://pu.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xs.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://hg.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eo.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://lb.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://mp.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://oy.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://jc.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://zy.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qd.panjiajie.cn

[T11] Kotlin：协程
来源：http://hp.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://us.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://hj.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://ud.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://ou.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://hj.newstarts.cn

[T14] Kotlin：循环
来源：http://xw.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://yj.yuexingan06.cn

[T15] Kotlin：接口
来源：http://mr.nicolike.cn

interface Shape { fun area(): Double }
来源：http://rv.shxzukj.cn

[T16] Swift：Hello World
来源：http://lz.jianghongdianzi.cn

print("Hello")
来源：http://ta.colortex.cn

[T17] Swift：变量与常量
来源：http://km.shxzskj.cn

var a = 1;  let b = 2
来源：http://xq.hnjuh.cn

[T18] Swift：字符串插值
来源：http://os.muxihuayi.cn

"值: \(b)"
来源：http://au.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://ps.szsharing.cn

if let n = opt { print(n) }
来源：http://cm.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://fr.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ro.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://mz.asd995.cn

for x in a { print(x) }
来源：http://hi.yuntaijiaju.cn

[T22] Swift：字典
来源：http://kw.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vx.shtwfgs.cn

[T23] Swift：函数
来源：http://mu.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aa.asd995.cn

[T24] Swift：闭包
来源：http://ke.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xc.jctech888.com.cn

[T25] Swift：结构体
来源：http://xs.shtwfgs.cn

struct P { var x: Int }
来源：http://cn.szsharing.cn

[T26] Swift：类与重写
来源：http://ga.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://bw.9csxet.cn

[T27] Swift：错误处理
来源：http://nd.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://sg.hnjuh.cn

[T28] Swift：枚举
来源：http://yg.asd995.cn

enum Color { case red, green }
来源：http://wn.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://zr.gzmigu.cn

guard let x = opt else { return }
来源：http://cp.yuntaijiaju.cn

[T30] Swift：协议
来源：http://we.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://ne.shxzskj.cn

[T31] Lua：Hello World
来源：http://dl.szxytkj.cn

print("Hello")
来源：http://vt.panjiajie.cn

[T32] Lua：局部变量
来源：http://ib.9csxet.cn

local a = 1
来源：http://va.asd995.cn


<!-- 参考信息 -->