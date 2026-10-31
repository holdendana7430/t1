代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://ky.521024.cn

[R14] C 风格 for
来源：http://lb.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ut.haigaiapp.cn

[R15] while 逐行读文件
来源：http://we.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ck.newstarts.cn

[R16] until 等待条件
来源：http://kd.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://es.521024.cn

[R17] 数组定义与取值
来源：http://ez.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bq.haigaiapp.cn

[R18] 遍历数组
来源：http://vh.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://no.haigaiapp.cn

[R19] 数组长度
来源：http://cl.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://wq.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://eb.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zt.shtwfgs.cn

[R21] 字符串长度
来源：http://xw.newstarts.cn

echo "${#s}"
来源：http://fa.panjiajie.cn

[R22] 截取子串
来源：http://tb.huixiangedu.cn

echo "${s:0:5}"
来源：http://tp.huixiangedu.cn

[R23] 字符串替换
来源：http://ul.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tv.colortex.cn

[R24] 大小写转换
来源：http://ky.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yb.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://qk.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://km.haigaiapp.cn

[R26] 命令替换
来源：http://lg.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://hc.jianghongdianzi.cn

[R27] 算术展开
来源：http://ty.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://bd.haigaiapp.cn

[R28] 浮点运算
来源：http://du.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://wg.szxytkj.cn

[R29] 定义函数
来源：http://gr.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://om.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://ox.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://yu.jctech888.com.cn

[R31] 局部变量
来源：http://gy.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://ls.huanxung.cn

[R32] 参数个数校验
来源：http://du.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yh.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://wc.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://do.newstarts.cn

[R34] 退出时清理
来源：http://cw.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zj.wgjwhj.cn

[R35] 后台执行并等待
来源：http://mf.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yy.9csxet.cn

[R36] 并发执行多个任务
来源：http://yt.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://og.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://hg.nszjky.cn

files=$(ls -1)
来源：http://ll.jianghongdianzi.cn

[R38] 管道串联
来源：http://vo.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://ux.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://wl.huanxung.cn

cmd > out.log 2>&1
来源：http://fs.hnjuh.cn

[R40] 追加写日志
来源：http://tf.jianghongdianzi.cn

echo "log" >> out.log
来源：http://dc.nicolike.cn

[R41] 丢弃输出
来源：http://mt.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://qj.szsharing.cn

[R42] 输入重定向
来源：http://uw.huanxung.cn

wc -l < a.txt
来源：http://qx.newstarts.cn

[R43] 按名字查找文件
来源：http://td.wgjwhj.cn

find . -name "*.log" -type f
来源：http://ew.shtwfgs.cn

[R44] 按修改时间查找
来源：http://qs.chemitech.net.cn

find . -mtime -7 -type f
来源：http://fk.jianghongdianzi.cn

[R45] 批量删除
来源：http://hx.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://qb.hnjuh.cn

[R46] 递归替换文件内容
来源：http://iq.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://on.jctech888.com.cn

[R47] sed 单行替换
来源：http://ab.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kc.muxihuayi.cn

[R48] awk 取指定列
来源：http://xc.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://jy.bookmarksfly.cn

[R49] awk 带条件
来源：http://bd.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://we.muxihuayi.cn

[R50] awk 求和
来源：http://ld.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://px.hahajie.cn

[R51] 排序去重取前几
来源：http://ad.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wx.huixinmuqiang.cn

[R52] 统计行数
来源：http://gy.shxzskj.cn

wc -l a.txt
来源：http://dc.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://tr.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ko.newstarts.cn

[R54] 比较两个文件
来源：http://yx.huanxung.cn

diff a.txt b.txt
来源：http://vu.huanxung.cn

[R55] 压缩与解压
来源：http://ax.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zl.nicolike.cn

[R56] 远程拷贝
来源：http://rq.panjiajie.cn

scp file user@host:/path/
来源：http://wk.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://yz.nicolike.cn

ssh user@host 'uptime'
来源：http://wv.wgjwhj.cn

[R58] 下载文件
来源：http://tr.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ai.huixiangedu.cn

[R59] 发 POST JSON
来源：http://zi.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kb.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://ga.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cm.hahajie.cn

[R61] 磁盘占用
来源：http://xi.lnxyls.cn

df -h;  du -sh *
来源：http://ul.huanxung.cn

