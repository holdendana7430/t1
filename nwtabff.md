代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gt.muxihuayi.cn

[R16] until 等待条件
来源：http://fx.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cf.chemitech.net.cn

[R17] 数组定义与取值
来源：http://zr.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pz.haigaiapp.cn

[R18] 遍历数组
来源：http://wi.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hg.szxytkj.cn

[R19] 数组长度
来源：http://ba.shxzskj.cn

echo "${#arr[@]}"
来源：http://et.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://xt.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gf.bjjhwx.cn

[R21] 字符串长度
来源：http://bn.gzmigu.cn

echo "${#s}"
来源：http://fs.shxzskj.cn

[R22] 截取子串
来源：http://ms.jctech888.com.cn

echo "${s:0:5}"
来源：http://sh.asd995.cn

[R23] 字符串替换
来源：http://wl.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uj.hahajie.cn

[R24] 大小写转换
来源：http://bf.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sh.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://zu.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kd.shxzskj.cn

[R26] 命令替换
来源：http://vm.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://ed.bookmarksfly.cn

[R27] 算术展开
来源：http://je.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://ug.hahajie.cn

[R28] 浮点运算
来源：http://te.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://zt.huixiangedu.cn

[R29] 定义函数
来源：http://ay.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rs.muxihuayi.cn

[R30] 函数返回状态码
来源：http://me.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://ul.bjjhwx.cn

[R31] 局部变量
来源：http://fx.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://qp.hahajie.cn

[R32] 参数个数校验
来源：http://jo.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://so.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://bp.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sr.szxytkj.cn

[R34] 退出时清理
来源：http://jt.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ea.nszjky.cn

[R35] 后台执行并等待
来源：http://xf.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qf.asd995.cn

[R36] 并发执行多个任务
来源：http://dn.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zg.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://pe.huanxung.cn

files=$(ls -1)
来源：http://pn.muxihuayi.cn

[R38] 管道串联
来源：http://rq.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://hw.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://zn.hahajie.cn

cmd > out.log 2>&1
来源：http://ue.gzmigu.cn

[R40] 追加写日志
来源：http://ns.haigaiapp.cn

echo "log" >> out.log
来源：http://bh.nicolike.cn

[R41] 丢弃输出
来源：http://zi.nicolike.cn

cmd >/dev/null 2>&1
来源：http://pu.haigaiapp.cn

[R42] 输入重定向
来源：http://dc.muxihuayi.cn

wc -l < a.txt
来源：http://qh.hahajie.cn

[R43] 按名字查找文件
来源：http://gt.gzmigu.cn

find . -name "*.log" -type f
来源：http://sj.shtwfgs.cn

[R44] 按修改时间查找
来源：http://bb.9csxet.cn

find . -mtime -7 -type f
来源：http://lk.wgjwhj.cn

[R45] 批量删除
来源：http://wa.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://to.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://wl.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hg.shxzskj.cn

[R47] sed 单行替换
来源：http://ub.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dd.wgjwhj.cn

[R48] awk 取指定列
来源：http://gu.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://ib.9csxet.cn

[R49] awk 带条件
来源：http://bh.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pq.colortex.cn

[R50] awk 求和
来源：http://jt.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qe.hahajie.cn

[R51] 排序去重取前几
来源：http://zh.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cy.jianghongdianzi.cn

[R52] 统计行数
来源：http://pp.newstarts.cn

wc -l a.txt
来源：http://hb.asd995.cn

[R53] 查看文件头与实时尾
来源：http://zz.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sp.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://ix.nicolike.cn

diff a.txt b.txt
来源：http://et.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://sm.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kf.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://tb.nicolike.cn

scp file user@host:/path/
来源：http://wl.gzmigu.cn

[R57] 远程执行命令
来源：http://lf.haigaiapp.cn

ssh user@host 'uptime'
来源：http://pd.yuexingan06.cn

[R58] 下载文件
来源：http://nc.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://st.wgjwhj.cn

[R59] 发 POST JSON
来源：http://nj.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://do.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://px.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ai.szxytkj.cn

[R61] 磁盘占用
来源：http://mq.shxzukj.cn

df -h;  du -sh *
来源：http://ha.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://ck.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://lv.hnjuh.cn

[R63] 内存与进程
来源：http://dm.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://ia.shxzukj.cn

