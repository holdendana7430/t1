代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ci.colortex.cn

[R16] until 等待条件
来源：http://az.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qn.chemitech.net.cn

[R17] 数组定义与取值
来源：http://nf.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bc.szsharing.cn

[R18] 遍历数组
来源：http://kf.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jl.asd995.cn

[R19] 数组长度
来源：http://am.colortex.cn

echo "${#arr[@]}"
来源：http://ma.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://bs.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ko.asd995.cn

[R21] 字符串长度
来源：http://uq.haigaiapp.cn

echo "${#s}"
来源：http://hw.yuexingan06.cn

[R22] 截取子串
来源：http://nu.szsharing.cn

echo "${s:0:5}"
来源：http://xz.bjjhwx.cn

[R23] 字符串替换
来源：http://zv.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://us.newstarts.cn

[R24] 大小写转换
来源：http://md.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://es.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://jc.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yz.yuexingan06.cn

[R26] 命令替换
来源：http://eo.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://si.bjjhwx.cn

[R27] 算术展开
来源：http://xq.colortex.cn

echo $((1 + 2 * 3))
来源：http://kf.huixinmuqiang.cn

[R28] 浮点运算
来源：http://zd.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://zp.shxzskj.cn

[R29] 定义函数
来源：http://bt.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tk.asd995.cn

[R30] 函数返回状态码
来源：http://gj.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://ac.9csxet.cn

[R31] 局部变量
来源：http://lz.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://zd.panjiajie.cn

[R32] 参数个数校验
来源：http://fw.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cp.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://wk.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uo.shtwfgs.cn

[R34] 退出时清理
来源：http://uk.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jk.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://sy.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bs.huanxung.cn

[R36] 并发执行多个任务
来源：http://lg.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rs.9csxet.cn

[R37] 把输出赋给变量
来源：http://jp.shxzskj.cn

files=$(ls -1)
来源：http://gz.lnxyls.cn

[R38] 管道串联
来源：http://ks.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://ej.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://pb.huixiangedu.cn

cmd > out.log 2>&1
来源：http://gg.hnjuh.cn

[R40] 追加写日志
来源：http://ft.9csxet.cn

echo "log" >> out.log
来源：http://cz.shxzskj.cn

[R41] 丢弃输出
来源：http://mq.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://oi.bookmarksfly.cn

[R42] 输入重定向
来源：http://lz.wgjwhj.cn

wc -l < a.txt
来源：http://ru.huanxung.cn

[R43] 按名字查找文件
来源：http://ew.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://dv.gzmigu.cn

[R44] 按修改时间查找
来源：http://ev.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://mb.bookmarksfly.cn

[R45] 批量删除
来源：http://gw.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://hk.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://xm.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jt.hnjuh.cn

[R47] sed 单行替换
来源：http://cs.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ht.hnjuh.cn

[R48] awk 取指定列
来源：http://nm.521024.cn

awk '{print $1, $3}' a.txt
来源：http://ol.szxytkj.cn

[R49] awk 带条件
来源：http://un.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qf.hnjuh.cn

[R50] awk 求和
来源：http://rv.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dn.szsharing.cn

[R51] 排序去重取前几
来源：http://xs.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://be.huanxung.cn

[R52] 统计行数
来源：http://gq.panjiajie.cn

wc -l a.txt
来源：http://nm.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://iy.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ew.hahajie.cn

[R54] 比较两个文件
来源：http://bn.lnxyls.cn

diff a.txt b.txt
来源：http://oo.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://ck.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://to.colortex.cn

[R56] 远程拷贝
来源：http://ji.nicolike.cn

scp file user@host:/path/
来源：http://uh.hahajie.cn

[R57] 远程执行命令
来源：http://op.521024.cn

ssh user@host 'uptime'
来源：http://zf.wgjwhj.cn

[R58] 下载文件
来源：http://px.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yh.wgjwhj.cn

[R59] 发 POST JSON
来源：http://vk.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vf.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://ca.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vs.shtwfgs.cn

[R61] 磁盘占用
来源：http://iq.hnjuh.cn

df -h;  du -sh *
来源：http://bw.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://hn.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://ot.bookmarksfly.cn

