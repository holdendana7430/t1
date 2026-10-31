代发 wailian999

esac
来源：http://bc.chemitech.net.cn

[R12] for 遍历文件
来源：http://zk.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://iw.bookmarksfly.cn

[R13] for 计数循环
来源：http://ei.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://dt.9csxet.cn

[R14] C 风格 for
来源：http://qq.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ql.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://af.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hb.shxzukj.cn

[R16] until 等待条件
来源：http://nt.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pe.bjjhwx.cn

[R17] 数组定义与取值
来源：http://if.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xm.wgjwhj.cn

[R18] 遍历数组
来源：http://no.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zq.chemitech.net.cn

[R19] 数组长度
来源：http://cd.nicolike.cn

echo "${#arr[@]}"
来源：http://sc.nicolike.cn

[R20] 关联数组（字典）
来源：http://zb.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ik.shtwfgs.cn

[R21] 字符串长度
来源：http://sj.hnjuh.cn

echo "${#s}"
来源：http://ac.yuexingan06.cn

[R22] 截取子串
来源：http://hd.chemitech.net.cn

echo "${s:0:5}"
来源：http://mg.asd995.cn

[R23] 字符串替换
来源：http://qu.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wm.jctech888.com.cn

[R24] 大小写转换
来源：http://re.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ix.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://rp.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rc.chemitech.net.cn

[R26] 命令替换
来源：http://il.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://zu.huixiangedu.cn

[R27] 算术展开
来源：http://jo.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://pu.shxzukj.cn

[R28] 浮点运算
来源：http://ps.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://mh.nicolike.cn

[R29] 定义函数
来源：http://cs.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uy.szsharing.cn

[R30] 函数返回状态码
来源：http://qz.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://xv.shxzskj.cn

[R31] 局部变量
来源：http://jl.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://pq.bookmarksfly.cn

[R32] 参数个数校验
来源：http://mk.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://se.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://oh.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://me.shxzukj.cn

[R34] 退出时清理
来源：http://yy.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qu.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://gn.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://se.9csxet.cn

[R36] 并发执行多个任务
来源：http://ht.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jx.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://tv.newstarts.cn

files=$(ls -1)
来源：http://el.bookmarksfly.cn

[R38] 管道串联
来源：http://pf.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://ua.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://is.jctech888.com.cn

cmd > out.log 2>&1
来源：http://ef.huixinmuqiang.cn

[R40] 追加写日志
来源：http://sv.bjjhwx.cn

echo "log" >> out.log
来源：http://fl.hnjuh.cn

[R41] 丢弃输出
来源：http://xs.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://he.szxytkj.cn

[R42] 输入重定向
来源：http://bc.muxihuayi.cn

wc -l < a.txt
来源：http://wk.shxzskj.cn

[R43] 按名字查找文件
来源：http://vz.9csxet.cn

find . -name "*.log" -type f
来源：http://fe.chemitech.net.cn

[R44] 按修改时间查找
来源：http://rc.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://kw.521024.cn

[R45] 批量删除
来源：http://sb.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://ae.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://pd.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ky.colortex.cn

[R47] sed 单行替换
来源：http://tr.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lo.szxytkj.cn

[R48] awk 取指定列
来源：http://uk.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://mb.newstarts.cn

[R49] awk 带条件
来源：http://xh.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eh.chemitech.net.cn

[R50] awk 求和
来源：http://xn.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kq.jctech888.com.cn

[R51] 排序去重取前几
来源：http://yx.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gn.colortex.cn

[R52] 统计行数
来源：http://wf.hahajie.cn

wc -l a.txt
来源：http://fj.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://tq.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hj.szxytkj.cn

[R54] 比较两个文件
来源：http://co.9csxet.cn

diff a.txt b.txt
来源：http://cm.asd995.cn

[R55] 压缩与解压
来源：http://dw.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pw.nszjky.cn

[R56] 远程拷贝
来源：http://oy.hnjuh.cn

scp file user@host:/path/
来源：http://ri.chemitech.net.cn

[R57] 远程执行命令
来源：http://ta.nicolike.cn

ssh user@host 'uptime'
来源：http://ry.szsharing.cn

[R58] 下载文件
来源：http://ob.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://su.szsharing.cn

