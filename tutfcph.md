代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bn.shxzukj.cn

[R08] 数值比较
来源：http://pk.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://as.yuexingan06.cn

[R09] 字符串比较
来源：http://zr.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pz.szxytkj.cn

[R10] 正则匹配
来源：http://yk.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lq.shxzskj.cn

[R11] case 多分支
来源：http://bd.shtwfgs.cn

case "$1" in
来源：http://fw.hnjuh.cn

start) echo "启动" ;;
来源：http://mi.hnjuh.cn

stop)  echo "停止" ;;
来源：http://yt.colortex.cn

*)     echo "未知命令" ;;
来源：http://qd.panjiajie.cn

esac
来源：http://wk.bjjhwx.cn

[R12] for 遍历文件
来源：http://jb.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://tj.chemitech.net.cn

[R13] for 计数循环
来源：http://ne.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://hz.shxzukj.cn

[R14] C 风格 for
来源：http://cu.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yp.szsharing.cn

[R15] while 逐行读文件
来源：http://ce.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://el.chemitech.net.cn

[R16] until 等待条件
来源：http://tv.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ta.shxzskj.cn

[R17] 数组定义与取值
来源：http://tj.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yl.nszjky.cn

[R18] 遍历数组
来源：http://iv.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dg.panjiajie.cn

[R19] 数组长度
来源：http://uj.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://gw.hnjuh.cn

[R20] 关联数组（字典）
来源：http://eo.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://de.hahajie.cn

[R21] 字符串长度
来源：http://qw.gzmigu.cn

echo "${#s}"
来源：http://mp.huixinmuqiang.cn

[R22] 截取子串
来源：http://hg.chemitech.net.cn

echo "${s:0:5}"
来源：http://cp.wgjwhj.cn

[R23] 字符串替换
来源：http://qn.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ii.szsharing.cn

[R24] 大小写转换
来源：http://kt.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zt.521024.cn

[R25] 去后缀 / 去前缀
来源：http://cf.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kc.nszjky.cn

[R26] 命令替换
来源：http://ur.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://cc.nszjky.cn

[R27] 算术展开
来源：http://wf.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://vd.wgjwhj.cn

[R28] 浮点运算
来源：http://ym.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://io.gzmigu.cn

[R29] 定义函数
来源：http://np.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xf.gzmigu.cn

[R30] 函数返回状态码
来源：http://da.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://bs.asd995.cn

[R31] 局部变量
来源：http://lw.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://rn.gzmigu.cn

[R32] 参数个数校验
来源：http://aq.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sh.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://mo.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ky.9csxet.cn

[R34] 退出时清理
来源：http://ky.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kr.bjjhwx.cn

[R35] 后台执行并等待
来源：http://jh.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tz.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://rx.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ro.newstarts.cn

[R37] 把输出赋给变量
来源：http://te.nicolike.cn

files=$(ls -1)
来源：http://vm.wgjwhj.cn

[R38] 管道串联
来源：http://pk.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://lp.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://wg.9csxet.cn

cmd > out.log 2>&1
来源：http://va.haigaiapp.cn

[R40] 追加写日志
来源：http://to.newstarts.cn

echo "log" >> out.log
来源：http://ta.shxzskj.cn

[R41] 丢弃输出
来源：http://bk.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://jb.jianghongdianzi.cn

[R42] 输入重定向
来源：http://qd.9csxet.cn

wc -l < a.txt
来源：http://zf.hahajie.cn

[R43] 按名字查找文件
来源：http://hv.jctech888.com.cn

find . -name "*.log" -type f
来源：http://pk.newstarts.cn

[R44] 按修改时间查找
来源：http://xd.newstarts.cn

find . -mtime -7 -type f
来源：http://ga.szxytkj.cn

[R45] 批量删除
来源：http://jy.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://fh.newstarts.cn

[R46] 递归替换文件内容
来源：http://ts.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zl.huixiangedu.cn

[R47] sed 单行替换
来源：http://wk.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bt.gzmigu.cn

[R48] awk 取指定列
来源：http://wy.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://sj.panjiajie.cn

[R49] awk 带条件
来源：http://pv.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ty.huixiangedu.cn

[R50] awk 求和
来源：http://hz.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bm.yuexingan06.cn

[R51] 排序去重取前几
来源：http://us.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lo.asd995.cn

[R52] 统计行数
来源：http://rh.shtwfgs.cn

wc -l a.txt
来源：http://iy.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://ws.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hf.muxihuayi.cn

