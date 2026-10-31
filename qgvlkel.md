代发 wailian999

esac
来源：http://pj.huanxung.cn

[R12] for 遍历文件
来源：http://xd.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://qs.colortex.cn

[R13] for 计数循环
来源：http://yu.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://fc.colortex.cn

[R14] C 风格 for
来源：http://et.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://st.hnjuh.cn

[R15] while 逐行读文件
来源：http://wg.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ft.huanxung.cn

[R16] until 等待条件
来源：http://rc.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hc.hahajie.cn

[R17] 数组定义与取值
来源：http://vm.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lo.521024.cn

[R18] 遍历数组
来源：http://na.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mt.newstarts.cn

[R19] 数组长度
来源：http://ma.shxzukj.cn

echo "${#arr[@]}"
来源：http://xd.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://rh.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rx.shxzukj.cn

[R21] 字符串长度
来源：http://xf.521024.cn

echo "${#s}"
来源：http://bo.jctech888.com.cn

[R22] 截取子串
来源：http://kf.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://ep.hahajie.cn

[R23] 字符串替换
来源：http://qv.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mu.nicolike.cn

[R24] 大小写转换
来源：http://li.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://oq.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://dz.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zs.yuntaijiaju.cn

[R26] 命令替换
来源：http://kg.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://ky.szxytkj.cn

[R27] 算术展开
来源：http://ff.asd995.cn

echo $((1 + 2 * 3))
来源：http://lh.haigaiapp.cn

[R28] 浮点运算
来源：http://ly.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://pf.szsharing.cn

[R29] 定义函数
来源：http://rx.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nd.asd995.cn

[R30] 函数返回状态码
来源：http://ee.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://bs.9csxet.cn

[R31] 局部变量
来源：http://hg.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://ky.hahajie.cn

[R32] 参数个数校验
来源：http://rl.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://va.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://tz.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iq.panjiajie.cn

[R34] 退出时清理
来源：http://uj.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fs.colortex.cn

[R35] 后台执行并等待
来源：http://lp.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gr.nszjky.cn

[R36] 并发执行多个任务
来源：http://ru.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uz.szsharing.cn

[R37] 把输出赋给变量
来源：http://ej.521024.cn

files=$(ls -1)
来源：http://ic.9csxet.cn

[R38] 管道串联
来源：http://ky.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://du.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://vq.gzmigu.cn

cmd > out.log 2>&1
来源：http://qh.shxzskj.cn

[R40] 追加写日志
来源：http://lg.panjiajie.cn

echo "log" >> out.log
来源：http://nh.9csxet.cn

[R41] 丢弃输出
来源：http://mt.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://fo.shtwfgs.cn

[R42] 输入重定向
来源：http://lw.wgjwhj.cn

wc -l < a.txt
来源：http://wc.shxzukj.cn

[R43] 按名字查找文件
来源：http://ru.szxytkj.cn

find . -name "*.log" -type f
来源：http://fh.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://uj.colortex.cn

find . -mtime -7 -type f
来源：http://xj.panjiajie.cn

[R45] 批量删除
来源：http://tc.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://og.gzmigu.cn

[R46] 递归替换文件内容
来源：http://gz.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ox.521024.cn

[R47] sed 单行替换
来源：http://vo.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ya.chemitech.net.cn

[R48] awk 取指定列
来源：http://ww.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://rq.asd995.cn

[R49] awk 带条件
来源：http://xq.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rn.colortex.cn

[R50] awk 求和
来源：http://vi.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yc.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://hx.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fd.bookmarksfly.cn

[R52] 统计行数
来源：http://jb.nicolike.cn

wc -l a.txt
来源：http://ql.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://uu.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jj.colortex.cn

[R54] 比较两个文件
来源：http://wr.szsharing.cn

diff a.txt b.txt
来源：http://lj.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://nl.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ir.hnjuh.cn

[R56] 远程拷贝
来源：http://aq.nszjky.cn

scp file user@host:/path/
来源：http://ep.yuexingan06.cn

[R57] 远程执行命令
来源：http://bp.huixiangedu.cn

ssh user@host 'uptime'
来源：http://ip.bjjhwx.cn

[R58] 下载文件
来源：http://hn.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pm.szsharing.cn

