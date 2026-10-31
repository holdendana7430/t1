代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://at.jianghongdianzi.cn

[R08] 数值比较
来源：http://bj.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://di.hnjuh.cn

[R09] 字符串比较
来源：http://os.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://re.huixiangedu.cn

[R10] 正则匹配
来源：http://vu.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qn.gzmigu.cn

[R11] case 多分支
来源：http://pp.9csxet.cn

case "$1" in
来源：http://gj.wgjwhj.cn

start) echo "启动" ;;
来源：http://dy.nszjky.cn

stop)  echo "停止" ;;
来源：http://gy.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://fx.haigaiapp.cn

esac
来源：http://qa.szxytkj.cn

[R12] for 遍历文件
来源：http://rq.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://ht.colortex.cn

[R13] for 计数循环
来源：http://fb.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://hz.chemitech.net.cn

[R14] C 风格 for
来源：http://sc.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gv.colortex.cn

[R15] while 逐行读文件
来源：http://ko.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qg.newstarts.cn

[R16] until 等待条件
来源：http://ih.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pa.shxzukj.cn

[R17] 数组定义与取值
来源：http://gy.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oj.jctech888.com.cn

[R18] 遍历数组
来源：http://dg.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xr.hahajie.cn

[R19] 数组长度
来源：http://ew.bjjhwx.cn

echo "${#arr[@]}"
来源：http://kl.hnjuh.cn

[R20] 关联数组（字典）
来源：http://zl.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ee.hahajie.cn

[R21] 字符串长度
来源：http://cd.jianghongdianzi.cn

echo "${#s}"
来源：http://fv.shtwfgs.cn

[R22] 截取子串
来源：http://pe.haigaiapp.cn

echo "${s:0:5}"
来源：http://hn.bjjhwx.cn

[R23] 字符串替换
来源：http://ic.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ce.szsharing.cn

[R24] 大小写转换
来源：http://ls.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dd.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://al.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ou.shtwfgs.cn

[R26] 命令替换
来源：http://lg.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://mm.huanxung.cn

[R27] 算术展开
来源：http://kf.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://sf.hnjuh.cn

[R28] 浮点运算
来源：http://av.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://tv.hnjuh.cn

[R29] 定义函数
来源：http://jb.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uf.jctech888.com.cn

[R30] 函数返回状态码
来源：http://ex.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://ee.huanxung.cn

[R31] 局部变量
来源：http://kc.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://oe.muxihuayi.cn

[R32] 参数个数校验
来源：http://ut.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ed.colortex.cn

[R33] 捕获错误并提示行号
来源：http://hf.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mx.panjiajie.cn

[R34] 退出时清理
来源：http://zn.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ae.nicolike.cn

[R35] 后台执行并等待
来源：http://ew.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wc.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://aj.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vd.shxzukj.cn

[R37] 把输出赋给变量
来源：http://nb.bjjhwx.cn

files=$(ls -1)
来源：http://ss.huixiangedu.cn

[R38] 管道串联
来源：http://xs.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://uz.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://jm.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://lu.huixiangedu.cn

[R40] 追加写日志
来源：http://ig.huanxung.cn

echo "log" >> out.log
来源：http://ar.nicolike.cn

[R41] 丢弃输出
来源：http://lc.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://ld.hahajie.cn

[R42] 输入重定向
来源：http://pd.szsharing.cn

wc -l < a.txt
来源：http://sd.hnjuh.cn

[R43] 按名字查找文件
来源：http://tc.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://zm.shxzskj.cn

[R44] 按修改时间查找
来源：http://fc.colortex.cn

find . -mtime -7 -type f
来源：http://px.hahajie.cn

[R45] 批量删除
来源：http://fy.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://ae.hnjuh.cn

[R46] 递归替换文件内容
来源：http://rd.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yf.wgjwhj.cn

[R47] sed 单行替换
来源：http://jr.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kf.colortex.cn

[R48] awk 取指定列
来源：http://qf.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://yv.muxihuayi.cn

[R49] awk 带条件
来源：http://sh.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fk.shxzukj.cn

[R50] awk 求和
来源：http://ch.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://iy.nicolike.cn

[R51] 排序去重取前几
来源：http://xq.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wg.521024.cn

[R52] 统计行数
来源：http://dv.huixiangedu.cn

