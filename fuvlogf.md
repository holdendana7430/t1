代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wl.yuexingan06.cn

[R16] until 等待条件
来源：http://ce.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://te.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://bl.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rp.hnjuh.cn

[R18] 遍历数组
来源：http://oz.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://er.521024.cn

[R19] 数组长度
来源：http://bz.shxzukj.cn

echo "${#arr[@]}"
来源：http://og.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://op.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rq.newstarts.cn

[R21] 字符串长度
来源：http://se.huixiangedu.cn

echo "${#s}"
来源：http://xk.nicolike.cn

[R22] 截取子串
来源：http://wx.shxzskj.cn

echo "${s:0:5}"
来源：http://gv.szxytkj.cn

[R23] 字符串替换
来源：http://bz.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qc.panjiajie.cn

[R24] 大小写转换
来源：http://tk.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ip.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://gk.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rz.huixiangedu.cn

[R26] 命令替换
来源：http://md.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://yi.szsharing.cn

[R27] 算术展开
来源：http://yp.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://qo.chemitech.net.cn

[R28] 浮点运算
来源：http://iw.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://nm.wgjwhj.cn

[R29] 定义函数
来源：http://ke.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://se.asd995.cn

[R30] 函数返回状态码
来源：http://rd.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://fg.nicolike.cn

[R31] 局部变量
来源：http://vz.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://es.szsharing.cn

[R32] 参数个数校验
来源：http://xr.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wf.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://rl.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jt.hnjuh.cn

[R34] 退出时清理
来源：http://xa.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ik.nicolike.cn

[R35] 后台执行并等待
来源：http://is.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cc.huanxung.cn

[R36] 并发执行多个任务
来源：http://xd.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rv.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://ss.bookmarksfly.cn

files=$(ls -1)
来源：http://mc.chemitech.net.cn

[R38] 管道串联
来源：http://od.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://vx.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://fu.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://oo.huixiangedu.cn

[R40] 追加写日志
来源：http://eb.hahajie.cn

echo "log" >> out.log
来源：http://gl.huixiangedu.cn

[R41] 丢弃输出
来源：http://mi.nszjky.cn

cmd >/dev/null 2>&1
来源：http://od.huanxung.cn

[R42] 输入重定向
来源：http://gz.jianghongdianzi.cn

wc -l < a.txt
来源：http://tu.asd995.cn

[R43] 按名字查找文件
来源：http://fu.panjiajie.cn

find . -name "*.log" -type f
来源：http://rz.shxzukj.cn

[R44] 按修改时间查找
来源：http://en.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://vd.panjiajie.cn

[R45] 批量删除
来源：http://at.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://dt.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://yr.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fh.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://xa.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ty.huanxung.cn

[R48] awk 取指定列
来源：http://zh.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://ka.muxihuayi.cn

[R49] awk 带条件
来源：http://so.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rz.wgjwhj.cn

[R50] awk 求和
来源：http://jx.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://po.huanxung.cn

[R51] 排序去重取前几
来源：http://oh.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nh.panjiajie.cn

[R52] 统计行数
来源：http://jh.nszjky.cn

wc -l a.txt
来源：http://ud.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://xt.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ve.bjjhwx.cn

[R54] 比较两个文件
来源：http://sf.shxzukj.cn

diff a.txt b.txt
来源：http://sx.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://bi.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ls.muxihuayi.cn

[R56] 远程拷贝
来源：http://pq.bookmarksfly.cn

scp file user@host:/path/
来源：http://gk.wgjwhj.cn

[R57] 远程执行命令
来源：http://gp.hahajie.cn

ssh user@host 'uptime'
来源：http://ql.szsharing.cn

[R58] 下载文件
来源：http://kz.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wi.jctech888.com.cn

[R59] 发 POST JSON
来源：http://kl.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bl.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://dr.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gu.chemitech.net.cn

[R61] 磁盘占用
来源：http://lv.szxytkj.cn

df -h;  du -sh *
来源：http://vs.panjiajie.cn

[R62] 找最占空间的文件
来源：http://lo.colortex.cn

du -ah . | sort -rh | head -10
来源：http://ly.szxytkj.cn

[R63] 内存与进程
来源：http://ne.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://fk.huanxung.cn

[R64] 结束进程
来源：http://cc.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://un.shtwfgs.cn

[R65] 查看端口占用
来源：http://ws.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pb.shxzukj.cn

