代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kc.newstarts.cn

[R08] 数值比较
来源：http://ud.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fo.bookmarksfly.cn

[R09] 字符串比较
来源：http://mf.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tj.huixinmuqiang.cn

[R10] 正则匹配
来源：http://cq.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pp.shtwfgs.cn

[R11] case 多分支
来源：http://wy.shtwfgs.cn

case "$1" in
来源：http://bw.newstarts.cn

start) echo "启动" ;;
来源：http://ce.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://am.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://vt.hnjuh.cn

esac
来源：http://ct.colortex.cn

[R12] for 遍历文件
来源：http://jc.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://fg.9csxet.cn

[R13] for 计数循环
来源：http://qk.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://dv.chemitech.net.cn

[R14] C 风格 for
来源：http://fv.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ma.chemitech.net.cn

[R15] while 逐行读文件
来源：http://kf.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lz.hnjuh.cn

[R16] until 等待条件
来源：http://yi.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ym.huanxung.cn

[R17] 数组定义与取值
来源：http://cu.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hs.szsharing.cn

[R18] 遍历数组
来源：http://oa.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zg.huixinmuqiang.cn

[R19] 数组长度
来源：http://cw.colortex.cn

echo "${#arr[@]}"
来源：http://sg.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://kj.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zl.jianghongdianzi.cn

[R21] 字符串长度
来源：http://yw.colortex.cn

echo "${#s}"
来源：http://jl.newstarts.cn

[R22] 截取子串
来源：http://vp.lnxyls.cn

echo "${s:0:5}"
来源：http://bi.colortex.cn

[R23] 字符串替换
来源：http://hh.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://et.asd995.cn

[R24] 大小写转换
来源：http://rn.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cw.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://vg.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wy.hahajie.cn

[R26] 命令替换
来源：http://bo.521024.cn

now=$(date +%F); echo "$now"
来源：http://pw.szsharing.cn

[R27] 算术展开
来源：http://la.colortex.cn

echo $((1 + 2 * 3))
来源：http://ns.szsharing.cn

[R28] 浮点运算
来源：http://yi.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://ok.shxzskj.cn

[R29] 定义函数
来源：http://vl.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rj.newstarts.cn

[R30] 函数返回状态码
来源：http://zf.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://xl.colortex.cn

[R31] 局部变量
来源：http://hu.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://hu.hnjuh.cn

[R32] 参数个数校验
来源：http://zi.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jy.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://by.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bp.hnjuh.cn

[R34] 退出时清理
来源：http://hh.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uw.521024.cn

[R35] 后台执行并等待
来源：http://kl.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ba.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://yo.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yo.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://sm.haigaiapp.cn

files=$(ls -1)
来源：http://ka.muxihuayi.cn

[R38] 管道串联
来源：http://au.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://ns.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://jh.gzmigu.cn

cmd > out.log 2>&1
来源：http://kv.shtwfgs.cn

[R40] 追加写日志
来源：http://yz.yuntaijiaju.cn

echo "log" >> out.log
来源：http://xz.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://iu.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://ia.9csxet.cn

[R42] 输入重定向
来源：http://ee.huixiangedu.cn

wc -l < a.txt
来源：http://vi.shtwfgs.cn

[R43] 按名字查找文件
来源：http://oh.szxytkj.cn

find . -name "*.log" -type f
来源：http://gr.newstarts.cn

[R44] 按修改时间查找
来源：http://sz.shtwfgs.cn

find . -mtime -7 -type f
来源：http://fi.muxihuayi.cn

[R45] 批量删除
来源：http://ee.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://yy.panjiajie.cn

[R46] 递归替换文件内容
来源：http://pg.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wf.shxzukj.cn

[R47] sed 单行替换
来源：http://lb.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ny.asd995.cn

[R48] awk 取指定列
来源：http://ei.521024.cn

awk '{print $1, $3}' a.txt
来源：http://by.hahajie.cn

[R49] awk 带条件
来源：http://ak.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ya.521024.cn

[R50] awk 求和
来源：http://zp.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ni.panjiajie.cn

[R51] 排序去重取前几
来源：http://hc.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ro.hnjuh.cn

[R52] 统计行数
来源：http://mm.hnjuh.cn

wc -l a.txt
来源：http://vo.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://ip.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hp.nicolike.cn

[R54] 比较两个文件
来源：http://ai.colortex.cn

