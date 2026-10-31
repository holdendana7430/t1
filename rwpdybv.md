代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://vs.haigaiapp.cn

[R14] C 风格 for
来源：http://sq.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gw.shtwfgs.cn

[R15] while 逐行读文件
来源：http://ww.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jo.bookmarksfly.cn

[R16] until 等待条件
来源：http://vh.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lc.lnxyls.cn

[R17] 数组定义与取值
来源：http://tu.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vi.chemitech.net.cn

[R18] 遍历数组
来源：http://xf.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fz.jctech888.com.cn

[R19] 数组长度
来源：http://ip.szsharing.cn

echo "${#arr[@]}"
来源：http://vc.huanxung.cn

[R20] 关联数组（字典）
来源：http://wr.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nu.9csxet.cn

[R21] 字符串长度
来源：http://ns.newstarts.cn

echo "${#s}"
来源：http://lc.lnxyls.cn

[R22] 截取子串
来源：http://dv.521024.cn

echo "${s:0:5}"
来源：http://jc.521024.cn

[R23] 字符串替换
来源：http://br.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://om.huanxung.cn

[R24] 大小写转换
来源：http://ay.nszjky.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bp.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://gh.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://er.panjiajie.cn

[R26] 命令替换
来源：http://yp.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://er.jctech888.com.cn

[R27] 算术展开
来源：http://yq.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://mj.chemitech.net.cn

[R28] 浮点运算
来源：http://tb.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://me.bookmarksfly.cn

[R29] 定义函数
来源：http://ee.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ss.haigaiapp.cn

[R30] 函数返回状态码
来源：http://mk.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://rk.shxzukj.cn

[R31] 局部变量
来源：http://am.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://jo.muxihuayi.cn

[R32] 参数个数校验
来源：http://yx.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xk.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://ai.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eo.haigaiapp.cn

[R34] 退出时清理
来源：http://gj.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rl.huanxung.cn

[R35] 后台执行并等待
来源：http://bi.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jk.huanxung.cn

[R36] 并发执行多个任务
来源：http://ef.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qn.shxzskj.cn

[R37] 把输出赋给变量
来源：http://ry.gzmigu.cn

files=$(ls -1)
来源：http://kc.hahajie.cn

[R38] 管道串联
来源：http://fw.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://fb.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://pg.bjjhwx.cn

cmd > out.log 2>&1
来源：http://bo.lnxyls.cn

[R40] 追加写日志
来源：http://fl.yuexingan06.cn

echo "log" >> out.log
来源：http://sc.chemitech.net.cn

[R41] 丢弃输出
来源：http://jk.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://vy.szsharing.cn

[R42] 输入重定向
来源：http://vl.bjjhwx.cn

wc -l < a.txt
来源：http://wm.haigaiapp.cn

[R43] 按名字查找文件
来源：http://gg.muxihuayi.cn

find . -name "*.log" -type f
来源：http://vc.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://bv.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://pp.jctech888.com.cn

[R45] 批量删除
来源：http://vy.nszjky.cn

find . -name "*.tmp" -delete
来源：http://ho.szxytkj.cn

[R46] 递归替换文件内容
来源：http://cb.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gc.lnxyls.cn

[R47] sed 单行替换
来源：http://tl.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jt.huixiangedu.cn

[R48] awk 取指定列
来源：http://yv.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://ts.yuntaijiaju.cn

[R49] awk 带条件
来源：http://nf.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gc.hnjuh.cn

[R50] awk 求和
来源：http://th.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hh.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://ek.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ps.panjiajie.cn

[R52] 统计行数
来源：http://ly.szxytkj.cn

wc -l a.txt
来源：http://pe.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://xd.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oz.wgjwhj.cn

[R54] 比较两个文件
来源：http://mf.shxzukj.cn

diff a.txt b.txt
来源：http://ue.jctech888.com.cn

[R55] 压缩与解压
来源：http://vz.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nc.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://fd.huixiangedu.cn

scp file user@host:/path/
来源：http://zm.lnxyls.cn

[R57] 远程执行命令
来源：http://zn.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://gy.huanxung.cn

[R58] 下载文件
来源：http://zt.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://az.nicolike.cn

