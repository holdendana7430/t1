代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vy.newstarts.cn

[R08] 数值比较
来源：http://kh.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wx.szxytkj.cn

[R09] 字符串比较
来源：http://sf.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xb.bjjhwx.cn

[R10] 正则匹配
来源：http://lx.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vo.hnjuh.cn

[R11] case 多分支
来源：http://jd.hnjuh.cn

case "$1" in
来源：http://st.lnxyls.cn

start) echo "启动" ;;
来源：http://cd.gzmigu.cn

stop)  echo "停止" ;;
来源：http://wm.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://jl.szxytkj.cn

esac
来源：http://gq.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://di.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://ou.huanxung.cn

[R13] for 计数循环
来源：http://ay.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://cm.shxzukj.cn

[R14] C 风格 for
来源：http://qo.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eq.9csxet.cn

[R15] while 逐行读文件
来源：http://cz.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nm.yuexingan06.cn

[R16] until 等待条件
来源：http://xi.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xd.muxihuayi.cn

[R17] 数组定义与取值
来源：http://jj.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oc.521024.cn

[R18] 遍历数组
来源：http://yu.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ex.nszjky.cn

[R19] 数组长度
来源：http://dl.yuexingan06.cn

echo "${#arr[@]}"
来源：http://xc.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://lc.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ta.szxytkj.cn

[R21] 字符串长度
来源：http://dc.asd995.cn

echo "${#s}"
来源：http://nd.huixiangedu.cn

[R22] 截取子串
来源：http://kf.jctech888.com.cn

echo "${s:0:5}"
来源：http://pa.nicolike.cn

[R23] 字符串替换
来源：http://zb.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dy.nszjky.cn

[R24] 大小写转换
来源：http://hk.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nu.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://jy.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fu.jctech888.com.cn

[R26] 命令替换
来源：http://zv.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://cn.haigaiapp.cn

[R27] 算术展开
来源：http://vq.huanxung.cn

echo $((1 + 2 * 3))
来源：http://fu.colortex.cn

[R28] 浮点运算
来源：http://uj.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://ch.szsharing.cn

[R29] 定义函数
来源：http://ay.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vg.lnxyls.cn

[R30] 函数返回状态码
来源：http://bu.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://lb.huanxung.cn

[R31] 局部变量
来源：http://yn.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://yg.hahajie.cn

[R32] 参数个数校验
来源：http://jy.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tt.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://ld.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rf.hnjuh.cn

[R34] 退出时清理
来源：http://bn.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wv.yuexingan06.cn

[R35] 后台执行并等待
来源：http://ng.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ti.shxzskj.cn

[R36] 并发执行多个任务
来源：http://gf.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mb.9csxet.cn

[R37] 把输出赋给变量
来源：http://st.9csxet.cn

files=$(ls -1)
来源：http://do.haigaiapp.cn

[R38] 管道串联
来源：http://bv.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://st.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://iv.nicolike.cn

cmd > out.log 2>&1
来源：http://vz.jctech888.com.cn

[R40] 追加写日志
来源：http://ht.bookmarksfly.cn

echo "log" >> out.log
来源：http://yp.panjiajie.cn

[R41] 丢弃输出
来源：http://cr.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://rw.huixiangedu.cn

[R42] 输入重定向
来源：http://er.jianghongdianzi.cn

wc -l < a.txt
来源：http://ql.colortex.cn

[R43] 按名字查找文件
来源：http://hm.yuexingan06.cn

find . -name "*.log" -type f
来源：http://we.muxihuayi.cn

[R44] 按修改时间查找
来源：http://ma.shxzukj.cn

find . -mtime -7 -type f
来源：http://bu.shtwfgs.cn

[R45] 批量删除
来源：http://xj.521024.cn

find . -name "*.tmp" -delete
来源：http://iu.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://kx.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qg.nszjky.cn

[R47] sed 单行替换
来源：http://vo.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bk.yuexingan06.cn

[R48] awk 取指定列
来源：http://pp.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://rh.panjiajie.cn

[R49] awk 带条件
来源：http://up.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vd.jctech888.com.cn

[R50] awk 求和
来源：http://pz.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yy.hahajie.cn

[R51] 排序去重取前几
来源：http://cz.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://en.yuexingan06.cn

[R52] 统计行数
来源：http://nh.hahajie.cn

wc -l a.txt
来源：http://bc.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://ml.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xo.bjjhwx.cn

