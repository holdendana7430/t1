代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://gm.jctech888.com.cn

[R14] C 风格 for
来源：http://qc.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vd.haigaiapp.cn

[R15] while 逐行读文件
来源：http://sm.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dj.gzmigu.cn

[R16] until 等待条件
来源：http://kp.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oe.521024.cn

[R17] 数组定义与取值
来源：http://gf.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fm.521024.cn

[R18] 遍历数组
来源：http://qn.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://do.newstarts.cn

[R19] 数组长度
来源：http://tq.521024.cn

echo "${#arr[@]}"
来源：http://qs.newstarts.cn

[R20] 关联数组（字典）
来源：http://vq.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wg.yuexingan06.cn

[R21] 字符串长度
来源：http://yq.gzmigu.cn

echo "${#s}"
来源：http://ry.shtwfgs.cn

[R22] 截取子串
来源：http://je.wgjwhj.cn

echo "${s:0:5}"
来源：http://ow.panjiajie.cn

[R23] 字符串替换
来源：http://ox.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mo.bookmarksfly.cn

[R24] 大小写转换
来源：http://pm.colortex.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xc.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://kd.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dz.shxzskj.cn

[R26] 命令替换
来源：http://tv.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://gj.newstarts.cn

[R27] 算术展开
来源：http://ft.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://nq.panjiajie.cn

[R28] 浮点运算
来源：http://nq.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://ej.newstarts.cn

[R29] 定义函数
来源：http://wu.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fy.gzmigu.cn

[R30] 函数返回状态码
来源：http://uw.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://xa.521024.cn

[R31] 局部变量
来源：http://dl.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://zn.newstarts.cn

[R32] 参数个数校验
来源：http://xc.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qx.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://yq.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wx.521024.cn

[R34] 退出时清理
来源：http://zb.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sd.9csxet.cn

[R35] 后台执行并等待
来源：http://hg.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ew.colortex.cn

[R36] 并发执行多个任务
来源：http://ii.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yp.panjiajie.cn

[R37] 把输出赋给变量
来源：http://ds.yuexingan06.cn

files=$(ls -1)
来源：http://tt.lnxyls.cn

[R38] 管道串联
来源：http://nn.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://cy.colortex.cn

[R39] 重定向标准输出与错误
来源：http://io.haigaiapp.cn

cmd > out.log 2>&1
来源：http://hb.panjiajie.cn

[R40] 追加写日志
来源：http://bm.panjiajie.cn

echo "log" >> out.log
来源：http://ts.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://dy.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://he.haigaiapp.cn

[R42] 输入重定向
来源：http://am.chemitech.net.cn

wc -l < a.txt
来源：http://za.szsharing.cn

[R43] 按名字查找文件
来源：http://hk.shxzskj.cn

find . -name "*.log" -type f
来源：http://pb.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://yo.panjiajie.cn

find . -mtime -7 -type f
来源：http://cf.asd995.cn

[R45] 批量删除
来源：http://ha.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://gh.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://lh.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ow.colortex.cn

[R47] sed 单行替换
来源：http://qj.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hx.chemitech.net.cn

[R48] awk 取指定列
来源：http://fp.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://lb.huanxung.cn

[R49] awk 带条件
来源：http://gl.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ut.bookmarksfly.cn

[R50] awk 求和
来源：http://pe.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qu.521024.cn

[R51] 排序去重取前几
来源：http://sr.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qc.huixiangedu.cn

[R52] 统计行数
来源：http://db.huixinmuqiang.cn

wc -l a.txt
来源：http://dg.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://bh.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qk.521024.cn

[R54] 比较两个文件
来源：http://fr.panjiajie.cn

diff a.txt b.txt
来源：http://tu.muxihuayi.cn

[R55] 压缩与解压
来源：http://jx.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vl.newstarts.cn

[R56] 远程拷贝
来源：http://tg.newstarts.cn

scp file user@host:/path/
来源：http://jt.asd995.cn

[R57] 远程执行命令
来源：http://ks.asd995.cn

ssh user@host 'uptime'
来源：http://zw.panjiajie.cn

[R58] 下载文件
来源：http://di.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ra.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://oc.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gc.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://zy.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://px.shtwfgs.cn

[R61] 磁盘占用
来源：http://hx.haigaiapp.cn

