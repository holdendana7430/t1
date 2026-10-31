代发 wailian999

esac
来源：http://zc.szsharing.cn

[R12] for 遍历文件
来源：http://mu.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://jg.bookmarksfly.cn

[R13] for 计数循环
来源：http://db.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://th.jianghongdianzi.cn

[R14] C 风格 for
来源：http://mg.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dg.nicolike.cn

[R15] while 逐行读文件
来源：http://kw.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aj.bookmarksfly.cn

[R16] until 等待条件
来源：http://su.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://se.nicolike.cn

[R17] 数组定义与取值
来源：http://ic.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cg.hahajie.cn

[R18] 遍历数组
来源：http://na.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ot.wgjwhj.cn

[R19] 数组长度
来源：http://di.szsharing.cn

echo "${#arr[@]}"
来源：http://iv.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://ei.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cv.jianghongdianzi.cn

[R21] 字符串长度
来源：http://im.yuntaijiaju.cn

echo "${#s}"
来源：http://je.521024.cn

[R22] 截取子串
来源：http://sx.shtwfgs.cn

echo "${s:0:5}"
来源：http://bk.szxytkj.cn

[R23] 字符串替换
来源：http://ah.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zp.9csxet.cn

[R24] 大小写转换
来源：http://dl.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xd.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://wu.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oi.bjjhwx.cn

[R26] 命令替换
来源：http://bt.colortex.cn

now=$(date +%F); echo "$now"
来源：http://rs.newstarts.cn

[R27] 算术展开
来源：http://nz.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://ps.wgjwhj.cn

[R28] 浮点运算
来源：http://vw.521024.cn

echo "scale=2; 10/3" | bc
来源：http://tp.newstarts.cn

[R29] 定义函数
来源：http://hr.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wu.9csxet.cn

[R30] 函数返回状态码
来源：http://dd.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://rz.9csxet.cn

[R31] 局部变量
来源：http://le.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://gc.wgjwhj.cn

[R32] 参数个数校验
来源：http://le.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eu.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://im.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vu.huixinmuqiang.cn

[R34] 退出时清理
来源：http://mx.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://op.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://ug.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cl.9csxet.cn

[R36] 并发执行多个任务
来源：http://yy.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://re.hnjuh.cn

[R37] 把输出赋给变量
来源：http://lb.muxihuayi.cn

files=$(ls -1)
来源：http://rp.chemitech.net.cn

[R38] 管道串联
来源：http://vt.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://li.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://wu.panjiajie.cn

cmd > out.log 2>&1
来源：http://cg.jianghongdianzi.cn

[R40] 追加写日志
来源：http://kw.jianghongdianzi.cn

echo "log" >> out.log
来源：http://ue.chemitech.net.cn

[R41] 丢弃输出
来源：http://as.nicolike.cn

cmd >/dev/null 2>&1
来源：http://nf.shxzukj.cn

[R42] 输入重定向
来源：http://ow.szsharing.cn

wc -l < a.txt
来源：http://lb.jctech888.com.cn

[R43] 按名字查找文件
来源：http://sd.hnjuh.cn

find . -name "*.log" -type f
来源：http://mg.colortex.cn

[R44] 按修改时间查找
来源：http://fm.asd995.cn

find . -mtime -7 -type f
来源：http://tc.huixiangedu.cn

[R45] 批量删除
来源：http://bf.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://px.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://tn.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cq.9csxet.cn

[R47] sed 单行替换
来源：http://cm.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mb.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://mc.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://io.huixinmuqiang.cn

[R49] awk 带条件
来源：http://rd.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ho.yuntaijiaju.cn

[R50] awk 求和
来源：http://mc.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yr.lnxyls.cn

[R51] 排序去重取前几
来源：http://ow.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bz.shxzukj.cn

[R52] 统计行数
来源：http://mh.shxzskj.cn

wc -l a.txt
来源：http://sq.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://tl.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tc.bookmarksfly.cn

[R54] 比较两个文件
来源：http://es.nszjky.cn

diff a.txt b.txt
来源：http://sb.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://pd.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lp.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://kl.yuexingan06.cn

scp file user@host:/path/
来源：http://qg.hnjuh.cn

[R57] 远程执行命令
来源：http://uu.9csxet.cn

ssh user@host 'uptime'
来源：http://mz.yuexingan06.cn

[R58] 下载文件
来源：http://ih.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://il.colortex.cn

