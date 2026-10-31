代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://xu.hahajie.cn

[R14] C 风格 for
来源：http://vc.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ls.panjiajie.cn

[R15] while 逐行读文件
来源：http://jq.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ni.muxihuayi.cn

[R16] until 等待条件
来源：http://qi.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://he.panjiajie.cn

[R17] 数组定义与取值
来源：http://as.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zu.9csxet.cn

[R18] 遍历数组
来源：http://nm.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ys.521024.cn

[R19] 数组长度
来源：http://pc.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://rq.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://bb.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ar.colortex.cn

[R21] 字符串长度
来源：http://ys.hnjuh.cn

echo "${#s}"
来源：http://xc.jctech888.com.cn

[R22] 截取子串
来源：http://uv.nszjky.cn

echo "${s:0:5}"
来源：http://xf.chemitech.net.cn

[R23] 字符串替换
来源：http://et.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://md.huixiangedu.cn

[R24] 大小写转换
来源：http://mz.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qb.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://gt.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jy.shxzskj.cn

[R26] 命令替换
来源：http://su.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://lt.panjiajie.cn

[R27] 算术展开
来源：http://ez.colortex.cn

echo $((1 + 2 * 3))
来源：http://ph.9csxet.cn

[R28] 浮点运算
来源：http://kd.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://ey.huixiangedu.cn

[R29] 定义函数
来源：http://an.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://za.bjjhwx.cn

[R30] 函数返回状态码
来源：http://ll.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://ju.lnxyls.cn

[R31] 局部变量
来源：http://ge.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://rs.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://xi.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pv.asd995.cn

[R33] 捕获错误并提示行号
来源：http://xr.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iz.newstarts.cn

[R34] 退出时清理
来源：http://bx.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qr.bjjhwx.cn

[R35] 后台执行并等待
来源：http://rl.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jf.gzmigu.cn

[R36] 并发执行多个任务
来源：http://zo.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sv.shxzukj.cn

[R37] 把输出赋给变量
来源：http://kk.bjjhwx.cn

files=$(ls -1)
来源：http://sa.muxihuayi.cn

[R38] 管道串联
来源：http://cu.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://xs.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://bm.jctech888.com.cn

cmd > out.log 2>&1
来源：http://so.lnxyls.cn

[R40] 追加写日志
来源：http://zu.nszjky.cn

echo "log" >> out.log
来源：http://eq.9csxet.cn

[R41] 丢弃输出
来源：http://hh.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://wo.jianghongdianzi.cn

[R42] 输入重定向
来源：http://aq.yuntaijiaju.cn

wc -l < a.txt
来源：http://zi.521024.cn

[R43] 按名字查找文件
来源：http://rp.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://vo.nicolike.cn

[R44] 按修改时间查找
来源：http://th.9csxet.cn

find . -mtime -7 -type f
来源：http://me.9csxet.cn

[R45] 批量删除
来源：http://ip.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://aq.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://kx.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qz.huanxung.cn

[R47] sed 单行替换
来源：http://hk.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ho.szsharing.cn

[R48] awk 取指定列
来源：http://dt.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://ps.newstarts.cn

[R49] awk 带条件
来源：http://hw.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sh.muxihuayi.cn

[R50] awk 求和
来源：http://nc.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nn.jctech888.com.cn

[R51] 排序去重取前几
来源：http://fz.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qj.huixinmuqiang.cn

[R52] 统计行数
来源：http://lz.shxzukj.cn

wc -l a.txt
来源：http://mi.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://qv.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tl.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://vn.hahajie.cn

diff a.txt b.txt
来源：http://ka.newstarts.cn

[R55] 压缩与解压
来源：http://hu.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ly.yuexingan06.cn

[R56] 远程拷贝
来源：http://li.521024.cn

scp file user@host:/path/
来源：http://cq.wgjwhj.cn

[R57] 远程执行命令
来源：http://io.yuexingan06.cn

ssh user@host 'uptime'
来源：http://iq.yuntaijiaju.cn

[R58] 下载文件
来源：http://mn.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wy.hahajie.cn

[R59] 发 POST JSON
来源：http://qb.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gw.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://la.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qf.jctech888.com.cn

[R61] 磁盘占用
来源：http://dr.yuntaijiaju.cn