[R54] 比较两个文件
来源：http://yv.gzmigu.cn

diff a.txt b.txt
来源：http://il.haigaiapp.cn

[R55] 压缩与解压
来源：http://ju.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pt.huanxung.cn

[R56] 远程拷贝
来源：http://wy.shtwfgs.cn

scp file user@host:/path/
来源：http://qt.hahajie.cn

[R57] 远程执行命令
来源：http://jm.nicolike.cn

ssh user@host 'uptime'
来源：http://ld.newstarts.cn

[R58] 下载文件
来源：http://ak.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ty.shxzskj.cn

[R59] 发 POST JSON
来源：http://zb.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zt.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://cp.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ti.hnjuh.cn

[R61] 磁盘占用
来源：http://lh.muxihuayi.cn

df -h;  du -sh *
来源：http://za.colortex.cn

[R62] 找最占空间的文件
来源：http://xu.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://yq.bookmarksfly.cn

[R63] 内存与进程
来源：http://nh.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://zn.shtwfgs.cn

[R64] 结束进程
来源：http://ob.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://iu.9csxet.cn

[R65] 查看端口占用
来源：http://ee.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dt.bjjhwx.cn

[R66] 定时任务
来源：http://yv.huanxung.cn

crontab -e;  crontab -l
来源：http://ll.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://xd.nszjky.cn

openssl rand -hex 16
来源：http://gj.shxzukj.cn

[R68] 计算文件校验值
来源：http://gu.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xf.newstarts.cn

[R69] 生成随机密码
来源：http://vj.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://tc.521024.cn

[R70] 时间戳与互转
来源：http://hq.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://kb.hahajie.cn

[R71] 日期格式化
来源：http://hz.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kn.yuexingan06.cn

[R72] 等待端口就绪
来源：http://wc.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yj.9csxet.cn

[R73] 分割大日志
来源：http://su.newstarts.cn

split -l 1000 big.log part_
来源：http://yi.yuexingan06.cn

[R74] 批量重命名
来源：http://cb.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ur.shtwfgs.cn

[R75] 导出环境变量
来源：http://mr.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://kq.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://an.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://du.shtwfgs.cn

[R77] 读取用户输入
来源：http://bw.hnjuh.cn

read -rp "请输入: " ans
来源：http://ca.bookmarksfly.cn

[R78] 交互式菜单
来源：http://ii.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xk.asd995.cn

[R79] 解析命令行选项
来源：http://ry.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ts.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://sw.bookmarksfly.cn

time ./run.sh
来源：http://vg.hahajie.cn

================================================================================
来源：http://zw.jctech888.com.cn

S. C / C++ 专题
来源：http://sg.521024.cn

================================================================================
来源：http://ea.chemitech.net.cn

[S01] C：Hello World
来源：http://bp.huanxung.cn

#include <stdio.h>
来源：http://wj.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://na.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://np.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://kp.colortex.cn

[S03] C：读入整数
来源：http://gh.hnjuh.cn

int x; scanf("%d", &x);
来源：http://qk.colortex.cn

[S04] C：字符串复制
来源：http://ok.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qy.huanxung.cn

[S05] C：字符串长度
来源：http://ye.panjiajie.cn

strlen(s)
来源：http://ce.wgjwhj.cn

[S06] C：字符串比较
来源：http://ss.asd995.cn

strcmp(a, b) == 0
来源：http://jw.hnjuh.cn

[S07] C：数组遍历求和
来源：http://nn.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dz.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://ox.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ma.asd995.cn

[S09] C：结构体定义与初始化
来源：http://wl.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ac.shtwfgs.cn

[S10] C：指针与解引用
来源：http://vb.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://hs.huanxung.cn

[S11] C：逐行读文件
来源：http://uj.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://sy.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://im.newstarts.cn

fclose(f);
来源：http://gl.szxytkj.cn

[S12] C：写文件
来源：http://pb.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nf.yuexingan06.cn

[S13] C：宏定义
来源：http://dq.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://el.huixiangedu.cn

[S14] C：枚举
来源：http://br.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://es.muxihuayi.cn

[S15] C：类型转换
来源：http://zq.szxytkj.cn

(double) a / b
来源：http://pd.muxihuayi.cn

[S16] C：位操作置位
来源：http://kh.huixiangedu.cn

x |= (1 << 3);
来源：http://pl.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://vf.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ti.haigaiapp.cn

[S18] C：命令行参数
来源：http://fk.9csxet.cn

int main(int argc, char **argv)
来源：http://qi.huanxung.cn