[R63] 内存与进程
来源：http://ds.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://vu.szsharing.cn

[R64] 结束进程
来源：http://zz.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://oa.521024.cn

[R65] 查看端口占用
来源：http://hd.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ad.bookmarksfly.cn

[R66] 定时任务
来源：http://oo.yuexingan06.cn

crontab -e;  crontab -l
来源：http://tf.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://jn.9csxet.cn

openssl rand -hex 16
来源：http://jn.panjiajie.cn

[R68] 计算文件校验值
来源：http://hr.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nz.panjiajie.cn

[R69] 生成随机密码
来源：http://we.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://fy.asd995.cn

[R70] 时间戳与互转
来源：http://kf.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://hu.gzmigu.cn

[R71] 日期格式化
来源：http://dc.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fs.nszjky.cn

[R72] 等待端口就绪
来源：http://zb.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uo.panjiajie.cn

[R73] 分割大日志
来源：http://fi.nszjky.cn

split -l 1000 big.log part_
来源：http://dm.shxzskj.cn

[R74] 批量重命名
来源：http://wj.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fc.shtwfgs.cn

[R75] 导出环境变量
来源：http://lr.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://nq.asd995.cn

[R76] 使用临时文件
来源：http://du.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pf.colortex.cn

[R77] 读取用户输入
来源：http://jo.hahajie.cn

read -rp "请输入: " ans
来源：http://qf.nicolike.cn

[R78] 交互式菜单
来源：http://co.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sf.panjiajie.cn

[R79] 解析命令行选项
来源：http://sj.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://im.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://om.huixinmuqiang.cn

time ./run.sh
来源：http://co.nszjky.cn

================================================================================
来源：http://vy.bjjhwx.cn

S. C / C++ 专题
来源：http://wj.panjiajie.cn

================================================================================
来源：http://gc.yuexingan06.cn

[S01] C：Hello World
来源：http://fe.521024.cn

#include <stdio.h>
来源：http://su.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hg.521024.cn

[S02] C：变量与格式化输出
来源：http://qm.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://bc.lnxyls.cn

[S03] C：读入整数
来源：http://ej.gzmigu.cn

int x; scanf("%d", &x);
来源：http://tp.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://ey.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yo.521024.cn

[S05] C：字符串长度
来源：http://yc.wgjwhj.cn

strlen(s)
来源：http://ky.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://ts.hnjuh.cn

strcmp(a, b) == 0
来源：http://wj.newstarts.cn

[S07] C：数组遍历求和
来源：http://ex.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mh.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://fp.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pj.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://gw.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ju.huixiangedu.cn

[S10] C：指针与解引用
来源：http://yc.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://yd.wgjwhj.cn

[S11] C：逐行读文件
来源：http://ua.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://vg.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vb.colortex.cn

fclose(f);
来源：http://gy.nicolike.cn

[S12] C：写文件
来源：http://pa.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qt.huixinmuqiang.cn

[S13] C：宏定义
来源：http://ni.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zn.yuexingan06.cn

[S14] C：枚举
来源：http://jv.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://ik.521024.cn

[S15] C：类型转换
来源：http://dw.huixiangedu.cn

(double) a / b
来源：http://qh.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://do.panjiajie.cn

x |= (1 << 3);
来源：http://kk.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://ji.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fd.asd995.cn

[S18] C：命令行参数
来源：http://yx.asd995.cn

int main(int argc, char **argv)
来源：http://io.521024.cn

[S19] C：快速排序
来源：http://lg.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oz.bjjhwx.cn

[S20] C：二分查找
来源：http://uz.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qu.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://hj.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hx.shxzukj.cn

[S22] C：字符串转数字
来源：http://tr.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://io.chemitech.net.cn

[S23] C：随机数
来源：http://cu.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xh.9csxet.cn

[S24] C：获取本地时间
来源：http://np.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ul.bjjhwx.cn

[S25] C：内存拷贝
来源：http://ys.newstarts.cn

memcpy(dst, src, n);
来源：http://js.521024.cn

[S26] C：内存清零
来源：http://go.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://fh.hahajie.cn

