代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://em.huixinmuqiang.cn

[R10] 正则匹配
来源：http://gi.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fc.521024.cn

[R11] case 多分支
来源：http://qt.huanxung.cn

case "$1" in
来源：http://wq.wgjwhj.cn

start) echo "启动" ;;
来源：http://mx.szxytkj.cn

stop)  echo "停止" ;;
来源：http://nq.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://ge.huixinmuqiang.cn

esac
来源：http://nt.asd995.cn

[R12] for 遍历文件
来源：http://sa.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://np.521024.cn

[R13] for 计数循环
来源：http://lg.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://jh.jctech888.com.cn

[R14] C 风格 for
来源：http://vk.9csxet.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vq.nszjky.cn

[R15] while 逐行读文件
来源：http://fa.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bx.jctech888.com.cn

[R16] until 等待条件
来源：http://sm.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yd.hahajie.cn

[R17] 数组定义与取值
来源：http://zz.huanxung.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ep.szsharing.cn

[R18] 遍历数组
来源：http://td.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ru.huixinmuqiang.cn

[R19] 数组长度
来源：http://qb.hahajie.cn

echo "${#arr[@]}"
来源：http://bw.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://xu.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gg.jianghongdianzi.cn

[R21] 字符串长度
来源：http://us.lnxyls.cn

echo "${#s}"
来源：http://sh.gzmigu.cn

[R22] 截取子串
来源：http://rh.shxzskj.cn

echo "${s:0:5}"
来源：http://ui.nszjky.cn

[R23] 字符串替换
来源：http://mq.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ii.newstarts.cn

[R24] 大小写转换
来源：http://mh.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sa.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://me.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qk.521024.cn

[R26] 命令替换
来源：http://gd.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://rx.hnjuh.cn

[R27] 算术展开
来源：http://at.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://bg.hahajie.cn

[R28] 浮点运算
来源：http://dy.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://da.szxytkj.cn

[R29] 定义函数
来源：http://ih.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uh.huanxung.cn

[R30] 函数返回状态码
来源：http://aj.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://co.huixiangedu.cn

[R31] 局部变量
来源：http://kq.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://fo.nicolike.cn

[R32] 参数个数校验
来源：http://pj.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mn.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://xh.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jg.lnxyls.cn

[R34] 退出时清理
来源：http://vp.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ae.muxihuayi.cn

[R35] 后台执行并等待
来源：http://sy.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xb.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://df.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dg.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://fd.shxzukj.cn

files=$(ls -1)
来源：http://bb.newstarts.cn

[R38] 管道串联
来源：http://td.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://rh.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://yh.9csxet.cn

cmd > out.log 2>&1
来源：http://tm.haigaiapp.cn

[R40] 追加写日志
来源：http://xr.asd995.cn

echo "log" >> out.log
来源：http://su.colortex.cn

[R41] 丢弃输出
来源：http://ky.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://kc.lnxyls.cn

[R42] 输入重定向
来源：http://oj.panjiajie.cn

wc -l < a.txt
来源：http://gf.colortex.cn

[R43] 按名字查找文件
来源：http://pc.szsharing.cn

find . -name "*.log" -type f
来源：http://et.colortex.cn

[R44] 按修改时间查找
来源：http://ki.lnxyls.cn

find . -mtime -7 -type f
来源：http://fi.hahajie.cn

[R45] 批量删除
来源：http://xf.hahajie.cn

find . -name "*.tmp" -delete
来源：http://qd.huanxung.cn

[R46] 递归替换文件内容
来源：http://yx.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uu.shxzukj.cn

[R47] sed 单行替换
来源：http://vr.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ff.wgjwhj.cn

[R48] awk 取指定列
来源：http://gs.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://uf.jianghongdianzi.cn

[R49] awk 带条件
来源：http://zj.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tu.bjjhwx.cn

[R50] awk 求和
来源：http://cn.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://on.bjjhwx.cn

[R51] 排序去重取前几
来源：http://wu.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yq.yuntaijiaju.cn

[R52] 统计行数
来源：http://nz.shxzskj.cn

wc -l a.txt
来源：http://uo.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://nf.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fk.nszjky.cn

[R54] 比较两个文件
来源：http://by.bookmarksfly.cn

diff a.txt b.txt
来源：http://hn.bookmarksfly.cn