diff a.txt b.txt
来源：http://mf.muxihuayi.cn

[R55] 压缩与解压
来源：http://ts.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lk.haigaiapp.cn

[R56] 远程拷贝
来源：http://qh.huixiangedu.cn

scp file user@host:/path/
来源：http://re.huanxung.cn

[R57] 远程执行命令
来源：http://fv.asd995.cn

ssh user@host 'uptime'
来源：http://st.jianghongdianzi.cn

[R58] 下载文件
来源：http://wp.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bi.hahajie.cn

[R59] 发 POST JSON
来源：http://sx.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ah.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://tr.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tp.shxzukj.cn

[R61] 磁盘占用
来源：http://pp.521024.cn

df -h;  du -sh *
来源：http://ek.colortex.cn

[R62] 找最占空间的文件
来源：http://lh.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://kp.yuntaijiaju.cn

[R63] 内存与进程
来源：http://yc.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://lr.gzmigu.cn

[R64] 结束进程
来源：http://by.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://en.shtwfgs.cn

[R65] 查看端口占用
来源：http://ji.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tl.haigaiapp.cn

[R66] 定时任务
来源：http://sg.haigaiapp.cn

crontab -e;  crontab -l
来源：http://aj.huanxung.cn

[R67] 生成随机十六进制串
来源：http://yp.shxzukj.cn

openssl rand -hex 16
来源：http://jf.szsharing.cn

[R68] 计算文件校验值
来源：http://ps.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kf.shxzukj.cn

[R69] 生成随机密码
来源：http://ms.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://yx.bjjhwx.cn

[R70] 时间戳与互转
来源：http://gf.nszjky.cn

date +%s;  date -d @1700000000
来源：http://li.521024.cn

[R71] 日期格式化
来源：http://oi.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://av.gzmigu.cn

[R72] 等待端口就绪
来源：http://oj.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cn.521024.cn

[R73] 分割大日志
来源：http://ob.9csxet.cn

split -l 1000 big.log part_
来源：http://xa.yuexingan06.cn

[R74] 批量重命名
来源：http://tu.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ix.9csxet.cn

[R75] 导出环境变量
来源：http://gy.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://mf.shxzskj.cn

[R76] 使用临时文件
来源：http://dy.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pj.szsharing.cn

[R77] 读取用户输入
来源：http://tr.szsharing.cn

read -rp "请输入: " ans
来源：http://jq.colortex.cn

[R78] 交互式菜单
来源：http://np.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tg.shxzskj.cn

[R79] 解析命令行选项
来源：http://ez.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bg.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://xv.huanxung.cn

time ./run.sh
来源：http://ix.nicolike.cn

================================================================================
来源：http://er.521024.cn

S. C / C++ 专题
来源：http://zg.newstarts.cn

================================================================================
来源：http://ua.jianghongdianzi.cn

[S01] C：Hello World
来源：http://tz.yuexingan06.cn

#include <stdio.h>
来源：http://vx.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ox.nicolike.cn

[S02] C：变量与格式化输出
来源：http://qj.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://yb.bookmarksfly.cn

[S03] C：读入整数
来源：http://ge.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://zm.bjjhwx.cn

[S04] C：字符串复制
来源：http://nl.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oz.gzmigu.cn

[S05] C：字符串长度
来源：http://xy.huixinmuqiang.cn

strlen(s)
来源：http://rr.shxzukj.cn

[S06] C：字符串比较
来源：http://qv.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://cz.panjiajie.cn

[S07] C：数组遍历求和
来源：http://hh.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gy.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://rs.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ri.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://od.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://er.nicolike.cn

[S10] C：指针与解引用
来源：http://ph.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://lf.wgjwhj.cn

[S11] C：逐行读文件
来源：http://tf.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://nm.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lj.jianghongdianzi.cn

fclose(f);
来源：http://bi.jctech888.com.cn

[S12] C：写文件
来源：http://gn.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vx.huanxung.cn

[S13] C：宏定义
来源：http://ru.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lk.9csxet.cn

[S14] C：枚举
来源：http://ui.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://ee.bookmarksfly.cn

[S15] C：类型转换
来源：http://wh.yuexingan06.cn

(double) a / b
来源：http://ze.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://id.hahajie.cn

x |= (1 << 3);
来源：http://ck.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://sk.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://az.shtwfgs.cn