[S27] C：定义常量
来源：http://uq.9csxet.cn

const double PI = 3.14159;
来源：http://kr.shxzukj.cn

[S28] C：静态变量
来源：http://os.huanxung.cn

static int counter = 0;
来源：http://pp.nicolike.cn

[S29] C：变参函数
来源：http://sb.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vn.9csxet.cn

[S30] C：头文件保护
来源：http://kv.chemitech.net.cn

#ifndef X_H
来源：http://bz.asd995.cn

#define X_H
来源：http://tw.huixinmuqiang.cn

#endif
来源：http://pc.jctech888.com.cn

[S31] C++：Hello World
来源：http://fb.huanxung.cn

#include <iostream>
来源：http://tu.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://hk.lnxyls.cn

[S32] C++：字符串
来源：http://rn.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://lp.521024.cn

[S33] C++：vector 增删
来源：http://qz.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ns.asd995.cn

[S34] C++：遍历 vector
来源：http://vs.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://ix.szxytkj.cn

[S35] C++：map
来源：http://fd.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xx.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://ps.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nb.nicolike.cn

[S37] C++：set
来源：http://sr.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ba.shtwfgs.cn

[S38] C++：排序
来源：http://pa.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://sk.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://aa.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vr.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://je.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dz.nicolike.cn

[S41] C++：类与构造函数
来源：http://vv.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xu.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://cq.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://bc.521024.cn

[S43] C++：智能指针
来源：http://dp.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://kw.panjiajie.cn

[S44] C++：引用传参
来源：http://an.nszjky.cn

void inc(int &x) { ++x; }
来源：http://ml.9csxet.cn

[S45] C++：lambda
来源：http://al.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fr.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://es.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zq.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://km.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mn.asd995.cn

[S48] C++：逐行读文件
来源：http://hr.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gh.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://jy.lnxyls.cn

[S49] C++：写文件
来源：http://zq.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bk.asd995.cn

[S50] C++：格式化数字
来源：http://ne.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qj.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://zr.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://aj.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://av.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://uk.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://wy.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://vw.szsharing.cn

[S54] C++：异常处理
来源：http://ak.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://um.asd995.cn

[S55] C++：结构化绑定
来源：http://rb.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yy.shxzskj.cn

[S56] C++：optional
来源：http://oj.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lp.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://ar.yuntaijiaju.cn

constexpr int N = 10;
来源：http://tc.shxzukj.cn

[S58] C++：命名空间
来源：http://gt.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://ky.panjiajie.cn

[S59] C++：静态断言
来源：http://bk.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cb.asd995.cn

[S60] C++：遍历并删除元素
来源：http://ez.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dq.newstarts.cn

================================================================================
来源：http://od.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rf.colortex.cn

================================================================================
来源：http://mt.asd995.cn

[T01] Kotlin：Hello World
来源：http://wl.szsharing.cn

println("Hello")
来源：http://ki.wgjwhj.cn

[T02] Kotlin：变量
来源：http://gl.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wd.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://zn.bookmarksfly.cn

"值: $b"
来源：http://lo.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://ir.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://ot.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://ad.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oe.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://kq.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ot.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://dg.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ss.nszjky.cn

[T08] Kotlin：数据类
来源：http://eb.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://vy.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://kz.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://gc.asd995.cn

[T10] Kotlin：默认参数
来源：http://cq.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zb.shxzskj.cn

[T11] Kotlin：协程
来源：http://bv.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eg.521024.cn

[T12] Kotlin：解构声明
来源：http://eu.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://qh.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://eq.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://xv.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://hk.huanxung.cn

for (i in 1..10) println(i)
来源：http://bj.hnjuh.cn

[T15] Kotlin：接口
来源：http://gf.nszjky.cn

interface Shape { fun area(): Double }
来源：http://lj.hahajie.cn

[T16] Swift：Hello World
来源：http://zj.shxzskj.cn

print("Hello")
来源：http://iy.hahajie.cn

[T17] Swift：变量与常量
来源：http://ga.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://qj.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://jy.haigaiapp.cn

"值: \(b)"
来源：http://sb.szxytkj.cn


<!-- 参考信息 -->