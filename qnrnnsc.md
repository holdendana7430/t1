代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://tg.colortex.cn

[R32] 参数个数校验
来源：http://le.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kh.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://ct.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nx.panjiajie.cn

[R34] 退出时清理
来源：http://kv.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gw.yuexingan06.cn

[R35] 后台执行并等待
来源：http://fb.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zk.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://fo.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://me.hnjuh.cn

[R37] 把输出赋给变量
来源：http://tf.huixiangedu.cn

files=$(ls -1)
来源：http://gq.nszjky.cn

[R38] 管道串联
来源：http://uc.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://kc.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://wd.lnxyls.cn

cmd > out.log 2>&1
来源：http://ql.shxzukj.cn

[R40] 追加写日志
来源：http://ti.colortex.cn

echo "log" >> out.log
来源：http://oq.shxzskj.cn

[R41] 丢弃输出
来源：http://qx.colortex.cn

cmd >/dev/null 2>&1
来源：http://sv.jctech888.com.cn

[R42] 输入重定向
来源：http://qq.haigaiapp.cn

wc -l < a.txt
来源：http://mr.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://wb.muxihuayi.cn

find . -name "*.log" -type f
来源：http://ww.newstarts.cn

[R44] 按修改时间查找
来源：http://sp.9csxet.cn

find . -mtime -7 -type f
来源：http://ff.yuntaijiaju.cn

[R45] 批量删除
来源：http://lq.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://ui.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://if.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bg.521024.cn

[R47] sed 单行替换
来源：http://zn.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nn.hahajie.cn

[R48] awk 取指定列
来源：http://el.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://xj.szsharing.cn

[R49] awk 带条件
来源：http://kv.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fk.asd995.cn

[R50] awk 求和
来源：http://pc.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://de.lnxyls.cn

[R51] 排序去重取前几
来源：http://yw.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zd.newstarts.cn

[R52] 统计行数
来源：http://tq.9csxet.cn

wc -l a.txt
来源：http://oa.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://oz.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://id.haigaiapp.cn

[R54] 比较两个文件
来源：http://fe.nicolike.cn

diff a.txt b.txt
来源：http://mc.hahajie.cn

[R55] 压缩与解压
来源：http://wx.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lb.jctech888.com.cn

[R56] 远程拷贝
来源：http://my.hahajie.cn

scp file user@host:/path/
来源：http://cm.szxytkj.cn

[R57] 远程执行命令
来源：http://ty.jctech888.com.cn

ssh user@host 'uptime'
来源：http://vz.chemitech.net.cn

[R58] 下载文件
来源：http://kt.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ie.shxzukj.cn

[R59] 发 POST JSON
来源：http://he.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xg.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://av.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://il.hahajie.cn

[R61] 磁盘占用
来源：http://lm.hahajie.cn

df -h;  du -sh *
来源：http://jw.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://fn.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://rw.nszjky.cn

[R63] 内存与进程
来源：http://tf.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://ts.shxzukj.cn

[R64] 结束进程
来源：http://lp.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://ti.521024.cn

[R65] 查看端口占用
来源：http://xp.shtwfgs.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nq.nszjky.cn

[R66] 定时任务
来源：http://ov.szsharing.cn

crontab -e;  crontab -l
来源：http://df.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://cz.521024.cn

openssl rand -hex 16
来源：http://zh.lnxyls.cn

[R68] 计算文件校验值
来源：http://qk.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ql.shtwfgs.cn

[R69] 生成随机密码
来源：http://sn.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://tz.wgjwhj.cn

[R70] 时间戳与互转
来源：http://ie.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://wn.521024.cn

[R71] 日期格式化
来源：http://ec.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qn.gzmigu.cn

[R72] 等待端口就绪
来源：http://ki.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oh.jianghongdianzi.cn

[R73] 分割大日志
来源：http://mi.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://wh.huanxung.cn

[R74] 批量重命名
来源：http://xr.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kl.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://be.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://es.jctech888.com.cn

[R76] 使用临时文件
来源：http://sm.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cb.panjiajie.cn

[R77] 读取用户输入
来源：http://dq.newstarts.cn

read -rp "请输入: " ans
来源：http://xu.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://fb.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ap.nicolike.cn

[R79] 解析命令行选项
来源：http://vu.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ze.asd995.cn

[R80] 查看脚本执行耗时
来源：http://ef.szxytkj.cn

