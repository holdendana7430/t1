代发 wailian999

esac
来源：http://ku.asd995.cn

[R12] for 遍历文件
来源：http://lu.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://mm.szxytkj.cn

[R13] for 计数循环
来源：http://mw.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://qq.newstarts.cn

[R14] C 风格 for
来源：http://io.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ht.szxytkj.cn

[R15] while 逐行读文件
来源：http://jg.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dz.hnjuh.cn

[R16] until 等待条件
来源：http://yp.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mk.gzmigu.cn

[R17] 数组定义与取值
来源：http://tq.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://le.muxihuayi.cn

[R18] 遍历数组
来源：http://wc.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zk.colortex.cn

[R19] 数组长度
来源：http://bt.newstarts.cn

echo "${#arr[@]}"
来源：http://gb.newstarts.cn

[R20] 关联数组（字典）
来源：http://dp.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vx.shtwfgs.cn

[R21] 字符串长度
来源：http://kz.shtwfgs.cn

echo "${#s}"
来源：http://um.bookmarksfly.cn

[R22] 截取子串
来源：http://hy.panjiajie.cn

echo "${s:0:5}"
来源：http://nf.hahajie.cn

[R23] 字符串替换
来源：http://nb.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gm.shtwfgs.cn

[R24] 大小写转换
来源：http://or.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://io.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://df.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://om.asd995.cn

[R26] 命令替换
来源：http://mx.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://qj.jctech888.com.cn

[R27] 算术展开
来源：http://gq.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://nv.huanxung.cn

[R28] 浮点运算
来源：http://vu.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://uk.521024.cn

[R29] 定义函数
来源：http://ux.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vj.szsharing.cn

[R30] 函数返回状态码
来源：http://gd.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://ag.huixiangedu.cn

[R31] 局部变量
来源：http://fc.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://lv.colortex.cn

[R32] 参数个数校验
来源：http://ru.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pa.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://jh.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://er.hahajie.cn

[R34] 退出时清理
来源：http://sf.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ul.bjjhwx.cn

[R35] 后台执行并等待
来源：http://mi.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qz.9csxet.cn

[R36] 并发执行多个任务
来源：http://dj.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rl.hnjuh.cn

[R37] 把输出赋给变量
来源：http://pn.yuexingan06.cn

files=$(ls -1)
来源：http://wn.muxihuayi.cn

[R38] 管道串联
来源：http://km.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://vi.asd995.cn

[R39] 重定向标准输出与错误
来源：http://uv.9csxet.cn

cmd > out.log 2>&1
来源：http://es.newstarts.cn

[R40] 追加写日志
来源：http://rw.yuntaijiaju.cn

echo "log" >> out.log
来源：http://wp.huixiangedu.cn

[R41] 丢弃输出
来源：http://tr.szsharing.cn

cmd >/dev/null 2>&1
来源：http://ao.shxzukj.cn

[R42] 输入重定向
来源：http://ek.bookmarksfly.cn

wc -l < a.txt
来源：http://ot.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://rd.gzmigu.cn

find . -name "*.log" -type f
来源：http://rm.shxzukj.cn

[R44] 按修改时间查找
来源：http://mm.panjiajie.cn

find . -mtime -7 -type f
来源：http://ec.chemitech.net.cn

[R45] 批量删除
来源：http://bu.huanxung.cn

find . -name "*.tmp" -delete
来源：http://qg.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://ev.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://up.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://wf.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://by.lnxyls.cn

[R48] awk 取指定列
来源：http://kr.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://is.jianghongdianzi.cn

[R49] awk 带条件
来源：http://dz.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yr.shxzskj.cn

[R50] awk 求和
来源：http://he.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fm.shtwfgs.cn

[R51] 排序去重取前几
来源：http://wy.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vf.jianghongdianzi.cn

[R52] 统计行数
来源：http://tt.9csxet.cn

wc -l a.txt
来源：http://qu.colortex.cn

[R53] 查看文件头与实时尾
来源：http://rm.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sp.colortex.cn

[R54] 比较两个文件
来源：http://ep.jianghongdianzi.cn

diff a.txt b.txt
来源：http://as.newstarts.cn

[R55] 压缩与解压
来源：http://fx.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ac.hahajie.cn

