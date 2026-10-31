代发 wailian999

case "$1" in
来源：http://hh.shxzskj.cn

start) echo "启动" ;;
来源：http://xi.nicolike.cn

stop)  echo "停止" ;;
来源：http://ad.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://bw.huixiangedu.cn

esac
来源：http://gz.huanxung.cn

[R12] for 遍历文件
来源：http://zq.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://hi.yuexingan06.cn

[R13] for 计数循环
来源：http://ir.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://cn.jctech888.com.cn

[R14] C 风格 for
来源：http://oz.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pu.yuexingan06.cn

[R15] while 逐行读文件
来源：http://bo.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rk.nicolike.cn

[R16] until 等待条件
来源：http://ly.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://te.chemitech.net.cn

[R17] 数组定义与取值
来源：http://rj.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bq.yuntaijiaju.cn

[R18] 遍历数组
来源：http://tf.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zn.nszjky.cn

[R19] 数组长度
来源：http://pt.szxytkj.cn

echo "${#arr[@]}"
来源：http://vz.9csxet.cn

[R20] 关联数组（字典）
来源：http://rn.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rl.nicolike.cn

[R21] 字符串长度
来源：http://mj.shtwfgs.cn

echo "${#s}"
来源：http://ou.bjjhwx.cn

[R22] 截取子串
来源：http://ug.lnxyls.cn

echo "${s:0:5}"
来源：http://lf.hahajie.cn

[R23] 字符串替换
来源：http://ru.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zx.chemitech.net.cn

[R24] 大小写转换
来源：http://fb.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sd.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://nf.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jf.szxytkj.cn

[R26] 命令替换
来源：http://rq.asd995.cn

now=$(date +%F); echo "$now"
来源：http://jd.newstarts.cn

[R27] 算术展开
来源：http://ft.521024.cn

echo $((1 + 2 * 3))
来源：http://fx.shxzukj.cn

[R28] 浮点运算
来源：http://rj.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://er.hahajie.cn

[R29] 定义函数
来源：http://ac.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qs.colortex.cn

[R30] 函数返回状态码
来源：http://ze.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://in.szsharing.cn

[R31] 局部变量
来源：http://ao.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://yv.9csxet.cn

[R32] 参数个数校验
来源：http://qu.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ta.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://yu.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qy.haigaiapp.cn

[R34] 退出时清理
来源：http://iq.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xn.wgjwhj.cn

[R35] 后台执行并等待
来源：http://yd.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ja.gzmigu.cn

[R36] 并发执行多个任务
来源：http://ym.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ao.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://zj.newstarts.cn

files=$(ls -1)
来源：http://ok.521024.cn

[R38] 管道串联
来源：http://me.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://zg.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://jm.shxzskj.cn

cmd > out.log 2>&1
来源：http://to.haigaiapp.cn

[R40] 追加写日志
来源：http://es.521024.cn

echo "log" >> out.log
来源：http://rg.huanxung.cn

[R41] 丢弃输出
来源：http://ek.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://bx.hahajie.cn

[R42] 输入重定向
来源：http://lo.asd995.cn

wc -l < a.txt
来源：http://bh.huixiangedu.cn

[R43] 按名字查找文件
来源：http://mj.nszjky.cn

find . -name "*.log" -type f
来源：http://zn.gzmigu.cn

[R44] 按修改时间查找
来源：http://rx.lnxyls.cn

find . -mtime -7 -type f
来源：http://kt.colortex.cn

[R45] 批量删除
来源：http://ns.521024.cn

find . -name "*.tmp" -delete
来源：http://bz.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://is.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yt.lnxyls.cn

[R47] sed 单行替换
来源：http://yi.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bt.szxytkj.cn

[R48] awk 取指定列
来源：http://es.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://vp.nszjky.cn

[R49] awk 带条件
来源：http://lv.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xa.yuexingan06.cn

[R50] awk 求和
来源：http://ut.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rz.lnxyls.cn

[R51] 排序去重取前几
来源：http://ed.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yt.shtwfgs.cn

[R52] 统计行数
来源：http://tn.gzmigu.cn

wc -l a.txt
来源：http://ji.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://rk.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jm.bjjhwx.cn

[R54] 比较两个文件
来源：http://bs.shtwfgs.cn

diff a.txt b.txt
来源：http://xa.szsharing.cn

