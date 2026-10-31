代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://re.hahajie.cn

[R16] until 等待条件
来源：http://er.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lq.szxytkj.cn

[R17] 数组定义与取值
来源：http://ri.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ds.nszjky.cn

[R18] 遍历数组
来源：http://ri.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ak.gzmigu.cn

[R19] 数组长度
来源：http://si.huanxung.cn

echo "${#arr[@]}"
来源：http://ni.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://le.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cy.jctech888.com.cn

[R21] 字符串长度
来源：http://qc.yuexingan06.cn

echo "${#s}"
来源：http://vo.9csxet.cn

[R22] 截取子串
来源：http://xz.nszjky.cn

echo "${s:0:5}"
来源：http://en.jctech888.com.cn

[R23] 字符串替换
来源：http://vc.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wk.hnjuh.cn

[R24] 大小写转换
来源：http://eh.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ws.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://iy.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sz.panjiajie.cn

[R26] 命令替换
来源：http://ub.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://dy.jianghongdianzi.cn

[R27] 算术展开
来源：http://an.szsharing.cn

echo $((1 + 2 * 3))
来源：http://dg.bjjhwx.cn

[R28] 浮点运算
来源：http://yd.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://hq.huixinmuqiang.cn

[R29] 定义函数
来源：http://pt.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://km.9csxet.cn

[R30] 函数返回状态码
来源：http://rg.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://xl.huixiangedu.cn

[R31] 局部变量
来源：http://lq.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://hg.bookmarksfly.cn

[R32] 参数个数校验
来源：http://wq.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jw.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://eo.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ym.521024.cn

[R34] 退出时清理
来源：http://ja.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cf.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://ih.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cv.shxzukj.cn

[R36] 并发执行多个任务
来源：http://hy.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ip.asd995.cn

[R37] 把输出赋给变量
来源：http://qw.newstarts.cn

files=$(ls -1)
来源：http://uy.shxzskj.cn

[R38] 管道串联
来源：http://ep.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://od.asd995.cn

[R39] 重定向标准输出与错误
来源：http://he.bjjhwx.cn

cmd > out.log 2>&1
来源：http://qr.hnjuh.cn

[R40] 追加写日志
来源：http://xx.huanxung.cn

echo "log" >> out.log
来源：http://rw.521024.cn

[R41] 丢弃输出
来源：http://yl.nszjky.cn

cmd >/dev/null 2>&1
来源：http://vd.szxytkj.cn

[R42] 输入重定向
来源：http://oz.panjiajie.cn

wc -l < a.txt
来源：http://ma.shtwfgs.cn

[R43] 按名字查找文件
来源：http://iq.wgjwhj.cn

find . -name "*.log" -type f
来源：http://zl.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://qe.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://cp.muxihuayi.cn

[R45] 批量删除
来源：http://am.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://ho.huanxung.cn

[R46] 递归替换文件内容
来源：http://xn.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vz.panjiajie.cn

[R47] sed 单行替换
来源：http://yh.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sa.asd995.cn

[R48] awk 取指定列
来源：http://py.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://id.colortex.cn

[R49] awk 带条件
来源：http://ui.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://to.521024.cn

[R50] awk 求和
来源：http://jt.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qe.gzmigu.cn

[R51] 排序去重取前几
来源：http://bj.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ck.shxzukj.cn

[R52] 统计行数
来源：http://ww.hahajie.cn

wc -l a.txt
来源：http://gt.asd995.cn

[R53] 查看文件头与实时尾
来源：http://me.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gb.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://we.wgjwhj.cn

diff a.txt b.txt
来源：http://rx.hnjuh.cn

[R55] 压缩与解压
来源：http://cr.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lj.9csxet.cn

[R56] 远程拷贝
来源：http://ws.asd995.cn

scp file user@host:/path/
来源：http://pc.hnjuh.cn

[R57] 远程执行命令
来源：http://ja.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://xf.szxytkj.cn

[R58] 下载文件
来源：http://kq.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ii.szxytkj.cn

[R59] 发 POST JSON
来源：http://xm.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ou.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://ji.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pd.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://yd.bjjhwx.cn

df -h;  du -sh *
来源：http://ij.hahajie.cn

[R62] 找最占空间的文件
来源：http://iz.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://tn.9csxet.cn

[R63] 内存与进程
来源：http://ev.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://lv.521024.cn