df -h;  du -sh *
来源：http://aw.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://au.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://re.yuexingan06.cn

[R63] 内存与进程
来源：http://el.521024.cn

free -h;  ps aux | grep nginx
来源：http://zw.nicolike.cn

[R64] 结束进程
来源：http://nk.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://dg.asd995.cn

[R65] 查看端口占用
来源：http://ai.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://si.9csxet.cn

[R66] 定时任务
来源：http://fz.521024.cn

crontab -e;  crontab -l
来源：http://bu.521024.cn

[R67] 生成随机十六进制串
来源：http://jm.huanxung.cn

openssl rand -hex 16
来源：http://pl.521024.cn

[R68] 计算文件校验值
来源：http://ee.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ua.bookmarksfly.cn

[R69] 生成随机密码
来源：http://qf.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://zl.newstarts.cn

[R70] 时间戳与互转
来源：http://mo.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://wb.bjjhwx.cn

[R71] 日期格式化
来源：http://ta.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gf.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://fb.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cz.szxytkj.cn

[R73] 分割大日志
来源：http://cw.nicolike.cn

split -l 1000 big.log part_
来源：http://dg.nicolike.cn

[R74] 批量重命名
来源：http://mu.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cu.nicolike.cn

[R75] 导出环境变量
来源：http://kr.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://cf.haigaiapp.cn

[R76] 使用临时文件
来源：http://jt.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kl.yuexingan06.cn

[R77] 读取用户输入
来源：http://gu.521024.cn

read -rp "请输入: " ans
来源：http://ld.shxzskj.cn

[R78] 交互式菜单
来源：http://nf.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xr.jctech888.com.cn

[R79] 解析命令行选项
来源：http://eu.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vt.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://zd.shxzskj.cn

time ./run.sh
来源：http://ca.9csxet.cn

================================================================================
来源：http://ow.shxzskj.cn

S. C / C++ 专题
来源：http://av.wgjwhj.cn

================================================================================
来源：http://ve.wgjwhj.cn

[S01] C：Hello World
来源：http://ct.yuntaijiaju.cn

#include <stdio.h>
来源：http://fc.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ly.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://ii.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://if.9csxet.cn

[S03] C：读入整数
来源：http://hu.huanxung.cn

int x; scanf("%d", &x);
来源：http://km.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://gr.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nh.bookmarksfly.cn

[S05] C：字符串长度
来源：http://uf.newstarts.cn

strlen(s)
来源：http://hp.colortex.cn

[S06] C：字符串比较
来源：http://em.jctech888.com.cn

strcmp(a, b) == 0
来源：http://vh.szxytkj.cn

[S07] C：数组遍历求和
来源：http://la.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vz.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://dm.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nj.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://sq.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zj.haigaiapp.cn

[S10] C：指针与解引用
来源：http://zc.hahajie.cn

int *p = &a;  *p = 5;
来源：http://tk.haigaiapp.cn

[S11] C：逐行读文件
来源：http://lp.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://px.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nk.chemitech.net.cn

fclose(f);
来源：http://dg.huixinmuqiang.cn

[S12] C：写文件
来源：http://fh.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kn.yuntaijiaju.cn

[S13] C：宏定义
来源：http://tc.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bu.newstarts.cn

[S14] C：枚举
来源：http://ta.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://tw.hnjuh.cn

[S15] C：类型转换
来源：http://qy.panjiajie.cn

(double) a / b
来源：http://rm.nicolike.cn

[S16] C：位操作置位
来源：http://so.yuntaijiaju.cn

x |= (1 << 3);
来源：http://af.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://ot.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hi.szxytkj.cn

[S18] C：命令行参数
来源：http://du.szsharing.cn

int main(int argc, char **argv)
来源：http://gc.huanxung.cn

[S19] C：快速排序
来源：http://ja.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xj.yuexingan06.cn

[S20] C：二分查找
来源：http://eh.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oe.chemitech.net.cn

[S21] C：字符类别判断
来源：http://ed.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xk.nicolike.cn

[S22] C：字符串转数字
来源：http://tx.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pz.szxytkj.cn

[S23] C：随机数
来源：http://yn.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://an.lnxyls.cn

[S24] C：获取本地时间
来源：http://sv.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ma.panjiajie.cn