[R64] 结束进程
来源：http://zh.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://aa.nszjky.cn

[R65] 查看端口占用
来源：http://hk.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ru.lnxyls.cn

[R66] 定时任务
来源：http://yg.szsharing.cn

crontab -e;  crontab -l
来源：http://iv.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://ps.szsharing.cn

openssl rand -hex 16
来源：http://jo.panjiajie.cn

[R68] 计算文件校验值
来源：http://va.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pv.yuexingan06.cn

[R69] 生成随机密码
来源：http://gm.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://zk.huixiangedu.cn

[R70] 时间戳与互转
来源：http://le.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://ua.chemitech.net.cn

[R71] 日期格式化
来源：http://ij.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bk.yuexingan06.cn

[R72] 等待端口就绪
来源：http://ho.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vj.hahajie.cn

[R73] 分割大日志
来源：http://hi.hahajie.cn

split -l 1000 big.log part_
来源：http://qp.yuexingan06.cn

[R74] 批量重命名
来源：http://yd.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ax.szsharing.cn

[R75] 导出环境变量
来源：http://zd.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://cq.huixiangedu.cn

[R76] 使用临时文件
来源：http://cz.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fy.colortex.cn

[R77] 读取用户输入
来源：http://rn.colortex.cn

read -rp "请输入: " ans
来源：http://qq.szxytkj.cn

[R78] 交互式菜单
来源：http://kt.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rk.panjiajie.cn

[R79] 解析命令行选项
来源：http://gv.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tg.asd995.cn

[R80] 查看脚本执行耗时
来源：http://po.huanxung.cn

time ./run.sh
来源：http://br.yuexingan06.cn

================================================================================
来源：http://gh.huanxung.cn

S. C / C++ 专题
来源：http://ex.shxzukj.cn

================================================================================
来源：http://ll.huixinmuqiang.cn

[S01] C：Hello World
来源：http://pg.bookmarksfly.cn

#include <stdio.h>
来源：http://bh.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ro.asd995.cn

[S02] C：变量与格式化输出
来源：http://xz.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://di.yuntaijiaju.cn

[S03] C：读入整数
来源：http://ke.9csxet.cn

int x; scanf("%d", &x);
来源：http://dk.panjiajie.cn

[S04] C：字符串复制
来源：http://ii.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ss.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://xo.szsharing.cn

strlen(s)
来源：http://li.shtwfgs.cn

[S06] C：字符串比较
来源：http://kt.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://ny.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://xp.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mg.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://hr.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vv.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://mm.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fl.huanxung.cn

[S10] C：指针与解引用
来源：http://tf.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://ey.chemitech.net.cn

[S11] C：逐行读文件
来源：http://hn.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://vl.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sw.9csxet.cn

fclose(f);
来源：http://kt.huanxung.cn

[S12] C：写文件
来源：http://jk.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uw.hahajie.cn

[S13] C：宏定义
来源：http://dv.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bl.newstarts.cn

[S14] C：枚举
来源：http://bq.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://uy.wgjwhj.cn

[S15] C：类型转换
来源：http://sq.bookmarksfly.cn

(double) a / b
来源：http://bl.jctech888.com.cn

[S16] C：位操作置位
来源：http://vu.nicolike.cn

x |= (1 << 3);
来源：http://ob.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://cj.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sf.chemitech.net.cn

[S18] C：命令行参数
来源：http://tm.bjjhwx.cn

int main(int argc, char **argv)
来源：http://rp.gzmigu.cn

[S19] C：快速排序
来源：http://nd.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ja.newstarts.cn

[S20] C：二分查找
来源：http://wf.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pj.huanxung.cn

[S21] C：字符类别判断
来源：http://vd.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xs.wgjwhj.cn

[S22] C：字符串转数字
来源：http://vx.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wv.muxihuayi.cn

[S23] C：随机数
来源：http://gb.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://um.jctech888.com.cn

[S24] C：获取本地时间
来源：http://dn.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://th.521024.cn

[S25] C：内存拷贝
来源：http://gv.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://mz.9csxet.cn

[S26] C：内存清零
来源：http://en.hahajie.cn

memset(a, 0, sizeof a);
来源：http://fm.jianghongdianzi.cn

[S27] C：定义常量
来源：http://wj.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://ez.lnxyls.cn