[R66] 定时任务
来源：http://bd.nicolike.cn

crontab -e;  crontab -l
来源：http://tr.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://vv.jctech888.com.cn

openssl rand -hex 16
来源：http://xg.nicolike.cn

[R68] 计算文件校验值
来源：http://pk.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cr.shxzukj.cn

[R69] 生成随机密码
来源：http://jt.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://fn.yuexingan06.cn

[R70] 时间戳与互转
来源：http://ne.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://ih.jctech888.com.cn

[R71] 日期格式化
来源：http://um.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ur.nicolike.cn

[R72] 等待端口就绪
来源：http://ar.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://aw.9csxet.cn

[R73] 分割大日志
来源：http://gw.chemitech.net.cn

split -l 1000 big.log part_
来源：http://ck.jianghongdianzi.cn

[R74] 批量重命名
来源：http://kg.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://so.muxihuayi.cn

[R75] 导出环境变量
来源：http://na.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://qy.gzmigu.cn

[R76] 使用临时文件
来源：http://pc.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lh.nszjky.cn

[R77] 读取用户输入
来源：http://um.nszjky.cn

read -rp "请输入: " ans
来源：http://jb.newstarts.cn

[R78] 交互式菜单
来源：http://eh.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jg.wgjwhj.cn

[R79] 解析命令行选项
来源：http://rt.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jv.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://id.szsharing.cn

time ./run.sh
来源：http://kq.huixinmuqiang.cn

================================================================================
来源：http://wn.nszjky.cn

S. C / C++ 专题
来源：http://ck.huixinmuqiang.cn

================================================================================
来源：http://lr.hahajie.cn

[S01] C：Hello World
来源：http://dw.shxzukj.cn

#include <stdio.h>
来源：http://hl.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yw.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://aa.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://ms.jctech888.com.cn

[S03] C：读入整数
来源：http://ai.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://rm.shtwfgs.cn

[S04] C：字符串复制
来源：http://ti.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kh.haigaiapp.cn

[S05] C：字符串长度
来源：http://oq.huanxung.cn

strlen(s)
来源：http://cc.9csxet.cn

[S06] C：字符串比较
来源：http://fj.chemitech.net.cn

strcmp(a, b) == 0
来源：http://zd.colortex.cn

[S07] C：数组遍历求和
来源：http://nc.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pu.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://xw.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gq.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://pb.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://io.asd995.cn

[S10] C：指针与解引用
来源：http://ql.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://sj.huixiangedu.cn

[S11] C：逐行读文件
来源：http://qj.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://vp.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mh.szxytkj.cn

fclose(f);
来源：http://zf.hahajie.cn

[S12] C：写文件
来源：http://hs.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ix.szxytkj.cn

[S13] C：宏定义
来源：http://ay.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yo.hahajie.cn

[S14] C：枚举
来源：http://xq.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://na.huixiangedu.cn

[S15] C：类型转换
来源：http://wg.szsharing.cn

(double) a / b
来源：http://at.szxytkj.cn

[S16] C：位操作置位
来源：http://zq.yuntaijiaju.cn

x |= (1 << 3);
来源：http://ab.szsharing.cn

[S17] C：安全拼接字符串
来源：http://vn.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ku.wgjwhj.cn

[S18] C：命令行参数
来源：http://dp.9csxet.cn

int main(int argc, char **argv)
来源：http://sa.lnxyls.cn

[S19] C：快速排序
来源：http://yu.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pw.asd995.cn

[S20] C：二分查找
来源：http://fr.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ml.colortex.cn

[S21] C：字符类别判断
来源：http://os.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qn.lnxyls.cn

[S22] C：字符串转数字
来源：http://ae.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pf.muxihuayi.cn

[S23] C：随机数
来源：http://ga.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fd.haigaiapp.cn

[S24] C：获取本地时间
来源：http://ab.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eq.nszjky.cn

[S25] C：内存拷贝
来源：http://kv.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://pb.szxytkj.cn

[S26] C：内存清零
来源：http://vi.colortex.cn

memset(a, 0, sizeof a);
来源：http://ra.shxzukj.cn

[S27] C：定义常量
来源：http://ur.szxytkj.cn

const double PI = 3.14159;
来源：http://us.szsharing.cn

[S28] C：静态变量
来源：http://ej.chemitech.net.cn

static int counter = 0;
来源：http://el.hahajie.cn

