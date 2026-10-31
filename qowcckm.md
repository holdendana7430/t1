代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://lj.hnjuh.cn

[R18] 遍历数组
来源：http://kv.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://em.yuntaijiaju.cn

[R19] 数组长度
来源：http://qm.chemitech.net.cn

echo "${#arr[@]}"
来源：http://zt.panjiajie.cn

[R20] 关联数组（字典）
来源：http://pe.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yr.jctech888.com.cn

[R21] 字符串长度
来源：http://xm.newstarts.cn

echo "${#s}"
来源：http://zl.bookmarksfly.cn

[R22] 截取子串
来源：http://pj.shtwfgs.cn

echo "${s:0:5}"
来源：http://ik.colortex.cn

[R23] 字符串替换
来源：http://ie.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eb.nszjky.cn

[R24] 大小写转换
来源：http://ub.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bv.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://bz.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uu.hnjuh.cn

[R26] 命令替换
来源：http://hq.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://jp.asd995.cn

[R27] 算术展开
来源：http://gg.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://px.huanxung.cn

[R28] 浮点运算
来源：http://pr.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://le.jctech888.com.cn

[R29] 定义函数
来源：http://jn.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qg.gzmigu.cn

[R30] 函数返回状态码
来源：http://zi.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://wd.muxihuayi.cn

[R31] 局部变量
来源：http://qq.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://im.9csxet.cn

[R32] 参数个数校验
来源：http://wt.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pt.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://yf.bookmarksfly.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rf.huanxung.cn

[R34] 退出时清理
来源：http://ut.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kz.yuexingan06.cn

[R35] 后台执行并等待
来源：http://en.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ev.hnjuh.cn

[R36] 并发执行多个任务
来源：http://id.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tv.shxzukj.cn

[R37] 把输出赋给变量
来源：http://uo.chemitech.net.cn

files=$(ls -1)
来源：http://sh.hahajie.cn

[R38] 管道串联
来源：http://fs.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://oa.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://ga.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://az.521024.cn

[R40] 追加写日志
来源：http://br.asd995.cn

echo "log" >> out.log
来源：http://ns.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://av.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://qs.jianghongdianzi.cn

[R42] 输入重定向
来源：http://zs.wgjwhj.cn

wc -l < a.txt
来源：http://ls.hahajie.cn

[R43] 按名字查找文件
来源：http://fm.521024.cn

find . -name "*.log" -type f
来源：http://ns.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://io.shxzukj.cn

find . -mtime -7 -type f
来源：http://fq.wgjwhj.cn

[R45] 批量删除
来源：http://el.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://kt.huanxung.cn

[R46] 递归替换文件内容
来源：http://wm.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yw.9csxet.cn

[R47] sed 单行替换
来源：http://sl.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dq.shxzukj.cn

[R48] awk 取指定列
来源：http://vg.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://dv.szxytkj.cn

[R49] awk 带条件
来源：http://iy.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://je.jianghongdianzi.cn

[R50] awk 求和
来源：http://mj.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bv.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://ae.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xj.chemitech.net.cn

[R52] 统计行数
来源：http://ee.jianghongdianzi.cn

wc -l a.txt
来源：http://kr.asd995.cn

[R53] 查看文件头与实时尾
来源：http://eb.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vw.szxytkj.cn

[R54] 比较两个文件
来源：http://xk.panjiajie.cn

diff a.txt b.txt
来源：http://jw.panjiajie.cn

[R55] 压缩与解压
来源：http://si.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wy.newstarts.cn

[R56] 远程拷贝
来源：http://bu.wgjwhj.cn

scp file user@host:/path/
来源：http://yj.haigaiapp.cn

[R57] 远程执行命令
来源：http://vg.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://zn.shxzskj.cn

[R58] 下载文件
来源：http://gz.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bk.chemitech.net.cn

[R59] 发 POST JSON
来源：http://wf.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ub.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://pt.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://op.9csxet.cn

[R61] 磁盘占用
来源：http://nv.bjjhwx.cn

df -h;  du -sh *
来源：http://ig.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://hh.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://cc.muxihuayi.cn

[R63] 内存与进程
来源：http://ru.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://al.muxihuayi.cn

[R64] 结束进程
来源：http://yk.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://dv.chemitech.net.cn

[R65] 查看端口占用
来源：http://bu.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uj.szsharing.cn

[R66] 定时任务
来源：http://fu.9csxet.cn