[R54] 比较两个文件
来源：http://we.huixiangedu.cn

diff a.txt b.txt
来源：http://kp.bookmarksfly.cn

[R55] 压缩与解压
来源：http://vi.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nz.gzmigu.cn

[R56] 远程拷贝
来源：http://jn.panjiajie.cn

scp file user@host:/path/
来源：http://cv.9csxet.cn

[R57] 远程执行命令
来源：http://xp.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://et.hnjuh.cn

[R58] 下载文件
来源：http://jf.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jv.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://fe.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wn.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://dv.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pr.newstarts.cn

[R61] 磁盘占用
来源：http://fk.jianghongdianzi.cn

df -h;  du -sh *
来源：http://uv.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://fp.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://eq.chemitech.net.cn

[R63] 内存与进程
来源：http://tc.asd995.cn

free -h;  ps aux | grep nginx
来源：http://nf.hahajie.cn

[R64] 结束进程
来源：http://wt.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://fc.yuexingan06.cn

[R65] 查看端口占用
来源：http://xx.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pk.szxytkj.cn

[R66] 定时任务
来源：http://rv.9csxet.cn

crontab -e;  crontab -l
来源：http://qv.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://bd.huixiangedu.cn

openssl rand -hex 16
来源：http://jb.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://ff.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vx.521024.cn

[R69] 生成随机密码
来源：http://ai.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://xo.hahajie.cn

[R70] 时间戳与互转
来源：http://sd.huanxung.cn

date +%s;  date -d @1700000000
来源：http://mc.huanxung.cn

[R71] 日期格式化
来源：http://rh.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xh.lnxyls.cn

[R72] 等待端口就绪
来源：http://wt.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pa.hahajie.cn

[R73] 分割大日志
来源：http://cy.colortex.cn

split -l 1000 big.log part_
来源：http://wa.huanxung.cn

[R74] 批量重命名
来源：http://xv.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ld.gzmigu.cn

[R75] 导出环境变量
来源：http://el.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://uo.haigaiapp.cn

[R76] 使用临时文件
来源：http://jd.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wp.bjjhwx.cn

[R77] 读取用户输入
来源：http://nb.yuexingan06.cn

read -rp "请输入: " ans
来源：http://us.bookmarksfly.cn

[R78] 交互式菜单
来源：http://yw.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zm.hnjuh.cn

[R79] 解析命令行选项
来源：http://fb.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://me.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://zf.panjiajie.cn

time ./run.sh
来源：http://qm.shxzskj.cn

================================================================================
来源：http://gn.muxihuayi.cn

S. C / C++ 专题
来源：http://tw.yuntaijiaju.cn

================================================================================
来源：http://ho.asd995.cn

[S01] C：Hello World
来源：http://pp.shxzskj.cn

#include <stdio.h>
来源：http://gx.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ur.9csxet.cn

[S02] C：变量与格式化输出
来源：http://cj.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://su.nicolike.cn

[S03] C：读入整数
来源：http://ki.9csxet.cn

int x; scanf("%d", &x);
来源：http://he.haigaiapp.cn

[S04] C：字符串复制
来源：http://zc.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ut.521024.cn

[S05] C：字符串长度
来源：http://wk.muxihuayi.cn

strlen(s)
来源：http://oc.hnjuh.cn

[S06] C：字符串比较
来源：http://gb.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://gt.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://sg.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ih.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://qx.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jg.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://zj.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://es.chemitech.net.cn

[S10] C：指针与解引用
来源：http://jn.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://jt.shtwfgs.cn

[S11] C：逐行读文件
来源：http://ah.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://kl.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ja.bjjhwx.cn

fclose(f);
来源：http://mz.muxihuayi.cn

[S12] C：写文件
来源：http://qh.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tq.bjjhwx.cn

[S13] C：宏定义
来源：http://jz.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sh.haigaiapp.cn

[S14] C：枚举
来源：http://bj.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://fh.shxzukj.cn

[S15] C：类型转换
来源：http://od.chemitech.net.cn

(double) a / b
来源：http://kz.huixiangedu.cn

[S16] C：位操作置位
来源：http://cp.haigaiapp.cn

x |= (1 << 3);
来源：http://ne.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://aw.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vj.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://xs.yuexingan06.cn

int main(int argc, char **argv)
来源：http://lq.nszjky.cn

[S19] C：快速排序
来源：http://yp.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wo.gzmigu.cn

