代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://ih.gzmigu.cn

[R18] 遍历数组
来源：http://wx.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xh.hahajie.cn

[R19] 数组长度
来源：http://lc.panjiajie.cn

echo "${#arr[@]}"
来源：http://lz.shxzukj.cn

[R20] 关联数组（字典）
来源：http://dv.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fs.shtwfgs.cn

[R21] 字符串长度
来源：http://zb.bookmarksfly.cn

echo "${#s}"
来源：http://qw.szsharing.cn

[R22] 截取子串
来源：http://lp.muxihuayi.cn

echo "${s:0:5}"
来源：http://wg.yuexingan06.cn

[R23] 字符串替换
来源：http://tg.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qu.gzmigu.cn

[R24] 大小写转换
来源：http://xm.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xd.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://ed.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ie.newstarts.cn

[R26] 命令替换
来源：http://ys.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://eo.newstarts.cn

[R27] 算术展开
来源：http://mp.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://wk.521024.cn

[R28] 浮点运算
来源：http://re.521024.cn

echo "scale=2; 10/3" | bc
来源：http://ij.szsharing.cn

[R29] 定义函数
来源：http://jz.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vs.shxzskj.cn

[R30] 函数返回状态码
来源：http://hs.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://xh.huanxung.cn

[R31] 局部变量
来源：http://rf.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://mn.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://xe.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kw.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://xu.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oc.jctech888.com.cn

[R34] 退出时清理
来源：http://zj.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hi.panjiajie.cn

[R35] 后台执行并等待
来源：http://sa.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ga.hnjuh.cn

[R36] 并发执行多个任务
来源：http://vx.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lv.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://zt.huixinmuqiang.cn

files=$(ls -1)
来源：http://jp.shxzukj.cn

[R38] 管道串联
来源：http://zu.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://kv.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://st.panjiajie.cn

cmd > out.log 2>&1
来源：http://cg.colortex.cn

[R40] 追加写日志
来源：http://cv.huanxung.cn

echo "log" >> out.log
来源：http://mf.muxihuayi.cn

[R41] 丢弃输出
来源：http://et.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://tt.haigaiapp.cn

[R42] 输入重定向
来源：http://yu.huixiangedu.cn

wc -l < a.txt
来源：http://um.shxzukj.cn

[R43] 按名字查找文件
来源：http://qd.shxzukj.cn

find . -name "*.log" -type f
来源：http://jy.9csxet.cn

[R44] 按修改时间查找
来源：http://pb.newstarts.cn

find . -mtime -7 -type f
来源：http://ko.asd995.cn

[R45] 批量删除
来源：http://bs.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://hh.colortex.cn

[R46] 递归替换文件内容
来源：http://xg.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cf.huixiangedu.cn

[R47] sed 单行替换
来源：http://qy.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ol.huanxung.cn

[R48] awk 取指定列
来源：http://ti.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://ko.hahajie.cn

[R49] awk 带条件
来源：http://rc.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tu.gzmigu.cn

[R50] awk 求和
来源：http://lp.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fd.panjiajie.cn

[R51] 排序去重取前几
来源：http://hi.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kp.muxihuayi.cn

[R52] 统计行数
来源：http://ea.colortex.cn

wc -l a.txt
来源：http://ta.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://wz.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cg.lnxyls.cn

[R54] 比较两个文件
来源：http://hr.shxzskj.cn

diff a.txt b.txt
来源：http://cm.szsharing.cn

[R55] 压缩与解压
来源：http://rj.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wk.chemitech.net.cn

[R56] 远程拷贝
来源：http://dc.jctech888.com.cn

scp file user@host:/path/
来源：http://gg.szxytkj.cn

[R57] 远程执行命令
来源：http://ee.colortex.cn

ssh user@host 'uptime'
来源：http://no.lnxyls.cn

[R58] 下载文件
来源：http://tr.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yz.szsharing.cn

[R59] 发 POST JSON
来源：http://km.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fd.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://ef.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fo.shxzskj.cn

[R61] 磁盘占用
来源：http://ox.shtwfgs.cn

df -h;  du -sh *
来源：http://uw.gzmigu.cn

[R62] 找最占空间的文件
来源：http://pi.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://jx.huanxung.cn

[R63] 内存与进程
来源：http://lp.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://nj.nicolike.cn

[R64] 结束进程
来源：http://bc.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://ab.huixiangedu.cn