[R55] 压缩与解压
来源：http://li.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ej.chemitech.net.cn

[R56] 远程拷贝
来源：http://cr.shxzskj.cn

scp file user@host:/path/
来源：http://km.newstarts.cn

[R57] 远程执行命令
来源：http://to.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://xs.9csxet.cn

[R58] 下载文件
来源：http://cb.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uk.nszjky.cn

[R59] 发 POST JSON
来源：http://ia.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lo.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://ta.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fj.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://ni.colortex.cn

df -h;  du -sh *
来源：http://nm.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://lk.colortex.cn

du -ah . | sort -rh | head -10
来源：http://kk.huixiangedu.cn

[R63] 内存与进程
来源：http://rs.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://su.huixiangedu.cn

[R64] 结束进程
来源：http://xk.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://mn.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://gv.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://my.szsharing.cn

[R66] 定时任务
来源：http://gf.shxzskj.cn

crontab -e;  crontab -l
来源：http://sz.nszjky.cn

[R67] 生成随机十六进制串
来源：http://ak.asd995.cn

openssl rand -hex 16
来源：http://gq.shxzskj.cn

[R68] 计算文件校验值
来源：http://gi.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tl.huanxung.cn

[R69] 生成随机密码
来源：http://rm.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://zu.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://rj.nicolike.cn

date +%s;  date -d @1700000000
来源：http://sq.jianghongdianzi.cn

[R71] 日期格式化
来源：http://lf.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tk.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://zl.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nr.shtwfgs.cn

[R73] 分割大日志
来源：http://rp.9csxet.cn

split -l 1000 big.log part_
来源：http://cu.huixinmuqiang.cn

[R74] 批量重命名
来源：http://kp.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xz.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://ba.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://nb.521024.cn

[R76] 使用临时文件
来源：http://pd.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dg.yuexingan06.cn

[R77] 读取用户输入
来源：http://ol.nicolike.cn

read -rp "请输入: " ans
来源：http://ni.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://mv.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uy.yuexingan06.cn

[R79] 解析命令行选项
来源：http://jc.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ub.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://dz.haigaiapp.cn

time ./run.sh
来源：http://ns.szsharing.cn

================================================================================
来源：http://bw.shtwfgs.cn

S. C / C++ 专题
来源：http://oo.colortex.cn

================================================================================
来源：http://fw.asd995.cn

[S01] C：Hello World
来源：http://qv.bjjhwx.cn

#include <stdio.h>
来源：http://tn.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mj.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://qo.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://gn.nicolike.cn

[S03] C：读入整数
来源：http://fb.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://uk.szsharing.cn

[S04] C：字符串复制
来源：http://km.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ad.jctech888.com.cn

[S05] C：字符串长度
来源：http://ol.haigaiapp.cn

strlen(s)
来源：http://yz.shxzskj.cn

[S06] C：字符串比较
来源：http://ra.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://ma.szsharing.cn

[S07] C：数组遍历求和
来源：http://kb.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ao.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://ai.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dx.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://ws.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rd.521024.cn

[S10] C：指针与解引用
来源：http://qu.huanxung.cn

int *p = &a;  *p = 5;
来源：http://nn.shxzukj.cn

[S11] C：逐行读文件
来源：http://xf.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://io.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ce.shtwfgs.cn

fclose(f);
来源：http://yd.colortex.cn

[S12] C：写文件
来源：http://hr.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vl.asd995.cn

[S13] C：宏定义
来源：http://iu.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sy.colortex.cn

[S14] C：枚举
来源：http://xq.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://xe.bookmarksfly.cn

[S15] C：类型转换
来源：http://ek.lnxyls.cn

(double) a / b
来源：http://gj.nicolike.cn

[S16] C：位操作置位
来源：http://xm.bjjhwx.cn

x |= (1 << 3);
来源：http://bl.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://wf.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jb.szsharing.cn

[S18] C：命令行参数
来源：http://qr.bjjhwx.cn

int main(int argc, char **argv)
来源：http://cm.bookmarksfly.cn

[S19] C：快速排序
来源：http://ct.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rz.hahajie.cn

[S20] C：二分查找
来源：http://ab.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xi.nszjky.cn

[S21] C：字符类别判断
来源：http://as.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nt.newstarts.cn