[S28] C：静态变量
来源：http://tz.wgjwhj.cn

static int counter = 0;
来源：http://vp.bjjhwx.cn

[S29] C：变参函数
来源：http://wt.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kh.hnjuh.cn

[S30] C：头文件保护
来源：http://ye.szxytkj.cn

#ifndef X_H
来源：http://wy.jianghongdianzi.cn

#define X_H
来源：http://zg.newstarts.cn

#endif
来源：http://rd.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://vo.bjjhwx.cn

#include <iostream>
来源：http://tw.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://nn.521024.cn

[S32] C++：字符串
来源：http://tz.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://kn.jctech888.com.cn

[S33] C++：vector 增删
来源：http://gs.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ff.huanxung.cn

[S34] C++：遍历 vector
来源：http://ao.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://rn.hahajie.cn

[S35] C++：map
来源：http://ze.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://in.asd995.cn

[S36] C++：unordered_map
来源：http://or.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dd.nicolike.cn

[S37] C++：set
来源：http://kp.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nf.nszjky.cn

[S38] C++：排序
来源：http://in.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://ws.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://rz.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vl.lnxyls.cn

[S40] C++：查找元素
来源：http://ay.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://io.nicolike.cn

[S41] C++：类与构造函数
来源：http://ht.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ef.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://lk.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://qn.colortex.cn

[S43] C++：智能指针
来源：http://et.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://iy.colortex.cn

[S44] C++：引用传参
来源：http://sy.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://qm.huixiangedu.cn

[S45] C++：lambda
来源：http://js.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zk.9csxet.cn

[S46] C++：函数模板
来源：http://an.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bq.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://ms.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qd.panjiajie.cn

[S48] C++：逐行读文件
来源：http://nd.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oz.colortex.cn

while (std::getline(in, line)) { }
来源：http://ud.szsharing.cn

[S49] C++：写文件
来源：http://vc.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ir.shxzskj.cn

[S50] C++：格式化数字
来源：http://iw.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bm.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://cp.lnxyls.cn

static_cast<double>(a) / b
来源：http://fq.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://pt.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://kz.shtwfgs.cn

[S53] C++：移动语义
来源：http://kq.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://vs.gzmigu.cn

[S54] C++：异常处理
来源：http://ym.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cj.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://ka.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zx.muxihuayi.cn

[S56] C++：optional
来源：http://iv.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://li.wgjwhj.cn

[S57] C++：编译期常量
来源：http://mm.huixiangedu.cn

constexpr int N = 10;
来源：http://ol.szsharing.cn

[S58] C++：命名空间
来源：http://gc.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://pq.bookmarksfly.cn

[S59] C++：静态断言
来源：http://om.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ze.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://iw.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dg.haigaiapp.cn

================================================================================
来源：http://do.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wc.colortex.cn

================================================================================
来源：http://po.521024.cn

[T01] Kotlin：Hello World
来源：http://rb.haigaiapp.cn

println("Hello")
来源：http://qp.newstarts.cn

[T02] Kotlin：变量
来源：http://te.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://up.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://uf.huanxung.cn

"值: $b"
来源：http://vx.lnxyls.cn

[T04] Kotlin：空安全
来源：http://ly.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://dk.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://xc.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ec.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://jh.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xl.521024.cn

[T07] Kotlin：集合过滤
来源：http://ds.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ls.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://ol.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://gi.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://ku.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://ox.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://kc.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tv.huanxung.cn

[T11] Kotlin：协程
来源：http://jt.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jd.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://cy.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://ui.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://tq.9csxet.cn

val m = mapOf("a" to 1)
来源：http://fh.shxzskj.cn

[T14] Kotlin：循环
来源：http://yz.szxytkj.cn

for (i in 1..10) println(i)
来源：http://dn.bjjhwx.cn

[T15] Kotlin：接口
来源：http://lh.szsharing.cn

interface Shape { fun area(): Double }
来源：http://ej.hnjuh.cn

[T16] Swift：Hello World
来源：http://zh.muxihuayi.cn

print("Hello")
来源：http://zt.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://ma.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://ka.panjiajie.cn

[T18] Swift：字符串插值
来源：http://zq.szsharing.cn

"值: \(b)"
来源：http://bn.szxytkj.cn


<!-- 参考信息 -->