time ./run.sh
来源：http://vn.nszjky.cn

================================================================================
来源：http://vo.muxihuayi.cn

S. C / C++ 专题
来源：http://bb.bookmarksfly.cn

================================================================================
来源：http://jp.yuexingan06.cn

[S01] C：Hello World
来源：http://wq.hnjuh.cn

#include <stdio.h>
来源：http://gt.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fc.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://bk.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://ws.szxytkj.cn

[S03] C：读入整数
来源：http://ma.hahajie.cn

int x; scanf("%d", &x);
来源：http://ba.asd995.cn

[S04] C：字符串复制
来源：http://mp.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ux.colortex.cn

[S05] C：字符串长度
来源：http://nz.521024.cn

strlen(s)
来源：http://wx.bookmarksfly.cn

[S06] C：字符串比较
来源：http://bs.muxihuayi.cn

strcmp(a, b) == 0
来源：http://ow.huanxung.cn

[S07] C：数组遍历求和
来源：http://ai.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ve.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://wl.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qh.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://pn.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://do.asd995.cn

[S10] C：指针与解引用
来源：http://sc.newstarts.cn

int *p = &a;  *p = 5;
来源：http://sg.muxihuayi.cn

[S11] C：逐行读文件
来源：http://ms.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://oc.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cl.shxzukj.cn

fclose(f);
来源：http://gm.shtwfgs.cn

[S12] C：写文件
来源：http://fb.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yo.yuntaijiaju.cn

[S13] C：宏定义
来源：http://ka.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xg.yuntaijiaju.cn

[S14] C：枚举
来源：http://oj.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://yc.newstarts.cn

[S15] C：类型转换
来源：http://ve.521024.cn

(double) a / b
来源：http://yi.shxzukj.cn

[S16] C：位操作置位
来源：http://lu.521024.cn

x |= (1 << 3);
来源：http://hk.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://xq.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fq.yuexingan06.cn

[S18] C：命令行参数
来源：http://nf.haigaiapp.cn

int main(int argc, char **argv)
来源：http://ex.chemitech.net.cn

[S19] C：快速排序
来源：http://sd.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://da.shtwfgs.cn

[S20] C：二分查找
来源：http://cl.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pk.jctech888.com.cn

[S21] C：字符类别判断
来源：http://br.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lq.wgjwhj.cn

[S22] C：字符串转数字
来源：http://ch.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://or.lnxyls.cn

[S23] C：随机数
来源：http://eo.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ry.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://zc.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eh.hnjuh.cn

[S25] C：内存拷贝
来源：http://mq.wgjwhj.cn

memcpy(dst, src, n);
来源：http://gs.haigaiapp.cn

[S26] C：内存清零
来源：http://gq.szsharing.cn

memset(a, 0, sizeof a);
来源：http://rz.haigaiapp.cn

[S27] C：定义常量
来源：http://ev.gzmigu.cn

const double PI = 3.14159;
来源：http://ay.shtwfgs.cn

[S28] C：静态变量
来源：http://ih.nszjky.cn

static int counter = 0;
来源：http://tu.colortex.cn

[S29] C：变参函数
来源：http://db.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oo.shtwfgs.cn

[S30] C：头文件保护
来源：http://di.shxzskj.cn

#ifndef X_H
来源：http://kw.huixiangedu.cn

#define X_H
来源：http://oj.hahajie.cn

#endif
来源：http://eu.huanxung.cn

[S31] C++：Hello World
来源：http://hn.bookmarksfly.cn

#include <iostream>
来源：http://jl.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://pt.colortex.cn

[S32] C++：字符串
来源：http://jg.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://it.9csxet.cn

[S33] C++：vector 增删
来源：http://vl.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qd.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://qk.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://ix.yuexingan06.cn

[S35] C++：map
来源：http://zo.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wr.colortex.cn

[S36] C++：unordered_map
来源：http://ue.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nu.shtwfgs.cn

[S37] C++：set
来源：http://nh.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://os.asd995.cn

[S38] C++：排序
来源：http://ro.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://vl.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://tw.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jq.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://cy.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bq.lnxyls.cn

[S41] C++：类与构造函数
来源：http://jl.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gy.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://or.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://dm.szxytkj.cn

[S43] C++：智能指针
来源：http://xo.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://cs.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://ra.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://ct.panjiajie.cn

[S45] C++：lambda
来源：http://gq.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://th.gzmigu.cn