[S22] C：字符串转数字
来源：http://hi.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ql.wgjwhj.cn

[S23] C：随机数
来源：http://pc.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zn.shtwfgs.cn

[S24] C：获取本地时间
来源：http://zr.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xu.muxihuayi.cn

[S25] C：内存拷贝
来源：http://ox.shxzskj.cn

memcpy(dst, src, n);
来源：http://hv.haigaiapp.cn

[S26] C：内存清零
来源：http://ju.newstarts.cn

memset(a, 0, sizeof a);
来源：http://wg.521024.cn

[S27] C：定义常量
来源：http://ia.chemitech.net.cn

const double PI = 3.14159;
来源：http://ml.newstarts.cn

[S28] C：静态变量
来源：http://ws.shxzukj.cn

static int counter = 0;
来源：http://ro.hahajie.cn

[S29] C：变参函数
来源：http://qh.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zm.colortex.cn

[S30] C：头文件保护
来源：http://hp.nszjky.cn

#ifndef X_H
来源：http://mk.huixiangedu.cn

#define X_H
来源：http://fm.nicolike.cn

#endif
来源：http://un.chemitech.net.cn

[S31] C++：Hello World
来源：http://oi.muxihuayi.cn

#include <iostream>
来源：http://pn.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://oc.shxzukj.cn

[S32] C++：字符串
来源：http://dc.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://lz.huanxung.cn

[S33] C++：vector 增删
来源：http://wm.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://de.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://wp.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://ua.panjiajie.cn

[S35] C++：map
来源：http://ft.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ib.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://wo.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nq.9csxet.cn

[S37] C++：set
来源：http://da.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://di.huixiangedu.cn

[S38] C++：排序
来源：http://fv.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://xw.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://kq.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zj.hahajie.cn

[S40] C++：查找元素
来源：http://hs.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://he.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://el.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dg.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://uu.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://gh.panjiajie.cn

[S43] C++：智能指针
来源：http://ax.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://wk.bjjhwx.cn

[S44] C++：引用传参
来源：http://fx.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://sd.haigaiapp.cn

[S45] C++：lambda
来源：http://gc.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lw.newstarts.cn

[S46] C++：函数模板
来源：http://ci.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kk.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://vk.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fb.shxzskj.cn

[S48] C++：逐行读文件
来源：http://ag.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yu.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://eo.shtwfgs.cn

[S49] C++：写文件
来源：http://sw.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xt.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://gn.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dw.521024.cn

[S51] C++：显式类型转换
来源：http://ua.nszjky.cn

static_cast<double>(a) / b
来源：http://oj.colortex.cn

[S52] C++：const 与 noexcept
来源：http://od.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://uf.gzmigu.cn

[S53] C++：移动语义
来源：http://ro.colortex.cn

std::vector<int> w = std::move(v);
来源：http://ns.asd995.cn

[S54] C++：异常处理
来源：http://ns.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pz.panjiajie.cn

[S55] C++：结构化绑定
来源：http://xx.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mh.huanxung.cn

[S56] C++：optional
来源：http://rq.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zv.hnjuh.cn

[S57] C++：编译期常量
来源：http://nr.szsharing.cn

constexpr int N = 10;
来源：http://ly.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://gi.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://rq.yuntaijiaju.cn

[S59] C++：静态断言
来源：http://fu.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ix.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://pc.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://md.szxytkj.cn

================================================================================
来源：http://yq.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xv.asd995.cn

================================================================================
来源：http://gl.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://kj.wgjwhj.cn

println("Hello")
来源：http://kd.lnxyls.cn

[T02] Kotlin：变量
来源：http://mt.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yh.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://hv.9csxet.cn

"值: $b"
来源：http://xq.panjiajie.cn

[T04] Kotlin：空安全
来源：http://bt.hahajie.cn

val n: String? = null;  n?.length
来源：http://on.colortex.cn

[T05] Kotlin：when 表达式
来源：http://cw.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pr.colortex.cn

[T06] Kotlin：集合映射
来源：http://pk.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nn.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://mx.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lh.szxytkj.cn

[T08] Kotlin：数据类
来源：http://ka.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://ui.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://rd.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://si.hahajie.cn

[T10] Kotlin：默认参数
来源：http://ft.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hx.yuntaijiaju.cn


<!-- 参考信息 -->