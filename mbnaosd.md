代发 wailian999

esac
来源：http://fu.colortex.cn

[R12] for 遍历文件
来源：http://sh.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://tk.asd995.cn

[R13] for 计数循环
来源：http://xy.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://na.chemitech.net.cn

[R14] C 风格 for
来源：http://cj.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zo.bjjhwx.cn

[R15] while 逐行读文件
来源：http://fl.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ex.yuntaijiaju.cn

[R16] until 等待条件
来源：http://rk.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cz.wgjwhj.cn

[R17] 数组定义与取值
来源：http://fx.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qf.lnxyls.cn

[R18] 遍历数组
来源：http://fo.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wd.bjjhwx.cn

[R19] 数组长度
来源：http://nu.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://gs.lnxyls.cn

[R20] 关联数组（字典）
来源：http://sy.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qq.chemitech.net.cn

[R21] 字符串长度
来源：http://cg.panjiajie.cn

echo "${#s}"
来源：http://mh.muxihuayi.cn

[R22] 截取子串
来源：http://mr.newstarts.cn

echo "${s:0:5}"
来源：http://si.jianghongdianzi.cn

[R23] 字符串替换
来源：http://qu.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xp.shxzukj.cn

[R24] 大小写转换
来源：http://ot.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jz.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://te.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dx.hnjuh.cn

[R26] 命令替换
来源：http://ov.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://fs.haigaiapp.cn

[R27] 算术展开
来源：http://pp.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://lr.hnjuh.cn

[R28] 浮点运算
来源：http://oy.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://tf.nicolike.cn

[R29] 定义函数
来源：http://tq.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dc.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://hd.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://hv.bjjhwx.cn

[R31] 局部变量
来源：http://vz.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://dt.asd995.cn

[R32] 参数个数校验
来源：http://pf.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oz.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://yd.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sl.jctech888.com.cn

[R34] 退出时清理
来源：http://jc.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hb.521024.cn

[R35] 后台执行并等待
来源：http://jl.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tr.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://pa.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ta.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://gs.yuexingan06.cn

files=$(ls -1)
来源：http://gg.nszjky.cn

[R38] 管道串联
来源：http://hn.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://gk.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://ez.shxzskj.cn

cmd > out.log 2>&1
来源：http://kt.nszjky.cn

[R40] 追加写日志
来源：http://tb.asd995.cn

echo "log" >> out.log
来源：http://ab.yuexingan06.cn

[R41] 丢弃输出
来源：http://eb.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://ks.bjjhwx.cn

[R42] 输入重定向
来源：http://jj.chemitech.net.cn

wc -l < a.txt
来源：http://ib.shxzukj.cn

[R43] 按名字查找文件
来源：http://zj.asd995.cn

find . -name "*.log" -type f
来源：http://xm.bjjhwx.cn

[R44] 按修改时间查找
来源：http://ih.yuexingan06.cn

find . -mtime -7 -type f
来源：http://ca.panjiajie.cn

[R45] 批量删除
来源：http://lj.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://rq.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://id.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ie.bookmarksfly.cn

[R47] sed 单行替换
来源：http://ek.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hw.muxihuayi.cn

[R48] awk 取指定列
来源：http://dt.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://mj.shtwfgs.cn

[R49] awk 带条件
来源：http://oe.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jx.huanxung.cn

[R50] awk 求和
来源：http://fz.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nr.shxzukj.cn

[R51] 排序去重取前几
来源：http://jz.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kr.huixinmuqiang.cn

[R52] 统计行数
来源：http://wd.yuntaijiaju.cn

wc -l a.txt
来源：http://cc.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://vz.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cg.lnxyls.cn

[R54] 比较两个文件
来源：http://st.huanxung.cn

diff a.txt b.txt
来源：http://pd.newstarts.cn

[R55] 压缩与解压
来源：http://up.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://te.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://mg.asd995.cn

scp file user@host:/path/
来源：http://aj.szsharing.cn

[R57] 远程执行命令
来源：http://hp.hnjuh.cn

ssh user@host 'uptime'
来源：http://ld.bjjhwx.cn

[R58] 下载文件
来源：http://ts.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qh.bjjhwx.cn

[R59] 发 POST JSON
来源：http://uo.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hd.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://rb.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uq.bjjhwx.cn