crontab -e;  crontab -l
来源：http://ty.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://hh.huixinmuqiang.cn

openssl rand -hex 16
来源：http://rg.yuexingan06.cn

[R68] 计算文件校验值
来源：http://tp.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fo.shxzukj.cn

[R69] 生成随机密码
来源：http://ny.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://ka.chemitech.net.cn

[R70] 时间戳与互转
来源：http://wh.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://as.shxzukj.cn

[R71] 日期格式化
来源：http://vg.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dm.huixiangedu.cn

[R72] 等待端口就绪
来源：http://es.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fs.jianghongdianzi.cn

[R73] 分割大日志
来源：http://ws.jctech888.com.cn

split -l 1000 big.log part_
来源：http://jn.huixinmuqiang.cn

[R74] 批量重命名
来源：http://mq.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ph.shtwfgs.cn

[R75] 导出环境变量
来源：http://uc.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://pc.szxytkj.cn

[R76] 使用临时文件
来源：http://zw.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tk.shxzskj.cn

[R77] 读取用户输入
来源：http://jn.huanxung.cn

read -rp "请输入: " ans
来源：http://xu.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://gw.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wn.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://we.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://on.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://fb.jctech888.com.cn

time ./run.sh
来源：http://at.newstarts.cn

================================================================================
来源：http://rd.nszjky.cn

S. C / C++ 专题
来源：http://xb.huixiangedu.cn

================================================================================
来源：http://ds.bjjhwx.cn

[S01] C：Hello World
来源：http://ge.huanxung.cn

#include <stdio.h>
来源：http://fe.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hd.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://qn.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://wr.hnjuh.cn

[S03] C：读入整数
来源：http://ws.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://by.nicolike.cn

[S04] C：字符串复制
来源：http://zh.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dr.hahajie.cn

[S05] C：字符串长度
来源：http://no.shxzukj.cn

strlen(s)
来源：http://rz.panjiajie.cn

[S06] C：字符串比较
来源：http://aa.nszjky.cn

strcmp(a, b) == 0
来源：http://lk.szsharing.cn

[S07] C：数组遍历求和
来源：http://cz.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://na.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://mp.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ac.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://ok.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hi.521024.cn

[S10] C：指针与解引用
来源：http://sr.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://nr.muxihuayi.cn

[S11] C：逐行读文件
来源：http://wc.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://ua.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dt.nicolike.cn

fclose(f);
来源：http://lr.wgjwhj.cn

[S12] C：写文件
来源：http://xr.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gw.colortex.cn

[S13] C：宏定义
来源：http://ut.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://um.jianghongdianzi.cn

[S14] C：枚举
来源：http://an.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://lj.lnxyls.cn

[S15] C：类型转换
来源：http://hd.9csxet.cn

(double) a / b
来源：http://av.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://yn.shxzskj.cn

x |= (1 << 3);
来源：http://wn.asd995.cn

[S17] C：安全拼接字符串
来源：http://vy.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://en.shxzskj.cn

[S18] C：命令行参数
来源：http://ih.bjjhwx.cn

int main(int argc, char **argv)
来源：http://hj.asd995.cn

[S19] C：快速排序
来源：http://qn.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://we.szsharing.cn

[S20] C：二分查找
来源：http://mf.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sk.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://qm.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vv.yuexingan06.cn

[S22] C：字符串转数字
来源：http://ov.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vj.colortex.cn

[S23] C：随机数
来源：http://st.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ii.hnjuh.cn

[S24] C：获取本地时间
来源：http://qq.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ci.newstarts.cn

[S25] C：内存拷贝
来源：http://eq.shxzskj.cn

memcpy(dst, src, n);
来源：http://ct.huixinmuqiang.cn

[S26] C：内存清零
来源：http://ix.szsharing.cn

memset(a, 0, sizeof a);
来源：http://nh.chemitech.net.cn

[S27] C：定义常量
来源：http://rn.shtwfgs.cn

const double PI = 3.14159;
来源：http://pa.bjjhwx.cn

[S28] C：静态变量
来源：http://uk.bookmarksfly.cn

static int counter = 0;
来源：http://zh.hnjuh.cn

[S29] C：变参函数
来源：http://sb.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pj.bjjhwx.cn

[S30] C：头文件保护
来源：http://fz.haigaiapp.cn

#ifndef X_H
来源：http://rg.huixiangedu.cn

#define X_H
来源：http://aq.huixiangedu.cn

#endif
来源：http://aq.gzmigu.cn

