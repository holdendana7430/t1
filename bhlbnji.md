代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://yg.shtwfgs.cn

[R14] C 风格 for
来源：http://mg.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ew.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://hk.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lo.hahajie.cn

[R16] until 等待条件
来源：http://ko.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ma.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://tu.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zi.nszjky.cn

[R18] 遍历数组
来源：http://fb.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kg.chemitech.net.cn

[R19] 数组长度
来源：http://rq.chemitech.net.cn

echo "${#arr[@]}"
来源：http://wc.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://br.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kq.nszjky.cn

[R21] 字符串长度
来源：http://zl.hahajie.cn

echo "${#s}"
来源：http://cz.huixiangedu.cn

[R22] 截取子串
来源：http://gb.hahajie.cn

echo "${s:0:5}"
来源：http://ys.521024.cn

[R23] 字符串替换
来源：http://kk.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mm.huixinmuqiang.cn

[R24] 大小写转换
来源：http://tx.colortex.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kz.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://iw.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qe.huixinmuqiang.cn

[R26] 命令替换
来源：http://eu.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://wx.nszjky.cn

[R27] 算术展开
来源：http://aq.szsharing.cn

echo $((1 + 2 * 3))
来源：http://to.shxzukj.cn

[R28] 浮点运算
来源：http://zd.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://rh.hnjuh.cn

[R29] 定义函数
来源：http://oj.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zk.nicolike.cn

[R30] 函数返回状态码
来源：http://dl.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://am.wgjwhj.cn

[R31] 局部变量
来源：http://jq.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://dp.bookmarksfly.cn

[R32] 参数个数校验
来源：http://cm.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pb.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://jo.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dr.jianghongdianzi.cn

[R34] 退出时清理
来源：http://yy.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://if.shxzskj.cn

[R35] 后台执行并等待
来源：http://vy.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ho.lnxyls.cn

[R36] 并发执行多个任务
来源：http://sn.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cc.521024.cn

[R37] 把输出赋给变量
来源：http://tb.521024.cn

files=$(ls -1)
来源：http://be.shtwfgs.cn

[R38] 管道串联
来源：http://jd.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://bj.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://el.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://os.9csxet.cn

[R40] 追加写日志
来源：http://mb.yuntaijiaju.cn

echo "log" >> out.log
来源：http://zw.521024.cn

[R41] 丢弃输出
来源：http://mj.nicolike.cn

cmd >/dev/null 2>&1
来源：http://hu.jianghongdianzi.cn

[R42] 输入重定向
来源：http://ok.wgjwhj.cn

wc -l < a.txt
来源：http://wd.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://vk.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://ny.shxzukj.cn

[R44] 按修改时间查找
来源：http://da.yuexingan06.cn

find . -mtime -7 -type f
来源：http://vt.colortex.cn

[R45] 批量删除
来源：http://kn.asd995.cn

find . -name "*.tmp" -delete
来源：http://ba.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://az.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xl.haigaiapp.cn

[R47] sed 单行替换
来源：http://gf.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xc.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://qj.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://px.huixinmuqiang.cn

[R49] awk 带条件
来源：http://wa.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gv.shtwfgs.cn

[R50] awk 求和
来源：http://az.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bn.szsharing.cn

[R51] 排序去重取前几
来源：http://an.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bv.muxihuayi.cn

[R52] 统计行数
来源：http://tc.yuexingan06.cn

wc -l a.txt
来源：http://ld.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://eg.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wm.colortex.cn

[R54] 比较两个文件
来源：http://vb.yuntaijiaju.cn

diff a.txt b.txt
来源：http://wa.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://wk.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://us.panjiajie.cn

[R56] 远程拷贝
来源：http://is.hahajie.cn

scp file user@host:/path/
来源：http://qt.hnjuh.cn

[R57] 远程执行命令
来源：http://uh.muxihuayi.cn

ssh user@host 'uptime'
来源：http://mb.asd995.cn

[R58] 下载文件
来源：http://re.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rs.9csxet.cn

[R59] 发 POST JSON
来源：http://td.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yv.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://jr.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jz.muxihuayi.cn

[R61] 磁盘占用
来源：http://zj.9csxet.cn

df -h;  du -sh *
来源：http://sv.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://ye.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://ti.yuexingan06.cn