[R59] 发 POST JSON
来源：http://hu.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eq.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://dr.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ge.chemitech.net.cn

[R61] 磁盘占用
来源：http://pn.huanxung.cn

df -h;  du -sh *
来源：http://ze.huanxung.cn

[R62] 找最占空间的文件
来源：http://rb.colortex.cn

du -ah . | sort -rh | head -10
来源：http://tw.panjiajie.cn

[R63] 内存与进程
来源：http://no.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://kk.szsharing.cn

[R64] 结束进程
来源：http://ql.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://or.szxytkj.cn

[R65] 查看端口占用
来源：http://zw.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.huixinmuqiang.cn

[R66] 定时任务
来源：http://rf.szxytkj.cn

crontab -e;  crontab -l
来源：http://zv.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://xh.shxzskj.cn

openssl rand -hex 16
来源：http://xq.nszjky.cn

[R68] 计算文件校验值
来源：http://hn.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yd.bjjhwx.cn

[R69] 生成随机密码
来源：http://dd.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://ok.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://eb.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://ox.bjjhwx.cn

[R71] 日期格式化
来源：http://ff.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gq.szsharing.cn

[R72] 等待端口就绪
来源：http://ff.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ej.chemitech.net.cn

[R73] 分割大日志
来源：http://ur.nszjky.cn

split -l 1000 big.log part_
来源：http://jf.nicolike.cn

[R74] 批量重命名
来源：http://mp.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ct.bookmarksfly.cn

[R75] 导出环境变量
来源：http://eh.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://fq.panjiajie.cn

[R76] 使用临时文件
来源：http://qj.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gp.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://bi.szxytkj.cn

read -rp "请输入: " ans
来源：http://rq.panjiajie.cn

[R78] 交互式菜单
来源：http://pl.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pt.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://lf.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sk.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://pr.chemitech.net.cn

time ./run.sh
来源：http://oh.bjjhwx.cn

================================================================================
来源：http://pb.521024.cn

S. C / C++ 专题
来源：http://so.shtwfgs.cn

================================================================================
来源：http://ps.nicolike.cn

[S01] C：Hello World
来源：http://gx.jctech888.com.cn

#include <stdio.h>
来源：http://za.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ql.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://tw.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://ri.szsharing.cn

[S03] C：读入整数
来源：http://eg.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://sv.haigaiapp.cn

[S04] C：字符串复制
来源：http://xi.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wm.muxihuayi.cn

[S05] C：字符串长度
来源：http://xa.gzmigu.cn

strlen(s)
来源：http://zu.lnxyls.cn

[S06] C：字符串比较
来源：http://ta.gzmigu.cn

strcmp(a, b) == 0
来源：http://js.gzmigu.cn

[S07] C：数组遍历求和
来源：http://jd.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ve.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://ps.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://td.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://mr.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qr.521024.cn

[S10] C：指针与解引用
来源：http://wo.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://vh.yuexingan06.cn

[S11] C：逐行读文件
来源：http://zd.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://nk.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tp.jianghongdianzi.cn

fclose(f);
来源：http://tp.521024.cn

[S12] C：写文件
来源：http://zh.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ay.panjiajie.cn

[S13] C：宏定义
来源：http://tc.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jt.szxytkj.cn

[S14] C：枚举
来源：http://cn.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://dx.wgjwhj.cn

[S15] C：类型转换
来源：http://bv.yuexingan06.cn

(double) a / b
来源：http://mm.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://jq.muxihuayi.cn

x |= (1 << 3);
来源：http://me.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://ga.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nd.huanxung.cn

[S18] C：命令行参数
来源：http://ve.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://wq.shxzskj.cn

[S19] C：快速排序
来源：http://fi.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qk.lnxyls.cn

[S20] C：二分查找
来源：http://du.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jk.colortex.cn

[S21] C：字符类别判断
来源：http://xy.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wp.hnjuh.cn

[S22] C：字符串转数字
来源：http://kw.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bs.yuexingan06.cn

[S23] C：随机数
来源：http://ts.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iv.521024.cn

[S24] C：获取本地时间
来源：http://fx.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vs.yuexingan06.cn

[S25] C：内存拷贝
来源：http://cs.shxzskj.cn

memcpy(dst, src, n);
来源：http://uv.nszjky.cn