[R56] 远程拷贝
来源：http://ov.hnjuh.cn

scp file user@host:/path/
来源：http://no.yuexingan06.cn

[R57] 远程执行命令
来源：http://vn.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://gp.haigaiapp.cn

[R58] 下载文件
来源：http://bl.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zj.panjiajie.cn

[R59] 发 POST JSON
来源：http://km.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qe.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://gs.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oa.bookmarksfly.cn

[R61] 磁盘占用
来源：http://wu.jianghongdianzi.cn

df -h;  du -sh *
来源：http://cd.newstarts.cn

[R62] 找最占空间的文件
来源：http://kc.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://ex.panjiajie.cn

[R63] 内存与进程
来源：http://tj.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://xi.huanxung.cn

[R64] 结束进程
来源：http://qm.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://ce.yuexingan06.cn

[R65] 查看端口占用
来源：http://id.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ap.asd995.cn

[R66] 定时任务
来源：http://ia.asd995.cn

crontab -e;  crontab -l
来源：http://bf.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://ue.9csxet.cn

openssl rand -hex 16
来源：http://eo.szxytkj.cn

[R68] 计算文件校验值
来源：http://dn.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hl.nicolike.cn

[R69] 生成随机密码
来源：http://ly.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://gj.yuexingan06.cn

[R70] 时间戳与互转
来源：http://zw.nicolike.cn

date +%s;  date -d @1700000000
来源：http://io.haigaiapp.cn

[R71] 日期格式化
来源：http://ni.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dy.huixiangedu.cn

[R72] 等待端口就绪
来源：http://so.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://es.szxytkj.cn

[R73] 分割大日志
来源：http://rf.9csxet.cn

split -l 1000 big.log part_
来源：http://uz.newstarts.cn

[R74] 批量重命名
来源：http://js.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hi.nszjky.cn

[R75] 导出环境变量
来源：http://rf.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ip.nszjky.cn

[R76] 使用临时文件
来源：http://tz.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ks.shxzukj.cn

[R77] 读取用户输入
来源：http://nm.shtwfgs.cn

read -rp "请输入: " ans
来源：http://au.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://pf.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bb.colortex.cn

[R79] 解析命令行选项
来源：http://lp.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mt.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://dt.nicolike.cn

time ./run.sh
来源：http://cf.shtwfgs.cn

================================================================================
来源：http://qf.shxzskj.cn

S. C / C++ 专题
来源：http://ue.shxzskj.cn

================================================================================
来源：http://hy.jianghongdianzi.cn

[S01] C：Hello World
来源：http://rn.shtwfgs.cn

#include <stdio.h>
来源：http://xe.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kv.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://nh.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://yn.bjjhwx.cn

[S03] C：读入整数
来源：http://ks.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://wn.szsharing.cn

[S04] C：字符串复制
来源：http://hk.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cq.chemitech.net.cn

[S05] C：字符串长度
来源：http://hk.asd995.cn

strlen(s)
来源：http://qj.nszjky.cn

[S06] C：字符串比较
来源：http://pw.shtwfgs.cn

strcmp(a, b) == 0
来源：http://re.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://uk.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fh.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://qk.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qp.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://lz.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ed.huixiangedu.cn

[S10] C：指针与解引用
来源：http://fq.nicolike.cn

int *p = &a;  *p = 5;
来源：http://gu.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://vj.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://xs.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bq.bookmarksfly.cn

fclose(f);
来源：http://er.szxytkj.cn

[S12] C：写文件
来源：http://mb.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kc.haigaiapp.cn

[S13] C：宏定义
来源：http://kk.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rp.wgjwhj.cn

[S14] C：枚举
来源：http://lb.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://wk.newstarts.cn

[S15] C：类型转换
来源：http://nk.newstarts.cn

(double) a / b
来源：http://bo.szxytkj.cn

[S16] C：位操作置位
来源：http://sh.muxihuayi.cn

x |= (1 << 3);
来源：http://il.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://et.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bj.haigaiapp.cn

[S18] C：命令行参数
来源：http://vx.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://sd.gzmigu.cn

[S19] C：快速排序
来源：http://wx.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wc.haigaiapp.cn

[S20] C：二分查找
来源：http://aw.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dl.yuexingan06.cn

[S21] C：字符类别判断
来源：http://hf.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ui.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://uj.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jk.nicolike.cn