[R59] 发 POST JSON
来源：http://bf.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ye.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://dd.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mc.szsharing.cn

[R61] 磁盘占用
来源：http://aa.colortex.cn

df -h;  du -sh *
来源：http://yk.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://lj.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://se.chemitech.net.cn

[R63] 内存与进程
来源：http://pg.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://jt.9csxet.cn

[R64] 结束进程
来源：http://ox.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://ab.521024.cn

[R65] 查看端口占用
来源：http://nx.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pa.huixiangedu.cn

[R66] 定时任务
来源：http://iy.huixiangedu.cn

crontab -e;  crontab -l
来源：http://pi.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://rs.szsharing.cn

openssl rand -hex 16
来源：http://jf.gzmigu.cn

[R68] 计算文件校验值
来源：http://rn.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ir.szsharing.cn

[R69] 生成随机密码
来源：http://kn.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://fk.panjiajie.cn

[R70] 时间戳与互转
来源：http://qn.nszjky.cn

date +%s;  date -d @1700000000
来源：http://mi.hnjuh.cn

[R71] 日期格式化
来源：http://um.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nl.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://um.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dt.chemitech.net.cn

[R73] 分割大日志
来源：http://sj.colortex.cn

split -l 1000 big.log part_
来源：http://ox.521024.cn

[R74] 批量重命名
来源：http://ly.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nh.nszjky.cn

[R75] 导出环境变量
来源：http://gf.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://hd.bjjhwx.cn

[R76] 使用临时文件
来源：http://af.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cu.huixiangedu.cn

[R77] 读取用户输入
来源：http://wj.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://od.shxzukj.cn

[R78] 交互式菜单
来源：http://wr.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uf.haigaiapp.cn

[R79] 解析命令行选项
来源：http://fy.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lo.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://ef.hahajie.cn

time ./run.sh
来源：http://ve.colortex.cn

================================================================================
来源：http://rn.jianghongdianzi.cn

S. C / C++ 专题
来源：http://kd.asd995.cn

================================================================================
来源：http://ez.huixiangedu.cn

[S01] C：Hello World
来源：http://xw.huixiangedu.cn

#include <stdio.h>
来源：http://qw.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cq.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://hg.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://vr.nicolike.cn

[S03] C：读入整数
来源：http://nx.panjiajie.cn

int x; scanf("%d", &x);
来源：http://au.bookmarksfly.cn

[S04] C：字符串复制
来源：http://yw.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://no.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://in.jctech888.com.cn

strlen(s)
来源：http://am.szsharing.cn

[S06] C：字符串比较
来源：http://io.chemitech.net.cn

strcmp(a, b) == 0
来源：http://aa.hnjuh.cn

[S07] C：数组遍历求和
来源：http://po.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://in.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://ak.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xx.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://ny.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lp.shxzukj.cn

[S10] C：指针与解引用
来源：http://yg.nszjky.cn

int *p = &a;  *p = 5;
来源：http://sg.hnjuh.cn

[S11] C：逐行读文件
来源：http://om.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://rl.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://au.asd995.cn

fclose(f);
来源：http://hm.hnjuh.cn

[S12] C：写文件
来源：http://dh.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dl.newstarts.cn

[S13] C：宏定义
来源：http://fq.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rr.yuntaijiaju.cn

[S14] C：枚举
来源：http://om.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://kj.jctech888.com.cn

[S15] C：类型转换
来源：http://ps.wgjwhj.cn

(double) a / b
来源：http://yg.wgjwhj.cn

[S16] C：位操作置位
来源：http://ds.shxzskj.cn

x |= (1 << 3);
来源：http://jh.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://un.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tt.wgjwhj.cn

[S18] C：命令行参数
来源：http://oh.hahajie.cn

int main(int argc, char **argv)
来源：http://qo.jctech888.com.cn

[S19] C：快速排序
来源：http://dr.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dz.yuntaijiaju.cn

[S20] C：二分查找
来源：http://ac.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bp.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://nl.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qq.521024.cn

[S22] C：字符串转数字
来源：http://ni.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oy.panjiajie.cn

[S23] C：随机数
来源：http://tp.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lo.wgjwhj.cn