[S20] C：二分查找
来源：http://wq.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aq.panjiajie.cn

[S21] C：字符类别判断
来源：http://ue.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xb.521024.cn

[S22] C：字符串转数字
来源：http://dq.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://of.szxytkj.cn

[S23] C：随机数
来源：http://oh.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oe.panjiajie.cn

[S24] C：获取本地时间
来源：http://yw.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sp.shxzukj.cn

[S25] C：内存拷贝
来源：http://qs.hnjuh.cn

memcpy(dst, src, n);
来源：http://rn.szxytkj.cn

[S26] C：内存清零
来源：http://em.szsharing.cn

memset(a, 0, sizeof a);
来源：http://hw.bookmarksfly.cn

[S27] C：定义常量
来源：http://ea.colortex.cn

const double PI = 3.14159;
来源：http://xq.nicolike.cn

[S28] C：静态变量
来源：http://ln.gzmigu.cn

static int counter = 0;
来源：http://gs.hnjuh.cn

[S29] C：变参函数
来源：http://by.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fq.gzmigu.cn

[S30] C：头文件保护
来源：http://vo.yuexingan06.cn

#ifndef X_H
来源：http://kj.szsharing.cn

#define X_H
来源：http://vi.muxihuayi.cn

#endif
来源：http://lb.shtwfgs.cn

[S31] C++：Hello World
来源：http://lw.shxzukj.cn

#include <iostream>
来源：http://bq.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://ii.huixinmuqiang.cn

[S32] C++：字符串
来源：http://rp.asd995.cn

std::string s = "hi";  s += "!";
来源：http://na.hahajie.cn

[S33] C++：vector 增删
来源：http://et.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qw.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://ru.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://rz.huixiangedu.cn

[S35] C++：map
来源：http://ss.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yg.shxzukj.cn

[S36] C++：unordered_map
来源：http://cu.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ag.yuexingan06.cn

[S37] C++：set
来源：http://tq.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aw.bjjhwx.cn

[S38] C++：排序
来源：http://jd.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://ug.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://qx.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://co.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://wb.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ab.gzmigu.cn

[S41] C++：类与构造函数
来源：http://bc.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yz.hahajie.cn

[S42] C++：继承与虚函数
来源：http://lx.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://vl.jctech888.com.cn

[S43] C++：智能指针
来源：http://uj.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://xc.9csxet.cn

[S44] C++：引用传参
来源：http://fz.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://cu.9csxet.cn

[S45] C++：lambda
来源：http://to.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ta.shxzskj.cn

[S46] C++：函数模板
来源：http://fi.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xx.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://hj.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ut.colortex.cn

[S48] C++：逐行读文件
来源：http://ld.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yo.hahajie.cn

while (std::getline(in, line)) { }
来源：http://mu.chemitech.net.cn

[S49] C++：写文件
来源：http://ec.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nh.muxihuayi.cn

[S50] C++：格式化数字
来源：http://zg.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gh.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://gq.shxzskj.cn

static_cast<double>(a) / b
来源：http://ge.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://ar.szsharing.cn

int size() const noexcept { return n_; }
来源：http://ki.yuexingan06.cn

[S53] C++：移动语义
来源：http://zh.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://ci.9csxet.cn

[S54] C++：异常处理
来源：http://qe.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vq.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://nf.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://er.gzmigu.cn

[S56] C++：optional
来源：http://xe.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zy.chemitech.net.cn

[S57] C++：编译期常量
来源：http://lc.panjiajie.cn

constexpr int N = 10;
来源：http://jt.asd995.cn

[S58] C++：命名空间
来源：http://rq.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://kd.asd995.cn

[S59] C++：静态断言
来源：http://qk.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jf.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://pv.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nb.hahajie.cn

================================================================================
来源：http://tc.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ro.nicolike.cn

================================================================================
来源：http://xr.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://zq.jianghongdianzi.cn

println("Hello")
来源：http://qp.asd995.cn

[T02] Kotlin：变量
来源：http://uq.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rj.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://cb.bookmarksfly.cn

"值: $b"
来源：http://nh.szsharing.cn

[T04] Kotlin：空安全
来源：http://ei.lnxyls.cn

val n: String? = null;  n?.length
来源：http://pk.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://dl.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ld.newstarts.cn

[T06] Kotlin：集合映射
来源：http://zr.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nc.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://qn.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://or.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://fl.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://ov.muxihuayi.cn


<!-- 参考信息 -->