[R59] 发 POST JSON
来源：http://yb.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://il.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://ow.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zb.shxzukj.cn

[R61] 磁盘占用
来源：http://dn.szxytkj.cn

df -h;  du -sh *
来源：http://ql.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://iv.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://pw.shtwfgs.cn

[R63] 内存与进程
来源：http://bh.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://ef.hahajie.cn

[R64] 结束进程
来源：http://vf.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://ok.521024.cn

[R65] 查看端口占用
来源：http://np.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pt.hahajie.cn

[R66] 定时任务
来源：http://ww.huixiangedu.cn

crontab -e;  crontab -l
来源：http://ez.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://iy.nszjky.cn

openssl rand -hex 16
来源：http://lq.colortex.cn

[R68] 计算文件校验值
来源：http://cd.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://du.hahajie.cn

[R69] 生成随机密码
来源：http://de.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://ey.hnjuh.cn

[R70] 时间戳与互转
来源：http://qk.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://py.szsharing.cn

[R71] 日期格式化
来源：http://ve.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://np.shxzukj.cn

[R72] 等待端口就绪
来源：http://hd.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ua.chemitech.net.cn

[R73] 分割大日志
来源：http://tt.yuexingan06.cn

split -l 1000 big.log part_
来源：http://qe.nicolike.cn

[R74] 批量重命名
来源：http://fg.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yb.jianghongdianzi.cn

[R75] 导出环境变量
来源：http://gq.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://qv.jctech888.com.cn

[R76] 使用临时文件
来源：http://pl.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://go.newstarts.cn

[R77] 读取用户输入
来源：http://ej.shtwfgs.cn

read -rp "请输入: " ans
来源：http://pq.shxzukj.cn

[R78] 交互式菜单
来源：http://od.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xg.colortex.cn

[R79] 解析命令行选项
来源：http://qv.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uy.521024.cn

[R80] 查看脚本执行耗时
来源：http://nu.szsharing.cn

time ./run.sh
来源：http://oa.huanxung.cn

================================================================================
来源：http://iq.shxzskj.cn

S. C / C++ 专题
来源：http://oo.gzmigu.cn

================================================================================
来源：http://bo.huanxung.cn

[S01] C：Hello World
来源：http://sk.yuntaijiaju.cn

#include <stdio.h>
来源：http://wj.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bq.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://nu.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://ba.asd995.cn

[S03] C：读入整数
来源：http://ps.szsharing.cn

int x; scanf("%d", &x);
来源：http://gp.asd995.cn

[S04] C：字符串复制
来源：http://dz.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pt.shtwfgs.cn

[S05] C：字符串长度
来源：http://ff.hahajie.cn

strlen(s)
来源：http://et.nicolike.cn

[S06] C：字符串比较
来源：http://my.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://vl.hnjuh.cn

[S07] C：数组遍历求和
来源：http://xo.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://et.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://cc.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bz.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://yz.jianghongdianzi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rv.asd995.cn

[S10] C：指针与解引用
来源：http://os.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://qg.chemitech.net.cn

[S11] C：逐行读文件
来源：http://fu.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://ev.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oq.szxytkj.cn

fclose(f);
来源：http://zb.bookmarksfly.cn

[S12] C：写文件
来源：http://ef.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yr.huixinmuqiang.cn

[S13] C：宏定义
来源：http://ak.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://le.nszjky.cn

[S14] C：枚举
来源：http://cx.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://bw.gzmigu.cn

[S15] C：类型转换
来源：http://hx.shxzskj.cn

(double) a / b
来源：http://qx.bookmarksfly.cn

[S16] C：位操作置位
来源：http://ns.hnjuh.cn

x |= (1 << 3);
来源：http://lg.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://lz.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zq.shtwfgs.cn

[S18] C：命令行参数
来源：http://tk.muxihuayi.cn

int main(int argc, char **argv)
来源：http://bj.shtwfgs.cn

[S19] C：快速排序
来源：http://pl.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vz.asd995.cn

[S20] C：二分查找
来源：http://ls.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cd.nszjky.cn

[S21] C：字符类别判断
来源：http://yi.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lb.shtwfgs.cn

[S22] C：字符串转数字
来源：http://bf.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://da.nicolike.cn

[S23] C：随机数
来源：http://qj.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ib.9csxet.cn

[S24] C：获取本地时间
来源：http://jf.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hj.nszjky.cn