[S19] C：快速排序
来源：http://vo.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mi.colortex.cn

[S20] C：二分查找
来源：http://ts.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rj.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://yp.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cp.huanxung.cn

[S22] C：字符串转数字
来源：http://iu.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vi.wgjwhj.cn

[S23] C：随机数
来源：http://sv.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nb.521024.cn

[S24] C：获取本地时间
来源：http://qn.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ut.muxihuayi.cn

[S25] C：内存拷贝
来源：http://zu.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://aa.huixiangedu.cn

[S26] C：内存清零
来源：http://oc.asd995.cn

memset(a, 0, sizeof a);
来源：http://tz.szxytkj.cn

[S27] C：定义常量
来源：http://zt.nicolike.cn

const double PI = 3.14159;
来源：http://fz.nicolike.cn

[S28] C：静态变量
来源：http://iu.hahajie.cn

static int counter = 0;
来源：http://wj.9csxet.cn

[S29] C：变参函数
来源：http://fh.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xk.521024.cn

[S30] C：头文件保护
来源：http://ja.shtwfgs.cn

#ifndef X_H
来源：http://qs.szsharing.cn

#define X_H
来源：http://mi.muxihuayi.cn

#endif
来源：http://cj.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://ls.chemitech.net.cn

#include <iostream>
来源：http://wz.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://bj.shxzukj.cn

[S32] C++：字符串
来源：http://ot.521024.cn

std::string s = "hi";  s += "!";
来源：http://ur.jctech888.com.cn

[S33] C++：vector 增删
来源：http://cr.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oe.hnjuh.cn

[S34] C++：遍历 vector
来源：http://ki.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://eh.chemitech.net.cn

[S35] C++：map
来源：http://en.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://in.9csxet.cn

[S36] C++：unordered_map
来源：http://qa.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ir.jianghongdianzi.cn

[S37] C++：set
来源：http://ov.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ga.szxytkj.cn

[S38] C++：排序
来源：http://bo.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://hp.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://jr.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zh.shxzskj.cn

[S40] C++：查找元素
来源：http://um.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zr.521024.cn

[S41] C++：类与构造函数
来源：http://mv.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kq.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://nw.521024.cn

class B : public Base { public: void f() override {} };
来源：http://nb.nicolike.cn

[S43] C++：智能指针
来源：http://gk.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://wr.panjiajie.cn

[S44] C++：引用传参
来源：http://cg.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://cg.colortex.cn

[S45] C++：lambda
来源：http://el.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ib.szsharing.cn

[S46] C++：函数模板
来源：http://cv.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gf.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://yr.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rf.nicolike.cn

[S48] C++：逐行读文件
来源：http://lh.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sr.521024.cn

while (std::getline(in, line)) { }
来源：http://fm.wgjwhj.cn

[S49] C++：写文件
来源：http://ud.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yg.newstarts.cn

[S50] C++：格式化数字
来源：http://si.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uh.newstarts.cn

[S51] C++：显式类型转换
来源：http://sn.szxytkj.cn

static_cast<double>(a) / b
来源：http://jo.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://fc.newstarts.cn

int size() const noexcept { return n_; }
来源：http://gb.asd995.cn

[S53] C++：移动语义
来源：http://qw.asd995.cn

std::vector<int> w = std::move(v);
来源：http://qy.panjiajie.cn

[S54] C++：异常处理
来源：http://mm.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xb.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://fn.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://js.nicolike.cn

[S56] C++：optional
来源：http://db.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://am.szsharing.cn

[S57] C++：编译期常量
来源：http://to.huixiangedu.cn

constexpr int N = 10;
来源：http://ck.bookmarksfly.cn

[S58] C++：命名空间
来源：http://ue.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://ze.hnjuh.cn

[S59] C++：静态断言
来源：http://px.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://od.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://fo.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wh.bookmarksfly.cn

================================================================================
来源：http://qr.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uq.bookmarksfly.cn

================================================================================
来源：http://qu.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://cr.szxytkj.cn

println("Hello")
来源：http://lk.colortex.cn

[T02] Kotlin：变量
来源：http://go.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://un.521024.cn

[T03] Kotlin：字符串模板
来源：http://cg.hahajie.cn

"值: $b"
来源：http://vg.nicolike.cn

[T04] Kotlin：空安全
来源：http://vj.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://vi.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://ms.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jt.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://tx.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ba.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://vl.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xl.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://lo.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://ig.huixinmuqiang.cn


<!-- 参考信息 -->