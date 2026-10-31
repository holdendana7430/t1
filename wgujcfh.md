代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ry.szsharing.cn

[R08] 数值比较
来源：http://og.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jj.jianghongdianzi.cn

[R09] 字符串比较
来源：http://yf.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jj.huanxung.cn

[R10] 正则匹配
来源：http://fa.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ll.huixiangedu.cn

[R11] case 多分支
来源：http://cl.bjjhwx.cn

case "$1" in
来源：http://sa.szsharing.cn

start) echo "启动" ;;
来源：http://gm.colortex.cn

stop)  echo "停止" ;;
来源：http://yv.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://hm.yuexingan06.cn

esac
来源：http://oq.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://ke.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://md.haigaiapp.cn

[R13] for 计数循环
来源：http://ms.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://az.colortex.cn

[R14] C 风格 for
来源：http://ry.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fe.lnxyls.cn

[R15] while 逐行读文件
来源：http://gk.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jn.chemitech.net.cn

[R16] until 等待条件
来源：http://xr.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lp.haigaiapp.cn

[R17] 数组定义与取值
来源：http://jp.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uj.yuntaijiaju.cn

[R18] 遍历数组
来源：http://cm.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hm.huixiangedu.cn

[R19] 数组长度
来源：http://nt.shxzskj.cn

echo "${#arr[@]}"
来源：http://im.bookmarksfly.cn

[R20] 关联数组（字典）
来源：http://ms.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://il.jctech888.com.cn

[R21] 字符串长度
来源：http://ka.jctech888.com.cn

echo "${#s}"
来源：http://hg.hnjuh.cn

[R22] 截取子串
来源：http://jn.chemitech.net.cn

echo "${s:0:5}"
来源：http://sb.shtwfgs.cn

[R23] 字符串替换
来源：http://qk.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mq.colortex.cn

[R24] 大小写转换
来源：http://dr.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qz.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://zf.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yo.yuexingan06.cn

[R26] 命令替换
来源：http://gh.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://fi.nicolike.cn

[R27] 算术展开
来源：http://ul.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://bj.nicolike.cn

[R28] 浮点运算
来源：http://yf.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://fx.panjiajie.cn

[R29] 定义函数
来源：http://vp.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bp.szxytkj.cn

[R30] 函数返回状态码
来源：http://ej.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://tx.shxzukj.cn

[R31] 局部变量
来源：http://bt.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://cb.nicolike.cn

[R32] 参数个数校验
来源：http://bw.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ez.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://hh.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dr.gzmigu.cn

[R34] 退出时清理
来源：http://dh.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lw.hahajie.cn

[R35] 后台执行并等待
来源：http://yr.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mr.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://zd.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ie.panjiajie.cn

[R37] 把输出赋给变量
来源：http://oo.bjjhwx.cn

files=$(ls -1)
来源：http://ix.muxihuayi.cn

[R38] 管道串联
来源：http://vs.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://rc.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://jf.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://dy.colortex.cn

[R40] 追加写日志
来源：http://xh.newstarts.cn

echo "log" >> out.log
来源：http://hp.newstarts.cn

[R41] 丢弃输出
来源：http://ct.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://kc.asd995.cn

[R42] 输入重定向
来源：http://gd.panjiajie.cn

wc -l < a.txt
来源：http://yl.chemitech.net.cn

[R43] 按名字查找文件
来源：http://cs.shxzskj.cn

find . -name "*.log" -type f
来源：http://zd.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://cy.szsharing.cn

find . -mtime -7 -type f
来源：http://vh.lnxyls.cn

[R45] 批量删除
来源：http://fi.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://za.asd995.cn

[R46] 递归替换文件内容
来源：http://qq.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tz.hahajie.cn

[R47] sed 单行替换
来源：http://ls.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vu.muxihuayi.cn

[R48] awk 取指定列
来源：http://kr.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://ee.muxihuayi.cn

[R49] awk 带条件
来源：http://wv.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hb.bookmarksfly.cn

[R50] awk 求和
来源：http://zn.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tu.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://dk.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hk.hahajie.cn

[R52] 统计行数
来源：http://iw.asd995.cn

wc -l a.txt
来源：http://vh.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://gp.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ab.szsharing.cn

[R54] 比较两个文件
来源：http://fm.hahajie.cn

diff a.txt b.txt
来源：http://zw.huixiangedu.cn