wc -l a.txt
来源：http://tp.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://eg.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zt.newstarts.cn

[R54] 比较两个文件
来源：http://mr.wgjwhj.cn

diff a.txt b.txt
来源：http://dz.asd995.cn

[R55] 压缩与解压
来源：http://st.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rs.panjiajie.cn

[R56] 远程拷贝
来源：http://ka.asd995.cn

scp file user@host:/path/
来源：http://ga.bookmarksfly.cn

[R57] 远程执行命令
来源：http://ff.nicolike.cn

ssh user@host 'uptime'
来源：http://su.shxzskj.cn

[R58] 下载文件
来源：http://nl.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ko.szsharing.cn

[R59] 发 POST JSON
来源：http://lj.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://az.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://gl.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tc.521024.cn

[R61] 磁盘占用
来源：http://eq.wgjwhj.cn

df -h;  du -sh *
来源：http://lg.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://nw.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://gj.nszjky.cn

[R63] 内存与进程
来源：http://vd.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://cz.nszjky.cn

[R64] 结束进程
来源：http://wo.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://fi.hnjuh.cn

[R65] 查看端口占用
来源：http://rt.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hk.shxzukj.cn

[R66] 定时任务
来源：http://fd.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://zt.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://fb.hahajie.cn

openssl rand -hex 16
来源：http://vv.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://gr.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://di.shxzskj.cn

[R69] 生成随机密码
来源：http://hr.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://pc.bjjhwx.cn

[R70] 时间戳与互转
来源：http://hz.9csxet.cn

date +%s;  date -d @1700000000
来源：http://jv.gzmigu.cn

[R71] 日期格式化
来源：http://qb.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ih.shxzukj.cn

[R72] 等待端口就绪
来源：http://lf.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jp.bjjhwx.cn

[R73] 分割大日志
来源：http://ht.szsharing.cn

split -l 1000 big.log part_
来源：http://mz.hahajie.cn

[R74] 批量重命名
来源：http://rx.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nr.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://ru.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://xu.shxzukj.cn

[R76] 使用临时文件
来源：http://dk.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sv.colortex.cn

[R77] 读取用户输入
来源：http://kk.huanxung.cn

read -rp "请输入: " ans
来源：http://lt.nicolike.cn

[R78] 交互式菜单
来源：http://ps.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eq.panjiajie.cn

[R79] 解析命令行选项
来源：http://ud.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cz.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://ye.gzmigu.cn

time ./run.sh
来源：http://gh.hahajie.cn

================================================================================
来源：http://va.shxzukj.cn

S. C / C++ 专题
来源：http://ox.9csxet.cn

================================================================================
来源：http://ra.panjiajie.cn

[S01] C：Hello World
来源：http://hj.newstarts.cn

#include <stdio.h>
来源：http://hc.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dz.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://ko.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://mp.9csxet.cn

[S03] C：读入整数
来源：http://bn.huanxung.cn

int x; scanf("%d", &x);
来源：http://id.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://rb.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ld.jctech888.com.cn

[S05] C：字符串长度
来源：http://op.9csxet.cn

strlen(s)
来源：http://qj.lnxyls.cn

[S06] C：字符串比较
来源：http://zt.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://cu.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://gc.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kg.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://bv.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://po.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://cq.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tb.521024.cn

[S10] C：指针与解引用
来源：http://uc.szsharing.cn

int *p = &a;  *p = 5;
来源：http://nm.bjjhwx.cn

[S11] C：逐行读文件
来源：http://ly.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://ho.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jn.shxzukj.cn

fclose(f);
来源：http://vz.gzmigu.cn

[S12] C：写文件
来源：http://is.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://da.nszjky.cn

[S13] C：宏定义
来源：http://qp.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aq.hahajie.cn

[S14] C：枚举
来源：http://zb.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://mw.nszjky.cn

[S15] C：类型转换
来源：http://sl.nszjky.cn

(double) a / b
来源：http://qc.panjiajie.cn

[S16] C：位操作置位
来源：http://pt.jianghongdianzi.cn

x |= (1 << 3);
来源：http://ee.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://vk.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://px.gzmigu.cn

[S18] C：命令行参数
来源：http://bj.shxzskj.cn

int main(int argc, char **argv)
来源：http://xf.lnxyls.cn