[R55] 压缩与解压
来源：http://nc.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ny.gzmigu.cn

[R56] 远程拷贝
来源：http://ah.panjiajie.cn

scp file user@host:/path/
来源：http://fh.shxzukj.cn

[R57] 远程执行命令
来源：http://xr.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://el.wgjwhj.cn

[R58] 下载文件
来源：http://eu.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vx.9csxet.cn

[R59] 发 POST JSON
来源：http://dh.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rx.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://ew.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oc.chemitech.net.cn

[R61] 磁盘占用
来源：http://df.shxzskj.cn

df -h;  du -sh *
来源：http://at.szxytkj.cn

[R62] 找最占空间的文件
来源：http://rx.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://kx.panjiajie.cn

[R63] 内存与进程
来源：http://sm.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://gu.jctech888.com.cn

[R64] 结束进程
来源：http://xm.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://cy.panjiajie.cn

[R65] 查看端口占用
来源：http://sh.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ly.asd995.cn

[R66] 定时任务
来源：http://cm.huixiangedu.cn

crontab -e;  crontab -l
来源：http://zq.nszjky.cn

[R67] 生成随机十六进制串
来源：http://ha.chemitech.net.cn

openssl rand -hex 16
来源：http://vz.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://mi.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yj.yuexingan06.cn

[R69] 生成随机密码
来源：http://ek.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://yo.hahajie.cn

[R70] 时间戳与互转
来源：http://ny.hahajie.cn

date +%s;  date -d @1700000000
来源：http://yt.jctech888.com.cn

[R71] 日期格式化
来源：http://od.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kn.newstarts.cn

[R72] 等待端口就绪
来源：http://oz.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dj.shxzukj.cn

[R73] 分割大日志
来源：http://bx.gzmigu.cn

split -l 1000 big.log part_
来源：http://gt.chemitech.net.cn

[R74] 批量重命名
来源：http://gq.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dh.yuexingan06.cn

[R75] 导出环境变量
来源：http://yx.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://ya.shtwfgs.cn

[R76] 使用临时文件
来源：http://hq.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://og.haigaiapp.cn

[R77] 读取用户输入
来源：http://mx.yuexingan06.cn

read -rp "请输入: " ans
来源：http://pg.shtwfgs.cn

[R78] 交互式菜单
来源：http://ic.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ns.colortex.cn

[R79] 解析命令行选项
来源：http://yf.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gp.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://kh.shtwfgs.cn

time ./run.sh
来源：http://ld.shxzukj.cn

================================================================================
来源：http://bw.huixiangedu.cn

S. C / C++ 专题
来源：http://zz.colortex.cn

================================================================================
来源：http://kn.huixinmuqiang.cn

[S01] C：Hello World
来源：http://kt.shtwfgs.cn

#include <stdio.h>
来源：http://nx.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://te.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://wa.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://dy.shxzskj.cn

[S03] C：读入整数
来源：http://yr.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://qy.bookmarksfly.cn

[S04] C：字符串复制
来源：http://wt.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nr.huixiangedu.cn

[S05] C：字符串长度
来源：http://ef.haigaiapp.cn

strlen(s)
来源：http://oi.haigaiapp.cn

[S06] C：字符串比较
来源：http://sg.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://zi.nicolike.cn

[S07] C：数组遍历求和
来源：http://wx.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uc.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://fs.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ke.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://il.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ks.gzmigu.cn

[S10] C：指针与解引用
来源：http://uf.nicolike.cn

int *p = &a;  *p = 5;
来源：http://nq.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://az.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://cp.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ds.shxzukj.cn

fclose(f);
来源：http://db.szsharing.cn

[S12] C：写文件
来源：http://et.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nk.hnjuh.cn

[S13] C：宏定义
来源：http://zw.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aa.muxihuayi.cn

[S14] C：枚举
来源：http://jp.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://ke.yuntaijiaju.cn

[S15] C：类型转换
来源：http://ru.chemitech.net.cn

(double) a / b
来源：http://fm.huanxung.cn

[S16] C：位操作置位
来源：http://fk.huixinmuqiang.cn

x |= (1 << 3);
来源：http://kw.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://ah.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lo.colortex.cn

[S18] C：命令行参数
来源：http://ug.muxihuayi.cn

int main(int argc, char **argv)
来源：http://xc.szxytkj.cn