[R62] 找最占空间的文件
来源：http://aq.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://vg.szxytkj.cn

[R63] 内存与进程
来源：http://gw.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://tn.newstarts.cn

[R64] 结束进程
来源：http://px.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://ap.shxzukj.cn

[R65] 查看端口占用
来源：http://zh.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://af.newstarts.cn

[R66] 定时任务
来源：http://im.szsharing.cn

crontab -e;  crontab -l
来源：http://zg.szsharing.cn

[R67] 生成随机十六进制串
来源：http://dd.9csxet.cn

openssl rand -hex 16
来源：http://kv.newstarts.cn

[R68] 计算文件校验值
来源：http://cw.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://df.panjiajie.cn

[R69] 生成随机密码
来源：http://zi.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://jk.shtwfgs.cn

[R70] 时间戳与互转
来源：http://iu.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://wh.yuntaijiaju.cn

[R71] 日期格式化
来源：http://af.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bt.hnjuh.cn

[R72] 等待端口就绪
来源：http://ju.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xq.jianghongdianzi.cn

[R73] 分割大日志
来源：http://zm.panjiajie.cn

split -l 1000 big.log part_
来源：http://od.huixiangedu.cn

[R74] 批量重命名
来源：http://un.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wo.nszjky.cn

[R75] 导出环境变量
来源：http://sr.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://yb.muxihuayi.cn

[R76] 使用临时文件
来源：http://if.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vz.wgjwhj.cn

[R77] 读取用户输入
来源：http://kf.haigaiapp.cn

read -rp "请输入: " ans
来源：http://zk.szxytkj.cn

[R78] 交互式菜单
来源：http://wd.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xc.shxzskj.cn

[R79] 解析命令行选项
来源：http://rn.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ik.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://uk.lnxyls.cn

time ./run.sh
来源：http://sz.bookmarksfly.cn

================================================================================
来源：http://iw.bjjhwx.cn

S. C / C++ 专题
来源：http://di.szsharing.cn

================================================================================
来源：http://fc.lnxyls.cn

[S01] C：Hello World
来源：http://ki.panjiajie.cn

#include <stdio.h>
来源：http://gj.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gv.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://hp.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://cw.szsharing.cn

[S03] C：读入整数
来源：http://bl.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://nn.521024.cn

[S04] C：字符串复制
来源：http://pz.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ol.huixiangedu.cn

[S05] C：字符串长度
来源：http://ud.haigaiapp.cn

strlen(s)
来源：http://cu.lnxyls.cn

[S06] C：字符串比较
来源：http://tq.shtwfgs.cn

strcmp(a, b) == 0
来源：http://zs.newstarts.cn

[S07] C：数组遍历求和
来源：http://kt.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sy.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://vu.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fw.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://ja.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ea.nicolike.cn

[S10] C：指针与解引用
来源：http://ig.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://ig.hnjuh.cn

[S11] C：逐行读文件
来源：http://dx.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://fy.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bc.szsharing.cn

fclose(f);
来源：http://ls.hnjuh.cn

[S12] C：写文件
来源：http://jc.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://re.bjjhwx.cn

[S13] C：宏定义
来源：http://bk.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ck.huixiangedu.cn

[S14] C：枚举
来源：http://rl.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://pm.szsharing.cn

[S15] C：类型转换
来源：http://jb.szsharing.cn

(double) a / b
来源：http://pg.jctech888.com.cn

[S16] C：位操作置位
来源：http://sa.9csxet.cn

x |= (1 << 3);
来源：http://ql.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://ec.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mu.panjiajie.cn

[S18] C：命令行参数
来源：http://kk.szsharing.cn

int main(int argc, char **argv)
来源：http://iw.gzmigu.cn

[S19] C：快速排序
来源：http://kf.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rw.hnjuh.cn

[S20] C：二分查找
来源：http://br.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qi.jctech888.com.cn

[S21] C：字符类别判断
来源：http://fj.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fn.9csxet.cn

[S22] C：字符串转数字
来源：http://sd.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tt.huixiangedu.cn

[S23] C：随机数
来源：http://id.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lz.gzmigu.cn

[S24] C：获取本地时间
来源：http://nw.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ty.szxytkj.cn

[S25] C：内存拷贝
来源：http://ld.bjjhwx.cn