[S24] C：获取本地时间
来源：http://fy.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://he.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://cu.muxihuayi.cn

memcpy(dst, src, n);
来源：http://cv.nszjky.cn

[S26] C：内存清零
来源：http://lw.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://kb.jianghongdianzi.cn

[S27] C：定义常量
来源：http://zj.shtwfgs.cn

const double PI = 3.14159;
来源：http://is.huanxung.cn

[S28] C：静态变量
来源：http://vf.9csxet.cn

static int counter = 0;
来源：http://qb.haigaiapp.cn

[S29] C：变参函数
来源：http://dk.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yl.colortex.cn

[S30] C：头文件保护
来源：http://xa.lnxyls.cn

#ifndef X_H
来源：http://ic.haigaiapp.cn

#define X_H
来源：http://xu.haigaiapp.cn

#endif
来源：http://il.panjiajie.cn

[S31] C++：Hello World
来源：http://oq.shxzukj.cn

#include <iostream>
来源：http://lk.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://kj.shxzukj.cn

[S32] C++：字符串
来源：http://jn.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://sh.huixiangedu.cn

[S33] C++：vector 增删
来源：http://kb.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wq.asd995.cn

[S34] C++：遍历 vector
来源：http://hi.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://rb.muxihuayi.cn

[S35] C++：map
来源：http://hu.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sq.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://dq.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jr.panjiajie.cn

[S37] C++：set
来源：http://ea.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fr.yuexingan06.cn

[S38] C++：排序
来源：http://ff.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://fr.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://tv.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xd.wgjwhj.cn

[S40] C++：查找元素
来源：http://vb.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wm.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://vw.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sf.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://an.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://vi.lnxyls.cn

[S43] C++：智能指针
来源：http://eq.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://nm.bjjhwx.cn

[S44] C++：引用传参
来源：http://ni.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://bc.shxzskj.cn

[S45] C++：lambda
来源：http://xd.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ur.hahajie.cn

[S46] C++：函数模板
来源：http://xx.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ja.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://ax.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zq.9csxet.cn

[S48] C++：逐行读文件
来源：http://fg.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vx.huanxung.cn

while (std::getline(in, line)) { }
来源：http://hp.bookmarksfly.cn

[S49] C++：写文件
来源：http://mr.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://at.hnjuh.cn

[S50] C++：格式化数字
来源：http://oi.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nh.newstarts.cn

[S51] C++：显式类型转换
来源：http://zq.asd995.cn

static_cast<double>(a) / b
来源：http://lv.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://xp.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://un.haigaiapp.cn

[S53] C++：移动语义
来源：http://rx.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://ro.muxihuayi.cn

[S54] C++：异常处理
来源：http://cz.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gt.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://tc.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wy.521024.cn

[S56] C++：optional
来源：http://rf.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sd.shxzukj.cn

[S57] C++：编译期常量
来源：http://sx.shxzukj.cn

constexpr int N = 10;
来源：http://ub.bookmarksfly.cn

[S58] C++：命名空间
来源：http://pa.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://tl.muxihuayi.cn

[S59] C++：静态断言
来源：http://rm.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ja.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://cm.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lj.521024.cn

================================================================================
来源：http://ep.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://im.lnxyls.cn

================================================================================
来源：http://mt.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://xb.nszjky.cn

println("Hello")
来源：http://dl.szxytkj.cn

[T02] Kotlin：变量
来源：http://nj.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yl.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://nz.gzmigu.cn

"值: $b"
来源：http://ss.colortex.cn

[T04] Kotlin：空安全
来源：http://ny.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://we.521024.cn

[T05] Kotlin：when 表达式
来源：http://ts.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zb.nicolike.cn

[T06] Kotlin：集合映射
来源：http://db.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jn.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://xb.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cn.nicolike.cn

[T08] Kotlin：数据类
来源：http://hi.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://hh.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://bk.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://jg.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://qj.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xa.shxzskj.cn

[T11] Kotlin：协程
来源：http://tu.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gz.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://uh.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://mw.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://yr.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://zf.nicolike.cn

[T14] Kotlin：循环
来源：http://so.nicolike.cn

for (i in 1..10) println(i)
来源：http://qo.jctech888.com.cn


<!-- 参考信息 -->