[S46] C++：函数模板
来源：http://in.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://if.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://gx.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ue.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://se.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pp.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://sg.haigaiapp.cn

[S49] C++：写文件
来源：http://bk.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://af.9csxet.cn

[S50] C++：格式化数字
来源：http://ri.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wy.szsharing.cn

[S51] C++：显式类型转换
来源：http://js.haigaiapp.cn

static_cast<double>(a) / b
来源：http://of.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://yq.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://rw.szsharing.cn

[S53] C++：移动语义
来源：http://xb.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://yz.panjiajie.cn

[S54] C++：异常处理
来源：http://qj.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://le.9csxet.cn

[S55] C++：结构化绑定
来源：http://fl.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rn.haigaiapp.cn

[S56] C++：optional
来源：http://py.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://as.bjjhwx.cn

[S57] C++：编译期常量
来源：http://iq.wgjwhj.cn

constexpr int N = 10;
来源：http://xt.asd995.cn

[S58] C++：命名空间
来源：http://zu.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://ov.shtwfgs.cn

[S59] C++：静态断言
来源：http://pm.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ub.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://rf.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://la.newstarts.cn

================================================================================
来源：http://vg.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ld.jctech888.com.cn

================================================================================
来源：http://ct.521024.cn

[T01] Kotlin：Hello World
来源：http://gd.lnxyls.cn

println("Hello")
来源：http://fg.bjjhwx.cn

[T02] Kotlin：变量
来源：http://om.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vg.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://xw.asd995.cn

"值: $b"
来源：http://ld.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://db.hnjuh.cn

val n: String? = null;  n?.length
来源：http://vw.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://yn.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ga.newstarts.cn

[T06] Kotlin：集合映射
来源：http://pc.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kk.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://vm.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ak.gzmigu.cn

[T08] Kotlin：数据类
来源：http://hz.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://ih.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://yr.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://fw.szsharing.cn

[T10] Kotlin：默认参数
来源：http://ka.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zq.newstarts.cn

[T11] Kotlin：协程
来源：http://du.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xs.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://jz.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://dt.asd995.cn

[T13] Kotlin：只读 Map
来源：http://km.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://pc.szsharing.cn

[T14] Kotlin：循环
来源：http://mq.colortex.cn

for (i in 1..10) println(i)
来源：http://ux.bjjhwx.cn

[T15] Kotlin：接口
来源：http://iu.newstarts.cn

interface Shape { fun area(): Double }
来源：http://sy.bjjhwx.cn

[T16] Swift：Hello World
来源：http://vi.jctech888.com.cn

print("Hello")
来源：http://ap.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://yy.shtwfgs.cn

var a = 1;  let b = 2
来源：http://jx.newstarts.cn

[T18] Swift：字符串插值
来源：http://jk.hnjuh.cn

"值: \(b)"
来源：http://ht.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://aa.9csxet.cn

if let n = opt { print(n) }
来源：http://xh.jctech888.com.cn

[T20] Swift：数组操作
来源：http://gk.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ov.jctech888.com.cn

[T21] Swift：遍历
来源：http://sn.chemitech.net.cn

for x in a { print(x) }
来源：http://jc.huixiangedu.cn

[T22] Swift：字典
来源：http://zj.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ph.haigaiapp.cn

[T23] Swift：函数
来源：http://fe.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nu.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://rg.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ox.chemitech.net.cn

[T25] Swift：结构体
来源：http://tf.lnxyls.cn

struct P { var x: Int }
来源：http://zt.shxzukj.cn

[T26] Swift：类与重写
来源：http://iu.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://yh.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://re.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://wu.nszjky.cn

[T28] Swift：枚举
来源：http://vc.hahajie.cn

enum Color { case red, green }
来源：http://dl.521024.cn

[T29] Swift：guard 提前返回
来源：http://ud.szsharing.cn

guard let x = opt else { return }
来源：http://nn.haigaiapp.cn

[T30] Swift：协议
来源：http://pp.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://lw.huixiangedu.cn

[T31] Lua：Hello World
来源：http://vc.panjiajie.cn

print("Hello")
来源：http://ma.gzmigu.cn

[T32] Lua：局部变量
来源：http://ob.yuntaijiaju.cn

local a = 1
来源：http://qa.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://af.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://my.521024.cn

[T34] Lua：遍历表
来源：http://qw.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ph.9csxet.cn


<!-- 参考信息 -->