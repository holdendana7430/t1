代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sv.colortex.cn

[R16] until 等待条件
来源：http://db.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kx.asd995.cn

[R17] 数组定义与取值
来源：http://hf.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sg.colortex.cn

[R18] 遍历数组
来源：http://mk.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jg.bjjhwx.cn

[R19] 数组长度
来源：http://uv.wgjwhj.cn

echo "${#arr[@]}"
来源：http://uk.hahajie.cn

[R20] 关联数组（字典）
来源：http://en.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qp.szxytkj.cn

[R21] 字符串长度
来源：http://sv.bookmarksfly.cn

echo "${#s}"
来源：http://fc.jctech888.com.cn

[R22] 截取子串
来源：http://yz.chemitech.net.cn

echo "${s:0:5}"
来源：http://or.huixinmuqiang.cn

[R23] 字符串替换
来源：http://nx.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mn.bjjhwx.cn

[R24] 大小写转换
来源：http://gf.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gh.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://te.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rx.nicolike.cn

[R26] 命令替换
来源：http://le.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://xj.newstarts.cn

[R27] 算术展开
来源：http://wn.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://hu.yuntaijiaju.cn

[R28] 浮点运算
来源：http://gg.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://hj.shtwfgs.cn

[R29] 定义函数
来源：http://ym.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sm.shtwfgs.cn

[R30] 函数返回状态码
来源：http://uy.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://oo.wgjwhj.cn

[R31] 局部变量
来源：http://ja.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://hn.521024.cn

[R32] 参数个数校验
来源：http://eu.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eo.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://dl.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ee.nszjky.cn

[R34] 退出时清理
来源：http://ab.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ub.panjiajie.cn

[R35] 后台执行并等待
来源：http://un.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://we.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://gl.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oz.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://yc.yuntaijiaju.cn

files=$(ls -1)
来源：http://th.9csxet.cn

[R38] 管道串联
来源：http://vh.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://sc.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://mk.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://ql.nszjky.cn

[R40] 追加写日志
来源：http://tn.9csxet.cn

echo "log" >> out.log
来源：http://oz.lnxyls.cn

[R41] 丢弃输出
来源：http://gu.hahajie.cn

cmd >/dev/null 2>&1
来源：http://no.szsharing.cn

[R42] 输入重定向
来源：http://ha.colortex.cn

wc -l < a.txt
来源：http://kl.shtwfgs.cn

[R43] 按名字查找文件
来源：http://rb.jctech888.com.cn

find . -name "*.log" -type f
来源：http://iq.chemitech.net.cn

[R44] 按修改时间查找
来源：http://ap.bjjhwx.cn

find . -mtime -7 -type f
来源：http://cx.nicolike.cn

[R45] 批量删除
来源：http://nc.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://yx.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://ke.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ax.wgjwhj.cn

[R47] sed 单行替换
来源：http://ql.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qs.szsharing.cn

[R48] awk 取指定列
来源：http://js.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://fb.chemitech.net.cn

[R49] awk 带条件
来源：http://nw.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cy.yuexingan06.cn

[R50] awk 求和
来源：http://iu.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ed.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://qm.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ji.jctech888.com.cn

[R52] 统计行数
来源：http://tq.newstarts.cn

wc -l a.txt
来源：http://vt.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://oy.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gt.nicolike.cn

[R54] 比较两个文件
来源：http://fr.nszjky.cn

diff a.txt b.txt
来源：http://oq.asd995.cn

[R55] 压缩与解压
来源：http://lc.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sy.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://fn.jctech888.com.cn

scp file user@host:/path/
来源：http://li.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://mu.chemitech.net.cn

ssh user@host 'uptime'
来源：http://jz.jctech888.com.cn

[R58] 下载文件
来源：http://sy.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wy.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://mt.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ae.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://dc.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pt.chemitech.net.cn

[R61] 磁盘占用
来源：http://nv.521024.cn

df -h;  du -sh *
来源：http://co.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://ny.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://nu.bookmarksfly.cn

[R63] 内存与进程
来源：http://au.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://om.bookmarksfly.cn

[R64] 结束进程
来源：http://li.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://bf.shxzukj.cn

[R65] 查看端口占用
来源：http://tl.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zt.jianghongdianzi.cn