[R61] 磁盘占用
来源：http://of.szxytkj.cn

df -h;  du -sh *
来源：http://zx.nszjky.cn

[R62] 找最占空间的文件
来源：http://gi.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://vj.muxihuayi.cn

[R63] 内存与进程
来源：http://gd.asd995.cn

free -h;  ps aux | grep nginx
来源：http://rl.yuntaijiaju.cn

[R64] 结束进程
来源：http://qv.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://oa.shxzukj.cn

[R65] 查看端口占用
来源：http://lh.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lc.huixiangedu.cn

[R66] 定时任务
来源：http://cp.szsharing.cn

crontab -e;  crontab -l
来源：http://yw.szsharing.cn

[R67] 生成随机十六进制串
来源：http://ti.huixiangedu.cn

openssl rand -hex 16
来源：http://jn.wgjwhj.cn

[R68] 计算文件校验值
来源：http://jr.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cw.szsharing.cn

[R69] 生成随机密码
来源：http://my.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://tm.newstarts.cn

[R70] 时间戳与互转
来源：http://rt.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://sn.nszjky.cn

[R71] 日期格式化
来源：http://ny.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wc.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://ko.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cu.9csxet.cn

[R73] 分割大日志
来源：http://fx.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://rh.huixiangedu.cn

[R74] 批量重命名
来源：http://rk.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zz.muxihuayi.cn

[R75] 导出环境变量
来源：http://pk.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://gk.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://qx.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jb.asd995.cn

[R77] 读取用户输入
来源：http://jb.hahajie.cn

read -rp "请输入: " ans
来源：http://zh.521024.cn

[R78] 交互式菜单
来源：http://bj.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nq.521024.cn

[R79] 解析命令行选项
来源：http://os.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sj.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://fw.nszjky.cn

time ./run.sh
来源：http://xt.huixinmuqiang.cn

================================================================================
来源：http://vi.huixiangedu.cn

S. C / C++ 专题
来源：http://lv.muxihuayi.cn

================================================================================
来源：http://ba.wgjwhj.cn

[S01] C：Hello World
来源：http://dz.shxzukj.cn

#include <stdio.h>
来源：http://vn.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yq.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://ob.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://mt.wgjwhj.cn

[S03] C：读入整数
来源：http://ut.hnjuh.cn

int x; scanf("%d", &x);
来源：http://sl.shtwfgs.cn

[S04] C：字符串复制
来源：http://uz.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gl.asd995.cn

[S05] C：字符串长度
来源：http://be.jctech888.com.cn

strlen(s)
来源：http://fx.shxzskj.cn

[S06] C：字符串比较
来源：http://yx.9csxet.cn

strcmp(a, b) == 0
来源：http://hd.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://jt.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lj.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://ai.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jf.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://rq.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qh.lnxyls.cn

[S10] C：指针与解引用
来源：http://iz.newstarts.cn

int *p = &a;  *p = 5;
来源：http://wy.bjjhwx.cn

[S11] C：逐行读文件
来源：http://el.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://rg.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://at.nszjky.cn

fclose(f);
来源：http://dc.bookmarksfly.cn

[S12] C：写文件
来源：http://ai.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ez.huixinmuqiang.cn

[S13] C：宏定义
来源：http://yo.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fv.haigaiapp.cn

[S14] C：枚举
来源：http://fb.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://le.gzmigu.cn

[S15] C：类型转换
来源：http://sd.9csxet.cn

(double) a / b
来源：http://ik.shxzskj.cn

[S16] C：位操作置位
来源：http://vu.lnxyls.cn

x |= (1 << 3);
来源：http://ll.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://oa.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fv.chemitech.net.cn

[S18] C：命令行参数
来源：http://re.shxzskj.cn

int main(int argc, char **argv)
来源：http://yo.jianghongdianzi.cn

[S19] C：快速排序
来源：http://xs.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vn.jianghongdianzi.cn

[S20] C：二分查找
来源：http://lu.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fb.shxzukj.cn

[S21] C：字符类别判断
来源：http://rv.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gt.colortex.cn

[S22] C：字符串转数字
来源：http://ig.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ge.hnjuh.cn

[S23] C：随机数
来源：http://fe.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cf.colortex.cn