[S26] C：内存清零
来源：http://qf.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://sw.jianghongdianzi.cn

[S27] C：定义常量
来源：http://og.yuexingan06.cn

const double PI = 3.14159;
来源：http://zx.9csxet.cn

[S28] C：静态变量
来源：http://cu.haigaiapp.cn

static int counter = 0;
来源：http://kt.shxzskj.cn

[S29] C：变参函数
来源：http://di.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wh.asd995.cn

[S30] C：头文件保护
来源：http://ct.chemitech.net.cn

#ifndef X_H
来源：http://ks.yuexingan06.cn

#define X_H
来源：http://wm.asd995.cn

#endif
来源：http://cw.huixiangedu.cn

[S31] C++：Hello World
来源：http://fm.chemitech.net.cn

#include <iostream>
来源：http://bu.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://wz.shxzskj.cn

[S32] C++：字符串
来源：http://mg.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://uh.yuexingan06.cn

[S33] C++：vector 增删
来源：http://is.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wr.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://my.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://nw.chemitech.net.cn

[S35] C++：map
来源：http://zd.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jctech888.com.cn

[S36] C++：unordered_map
来源：http://ln.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zx.muxihuayi.cn

[S37] C++：set
来源：http://ao.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ms.nszjky.cn

[S38] C++：排序
来源：http://vr.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://is.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://za.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kv.colortex.cn

[S40] C++：查找元素
来源：http://kx.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zj.szxytkj.cn

[S41] C++：类与构造函数
来源：http://ef.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xo.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://ag.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://gn.yuexingan06.cn

[S43] C++：智能指针
来源：http://tt.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://rp.asd995.cn

[S44] C++：引用传参
来源：http://et.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://ep.nicolike.cn

[S45] C++：lambda
来源：http://tx.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://os.lnxyls.cn

[S46] C++：函数模板
来源：http://fj.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fm.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://lq.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yu.lnxyls.cn

[S48] C++：逐行读文件
来源：http://iz.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ze.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://gk.nicolike.cn

[S49] C++：写文件
来源：http://sp.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ke.panjiajie.cn

[S50] C++：格式化数字
来源：http://yq.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ip.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://tl.huixiangedu.cn

static_cast<double>(a) / b
来源：http://qb.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://rc.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://hq.jctech888.com.cn

[S53] C++：移动语义
来源：http://fu.colortex.cn

std::vector<int> w = std::move(v);
来源：http://lk.panjiajie.cn

[S54] C++：异常处理
来源：http://fc.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nt.newstarts.cn

[S55] C++：结构化绑定
来源：http://gu.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gf.muxihuayi.cn

[S56] C++：optional
来源：http://ey.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iq.nicolike.cn

[S57] C++：编译期常量
来源：http://sl.yuntaijiaju.cn

constexpr int N = 10;
来源：http://qt.huixiangedu.cn

[S58] C++：命名空间
来源：http://zu.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://qc.hahajie.cn

[S59] C++：静态断言
来源：http://wc.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://do.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://xo.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yt.shxzukj.cn

================================================================================
来源：http://sl.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dl.yuexingan06.cn

================================================================================
来源：http://qu.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://ey.huixiangedu.cn

println("Hello")
来源：http://cs.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://ej.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vb.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://ts.yuexingan06.cn

"值: $b"
来源：http://dd.hahajie.cn

[T04] Kotlin：空安全
来源：http://ok.shxzukj.cn

val n: String? = null;  n?.length
来源：http://we.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://xa.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gt.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://vj.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yh.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://ot.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qq.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://ko.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://bm.asd995.cn

[T09] Kotlin：扩展函数
来源：http://hh.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://gp.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://ha.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uf.asd995.cn

[T11] Kotlin：协程
来源：http://ny.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yp.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://wj.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://uu.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://yb.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://is.huixiangedu.cn

[T14] Kotlin：循环
来源：http://dy.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://au.newstarts.cn

[T15] Kotlin：接口
来源：http://cj.nicolike.cn

interface Shape { fun area(): Double }
来源：http://gl.panjiajie.cn

[T16] Swift：Hello World
来源：http://od.haigaiapp.cn

print("Hello")
来源：http://wy.shxzskj.cn


<!-- 参考信息 -->