[R55] 压缩与解压
来源：http://dv.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ah.colortex.cn

[R56] 远程拷贝
来源：http://fs.yuntaijiaju.cn

scp file user@host:/path/
来源：http://ll.muxihuayi.cn

[R57] 远程执行命令
来源：http://rn.wgjwhj.cn

ssh user@host 'uptime'
来源：http://kw.newstarts.cn

[R58] 下载文件
来源：http://dm.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://im.shxzskj.cn

[R59] 发 POST JSON
来源：http://xd.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vn.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://ug.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rd.colortex.cn

[R61] 磁盘占用
来源：http://sh.gzmigu.cn

df -h;  du -sh *
来源：http://rz.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://ui.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://fd.newstarts.cn

[R63] 内存与进程
来源：http://mv.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://mf.panjiajie.cn

[R64] 结束进程
来源：http://wv.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://jm.bookmarksfly.cn

[R65] 查看端口占用
来源：http://ii.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mn.gzmigu.cn

[R66] 定时任务
来源：http://iu.shxzukj.cn

crontab -e;  crontab -l
来源：http://ez.521024.cn

[R67] 生成随机十六进制串
来源：http://yd.chemitech.net.cn

openssl rand -hex 16
来源：http://jv.9csxet.cn

[R68] 计算文件校验值
来源：http://es.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xb.huanxung.cn

[R69] 生成随机密码
来源：http://qx.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://gl.szsharing.cn

[R70] 时间戳与互转
来源：http://qk.nicolike.cn

date +%s;  date -d @1700000000
来源：http://ua.nicolike.cn

[R71] 日期格式化
来源：http://ri.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ua.newstarts.cn

[R72] 等待端口就绪
来源：http://yq.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vh.bjjhwx.cn

[R73] 分割大日志
来源：http://ax.haigaiapp.cn

split -l 1000 big.log part_
来源：http://sc.colortex.cn

[R74] 批量重命名
来源：http://ti.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sh.gzmigu.cn

[R75] 导出环境变量
来源：http://nr.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://ct.huanxung.cn

[R76] 使用临时文件
来源：http://wu.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qr.shtwfgs.cn

[R77] 读取用户输入
来源：http://da.gzmigu.cn

read -rp "请输入: " ans
来源：http://jd.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://cv.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tf.huixiangedu.cn

[R79] 解析命令行选项
来源：http://dc.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sn.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://ay.panjiajie.cn

time ./run.sh
来源：http://sb.chemitech.net.cn

================================================================================
来源：http://mg.panjiajie.cn

S. C / C++ 专题
来源：http://vx.yuexingan06.cn

================================================================================
来源：http://tk.yuexingan06.cn

[S01] C：Hello World
来源：http://ck.huixiangedu.cn

#include <stdio.h>
来源：http://ft.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://us.521024.cn

[S02] C：变量与格式化输出
来源：http://wl.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://ni.asd995.cn

[S03] C：读入整数
来源：http://eb.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://xg.nicolike.cn

[S04] C：字符串复制
来源：http://bb.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://po.szsharing.cn

[S05] C：字符串长度
来源：http://tl.yuntaijiaju.cn

strlen(s)
来源：http://bz.hahajie.cn

[S06] C：字符串比较
来源：http://ix.szsharing.cn

strcmp(a, b) == 0
来源：http://fp.lnxyls.cn

[S07] C：数组遍历求和
来源：http://ev.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yk.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://ik.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zm.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://ro.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pd.muxihuayi.cn

[S10] C：指针与解引用
来源：http://cn.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://re.hnjuh.cn

[S11] C：逐行读文件
来源：http://tl.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://yy.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cj.yuexingan06.cn

fclose(f);
来源：http://dp.muxihuayi.cn

[S12] C：写文件
来源：http://pl.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vy.muxihuayi.cn

[S13] C：宏定义
来源：http://vd.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uw.bjjhwx.cn

[S14] C：枚举
来源：http://nj.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://pp.lnxyls.cn

[S15] C：类型转换
来源：http://ls.huixinmuqiang.cn

(double) a / b
来源：http://xy.lnxyls.cn

[S16] C：位操作置位
来源：http://oe.bjjhwx.cn

x |= (1 << 3);
来源：http://he.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://iw.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rc.hnjuh.cn