[R64] 结束进程
来源：http://vp.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://ox.nszjky.cn

[R65] 查看端口占用
来源：http://bj.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://db.huixinmuqiang.cn

[R66] 定时任务
来源：http://lp.lnxyls.cn

crontab -e;  crontab -l
来源：http://to.newstarts.cn

[R67] 生成随机十六进制串
来源：http://tg.panjiajie.cn

openssl rand -hex 16
来源：http://ui.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://cv.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iv.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://yv.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://jf.huanxung.cn

[R70] 时间戳与互转
来源：http://jw.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://wu.szsharing.cn

[R71] 日期格式化
来源：http://nr.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lr.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://el.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vt.shxzskj.cn

[R73] 分割大日志
来源：http://fr.shxzukj.cn

split -l 1000 big.log part_
来源：http://wl.muxihuayi.cn

[R74] 批量重命名
来源：http://wq.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gj.9csxet.cn

[R75] 导出环境变量
来源：http://zh.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://lv.huixiangedu.cn

[R76] 使用临时文件
来源：http://lg.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nt.szsharing.cn

[R77] 读取用户输入
来源：http://vg.colortex.cn

read -rp "请输入: " ans
来源：http://ig.asd995.cn

[R78] 交互式菜单
来源：http://ic.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pm.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://fs.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ye.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://yf.chemitech.net.cn

time ./run.sh
来源：http://hj.gzmigu.cn

================================================================================
来源：http://os.huixinmuqiang.cn

S. C / C++ 专题
来源：http://ms.bookmarksfly.cn

================================================================================
来源：http://qc.shxzukj.cn

[S01] C：Hello World
来源：http://bd.9csxet.cn

#include <stdio.h>
来源：http://zf.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bg.asd995.cn

[S02] C：变量与格式化输出
来源：http://ie.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://bu.bookmarksfly.cn

[S03] C：读入整数
来源：http://wd.shxzukj.cn

int x; scanf("%d", &x);
来源：http://bm.hahajie.cn

[S04] C：字符串复制
来源：http://jg.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pr.hahajie.cn

[S05] C：字符串长度
来源：http://jz.jianghongdianzi.cn

strlen(s)
来源：http://zg.haigaiapp.cn

[S06] C：字符串比较
来源：http://je.bjjhwx.cn

strcmp(a, b) == 0
来源：http://ut.shxzukj.cn

[S07] C：数组遍历求和
来源：http://oi.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cb.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://zx.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sp.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://wm.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sa.bjjhwx.cn

[S10] C：指针与解引用
来源：http://oe.colortex.cn

int *p = &a;  *p = 5;
来源：http://nz.huanxung.cn

[S11] C：逐行读文件
来源：http://xj.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://zk.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iy.huixinmuqiang.cn

fclose(f);
来源：http://ok.haigaiapp.cn

[S12] C：写文件
来源：http://wh.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hf.gzmigu.cn

[S13] C：宏定义
来源：http://zh.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ln.colortex.cn

[S14] C：枚举
来源：http://kf.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://dc.jianghongdianzi.cn

[S15] C：类型转换
来源：http://vc.lnxyls.cn

(double) a / b
来源：http://ty.nicolike.cn

[S16] C：位操作置位
来源：http://dc.nszjky.cn

x |= (1 << 3);
来源：http://ty.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://yu.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xc.szxytkj.cn

[S18] C：命令行参数
来源：http://qz.lnxyls.cn

int main(int argc, char **argv)
来源：http://hc.szsharing.cn

[S19] C：快速排序
来源：http://qv.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rd.lnxyls.cn

[S20] C：二分查找
来源：http://ta.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oe.nicolike.cn

[S21] C：字符类别判断
来源：http://yx.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cq.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://sh.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pn.gzmigu.cn

[S23] C：随机数
来源：http://hp.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ws.colortex.cn

[S24] C：获取本地时间
来源：http://dm.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wu.newstarts.cn

[S25] C：内存拷贝
来源：http://ss.shtwfgs.cn

memcpy(dst, src, n);
来源：http://un.jianghongdianzi.cn

[S26] C：内存清零
来源：http://zm.szsharing.cn

memset(a, 0, sizeof a);
来源：http://fw.yuexingan06.cn

[S27] C：定义常量
来源：http://ya.muxihuayi.cn