[R63] 内存与进程
来源：http://zv.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://ug.chemitech.net.cn

[R64] 结束进程
来源：http://an.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://fo.shxzskj.cn

[R65] 查看端口占用
来源：http://pj.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ju.9csxet.cn

[R66] 定时任务
来源：http://ey.colortex.cn

crontab -e;  crontab -l
来源：http://ty.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://od.yuntaijiaju.cn

openssl rand -hex 16
来源：http://cc.wgjwhj.cn

[R68] 计算文件校验值
来源：http://gi.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mr.panjiajie.cn

[R69] 生成随机密码
来源：http://pk.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://im.nicolike.cn

[R70] 时间戳与互转
来源：http://gk.521024.cn

date +%s;  date -d @1700000000
来源：http://jd.lnxyls.cn

[R71] 日期格式化
来源：http://wc.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qy.lnxyls.cn

[R72] 等待端口就绪
来源：http://yr.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://el.colortex.cn

[R73] 分割大日志
来源：http://zi.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://ng.bookmarksfly.cn

[R74] 批量重命名
来源：http://jd.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bz.colortex.cn

[R75] 导出环境变量
来源：http://lo.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://zn.gzmigu.cn

[R76] 使用临时文件
来源：http://hs.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ra.szxytkj.cn

[R77] 读取用户输入
来源：http://un.panjiajie.cn

read -rp "请输入: " ans
来源：http://ph.shxzskj.cn

[R78] 交互式菜单
来源：http://lt.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cl.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://mr.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bx.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://hv.panjiajie.cn

time ./run.sh
来源：http://gj.muxihuayi.cn

================================================================================
来源：http://vr.jctech888.com.cn

S. C / C++ 专题
来源：http://ii.muxihuayi.cn

================================================================================
来源：http://cn.haigaiapp.cn

[S01] C：Hello World
来源：http://lq.9csxet.cn

#include <stdio.h>
来源：http://rf.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pe.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://fr.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://zf.521024.cn

[S03] C：读入整数
来源：http://lr.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://rq.lnxyls.cn

[S04] C：字符串复制
来源：http://cr.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nq.nszjky.cn

[S05] C：字符串长度
来源：http://gj.haigaiapp.cn

strlen(s)
来源：http://zj.asd995.cn

[S06] C：字符串比较
来源：http://je.muxihuayi.cn

strcmp(a, b) == 0
来源：http://yl.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://xe.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nn.asd995.cn

[S08] C：动态内存分配与释放
来源：http://my.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rf.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://rv.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oz.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://zs.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://wo.newstarts.cn

[S11] C：逐行读文件
来源：http://ps.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://ew.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lj.huanxung.cn

fclose(f);
来源：http://ng.gzmigu.cn

[S12] C：写文件
来源：http://ba.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tx.shxzskj.cn

[S13] C：宏定义
来源：http://el.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fj.huixiangedu.cn

[S14] C：枚举
来源：http://qd.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://bb.jctech888.com.cn

[S15] C：类型转换
来源：http://vz.bjjhwx.cn

(double) a / b
来源：http://cl.shxzskj.cn

[S16] C：位操作置位
来源：http://dh.bookmarksfly.cn

x |= (1 << 3);
来源：http://qd.colortex.cn

[S17] C：安全拼接字符串
来源：http://gb.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dp.9csxet.cn

[S18] C：命令行参数
来源：http://oi.chemitech.net.cn

int main(int argc, char **argv)
来源：http://ez.521024.cn

[S19] C：快速排序
来源：http://mh.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hw.asd995.cn

[S20] C：二分查找
来源：http://qc.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aw.szsharing.cn

[S21] C：字符类别判断
来源：http://ax.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hp.lnxyls.cn

[S22] C：字符串转数字
来源：http://ed.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pp.panjiajie.cn

[S23] C：随机数
来源：http://vo.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tn.yuexingan06.cn

[S24] C：获取本地时间
来源：http://jl.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kg.huanxung.cn

[S25] C：内存拷贝
来源：http://eg.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://mu.nszjky.cn

[S26] C：内存清零
来源：http://kd.szsharing.cn

memset(a, 0, sizeof a);
来源：http://gi.jianghongdianzi.cn