[S25] C：内存拷贝
来源：http://lo.9csxet.cn

memcpy(dst, src, n);
来源：http://cu.chemitech.net.cn

[S26] C：内存清零
来源：http://zx.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://il.bookmarksfly.cn

[S27] C：定义常量
来源：http://rr.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://ql.huanxung.cn

[S28] C：静态变量
来源：http://vq.jctech888.com.cn

static int counter = 0;
来源：http://te.huanxung.cn

[S29] C：变参函数
来源：http://yk.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://om.gzmigu.cn

[S30] C：头文件保护
来源：http://sk.huanxung.cn

#ifndef X_H
来源：http://ex.521024.cn

#define X_H
来源：http://ie.lnxyls.cn

#endif
来源：http://zh.haigaiapp.cn

[S31] C++：Hello World
来源：http://pn.yuntaijiaju.cn

#include <iostream>
来源：http://ve.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://pb.jctech888.com.cn

[S32] C++：字符串
来源：http://cn.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://gc.szsharing.cn

[S33] C++：vector 增删
来源：http://lp.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://of.huanxung.cn

[S34] C++：遍历 vector
来源：http://jp.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://dr.shxzukj.cn

[S35] C++：map
来源：http://zv.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gt.szsharing.cn

[S36] C++：unordered_map
来源：http://pq.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rn.hnjuh.cn

[S37] C++：set
来源：http://fx.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ks.hahajie.cn

[S38] C++：排序
来源：http://yh.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://pf.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://qh.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fq.nszjky.cn

[S40] C++：查找元素
来源：http://rf.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hh.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://oc.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zr.colortex.cn

[S42] C++：继承与虚函数
来源：http://ki.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://gz.panjiajie.cn

[S43] C++：智能指针
来源：http://in.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://pg.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://wj.huanxung.cn

void inc(int &x) { ++x; }
来源：http://fb.huixiangedu.cn

[S45] C++：lambda
来源：http://jh.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rd.9csxet.cn

[S46] C++：函数模板
来源：http://zp.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pt.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://vx.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bv.asd995.cn

[S48] C++：逐行读文件
来源：http://uy.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zt.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://bp.shxzukj.cn

[S49] C++：写文件
来源：http://lc.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jq.newstarts.cn

[S50] C++：格式化数字
来源：http://ax.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uq.huanxung.cn

[S51] C++：显式类型转换
来源：http://jo.lnxyls.cn

static_cast<double>(a) / b
来源：http://rz.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://jd.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://uf.panjiajie.cn

[S53] C++：移动语义
来源：http://jw.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://rf.chemitech.net.cn

[S54] C++：异常处理
来源：http://qy.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pi.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://gn.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pb.nszjky.cn

[S56] C++：optional
来源：http://xq.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ge.panjiajie.cn

[S57] C++：编译期常量
来源：http://vh.shxzukj.cn

constexpr int N = 10;
来源：http://ef.shxzskj.cn

[S58] C++：命名空间
来源：http://re.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://vb.chemitech.net.cn

[S59] C++：静态断言
来源：http://lz.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vq.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://vi.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ny.hnjuh.cn

================================================================================
来源：http://sb.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yw.lnxyls.cn

================================================================================
来源：http://kn.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://cp.huanxung.cn

println("Hello")
来源：http://ct.521024.cn

[T02] Kotlin：变量
来源：http://ot.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ts.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://qk.shtwfgs.cn

"值: $b"
来源：http://sc.colortex.cn

[T04] Kotlin：空安全
来源：http://th.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://nc.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://oq.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://km.colortex.cn

[T06] Kotlin：集合映射
来源：http://im.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ln.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://en.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tk.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://zy.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://ag.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://kh.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://vy.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://wq.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yc.gzmigu.cn

[T11] Kotlin：协程
来源：http://bt.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ab.hahajie.cn

[T12] Kotlin：解构声明
来源：http://au.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://sz.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://aw.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://oh.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://vo.9csxet.cn

for (i in 1..10) println(i)
来源：http://ic.hnjuh.cn

[T15] Kotlin：接口
来源：http://mb.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://qd.yuexingan06.cn

[T16] Swift：Hello World
来源：http://pe.huixiangedu.cn

print("Hello")
来源：http://du.hnjuh.cn


<!-- 参考信息 -->