[S19] C：快速排序
来源：http://nx.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yr.bookmarksfly.cn

[S20] C：二分查找
来源：http://md.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uv.9csxet.cn

[S21] C：字符类别判断
来源：http://ci.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dx.shtwfgs.cn

[S22] C：字符串转数字
来源：http://up.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tc.nicolike.cn

[S23] C：随机数
来源：http://jl.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pl.wgjwhj.cn

[S24] C：获取本地时间
来源：http://vj.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://py.muxihuayi.cn

[S25] C：内存拷贝
来源：http://od.hnjuh.cn

memcpy(dst, src, n);
来源：http://jd.muxihuayi.cn

[S26] C：内存清零
来源：http://xz.colortex.cn

memset(a, 0, sizeof a);
来源：http://nl.nszjky.cn

[S27] C：定义常量
来源：http://dx.muxihuayi.cn

const double PI = 3.14159;
来源：http://pz.shxzukj.cn

[S28] C：静态变量
来源：http://pv.yuexingan06.cn

static int counter = 0;
来源：http://le.shxzskj.cn

[S29] C：变参函数
来源：http://ln.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mr.haigaiapp.cn

[S30] C：头文件保护
来源：http://bn.bookmarksfly.cn

#ifndef X_H
来源：http://fy.yuntaijiaju.cn

#define X_H
来源：http://ha.jctech888.com.cn

#endif
来源：http://qn.huanxung.cn

[S31] C++：Hello World
来源：http://pv.jianghongdianzi.cn

#include <iostream>
来源：http://wl.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://oj.szxytkj.cn

[S32] C++：字符串
来源：http://jl.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://vh.shtwfgs.cn

[S33] C++：vector 增删
来源：http://jd.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ne.asd995.cn

[S34] C++：遍历 vector
来源：http://jg.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://fj.szsharing.cn

[S35] C++：map
来源：http://ly.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gm.panjiajie.cn

[S36] C++：unordered_map
来源：http://ox.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mb.shtwfgs.cn

[S37] C++：set
来源：http://iv.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wh.huixiangedu.cn

[S38] C++：排序
来源：http://kf.asd995.cn

std::sort(v.begin(), v.end());
来源：http://gv.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://nq.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yd.wgjwhj.cn

[S40] C++：查找元素
来源：http://ia.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kk.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://uu.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://li.nszjky.cn

[S42] C++：继承与虚函数
来源：http://ft.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://fa.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://we.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://pk.huanxung.cn

[S44] C++：引用传参
来源：http://xz.nicolike.cn

void inc(int &x) { ++x; }
来源：http://vw.huixinmuqiang.cn

[S45] C++：lambda
来源：http://ez.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vd.521024.cn

[S46] C++：函数模板
来源：http://dz.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xq.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://dk.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://go.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://gp.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yw.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://hq.lnxyls.cn

[S49] C++：写文件
来源：http://gu.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ix.9csxet.cn

[S50] C++：格式化数字
来源：http://vr.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hl.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://vl.nszjky.cn

static_cast<double>(a) / b
来源：http://pe.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://ft.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://oe.colortex.cn

[S53] C++：移动语义
来源：http://wc.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://uv.muxihuayi.cn

[S54] C++：异常处理
来源：http://mr.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ql.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://ck.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ep.hnjuh.cn

[S56] C++：optional
来源：http://pq.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ro.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://mv.yuntaijiaju.cn

constexpr int N = 10;
来源：http://vr.bjjhwx.cn

[S58] C++：命名空间
来源：http://eg.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://nr.asd995.cn

[S59] C++：静态断言
来源：http://jv.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mh.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://ji.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wf.bookmarksfly.cn

================================================================================
来源：http://sw.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ei.shtwfgs.cn

================================================================================
来源：http://yv.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://fd.jctech888.com.cn

println("Hello")
来源：http://hc.newstarts.cn

[T02] Kotlin：变量
来源：http://kj.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lk.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://yq.lnxyls.cn

"值: $b"
来源：http://kg.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://bo.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://hx.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://bm.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ti.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://jt.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xu.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://jb.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jf.nszjky.cn

[T08] Kotlin：数据类
来源：http://du.521024.cn

data class User(val name: String, val age: Int)
来源：http://sw.jianghongdianzi.cn


<!-- 参考信息 -->