[S31] C++：Hello World
来源：http://pb.asd995.cn

#include <iostream>
来源：http://ix.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://fp.szxytkj.cn

[S32] C++：字符串
来源：http://mx.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://pf.jctech888.com.cn

[S33] C++：vector 增删
来源：http://kt.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jh.nicolike.cn

[S34] C++：遍历 vector
来源：http://et.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://lo.wgjwhj.cn

[S35] C++：map
来源：http://bx.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wd.szsharing.cn

[S36] C++：unordered_map
来源：http://cp.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://un.shxzskj.cn

[S37] C++：set
来源：http://ot.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kw.bookmarksfly.cn

[S38] C++：排序
来源：http://yz.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://px.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://vt.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ux.haigaiapp.cn

[S40] C++：查找元素
来源：http://tt.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yz.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://cb.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bv.asd995.cn

[S42] C++：继承与虚函数
来源：http://xy.521024.cn

class B : public Base { public: void f() override {} };
来源：http://nl.szsharing.cn

[S43] C++：智能指针
来源：http://ew.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://nd.yuexingan06.cn

[S44] C++：引用传参
来源：http://vn.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://xh.newstarts.cn

[S45] C++：lambda
来源：http://aq.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zm.szxytkj.cn

[S46] C++：函数模板
来源：http://vm.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nn.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://sd.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kf.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://eh.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wa.szsharing.cn

while (std::getline(in, line)) { }
来源：http://lr.chemitech.net.cn

[S49] C++：写文件
来源：http://jo.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ju.nszjky.cn

[S50] C++：格式化数字
来源：http://qy.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nn.huanxung.cn

[S51] C++：显式类型转换
来源：http://gt.panjiajie.cn

static_cast<double>(a) / b
来源：http://rh.asd995.cn

[S52] C++：const 与 noexcept
来源：http://ky.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://dz.szxytkj.cn

[S53] C++：移动语义
来源：http://rn.colortex.cn

std::vector<int> w = std::move(v);
来源：http://sy.shxzukj.cn

[S54] C++：异常处理
来源：http://vx.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ja.szsharing.cn

[S55] C++：结构化绑定
来源：http://ww.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jctech888.com.cn

[S56] C++：optional
来源：http://pa.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mo.panjiajie.cn

[S57] C++：编译期常量
来源：http://uz.haigaiapp.cn

constexpr int N = 10;
来源：http://jy.haigaiapp.cn

[S58] C++：命名空间
来源：http://uu.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://gz.shtwfgs.cn

[S59] C++：静态断言
来源：http://ys.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://um.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://ra.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rs.521024.cn

================================================================================
来源：http://nh.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ji.chemitech.net.cn

================================================================================
来源：http://un.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://wu.nszjky.cn

println("Hello")
来源：http://ia.muxihuayi.cn

[T02] Kotlin：变量
来源：http://ql.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ji.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://qa.asd995.cn

"值: $b"
来源：http://fp.panjiajie.cn

[T04] Kotlin：空安全
来源：http://tp.9csxet.cn

val n: String? = null;  n?.length
来源：http://jh.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://xj.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://go.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://wt.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nn.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://kc.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kb.lnxyls.cn

[T08] Kotlin：数据类
来源：http://hn.521024.cn

data class User(val name: String, val age: Int)
来源：http://an.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://zm.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://kx.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://hi.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yt.huixiangedu.cn

[T11] Kotlin：协程
来源：http://zw.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ey.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://mx.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://mp.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://no.asd995.cn

val m = mapOf("a" to 1)
来源：http://gi.szxytkj.cn

[T14] Kotlin：循环
来源：http://ap.shxzskj.cn

for (i in 1..10) println(i)
来源：http://vn.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://kl.newstarts.cn

interface Shape { fun area(): Double }
来源：http://jb.bjjhwx.cn

[T16] Swift：Hello World
来源：http://cc.panjiajie.cn

print("Hello")
来源：http://nh.shxzukj.cn

[T17] Swift：变量与常量
来源：http://al.newstarts.cn

var a = 1;  let b = 2
来源：http://tw.nszjky.cn

[T18] Swift：字符串插值
来源：http://kn.asd995.cn

"值: \(b)"
来源：http://zo.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://ml.bjjhwx.cn

if let n = opt { print(n) }
来源：http://ho.nszjky.cn

[T20] Swift：数组操作
来源：http://oj.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://be.newstarts.cn


<!-- 参考信息 -->