[R66] 定时任务
来源：http://yg.muxihuayi.cn

crontab -e;  crontab -l
来源：http://fw.huanxung.cn

[R67] 生成随机十六进制串
来源：http://bx.newstarts.cn

openssl rand -hex 16
来源：http://ha.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://gz.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ep.asd995.cn

[R69] 生成随机密码
来源：http://lf.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://so.hnjuh.cn

[R70] 时间戳与互转
来源：http://xv.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://vq.jianghongdianzi.cn

[R71] 日期格式化
来源：http://bf.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fn.huixiangedu.cn

[R72] 等待端口就绪
来源：http://fq.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fy.gzmigu.cn

[R73] 分割大日志
来源：http://cs.muxihuayi.cn

split -l 1000 big.log part_
来源：http://xm.shxzskj.cn

[R74] 批量重命名
来源：http://cc.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ij.wgjwhj.cn

[R75] 导出环境变量
来源：http://ov.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://gc.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://zd.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dk.nicolike.cn

[R77] 读取用户输入
来源：http://pm.yuexingan06.cn

read -rp "请输入: " ans
来源：http://ov.huanxung.cn

[R78] 交互式菜单
来源：http://nc.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ql.521024.cn

[R79] 解析命令行选项
来源：http://kr.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ud.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://cj.huanxung.cn

time ./run.sh
来源：http://ot.bjjhwx.cn

================================================================================
来源：http://zu.bookmarksfly.cn

S. C / C++ 专题
来源：http://ep.nszjky.cn

================================================================================
来源：http://wl.huixiangedu.cn

[S01] C：Hello World
来源：http://mn.bjjhwx.cn

#include <stdio.h>
来源：http://ok.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zt.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://cm.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://lc.bjjhwx.cn

[S03] C：读入整数
来源：http://as.gzmigu.cn

int x; scanf("%d", &x);
来源：http://lv.shxzukj.cn

[S04] C：字符串复制
来源：http://mg.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rc.521024.cn

[S05] C：字符串长度
来源：http://kl.asd995.cn

strlen(s)
来源：http://vu.szsharing.cn

[S06] C：字符串比较
来源：http://he.yuexingan06.cn

strcmp(a, b) == 0
来源：http://wg.colortex.cn

[S07] C：数组遍历求和
来源：http://sc.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://on.521024.cn

[S08] C：动态内存分配与释放
来源：http://bm.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nu.colortex.cn

[S09] C：结构体定义与初始化
来源：http://ah.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cd.newstarts.cn

[S10] C：指针与解引用
来源：http://bm.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://jk.wgjwhj.cn

[S11] C：逐行读文件
来源：http://cc.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://kz.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hk.szxytkj.cn

fclose(f);
来源：http://ks.shxzskj.cn

[S12] C：写文件
来源：http://ke.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uc.wgjwhj.cn

[S13] C：宏定义
来源：http://wf.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sj.hahajie.cn

[S14] C：枚举
来源：http://gt.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://cp.lnxyls.cn

[S15] C：类型转换
来源：http://le.shxzskj.cn

(double) a / b
来源：http://df.panjiajie.cn

[S16] C：位操作置位
来源：http://rn.bookmarksfly.cn

x |= (1 << 3);
来源：http://be.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://he.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ne.jctech888.com.cn

[S18] C：命令行参数
来源：http://du.szxytkj.cn

int main(int argc, char **argv)
来源：http://sm.9csxet.cn

[S19] C：快速排序
来源：http://dc.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zo.newstarts.cn

[S20] C：二分查找
来源：http://zi.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://es.newstarts.cn

[S21] C：字符类别判断
来源：http://ym.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kp.bjjhwx.cn

[S22] C：字符串转数字
来源：http://rc.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dx.szsharing.cn

[S23] C：随机数
来源：http://di.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nl.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://wo.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vv.huixiangedu.cn

[S25] C：内存拷贝
来源：http://ml.bjjhwx.cn

memcpy(dst, src, n);
来源：http://fl.muxihuayi.cn

[S26] C：内存清零
来源：http://db.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://hi.yuntaijiaju.cn

[S27] C：定义常量
来源：http://ze.newstarts.cn

const double PI = 3.14159;
来源：http://jm.wgjwhj.cn

[S28] C：静态变量
来源：http://pd.yuntaijiaju.cn