[S25] C：内存拷贝
来源：http://bn.yuexingan06.cn

memcpy(dst, src, n);
来源：http://zx.shxzukj.cn

[S26] C：内存清零
来源：http://jd.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://ps.panjiajie.cn

[S27] C：定义常量
来源：http://bm.wgjwhj.cn

const double PI = 3.14159;
来源：http://wr.jianghongdianzi.cn

[S28] C：静态变量
来源：http://ve.colortex.cn

static int counter = 0;
来源：http://id.panjiajie.cn

[S29] C：变参函数
来源：http://qv.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://db.bookmarksfly.cn

[S30] C：头文件保护
来源：http://nr.yuntaijiaju.cn

#ifndef X_H
来源：http://wu.jctech888.com.cn

#define X_H
来源：http://sg.jianghongdianzi.cn

#endif
来源：http://sq.szxytkj.cn

[S31] C++：Hello World
来源：http://hl.jianghongdianzi.cn

#include <iostream>
来源：http://yd.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://ph.muxihuayi.cn

[S32] C++：字符串
来源：http://rn.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://gm.521024.cn

[S33] C++：vector 增删
来源：http://wh.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rh.nszjky.cn

[S34] C++：遍历 vector
来源：http://uk.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://hs.jianghongdianzi.cn

[S35] C++：map
来源：http://xn.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fz.newstarts.cn

[S36] C++：unordered_map
来源：http://cs.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iz.szsharing.cn

[S37] C++：set
来源：http://ya.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qe.haigaiapp.cn

[S38] C++：排序
来源：http://gt.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://mf.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://zn.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jv.wgjwhj.cn

[S40] C++：查找元素
来源：http://oe.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://me.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://cz.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ag.newstarts.cn

[S42] C++：继承与虚函数
来源：http://gg.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://ab.nszjky.cn

[S43] C++：智能指针
来源：http://hz.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://iq.gzmigu.cn

[S44] C++：引用传参
来源：http://dm.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://ww.szsharing.cn

[S45] C++：lambda
来源：http://mf.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ls.jctech888.com.cn

[S46] C++：函数模板
来源：http://ob.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fq.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://ug.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tc.szsharing.cn

[S48] C++：逐行读文件
来源：http://pe.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gy.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://ft.szsharing.cn

[S49] C++：写文件
来源：http://za.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jh.521024.cn

[S50] C++：格式化数字
来源：http://fe.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xo.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://qn.521024.cn

static_cast<double>(a) / b
来源：http://an.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://sv.huanxung.cn

int size() const noexcept { return n_; }
来源：http://am.hahajie.cn

[S53] C++：移动语义
来源：http://lk.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://md.huixiangedu.cn

[S54] C++：异常处理
来源：http://la.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oc.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://dw.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bi.9csxet.cn

[S56] C++：optional
来源：http://tg.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://va.shxzskj.cn

[S57] C++：编译期常量
来源：http://bi.colortex.cn

constexpr int N = 10;
来源：http://ho.nszjky.cn

[S58] C++：命名空间
来源：http://zq.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://np.shtwfgs.cn

[S59] C++：静态断言
来源：http://nv.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bt.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://uf.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pz.panjiajie.cn

================================================================================
来源：http://rc.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jh.haigaiapp.cn

================================================================================
来源：http://xd.szsharing.cn

[T01] Kotlin：Hello World
来源：http://rz.shtwfgs.cn

println("Hello")
来源：http://kd.521024.cn

[T02] Kotlin：变量
来源：http://dw.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jj.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://gy.jianghongdianzi.cn

"值: $b"
来源：http://au.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://pb.newstarts.cn

val n: String? = null;  n?.length
来源：http://tu.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://kv.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dk.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://cy.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ik.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://we.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lo.nszjky.cn

[T08] Kotlin：数据类
来源：http://fm.521024.cn

data class User(val name: String, val age: Int)
来源：http://kg.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://of.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://kf.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://od.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sj.huanxung.cn

[T11] Kotlin：协程
来源：http://tg.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sk.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://ha.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://cr.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://dz.nicolike.cn

val m = mapOf("a" to 1)
来源：http://mj.szxytkj.cn

[T14] Kotlin：循环
来源：http://xq.newstarts.cn

for (i in 1..10) println(i)
来源：http://wj.colortex.cn


<!-- 参考信息 -->