[S23] C：随机数
来源：http://yc.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ud.nicolike.cn

[S24] C：获取本地时间
来源：http://od.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ei.chemitech.net.cn

[S25] C：内存拷贝
来源：http://in.521024.cn

memcpy(dst, src, n);
来源：http://gg.asd995.cn

[S26] C：内存清零
来源：http://pp.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://gg.bookmarksfly.cn

[S27] C：定义常量
来源：http://kx.nszjky.cn

const double PI = 3.14159;
来源：http://xc.szxytkj.cn

[S28] C：静态变量
来源：http://gm.shxzskj.cn

static int counter = 0;
来源：http://jb.chemitech.net.cn

[S29] C：变参函数
来源：http://ya.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fi.panjiajie.cn

[S30] C：头文件保护
来源：http://wd.chemitech.net.cn

#ifndef X_H
来源：http://fz.lnxyls.cn

#define X_H
来源：http://xw.huanxung.cn

#endif
来源：http://he.szxytkj.cn

[S31] C++：Hello World
来源：http://xt.haigaiapp.cn

#include <iostream>
来源：http://ss.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://ov.gzmigu.cn

[S32] C++：字符串
来源：http://sq.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://je.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://mr.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ep.huanxung.cn

[S34] C++：遍历 vector
来源：http://yr.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://hu.yuexingan06.cn

[S35] C++：map
来源：http://kg.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sp.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://ak.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rn.shxzskj.cn

[S37] C++：set
来源：http://en.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ac.hahajie.cn

[S38] C++：排序
来源：http://we.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://xw.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://ga.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ki.bookmarksfly.cn

[S40] C++：查找元素
来源：http://up.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gz.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://rq.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ea.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://ip.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://fw.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://rp.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://ah.wgjwhj.cn

[S44] C++：引用传参
来源：http://ig.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://bx.panjiajie.cn

[S45] C++：lambda
来源：http://ct.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://up.colortex.cn

[S46] C++：函数模板
来源：http://bd.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nz.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://by.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lk.521024.cn

[S48] C++：逐行读文件
来源：http://er.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uy.9csxet.cn

while (std::getline(in, line)) { }
来源：http://sz.shtwfgs.cn

[S49] C++：写文件
来源：http://qo.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://us.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://tv.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sw.shxzskj.cn

[S51] C++：显式类型转换
来源：http://rl.asd995.cn

static_cast<double>(a) / b
来源：http://gx.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://uz.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://pl.bookmarksfly.cn

[S53] C++：移动语义
来源：http://qc.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://xk.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://pf.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ir.hahajie.cn

[S55] C++：结构化绑定
来源：http://ug.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ba.colortex.cn

[S56] C++：optional
来源：http://uf.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ux.hnjuh.cn

[S57] C++：编译期常量
来源：http://rf.huixinmuqiang.cn

constexpr int N = 10;
来源：http://sr.shxzskj.cn

[S58] C++：命名空间
来源：http://hy.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://im.hahajie.cn

[S59] C++：静态断言
来源：http://qb.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ob.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://kq.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lp.newstarts.cn

================================================================================
来源：http://nz.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://in.szxytkj.cn

================================================================================
来源：http://gc.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://xn.hnjuh.cn

println("Hello")
来源：http://nx.panjiajie.cn

[T02] Kotlin：变量
来源：http://la.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uj.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://st.nicolike.cn

"值: $b"
来源：http://ru.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://fe.asd995.cn

val n: String? = null;  n?.length
来源：http://jk.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://zp.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qp.colortex.cn

[T06] Kotlin：集合映射
来源：http://yl.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://su.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://fp.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kb.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://nn.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://xz.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://to.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://oz.newstarts.cn

[T10] Kotlin：默认参数
来源：http://es.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xa.jctech888.com.cn

[T11] Kotlin：协程
来源：http://ck.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://op.hahajie.cn

[T12] Kotlin：解构声明
来源：http://by.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://bn.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://mr.521024.cn

val m = mapOf("a" to 1)
来源：http://et.shxzukj.cn

[T14] Kotlin：循环
来源：http://aa.huanxung.cn

for (i in 1..10) println(i)
来源：http://as.hahajie.cn


<!-- 参考信息 -->