static int counter = 0;
来源：http://fv.shtwfgs.cn

[S29] C：变参函数
来源：http://lv.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pa.lnxyls.cn

[S30] C：头文件保护
来源：http://ge.yuexingan06.cn

#ifndef X_H
来源：http://gk.panjiajie.cn

#define X_H
来源：http://ab.gzmigu.cn

#endif
来源：http://uz.hnjuh.cn

[S31] C++：Hello World
来源：http://jc.hahajie.cn

#include <iostream>
来源：http://zo.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://rd.jianghongdianzi.cn

[S32] C++：字符串
来源：http://yb.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://si.shtwfgs.cn

[S33] C++：vector 增删
来源：http://nd.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zb.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://hp.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://wn.shtwfgs.cn

[S35] C++：map
来源：http://jf.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://np.panjiajie.cn

[S36] C++：unordered_map
来源：http://ic.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sf.nszjky.cn

[S37] C++：set
来源：http://gt.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hq.wgjwhj.cn

[S38] C++：排序
来源：http://mg.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://un.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://pc.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ct.shtwfgs.cn

[S40] C++：查找元素
来源：http://ct.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hw.9csxet.cn

[S41] C++：类与构造函数
来源：http://jq.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cg.szsharing.cn

[S42] C++：继承与虚函数
来源：http://wi.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://se.wgjwhj.cn

[S43] C++：智能指针
来源：http://av.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://xv.9csxet.cn

[S44] C++：引用传参
来源：http://bk.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://yu.huixiangedu.cn

[S45] C++：lambda
来源：http://bh.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ik.jctech888.com.cn

[S46] C++：函数模板
来源：http://mk.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hb.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://yl.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yh.521024.cn

[S48] C++：逐行读文件
来源：http://yh.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xj.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://ju.gzmigu.cn

[S49] C++：写文件
来源：http://vv.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://su.newstarts.cn

[S50] C++：格式化数字
来源：http://je.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uu.szsharing.cn

[S51] C++：显式类型转换
来源：http://kx.hahajie.cn

static_cast<double>(a) / b
来源：http://wi.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://rw.nszjky.cn

int size() const noexcept { return n_; }
来源：http://do.521024.cn

[S53] C++：移动语义
来源：http://bq.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://ry.huanxung.cn

[S54] C++：异常处理
来源：http://xi.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nm.gzmigu.cn

[S55] C++：结构化绑定
来源：http://nv.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jm.hnjuh.cn

[S56] C++：optional
来源：http://mt.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wl.hahajie.cn

[S57] C++：编译期常量
来源：http://fv.wgjwhj.cn

constexpr int N = 10;
来源：http://zw.nicolike.cn

[S58] C++：命名空间
来源：http://dp.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://ru.szxytkj.cn

[S59] C++：静态断言
来源：http://op.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qg.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://ga.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ec.jianghongdianzi.cn

================================================================================
来源：http://xs.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bj.huixiangedu.cn

================================================================================
来源：http://po.asd995.cn

[T01] Kotlin：Hello World
来源：http://nd.jctech888.com.cn

println("Hello")
来源：http://sz.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://bl.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ol.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://wr.shxzskj.cn

"值: $b"
来源：http://ev.nicolike.cn

[T04] Kotlin：空安全
来源：http://ls.colortex.cn

val n: String? = null;  n?.length
来源：http://wj.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://db.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zf.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://uh.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nu.asd995.cn

[T07] Kotlin：集合过滤
来源：http://oc.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uu.newstarts.cn

[T08] Kotlin：数据类
来源：http://wd.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://vk.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://kg.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://nv.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://hw.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yp.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://ir.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ov.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://gw.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://cn.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://fz.521024.cn

val m = mapOf("a" to 1)
来源：http://pa.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://mo.hahajie.cn

for (i in 1..10) println(i)
来源：http://iq.521024.cn

[T15] Kotlin：接口
来源：http://mn.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://sv.lnxyls.cn

[T16] Swift：Hello World
来源：http://jr.szxytkj.cn

print("Hello")
来源：http://ag.gzmigu.cn

[T17] Swift：变量与常量
来源：http://xy.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://mt.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://ko.newstarts.cn

"值: \(b)"
来源：http://zr.chemitech.net.cn


<!-- 参考信息 -->