[R59] 发 POST JSON
来源：http://sn.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rj.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://zf.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ji.shxzukj.cn

[R61] 磁盘占用
来源：http://yh.asd995.cn

df -h;  du -sh *
来源：http://mx.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://zm.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://mh.huanxung.cn

[R63] 内存与进程
来源：http://wg.521024.cn

free -h;  ps aux | grep nginx
来源：http://cc.wgjwhj.cn

[R64] 结束进程
来源：http://ur.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://dx.hahajie.cn

[R65] 查看端口占用
来源：http://uq.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wl.haigaiapp.cn

[R66] 定时任务
来源：http://nm.wgjwhj.cn

crontab -e;  crontab -l
来源：http://yr.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://mk.hahajie.cn

openssl rand -hex 16
来源：http://zm.chemitech.net.cn

[R68] 计算文件校验值
来源：http://sy.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jc.chemitech.net.cn

[R69] 生成随机密码
来源：http://gx.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://pa.shxzukj.cn

[R70] 时间戳与互转
来源：http://qf.521024.cn

date +%s;  date -d @1700000000
来源：http://ff.hnjuh.cn

[R71] 日期格式化
来源：http://an.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xg.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://mw.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wu.bjjhwx.cn

[R73] 分割大日志
来源：http://xr.chemitech.net.cn

split -l 1000 big.log part_
来源：http://nm.muxihuayi.cn

[R74] 批量重命名
来源：http://ah.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rm.asd995.cn

[R75] 导出环境变量
来源：http://hv.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://xv.huanxung.cn

[R76] 使用临时文件
来源：http://ae.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://du.panjiajie.cn

[R77] 读取用户输入
来源：http://ks.huixiangedu.cn

read -rp "请输入: " ans
来源：http://sq.asd995.cn

[R78] 交互式菜单
来源：http://lc.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://am.huanxung.cn

[R79] 解析命令行选项
来源：http://wj.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ph.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://sd.jianghongdianzi.cn

time ./run.sh
来源：http://ec.newstarts.cn

================================================================================
来源：http://vm.nszjky.cn

S. C / C++ 专题
来源：http://uo.yuexingan06.cn

================================================================================
来源：http://df.yuntaijiaju.cn

[S01] C：Hello World
来源：http://vd.shtwfgs.cn

#include <stdio.h>
来源：http://uh.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zz.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://qc.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://tr.szxytkj.cn

[S03] C：读入整数
来源：http://vz.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://lt.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://yt.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://na.gzmigu.cn

[S05] C：字符串长度
来源：http://jk.muxihuayi.cn

strlen(s)
来源：http://gw.lnxyls.cn

[S06] C：字符串比较
来源：http://tx.newstarts.cn

strcmp(a, b) == 0
来源：http://bo.nicolike.cn

[S07] C：数组遍历求和
来源：http://ux.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fu.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://hk.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://il.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://or.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sr.huanxung.cn

[S10] C：指针与解引用
来源：http://gf.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://fe.hnjuh.cn

[S11] C：逐行读文件
来源：http://nc.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://ob.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oe.huanxung.cn

fclose(f);
来源：http://io.szxytkj.cn

[S12] C：写文件
来源：http://dy.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ge.chemitech.net.cn

[S13] C：宏定义
来源：http://gp.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oa.521024.cn

[S14] C：枚举
来源：http://et.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://sd.newstarts.cn

[S15] C：类型转换
来源：http://xe.shxzukj.cn

(double) a / b
来源：http://sv.nicolike.cn

[S16] C：位操作置位
来源：http://zy.huanxung.cn

x |= (1 << 3);
来源：http://zo.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://hd.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mq.lnxyls.cn

[S18] C：命令行参数
来源：http://vv.colortex.cn

int main(int argc, char **argv)
来源：http://xg.hahajie.cn

[S19] C：快速排序
来源：http://mg.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cd.nicolike.cn

[S20] C：二分查找
来源：http://lg.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nx.chemitech.net.cn

[S21] C：字符类别判断
来源：http://wk.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wv.shtwfgs.cn

[S22] C：字符串转数字
来源：http://ft.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dd.haigaiapp.cn

[S23] C：随机数
来源：http://es.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ww.newstarts.cn

[S24] C：获取本地时间
来源：http://nd.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://co.9csxet.cn