const double PI = 3.14159;
来源：http://ia.asd995.cn

[S28] C：静态变量
来源：http://uy.huixinmuqiang.cn

static int counter = 0;
来源：http://io.shtwfgs.cn

[S29] C：变参函数
来源：http://vm.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ez.wgjwhj.cn

[S30] C：头文件保护
来源：http://pm.hahajie.cn

#ifndef X_H
来源：http://jr.hnjuh.cn

#define X_H
来源：http://pj.yuexingan06.cn

#endif
来源：http://yv.szsharing.cn

[S31] C++：Hello World
来源：http://xt.yuntaijiaju.cn

#include <iostream>
来源：http://dp.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://lm.9csxet.cn

[S32] C++：字符串
来源：http://pa.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://jh.newstarts.cn

[S33] C++：vector 增删
来源：http://gn.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wr.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://wf.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://cu.shxzskj.cn

[S35] C++：map
来源：http://ek.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mu.shtwfgs.cn

[S36] C++：unordered_map
来源：http://lv.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ai.shtwfgs.cn

[S37] C++：set
来源：http://ev.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ng.9csxet.cn

[S38] C++：排序
来源：http://ar.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://ip.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://co.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ol.chemitech.net.cn

[S40] C++：查找元素
来源：http://do.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uh.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://nf.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dh.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://zl.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://ah.lnxyls.cn

[S43] C++：智能指针
来源：http://nv.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://pl.hahajie.cn

[S44] C++：引用传参
来源：http://hw.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://li.panjiajie.cn

[S45] C++：lambda
来源：http://ck.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mv.szxytkj.cn

[S46] C++：函数模板
来源：http://xa.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jz.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://oe.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ml.asd995.cn

[S48] C++：逐行读文件
来源：http://ki.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://eq.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://ti.shxzskj.cn

[S49] C++：写文件
来源：http://tr.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jr.wgjwhj.cn

[S50] C++：格式化数字
来源：http://xy.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uf.newstarts.cn

[S51] C++：显式类型转换
来源：http://do.colortex.cn

static_cast<double>(a) / b
来源：http://rf.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://by.521024.cn

int size() const noexcept { return n_; }
来源：http://ty.shxzskj.cn

[S53] C++：移动语义
来源：http://gb.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://rd.bjjhwx.cn

[S54] C++：异常处理
来源：http://hg.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ns.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://yn.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ko.jctech888.com.cn

[S56] C++：optional
来源：http://qw.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://my.newstarts.cn

[S57] C++：编译期常量
来源：http://vj.bjjhwx.cn

constexpr int N = 10;
来源：http://vg.hnjuh.cn

[S58] C++：命名空间
来源：http://nn.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://bl.colortex.cn

[S59] C++：静态断言
来源：http://gh.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ol.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://dy.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cj.hahajie.cn

================================================================================
来源：http://sf.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dj.szxytkj.cn

================================================================================
来源：http://qc.huanxung.cn

[T01] Kotlin：Hello World
来源：http://df.asd995.cn

println("Hello")
来源：http://kh.lnxyls.cn

[T02] Kotlin：变量
来源：http://pl.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gj.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://vx.haigaiapp.cn

"值: $b"
来源：http://hy.nicolike.cn

[T04] Kotlin：空安全
来源：http://mi.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://aw.521024.cn

[T05] Kotlin：when 表达式
来源：http://gm.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bt.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://mi.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uz.huixinmuqiang.cn

[T07] Kotlin：集合过滤
来源：http://hk.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://av.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://fl.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://hq.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://gv.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://ku.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://jq.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qh.gzmigu.cn

[T11] Kotlin：协程
来源：http://ap.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wi.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://ze.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://zn.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://mo.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://el.521024.cn

[T14] Kotlin：循环
来源：http://gs.521024.cn

for (i in 1..10) println(i)
来源：http://yj.szxytkj.cn

[T15] Kotlin：接口
来源：http://ql.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://qt.muxihuayi.cn

[T16] Swift：Hello World
来源：http://kt.shxzukj.cn

print("Hello")
来源：http://wj.huanxung.cn

[T17] Swift：变量与常量
来源：http://ed.colortex.cn

var a = 1;  let b = 2
来源：http://ar.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://pv.9csxet.cn

"值: \(b)"
来源：http://ex.yuexingan06.cn


<!-- 参考信息 -->