df -h;  du -sh *
来源：http://dj.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://sk.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://ef.colortex.cn

[R63] 内存与进程
来源：http://dl.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://mc.yuntaijiaju.cn

[R64] 结束进程
来源：http://wm.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://iw.huixiangedu.cn

[R65] 查看端口占用
来源：http://lr.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hw.muxihuayi.cn

[R66] 定时任务
来源：http://hv.newstarts.cn

crontab -e;  crontab -l
来源：http://bj.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://ei.yuexingan06.cn

openssl rand -hex 16
来源：http://tt.colortex.cn

[R68] 计算文件校验值
来源：http://ay.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gd.bjjhwx.cn

[R69] 生成随机密码
来源：http://wi.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://id.szxytkj.cn

[R70] 时间戳与互转
来源：http://qx.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://ms.nicolike.cn

[R71] 日期格式化
来源：http://qk.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ia.nszjky.cn

[R72] 等待端口就绪
来源：http://rd.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bj.panjiajie.cn

[R73] 分割大日志
来源：http://ji.nicolike.cn

split -l 1000 big.log part_
来源：http://wr.asd995.cn

[R74] 批量重命名
来源：http://rd.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uy.colortex.cn

[R75] 导出环境变量
来源：http://xv.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://yd.shxzukj.cn

[R76] 使用临时文件
来源：http://ea.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qr.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://nl.lnxyls.cn

read -rp "请输入: " ans
来源：http://bd.newstarts.cn

[R78] 交互式菜单
来源：http://xo.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wl.colortex.cn

[R79] 解析命令行选项
来源：http://im.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wh.521024.cn

[R80] 查看脚本执行耗时
来源：http://xh.newstarts.cn

time ./run.sh
来源：http://bn.jianghongdianzi.cn

================================================================================
来源：http://ca.yuntaijiaju.cn

S. C / C++ 专题
来源：http://hd.huixinmuqiang.cn

================================================================================
来源：http://pz.hahajie.cn

[S01] C：Hello World
来源：http://pq.asd995.cn

#include <stdio.h>
来源：http://in.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lx.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://vr.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://ua.asd995.cn

[S03] C：读入整数
来源：http://qn.asd995.cn

int x; scanf("%d", &x);
来源：http://xb.panjiajie.cn

[S04] C：字符串复制
来源：http://we.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oq.colortex.cn

[S05] C：字符串长度
来源：http://hn.jianghongdianzi.cn

strlen(s)
来源：http://jq.huixiangedu.cn

[S06] C：字符串比较
来源：http://rp.szxytkj.cn

strcmp(a, b) == 0
来源：http://lk.lnxyls.cn

[S07] C：数组遍历求和
来源：http://is.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xt.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://qr.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sn.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://pb.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zf.wgjwhj.cn

[S10] C：指针与解引用
来源：http://yd.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://ye.chemitech.net.cn

[S11] C：逐行读文件
来源：http://ub.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://ok.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lp.hnjuh.cn

fclose(f);
来源：http://oq.gzmigu.cn

[S12] C：写文件
来源：http://hq.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nd.haigaiapp.cn

[S13] C：宏定义
来源：http://hd.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tm.shtwfgs.cn

[S14] C：枚举
来源：http://bf.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://yf.huixiangedu.cn

[S15] C：类型转换
来源：http://bn.yuexingan06.cn

(double) a / b
来源：http://ar.newstarts.cn

[S16] C：位操作置位
来源：http://vw.bookmarksfly.cn

x |= (1 << 3);
来源：http://fu.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://dz.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pm.colortex.cn

[S18] C：命令行参数
来源：http://zf.9csxet.cn

int main(int argc, char **argv)
来源：http://ys.521024.cn

[S19] C：快速排序
来源：http://ww.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lz.nicolike.cn

[S20] C：二分查找
来源：http://qd.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mp.bjjhwx.cn

[S21] C：字符类别判断
来源：http://ip.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wg.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://sa.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ay.bjjhwx.cn

[S23] C：随机数
来源：http://cg.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pj.hahajie.cn

[S24] C：获取本地时间
来源：http://ba.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cn.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://re.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://qi.jctech888.com.cn

[S26] C：内存清零
来源：http://wt.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://jc.shtwfgs.cn