[S25] C：内存拷贝
来源：http://id.yuexingan06.cn

memcpy(dst, src, n);
来源：http://pc.shtwfgs.cn

[S26] C：内存清零
来源：http://ks.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://oe.bookmarksfly.cn

[S27] C：定义常量
来源：http://cl.521024.cn

const double PI = 3.14159;
来源：http://qm.haigaiapp.cn

[S28] C：静态变量
来源：http://ll.nszjky.cn

static int counter = 0;
来源：http://js.shtwfgs.cn

[S29] C：变参函数
来源：http://xa.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pb.wgjwhj.cn

[S30] C：头文件保护
来源：http://yl.shxzskj.cn

#ifndef X_H
来源：http://rl.bookmarksfly.cn

#define X_H
来源：http://wx.chemitech.net.cn

#endif
来源：http://gz.jctech888.com.cn

[S31] C++：Hello World
来源：http://ze.panjiajie.cn

#include <iostream>
来源：http://lc.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://gs.haigaiapp.cn

[S32] C++：字符串
来源：http://ks.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://oa.panjiajie.cn

[S33] C++：vector 增删
来源：http://ju.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mw.szsharing.cn

[S34] C++：遍历 vector
来源：http://il.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://ar.shxzskj.cn

[S35] C++：map
来源：http://yy.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sd.jctech888.com.cn

[S36] C++：unordered_map
来源：http://nv.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gn.bjjhwx.cn

[S37] C++：set
来源：http://mo.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qj.yuexingan06.cn

[S38] C++：排序
来源：http://gv.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://er.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://la.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://og.nszjky.cn

[S40] C++：查找元素
来源：http://vh.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jj.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://lp.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cf.colortex.cn

[S42] C++：继承与虚函数
来源：http://ji.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://tr.shtwfgs.cn

[S43] C++：智能指针
来源：http://kv.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://oy.muxihuayi.cn

[S44] C++：引用传参
来源：http://eh.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://zm.huanxung.cn

[S45] C++：lambda
来源：http://in.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zg.nicolike.cn

[S46] C++：函数模板
来源：http://qp.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://du.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://if.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://px.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://ed.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fe.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://uf.jctech888.com.cn

[S49] C++：写文件
来源：http://yj.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dh.colortex.cn

[S50] C++：格式化数字
来源：http://rq.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lp.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://su.asd995.cn

static_cast<double>(a) / b
来源：http://ue.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://kg.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://cm.chemitech.net.cn

[S53] C++：移动语义
来源：http://db.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://rb.521024.cn

[S54] C++：异常处理
来源：http://yr.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wa.panjiajie.cn

[S55] C++：结构化绑定
来源：http://bm.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xs.panjiajie.cn

[S56] C++：optional
来源：http://ae.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pz.lnxyls.cn

[S57] C++：编译期常量
来源：http://sv.muxihuayi.cn

constexpr int N = 10;
来源：http://ve.szsharing.cn

[S58] C++：命名空间
来源：http://nq.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://hs.szxytkj.cn

[S59] C++：静态断言
来源：http://os.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dl.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://bb.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yl.panjiajie.cn

================================================================================
来源：http://xg.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rv.gzmigu.cn

================================================================================
来源：http://ew.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://lt.nicolike.cn

println("Hello")
来源：http://sg.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://ky.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ki.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://yw.colortex.cn

"值: $b"
来源：http://cz.9csxet.cn

[T04] Kotlin：空安全
来源：http://kv.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://xh.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://tn.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jx.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://dt.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://td.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://ar.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bn.nicolike.cn

[T08] Kotlin：数据类
来源：http://dm.colortex.cn

data class User(val name: String, val age: Int)
来源：http://yy.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://bt.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://hc.521024.cn

[T10] Kotlin：默认参数
来源：http://em.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uj.bjjhwx.cn

[T11] Kotlin：协程
来源：http://cb.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hx.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://jo.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://hn.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://hj.nicolike.cn

val m = mapOf("a" to 1)
来源：http://fk.9csxet.cn

[T14] Kotlin：循环
来源：http://ft.szxytkj.cn

for (i in 1..10) println(i)
来源：http://eo.jianghongdianzi.cn


<!-- 参考信息 -->