[R65] 查看端口占用
来源：http://lc.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kh.szxytkj.cn

[R66] 定时任务
来源：http://sn.yuexingan06.cn

crontab -e;  crontab -l
来源：http://qh.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://ld.jctech888.com.cn

openssl rand -hex 16
来源：http://sw.newstarts.cn

[R68] 计算文件校验值
来源：http://ck.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bp.shtwfgs.cn

[R69] 生成随机密码
来源：http://ov.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://fn.9csxet.cn

[R70] 时间戳与互转
来源：http://lj.nicolike.cn

date +%s;  date -d @1700000000
来源：http://vv.nszjky.cn

[R71] 日期格式化
来源：http://jj.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hx.huanxung.cn

[R72] 等待端口就绪
来源：http://om.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zj.bookmarksfly.cn

[R73] 分割大日志
来源：http://bb.yuexingan06.cn

split -l 1000 big.log part_
来源：http://zr.huanxung.cn

[R74] 批量重命名
来源：http://kp.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://co.521024.cn

[R75] 导出环境变量
来源：http://az.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://ub.nicolike.cn

[R76] 使用临时文件
来源：http://uf.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yb.colortex.cn

[R77] 读取用户输入
来源：http://jz.lnxyls.cn

read -rp "请输入: " ans
来源：http://zq.huanxung.cn

[R78] 交互式菜单
来源：http://iq.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yy.asd995.cn

[R79] 解析命令行选项
来源：http://zk.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gs.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://hk.haigaiapp.cn

time ./run.sh
来源：http://mh.yuexingan06.cn

================================================================================
来源：http://ze.newstarts.cn

S. C / C++ 专题
来源：http://xv.colortex.cn

================================================================================
来源：http://np.bookmarksfly.cn

[S01] C：Hello World
来源：http://jh.panjiajie.cn

#include <stdio.h>
来源：http://xd.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pi.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://pp.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://hp.shxzskj.cn

[S03] C：读入整数
来源：http://ey.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://bm.chemitech.net.cn

[S04] C：字符串复制
来源：http://vb.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ab.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://ni.haigaiapp.cn

strlen(s)
来源：http://aw.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://ka.muxihuayi.cn

strcmp(a, b) == 0
来源：http://mx.panjiajie.cn

[S07] C：数组遍历求和
来源：http://ds.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ta.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://yk.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fr.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://ee.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oh.asd995.cn

[S10] C：指针与解引用
来源：http://wz.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://uh.szsharing.cn

[S11] C：逐行读文件
来源：http://pu.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://we.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hc.lnxyls.cn

fclose(f);
来源：http://dn.panjiajie.cn

[S12] C：写文件
来源：http://zm.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ae.muxihuayi.cn

[S13] C：宏定义
来源：http://xr.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qs.wgjwhj.cn

[S14] C：枚举
来源：http://io.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://kg.szxytkj.cn

[S15] C：类型转换
来源：http://tn.huixinmuqiang.cn

(double) a / b
来源：http://jf.panjiajie.cn

[S16] C：位操作置位
来源：http://bd.szsharing.cn

x |= (1 << 3);
来源：http://bz.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://zz.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://by.nicolike.cn

[S18] C：命令行参数
来源：http://ey.521024.cn

int main(int argc, char **argv)
来源：http://or.szsharing.cn

[S19] C：快速排序
来源：http://ph.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zu.szxytkj.cn

[S20] C：二分查找
来源：http://qi.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cp.521024.cn

[S21] C：字符类别判断
来源：http://ad.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qw.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://nf.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hd.huanxung.cn

[S23] C：随机数
来源：http://zk.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wj.shxzskj.cn

[S24] C：获取本地时间
来源：http://lu.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://of.yuexingan06.cn

[S25] C：内存拷贝
来源：http://ya.huixiangedu.cn

memcpy(dst, src, n);
来源：http://dl.yuexingan06.cn

[S26] C：内存清零
来源：http://ae.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://ko.nszjky.cn

[S27] C：定义常量
来源：http://fh.nszjky.cn

const double PI = 3.14159;
来源：http://kc.huanxung.cn

[S28] C：静态变量
来源：http://xd.asd995.cn

static int counter = 0;
来源：http://ov.shxzskj.cn

[S29] C：变参函数
来源：http://qq.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ad.bookmarksfly.cn