[S18] C：命令行参数
来源：http://gk.haigaiapp.cn

int main(int argc, char **argv)
来源：http://uu.bjjhwx.cn

[S19] C：快速排序
来源：http://uu.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://of.yuntaijiaju.cn

[S20] C：二分查找
来源：http://jv.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ny.hahajie.cn

[S21] C：字符类别判断
来源：http://qb.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jm.jctech888.com.cn

[S22] C：字符串转数字
来源：http://up.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fu.newstarts.cn

[S23] C：随机数
来源：http://wn.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lv.lnxyls.cn

[S24] C：获取本地时间
来源：http://ey.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kb.szxytkj.cn

[S25] C：内存拷贝
来源：http://cg.9csxet.cn

memcpy(dst, src, n);
来源：http://ie.panjiajie.cn

[S26] C：内存清零
来源：http://ur.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://pr.newstarts.cn

[S27] C：定义常量
来源：http://vc.huanxung.cn

const double PI = 3.14159;
来源：http://sx.gzmigu.cn

[S28] C：静态变量
来源：http://ta.yuexingan06.cn

static int counter = 0;
来源：http://as.bookmarksfly.cn

[S29] C：变参函数
来源：http://vs.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vt.gzmigu.cn

[S30] C：头文件保护
来源：http://yi.panjiajie.cn

#ifndef X_H
来源：http://ju.huanxung.cn

#define X_H
来源：http://vl.yuntaijiaju.cn

#endif
来源：http://kq.asd995.cn

[S31] C++：Hello World
来源：http://qm.hahajie.cn

#include <iostream>
来源：http://ou.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://ur.521024.cn

[S32] C++：字符串
来源：http://cj.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://vv.szxytkj.cn

[S33] C++：vector 增删
来源：http://oo.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ep.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://dz.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://cy.newstarts.cn

[S35] C++：map
来源：http://ru.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ey.yuexingan06.cn

[S36] C++：unordered_map
来源：http://qs.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kv.nicolike.cn

[S37] C++：set
来源：http://vh.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://am.chemitech.net.cn

[S38] C++：排序
来源：http://wm.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://lg.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://ut.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oe.asd995.cn

[S40] C++：查找元素
来源：http://xz.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://re.szsharing.cn

[S41] C++：类与构造函数
来源：http://yw.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yn.hahajie.cn

[S42] C++：继承与虚函数
来源：http://yv.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://ga.jctech888.com.cn

[S43] C++：智能指针
来源：http://ci.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://wz.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://wl.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://xz.shxzskj.cn

[S45] C++：lambda
来源：http://dj.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oh.panjiajie.cn

[S46] C++：函数模板
来源：http://bx.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xw.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://sl.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wa.gzmigu.cn

[S48] C++：逐行读文件
来源：http://pa.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ev.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://vj.chemitech.net.cn

[S49] C++：写文件
来源：http://no.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mn.gzmigu.cn

[S50] C++：格式化数字
来源：http://va.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xi.panjiajie.cn

[S51] C++：显式类型转换
来源：http://bw.muxihuayi.cn

static_cast<double>(a) / b
来源：http://zb.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://lo.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://pz.muxihuayi.cn

[S53] C++：移动语义
来源：http://pv.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://yc.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://lm.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lg.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://ew.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ca.huanxung.cn

[S56] C++：optional
来源：http://ge.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zv.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://vx.chemitech.net.cn

constexpr int N = 10;
来源：http://vx.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://aw.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://pu.hahajie.cn

[S59] C++：静态断言
来源：http://al.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bt.colortex.cn

[S60] C++：遍历并删除元素
来源：http://hu.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jm.bookmarksfly.cn

================================================================================
来源：http://dx.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lw.colortex.cn

================================================================================
来源：http://qh.asd995.cn

[T01] Kotlin：Hello World
来源：http://ve.lnxyls.cn

println("Hello")
来源：http://dq.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://qi.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ee.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://tt.haigaiapp.cn

"值: $b"
来源：http://qn.nszjky.cn

[T04] Kotlin：空安全
来源：http://yt.521024.cn

val n: String? = null;  n?.length
来源：http://qs.521024.cn

[T05] Kotlin：when 表达式
来源：http://tr.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cn.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://dy.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sc.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://uv.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tx.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://ds.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://rz.hahajie.cn


<!-- 参考信息 -->