[S18] C：命令行参数
来源：http://gs.nszjky.cn

int main(int argc, char **argv)
来源：http://of.huixinmuqiang.cn

[S19] C：快速排序
来源：http://yb.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wp.yuntaijiaju.cn

[S20] C：二分查找
来源：http://at.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sw.bjjhwx.cn

[S21] C：字符类别判断
来源：http://xz.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fk.haigaiapp.cn

[S22] C：字符串转数字
来源：http://de.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://es.jianghongdianzi.cn

[S23] C：随机数
来源：http://rt.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dq.jctech888.com.cn

[S24] C：获取本地时间
来源：http://fo.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://en.shxzskj.cn

[S25] C：内存拷贝
来源：http://rc.bjjhwx.cn

memcpy(dst, src, n);
来源：http://bg.panjiajie.cn

[S26] C：内存清零
来源：http://es.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://td.bookmarksfly.cn

[S27] C：定义常量
来源：http://st.huixiangedu.cn

const double PI = 3.14159;
来源：http://cj.shxzskj.cn

[S28] C：静态变量
来源：http://ip.szsharing.cn

static int counter = 0;
来源：http://mh.shxzukj.cn

[S29] C：变参函数
来源：http://bt.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vs.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://sv.yuntaijiaju.cn

#ifndef X_H
来源：http://bd.newstarts.cn

#define X_H
来源：http://es.gzmigu.cn

#endif
来源：http://dp.bookmarksfly.cn

[S31] C++：Hello World
来源：http://rd.bookmarksfly.cn

#include <iostream>
来源：http://pq.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://fr.colortex.cn

[S32] C++：字符串
来源：http://jb.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://je.shxzukj.cn

[S33] C++：vector 增删
来源：http://fk.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tp.shxzukj.cn

[S34] C++：遍历 vector
来源：http://hu.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://cv.shxzskj.cn

[S35] C++：map
来源：http://pz.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://js.jctech888.com.cn

[S36] C++：unordered_map
来源：http://mc.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fj.521024.cn

[S37] C++：set
来源：http://py.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qv.wgjwhj.cn

[S38] C++：排序
来源：http://vw.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://fj.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://gy.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ge.muxihuayi.cn

[S40] C++：查找元素
来源：http://cy.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zk.nszjky.cn

[S41] C++：类与构造函数
来源：http://dw.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hy.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://kk.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://zf.gzmigu.cn

[S43] C++：智能指针
来源：http://un.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://ef.haigaiapp.cn

[S44] C++：引用传参
来源：http://yf.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://lf.hahajie.cn

[S45] C++：lambda
来源：http://yk.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://co.huixiangedu.cn

[S46] C++：函数模板
来源：http://hg.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cq.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://rb.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ge.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://hr.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ey.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://qz.szsharing.cn

[S49] C++：写文件
来源：http://zv.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xu.haigaiapp.cn

[S50] C++：格式化数字
来源：http://sw.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sp.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://ab.shxzskj.cn

static_cast<double>(a) / b
来源：http://jn.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://fj.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://zh.huixiangedu.cn

[S53] C++：移动语义
来源：http://zh.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://wb.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://ec.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mx.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://kr.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yp.szxytkj.cn

[S56] C++：optional
来源：http://wr.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ev.shtwfgs.cn

[S57] C++：编译期常量
来源：http://ro.yuntaijiaju.cn

constexpr int N = 10;
来源：http://zi.wgjwhj.cn

[S58] C++：命名空间
来源：http://aj.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://vg.szxytkj.cn

[S59] C++：静态断言
来源：http://pd.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ij.521024.cn

[S60] C++：遍历并删除元素
来源：http://cf.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kg.521024.cn

================================================================================
来源：http://sj.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bq.colortex.cn

================================================================================
来源：http://pf.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://ss.yuntaijiaju.cn

println("Hello")
来源：http://ii.huixiangedu.cn

[T02] Kotlin：变量
来源：http://po.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vi.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://nh.yuexingan06.cn

"值: $b"
来源：http://qs.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://hf.colortex.cn

val n: String? = null;  n?.length
来源：http://wj.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://bc.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://in.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://lq.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pr.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://mr.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qd.hahajie.cn

[T08] Kotlin：数据类
来源：http://bn.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://ho.colortex.cn


<!-- 参考信息 -->