[S30] C：头文件保护
来源：http://jv.nszjky.cn

#ifndef X_H
来源：http://im.muxihuayi.cn

#define X_H
来源：http://jg.jianghongdianzi.cn

#endif
来源：http://ab.shxzukj.cn

[S31] C++：Hello World
来源：http://ey.521024.cn

#include <iostream>
来源：http://ug.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://co.shtwfgs.cn

[S32] C++：字符串
来源：http://fj.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://ik.nicolike.cn

[S33] C++：vector 增删
来源：http://os.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iq.lnxyls.cn

[S34] C++：遍历 vector
来源：http://rz.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://zo.shxzukj.cn

[S35] C++：map
来源：http://wh.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qu.haigaiapp.cn

[S36] C++：unordered_map
来源：http://pf.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sz.jianghongdianzi.cn

[S37] C++：set
来源：http://rp.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fi.szsharing.cn

[S38] C++：排序
来源：http://xl.asd995.cn

std::sort(v.begin(), v.end());
来源：http://jr.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://gv.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dc.nszjky.cn

[S40] C++：查找元素
来源：http://yv.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fm.asd995.cn

[S41] C++：类与构造函数
来源：http://hb.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xv.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://nd.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://jb.nicolike.cn

[S43] C++：智能指针
来源：http://oc.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://sp.yuexingan06.cn

[S44] C++：引用传参
来源：http://hm.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://jm.haigaiapp.cn

[S45] C++：lambda
来源：http://ur.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ic.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://tv.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gv.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://rc.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zo.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://uy.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pk.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://zl.shxzskj.cn

[S49] C++：写文件
来源：http://mg.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://it.hnjuh.cn

[S50] C++：格式化数字
来源：http://tk.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ob.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://be.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://ov.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://nv.nicolike.cn

int size() const noexcept { return n_; }
来源：http://ql.shxzskj.cn

[S53] C++：移动语义
来源：http://hi.521024.cn

std::vector<int> w = std::move(v);
来源：http://ds.wgjwhj.cn

[S54] C++：异常处理
来源：http://vm.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ce.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://ld.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fe.lnxyls.cn

[S56] C++：optional
来源：http://xc.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yj.shxzukj.cn

[S57] C++：编译期常量
来源：http://ob.newstarts.cn

constexpr int N = 10;
来源：http://za.chemitech.net.cn

[S58] C++：命名空间
来源：http://st.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://pl.szxytkj.cn

[S59] C++：静态断言
来源：http://ie.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jj.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://sh.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xg.asd995.cn

================================================================================
来源：http://ml.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ak.bookmarksfly.cn

================================================================================
来源：http://wv.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://dn.bookmarksfly.cn

println("Hello")
来源：http://ef.szsharing.cn

[T02] Kotlin：变量
来源：http://tz.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jx.asd995.cn

[T03] Kotlin：字符串模板
来源：http://xd.bookmarksfly.cn

"值: $b"
来源：http://kt.huanxung.cn

[T04] Kotlin：空安全
来源：http://zr.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://ul.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://mp.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yo.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://cf.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kj.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://pv.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wf.huanxung.cn

[T08] Kotlin：数据类
来源：http://vp.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://pq.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://fu.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://us.nszjky.cn

[T10] Kotlin：默认参数
来源：http://az.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rc.shxzukj.cn

[T11] Kotlin：协程
来源：http://rh.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mi.asd995.cn

[T12] Kotlin：解构声明
来源：http://tw.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://dy.521024.cn

[T13] Kotlin：只读 Map
来源：http://gm.521024.cn

val m = mapOf("a" to 1)
来源：http://rg.huixiangedu.cn

[T14] Kotlin：循环
来源：http://nr.asd995.cn

for (i in 1..10) println(i)
来源：http://pg.yuexingan06.cn

[T15] Kotlin：接口
来源：http://cc.asd995.cn

interface Shape { fun area(): Double }
来源：http://wt.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://zv.asd995.cn

print("Hello")
来源：http://mz.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://fw.huanxung.cn

var a = 1;  let b = 2
来源：http://yq.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://yo.shxzukj.cn

"值: \(b)"
来源：http://ci.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://ai.muxihuayi.cn

if let n = opt { print(n) }
来源：http://tw.lnxyls.cn

[T20] Swift：数组操作
来源：http://na.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kn.bjjhwx.cn


<!-- 参考信息 -->