[S27] C：定义常量
来源：http://ro.chemitech.net.cn

const double PI = 3.14159;
来源：http://uc.shxzskj.cn

[S28] C：静态变量
来源：http://cn.huixiangedu.cn

static int counter = 0;
来源：http://tx.huixinmuqiang.cn

[S29] C：变参函数
来源：http://gn.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xs.shtwfgs.cn

[S30] C：头文件保护
来源：http://vn.panjiajie.cn

#ifndef X_H
来源：http://bi.szxytkj.cn

#define X_H
来源：http://lq.asd995.cn

#endif
来源：http://mu.huanxung.cn

[S31] C++：Hello World
来源：http://lw.lnxyls.cn

#include <iostream>
来源：http://px.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://uf.yuntaijiaju.cn

[S32] C++：字符串
来源：http://xg.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://ck.shxzskj.cn

[S33] C++：vector 增删
来源：http://cz.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tc.gzmigu.cn

[S34] C++：遍历 vector
来源：http://ec.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://px.shxzukj.cn

[S35] C++：map
来源：http://cq.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://un.nicolike.cn

[S36] C++：unordered_map
来源：http://oy.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rx.jianghongdianzi.cn

[S37] C++：set
来源：http://xw.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qg.huanxung.cn

[S38] C++：排序
来源：http://is.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://ab.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://hg.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mk.hahajie.cn

[S40] C++：查找元素
来源：http://wd.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ya.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://kv.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nr.szsharing.cn

[S42] C++：继承与虚函数
来源：http://rg.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://cq.nszjky.cn

[S43] C++：智能指针
来源：http://se.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://sb.szsharing.cn

[S44] C++：引用传参
来源：http://ii.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://rr.gzmigu.cn

[S45] C++：lambda
来源：http://nu.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sk.haigaiapp.cn

[S46] C++：函数模板
来源：http://da.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lh.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://ue.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://me.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://ap.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tv.nszjky.cn

while (std::getline(in, line)) { }
来源：http://ew.jctech888.com.cn

[S49] C++：写文件
来源：http://kk.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yu.jctech888.com.cn

[S50] C++：格式化数字
来源：http://ok.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nu.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://kd.hahajie.cn

static_cast<double>(a) / b
来源：http://ph.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://st.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://pi.nszjky.cn

[S53] C++：移动语义
来源：http://wj.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://db.bjjhwx.cn

[S54] C++：异常处理
来源：http://yj.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ay.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://ny.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yb.szsharing.cn

[S56] C++：optional
来源：http://lu.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iy.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://wo.haigaiapp.cn

constexpr int N = 10;
来源：http://uv.shtwfgs.cn

[S58] C++：命名空间
来源：http://zg.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://ii.bookmarksfly.cn

[S59] C++：静态断言
来源：http://ae.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yh.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://kc.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uz.shtwfgs.cn

================================================================================
来源：http://tr.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bm.colortex.cn

================================================================================
来源：http://bw.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://kw.chemitech.net.cn

println("Hello")
来源：http://hn.muxihuayi.cn

[T02] Kotlin：变量
来源：http://kc.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fr.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://ex.colortex.cn

"值: $b"
来源：http://pw.szxytkj.cn

[T04] Kotlin：空安全
来源：http://mb.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://ld.asd995.cn

[T05] Kotlin：when 表达式
来源：http://vr.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pl.nszjky.cn

[T06] Kotlin：集合映射
来源：http://ib.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vp.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://rl.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cy.panjiajie.cn

[T08] Kotlin：数据类
来源：http://rs.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://ns.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://ef.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://dj.9csxet.cn

[T10] Kotlin：默认参数
来源：http://oc.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pr.colortex.cn

[T11] Kotlin：协程
来源：http://ro.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ns.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://yp.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://bz.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://jg.szsharing.cn

val m = mapOf("a" to 1)
来源：http://td.colortex.cn

[T14] Kotlin：循环
来源：http://uf.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://md.shtwfgs.cn

[T15] Kotlin：接口
来源：http://ra.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://sn.521024.cn

[T16] Swift：Hello World
来源：http://wg.shxzskj.cn

print("Hello")
来源：http://ny.panjiajie.cn


<!-- 参考信息 -->