[S27] C：定义常量
来源：http://hz.bookmarksfly.cn

const double PI = 3.14159;
来源：http://kc.bjjhwx.cn

[S28] C：静态变量
来源：http://vx.jianghongdianzi.cn

static int counter = 0;
来源：http://es.colortex.cn

[S29] C：变参函数
来源：http://df.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rs.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://um.bjjhwx.cn

#ifndef X_H
来源：http://zl.szsharing.cn

#define X_H
来源：http://vg.nicolike.cn

#endif
来源：http://vy.wgjwhj.cn

[S31] C++：Hello World
来源：http://mf.lnxyls.cn

#include <iostream>
来源：http://al.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://va.shxzskj.cn

[S32] C++：字符串
来源：http://zz.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://sv.muxihuayi.cn

[S33] C++：vector 增删
来源：http://bk.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xd.nicolike.cn

[S34] C++：遍历 vector
来源：http://ri.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://zh.muxihuayi.cn

[S35] C++：map
来源：http://zl.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ez.hnjuh.cn

[S36] C++：unordered_map
来源：http://xf.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dz.asd995.cn

[S37] C++：set
来源：http://fh.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qf.shxzskj.cn

[S38] C++：排序
来源：http://cl.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://ey.asd995.cn

[S39] C++：自定义比较器排序
来源：http://wn.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://du.521024.cn

[S40] C++：查找元素
来源：http://fj.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zm.shxzukj.cn

[S41] C++：类与构造函数
来源：http://hf.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lf.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://ll.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://sp.panjiajie.cn

[S43] C++：智能指针
来源：http://zj.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://cx.shxzukj.cn

[S44] C++：引用传参
来源：http://qj.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://uo.shtwfgs.cn

[S45] C++：lambda
来源：http://br.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kf.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://ji.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gq.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://tn.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fp.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://dq.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xz.hahajie.cn

while (std::getline(in, line)) { }
来源：http://gl.hahajie.cn

[S49] C++：写文件
来源：http://nr.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pt.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://ee.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wl.szxytkj.cn

[S51] C++：显式类型转换
来源：http://hp.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://pr.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://qt.huanxung.cn

int size() const noexcept { return n_; }
来源：http://cv.shxzskj.cn

[S53] C++：移动语义
来源：http://gm.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://pu.colortex.cn

[S54] C++：异常处理
来源：http://ac.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sk.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://ad.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ys.yuexingan06.cn

[S56] C++：optional
来源：http://fq.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qr.nicolike.cn

[S57] C++：编译期常量
来源：http://yk.huixinmuqiang.cn

constexpr int N = 10;
来源：http://km.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://gf.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://dx.huixiangedu.cn

[S59] C++：静态断言
来源：http://pm.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ez.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://id.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uo.9csxet.cn

================================================================================
来源：http://sg.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jv.bjjhwx.cn

================================================================================
来源：http://ka.nszjky.cn

[T01] Kotlin：Hello World
来源：http://lo.huixinmuqiang.cn

println("Hello")
来源：http://zu.yuexingan06.cn

[T02] Kotlin：变量
来源：http://jo.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yo.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://es.colortex.cn

"值: $b"
来源：http://uk.szxytkj.cn

[T04] Kotlin：空安全
来源：http://mi.gzmigu.cn

val n: String? = null;  n?.length
来源：http://aa.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://xy.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ae.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://cg.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wn.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://ac.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rx.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://wh.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://sr.asd995.cn

[T09] Kotlin：扩展函数
来源：http://ld.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://xw.nszjky.cn

[T10] Kotlin：默认参数
来源：http://uq.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cq.jctech888.com.cn

[T11] Kotlin：协程
来源：http://pm.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qf.9csxet.cn

[T12] Kotlin：解构声明
来源：http://fc.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://pv.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://vg.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://eh.haigaiapp.cn

[T14] Kotlin：循环
来源：http://tb.panjiajie.cn

for (i in 1..10) println(i)
来源：http://cy.shxzskj.cn

[T15] Kotlin：接口
来源：http://bf.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://gx.shxzukj.cn

[T16] Swift：Hello World
来源：http://va.chemitech.net.cn

print("Hello")
来源：http://xx.shtwfgs.cn


<!-- 参考信息 -->