[S29] C：变参函数
来源：http://yn.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ki.szsharing.cn

[S30] C：头文件保护
来源：http://nz.jianghongdianzi.cn

#ifndef X_H
来源：http://pm.colortex.cn

#define X_H
来源：http://iz.huixiangedu.cn

#endif
来源：http://lg.chemitech.net.cn

[S31] C++：Hello World
来源：http://ly.521024.cn

#include <iostream>
来源：http://gn.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://iq.shxzukj.cn

[S32] C++：字符串
来源：http://zl.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://gf.huixiangedu.cn

[S33] C++：vector 增删
来源：http://xg.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sp.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://mn.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://sg.panjiajie.cn

[S35] C++：map
来源：http://fr.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nm.huanxung.cn

[S36] C++：unordered_map
来源：http://yj.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tn.bookmarksfly.cn

[S37] C++：set
来源：http://hd.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yz.wgjwhj.cn

[S38] C++：排序
来源：http://qx.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://ah.521024.cn

[S39] C++：自定义比较器排序
来源：http://qt.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ka.lnxyls.cn

[S40] C++：查找元素
来源：http://ni.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vn.nszjky.cn

[S41] C++：类与构造函数
来源：http://cm.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mr.newstarts.cn

[S42] C++：继承与虚函数
来源：http://fi.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://by.lnxyls.cn

[S43] C++：智能指针
来源：http://iu.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://zh.nicolike.cn

[S44] C++：引用传参
来源：http://fm.colortex.cn

void inc(int &x) { ++x; }
来源：http://ev.yuexingan06.cn

[S45] C++：lambda
来源：http://wj.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gn.haigaiapp.cn

[S46] C++：函数模板
来源：http://jz.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lv.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://xf.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jt.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://zq.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://js.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://ob.szsharing.cn

[S49] C++：写文件
来源：http://pc.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hn.newstarts.cn

[S50] C++：格式化数字
来源：http://gp.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pi.huanxung.cn

[S51] C++：显式类型转换
来源：http://ec.haigaiapp.cn

static_cast<double>(a) / b
来源：http://dh.521024.cn

[S52] C++：const 与 noexcept
来源：http://ts.asd995.cn

int size() const noexcept { return n_; }
来源：http://qk.yuexingan06.cn

[S53] C++：移动语义
来源：http://vb.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://hq.hahajie.cn

[S54] C++：异常处理
来源：http://zn.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fu.hnjuh.cn

[S55] C++：结构化绑定
来源：http://sr.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gt.wgjwhj.cn

[S56] C++：optional
来源：http://jf.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nj.wgjwhj.cn

[S57] C++：编译期常量
来源：http://uj.colortex.cn

constexpr int N = 10;
来源：http://wl.huanxung.cn

[S58] C++：命名空间
来源：http://jr.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://qa.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://dt.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iw.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://ur.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xp.nszjky.cn

================================================================================
来源：http://qa.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://id.muxihuayi.cn

================================================================================
来源：http://ht.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://ea.jctech888.com.cn

println("Hello")
来源：http://tn.lnxyls.cn

[T02] Kotlin：变量
来源：http://sf.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kz.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://bh.szsharing.cn

"值: $b"
来源：http://yo.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://sv.huanxung.cn

val n: String? = null;  n?.length
来源：http://ix.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://ab.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ua.9csxet.cn

[T06] Kotlin：集合映射
来源：http://bj.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pq.521024.cn

[T07] Kotlin：集合过滤
来源：http://jg.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cd.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://je.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://ib.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://mi.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://sf.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://vo.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ik.gzmigu.cn

[T11] Kotlin：协程
来源：http://ui.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wp.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://pp.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://cc.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://vh.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://vn.nicolike.cn

[T14] Kotlin：循环
来源：http://we.shxzskj.cn

for (i in 1..10) println(i)
来源：http://qe.521024.cn

[T15] Kotlin：接口
来源：http://zr.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://gj.9csxet.cn

[T16] Swift：Hello World
来源：http://yh.newstarts.cn

print("Hello")
来源：http://rq.shxzukj.cn

[T17] Swift：变量与常量
来源：http://nw.hahajie.cn

var a = 1;  let b = 2
来源：http://ie.9csxet.cn

[T18] Swift：字符串插值
来源：http://wb.szsharing.cn

"值: \(b)"
来源：http://cg.hnjuh.cn


<!-- 参考信息 -->