[S19] C：快速排序
来源：http://yk.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iw.9csxet.cn

[S20] C：二分查找
来源：http://ip.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uo.nszjky.cn

[S21] C：字符类别判断
来源：http://ha.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cn.wgjwhj.cn

[S22] C：字符串转数字
来源：http://ik.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://of.huanxung.cn

[S23] C：随机数
来源：http://jk.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://os.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://wu.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vc.hnjuh.cn

[S25] C：内存拷贝
来源：http://ke.gzmigu.cn

memcpy(dst, src, n);
来源：http://ce.wgjwhj.cn

[S26] C：内存清零
来源：http://ye.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://bt.colortex.cn

[S27] C：定义常量
来源：http://ov.bjjhwx.cn

const double PI = 3.14159;
来源：http://hn.jianghongdianzi.cn

[S28] C：静态变量
来源：http://bd.jianghongdianzi.cn

static int counter = 0;
来源：http://ib.bookmarksfly.cn

[S29] C：变参函数
来源：http://tj.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qn.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://yb.szsharing.cn

#ifndef X_H
来源：http://lf.nszjky.cn

#define X_H
来源：http://cp.shxzukj.cn

#endif
来源：http://wm.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://yt.haigaiapp.cn

#include <iostream>
来源：http://sf.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://fb.yuntaijiaju.cn

[S32] C++：字符串
来源：http://uq.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://pp.haigaiapp.cn

[S33] C++：vector 增删
来源：http://tn.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ok.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://pv.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://jn.panjiajie.cn

[S35] C++：map
来源：http://tl.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://im.haigaiapp.cn

[S36] C++：unordered_map
来源：http://oc.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wh.shxzukj.cn

[S37] C++：set
来源：http://oz.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ai.shtwfgs.cn

[S38] C++：排序
来源：http://dt.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://nd.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://gp.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rh.huixiangedu.cn

[S40] C++：查找元素
来源：http://se.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://db.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://pn.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aq.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://ah.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://ph.haigaiapp.cn

[S43] C++：智能指针
来源：http://ra.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://fm.shtwfgs.cn

[S44] C++：引用传参
来源：http://vi.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://pb.gzmigu.cn

[S45] C++：lambda
来源：http://ub.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ik.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://ka.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xl.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://qk.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eh.shxzukj.cn

[S48] C++：逐行读文件
来源：http://nv.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ic.newstarts.cn

while (std::getline(in, line)) { }
来源：http://ev.nszjky.cn

[S49] C++：写文件
来源：http://xj.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mi.panjiajie.cn

[S50] C++：格式化数字
来源：http://vu.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pq.huanxung.cn

[S51] C++：显式类型转换
来源：http://fm.panjiajie.cn

static_cast<double>(a) / b
来源：http://ju.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://qy.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://pe.wgjwhj.cn

[S53] C++：移动语义
来源：http://fl.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://zl.shxzukj.cn

[S54] C++：异常处理
来源：http://os.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://th.9csxet.cn

[S55] C++：结构化绑定
来源：http://ge.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mg.huanxung.cn

[S56] C++：optional
来源：http://jx.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mf.shtwfgs.cn

[S57] C++：编译期常量
来源：http://hw.shxzskj.cn

constexpr int N = 10;
来源：http://ck.bookmarksfly.cn

[S58] C++：命名空间
来源：http://rp.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://fu.chemitech.net.cn

[S59] C++：静态断言
来源：http://ck.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wk.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://md.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zj.szsharing.cn

================================================================================
来源：http://wg.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tt.muxihuayi.cn

================================================================================
来源：http://cb.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://zz.panjiajie.cn

println("Hello")
来源：http://ek.shxzukj.cn

[T02] Kotlin：变量
来源：http://ki.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kc.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://fo.asd995.cn

"值: $b"
来源：http://nw.shxzskj.cn

[T04] Kotlin：空安全
来源：http://zc.asd995.cn

val n: String? = null;  n?.length
来源：http://bu.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://cv.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mk.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://gi.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mb.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://ta.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qy.shxzskj.cn

[T08] Kotlin：数据类
来源：http://wa.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://ix.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://pg.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://xw.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://zz.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qi.colortex.cn

[T11] Kotlin：协程
来源：http://be.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://an.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://lt.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://pc.colortex.cn


<!-- 参考信息 -->