memcpy(dst, src, n);
来源：http://pf.gzmigu.cn

[S26] C：内存清零
来源：http://tb.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://pj.newstarts.cn

[S27] C：定义常量
来源：http://qq.szxytkj.cn

const double PI = 3.14159;
来源：http://fg.colortex.cn

[S28] C：静态变量
来源：http://fu.jianghongdianzi.cn

static int counter = 0;
来源：http://bc.nicolike.cn

[S29] C：变参函数
来源：http://cd.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vm.shtwfgs.cn

[S30] C：头文件保护
来源：http://up.asd995.cn

#ifndef X_H
来源：http://lb.yuexingan06.cn

#define X_H
来源：http://ao.szxytkj.cn

#endif
来源：http://rk.nicolike.cn

[S31] C++：Hello World
来源：http://ag.hahajie.cn

#include <iostream>
来源：http://fa.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://fd.wgjwhj.cn

[S32] C++：字符串
来源：http://br.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://zl.hnjuh.cn

[S33] C++：vector 增删
来源：http://ri.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cb.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://zc.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://re.jianghongdianzi.cn

[S35] C++：map
来源：http://lv.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gq.9csxet.cn

[S36] C++：unordered_map
来源：http://iq.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://be.lnxyls.cn

[S37] C++：set
来源：http://se.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zc.newstarts.cn

[S38] C++：排序
来源：http://dy.521024.cn

std::sort(v.begin(), v.end());
来源：http://uo.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://hz.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://px.szsharing.cn

[S40] C++：查找元素
来源：http://gb.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jb.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://ys.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nh.colortex.cn

[S42] C++：继承与虚函数
来源：http://io.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://rx.huanxung.cn

[S43] C++：智能指针
来源：http://gj.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://zc.9csxet.cn

[S44] C++：引用传参
来源：http://bg.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://tk.huanxung.cn

[S45] C++：lambda
来源：http://sz.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wi.gzmigu.cn

[S46] C++：函数模板
来源：http://vd.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://te.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://kb.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cx.nszjky.cn

[S48] C++：逐行读文件
来源：http://ch.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nw.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://fb.bjjhwx.cn

[S49] C++：写文件
来源：http://da.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vp.chemitech.net.cn

[S50] C++：格式化数字
来源：http://vd.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eo.huanxung.cn

[S51] C++：显式类型转换
来源：http://fe.521024.cn

static_cast<double>(a) / b
来源：http://mm.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://hu.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://ge.szsharing.cn

[S53] C++：移动语义
来源：http://ju.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://ev.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://yi.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aj.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://rh.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ko.lnxyls.cn

[S56] C++：optional
来源：http://mq.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://md.huixiangedu.cn

[S57] C++：编译期常量
来源：http://qh.huanxung.cn

constexpr int N = 10;
来源：http://nq.asd995.cn

[S58] C++：命名空间
来源：http://tl.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://vr.panjiajie.cn

[S59] C++：静态断言
来源：http://lz.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mm.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://ci.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tt.shtwfgs.cn

================================================================================
来源：http://vo.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ck.521024.cn

================================================================================
来源：http://ob.nicolike.cn

[T01] Kotlin：Hello World
来源：http://id.haigaiapp.cn

println("Hello")
来源：http://lr.yuexingan06.cn

[T02] Kotlin：变量
来源：http://ci.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tv.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://wv.muxihuayi.cn

"值: $b"
来源：http://tl.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://gj.521024.cn

val n: String? = null;  n?.length
来源：http://wc.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://ip.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://as.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://nb.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pz.colortex.cn

[T07] Kotlin：集合过滤
来源：http://lf.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sq.9csxet.cn

[T08] Kotlin：数据类
来源：http://db.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://dq.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://gs.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://rl.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://rj.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vx.shxzukj.cn

[T11] Kotlin：协程
来源：http://lw.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uz.asd995.cn

[T12] Kotlin：解构声明
来源：http://ep.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://ir.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://xn.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://gn.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://eu.huanxung.cn

for (i in 1..10) println(i)
来源：http://kf.jctech888.com.cn

[T15] Kotlin：接口
来源：http://jz.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://zb.huixiangedu.cn

[T16] Swift：Hello World
来源：http://br.jianghongdianzi.cn

print("Hello")
来源：http://ly.panjiajie.cn


<!-- 参考信息 -->