[S24] C：获取本地时间
来源：http://nm.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vw.haigaiapp.cn

[S25] C：内存拷贝
来源：http://te.gzmigu.cn

memcpy(dst, src, n);
来源：http://gs.jianghongdianzi.cn

[S26] C：内存清零
来源：http://hs.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://ti.szxytkj.cn

[S27] C：定义常量
来源：http://xq.panjiajie.cn

const double PI = 3.14159;
来源：http://my.muxihuayi.cn

[S28] C：静态变量
来源：http://fm.9csxet.cn

static int counter = 0;
来源：http://fz.newstarts.cn

[S29] C：变参函数
来源：http://by.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cw.huanxung.cn

[S30] C：头文件保护
来源：http://ie.huanxung.cn

#ifndef X_H
来源：http://pq.jianghongdianzi.cn

#define X_H
来源：http://fq.521024.cn

#endif
来源：http://zk.9csxet.cn

[S31] C++：Hello World
来源：http://vh.shxzskj.cn

#include <iostream>
来源：http://my.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://ge.szxytkj.cn

[S32] C++：字符串
来源：http://ax.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://hu.nszjky.cn

[S33] C++：vector 增删
来源：http://qy.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zg.panjiajie.cn

[S34] C++：遍历 vector
来源：http://hv.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://vc.lnxyls.cn

[S35] C++：map
来源：http://hb.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ml.nszjky.cn

[S36] C++：unordered_map
来源：http://bu.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://my.huixinmuqiang.cn

[S37] C++：set
来源：http://hl.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ol.huanxung.cn

[S38] C++：排序
来源：http://sh.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://fn.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://dj.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://az.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://sb.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zt.szxytkj.cn

[S41] C++：类与构造函数
来源：http://xj.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jz.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://jx.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://uu.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://bu.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://gd.jctech888.com.cn

[S44] C++：引用传参
来源：http://qh.colortex.cn

void inc(int &x) { ++x; }
来源：http://tq.muxihuayi.cn

[S45] C++：lambda
来源：http://lh.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vu.gzmigu.cn

[S46] C++：函数模板
来源：http://we.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ud.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://wq.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kj.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://bd.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jh.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://ll.9csxet.cn

[S49] C++：写文件
来源：http://el.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wh.lnxyls.cn

[S50] C++：格式化数字
来源：http://dx.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ig.colortex.cn

[S51] C++：显式类型转换
来源：http://tf.521024.cn

static_cast<double>(a) / b
来源：http://qf.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://fv.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://bd.haigaiapp.cn

[S53] C++：移动语义
来源：http://pg.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://ah.haigaiapp.cn

[S54] C++：异常处理
来源：http://ba.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mq.nszjky.cn

[S55] C++：结构化绑定
来源：http://ty.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://it.shxzskj.cn

[S56] C++：optional
来源：http://aa.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iz.huanxung.cn

[S57] C++：编译期常量
来源：http://cu.wgjwhj.cn

constexpr int N = 10;
来源：http://lw.9csxet.cn

[S58] C++：命名空间
来源：http://qy.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://zn.shtwfgs.cn

[S59] C++：静态断言
来源：http://qy.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yk.521024.cn

[S60] C++：遍历并删除元素
来源：http://mx.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fj.9csxet.cn

================================================================================
来源：http://rm.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gw.szsharing.cn

================================================================================
来源：http://wm.nicolike.cn

[T01] Kotlin：Hello World
来源：http://wa.asd995.cn

println("Hello")
来源：http://lw.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://ap.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hv.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://gc.asd995.cn

"值: $b"
来源：http://rx.szxytkj.cn

[T04] Kotlin：空安全
来源：http://aa.panjiajie.cn

val n: String? = null;  n?.length
来源：http://ky.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://vq.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wt.newstarts.cn

[T06] Kotlin：集合映射
来源：http://ei.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ms.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://dq.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cx.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://be.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://st.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://il.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://ot.nszjky.cn

[T10] Kotlin：默认参数
来源：http://bn.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nw.szsharing.cn

[T11] Kotlin：协程
来源：http://tg.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ta.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://bk.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://on.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://oh.szsharing.cn

val m = mapOf("a" to 1)
来源：http://ho.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://qi.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://vv.chemitech.net.cn


<!-- 参考信息 -->