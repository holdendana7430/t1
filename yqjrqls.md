代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wh.521024.cn

[R10] 正则匹配
来源：http://pd.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vz.hnjuh.cn

[R11] case 多分支
来源：http://cd.gzmigu.cn

case "$1" in
来源：http://ji.lnxyls.cn

start) echo "启动" ;;
来源：http://py.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://aw.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://rh.chemitech.net.cn

esac
来源：http://yz.bookmarksfly.cn

[R12] for 遍历文件
来源：http://jd.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://vz.nszjky.cn

[R13] for 计数循环
来源：http://ve.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://bg.nicolike.cn

[R14] C 风格 for
来源：http://vh.9csxet.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gi.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://oa.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vq.bjjhwx.cn

[R16] until 等待条件
来源：http://jv.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jn.szxytkj.cn

[R17] 数组定义与取值
来源：http://tr.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yu.shxzskj.cn

[R18] 遍历数组
来源：http://xe.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qr.nicolike.cn

[R19] 数组长度
来源：http://ph.yuexingan06.cn

echo "${#arr[@]}"
来源：http://rw.lnxyls.cn

[R20] 关联数组（字典）
来源：http://wt.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uh.jianghongdianzi.cn

[R21] 字符串长度
来源：http://ak.yuexingan06.cn

echo "${#s}"
来源：http://al.muxihuayi.cn

[R22] 截取子串
来源：http://uf.yuexingan06.cn

echo "${s:0:5}"
来源：http://hd.shtwfgs.cn

[R23] 字符串替换
来源：http://gj.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zq.szxytkj.cn

[R24] 大小写转换
来源：http://ys.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bc.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://hp.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ir.shxzukj.cn

[R26] 命令替换
来源：http://vl.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://no.gzmigu.cn

[R27] 算术展开
来源：http://nh.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://xf.asd995.cn

[R28] 浮点运算
来源：http://kl.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://nv.9csxet.cn

[R29] 定义函数
来源：http://fk.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tp.szxytkj.cn

[R30] 函数返回状态码
来源：http://nd.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://zf.shxzukj.cn

[R31] 局部变量
来源：http://ci.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://aw.lnxyls.cn

[R32] 参数个数校验
来源：http://co.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mu.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://vq.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zd.szxytkj.cn

[R34] 退出时清理
来源：http://sv.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sf.yuexingan06.cn

[R35] 后台执行并等待
来源：http://os.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rp.521024.cn

[R36] 并发执行多个任务
来源：http://iz.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ay.521024.cn

[R37] 把输出赋给变量
来源：http://nj.yuexingan06.cn

files=$(ls -1)
来源：http://vy.yuntaijiaju.cn

[R38] 管道串联
来源：http://xm.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://lm.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://ua.jctech888.com.cn

cmd > out.log 2>&1
来源：http://dm.nszjky.cn

[R40] 追加写日志
来源：http://bs.lnxyls.cn

echo "log" >> out.log
来源：http://rp.jctech888.com.cn

[R41] 丢弃输出
来源：http://ji.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://eu.bookmarksfly.cn

[R42] 输入重定向
来源：http://tm.haigaiapp.cn

wc -l < a.txt
来源：http://fp.shxzukj.cn

[R43] 按名字查找文件
来源：http://fa.szxytkj.cn

find . -name "*.log" -type f
来源：http://yl.shtwfgs.cn

[R44] 按修改时间查找
来源：http://bj.shtwfgs.cn

find . -mtime -7 -type f
来源：http://dq.colortex.cn

[R45] 批量删除
来源：http://vw.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://cf.panjiajie.cn

[R46] 递归替换文件内容
来源：http://kj.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pk.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://tk.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ip.shxzskj.cn

[R48] awk 取指定列
来源：http://wv.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://xt.bookmarksfly.cn

[R49] awk 带条件
来源：http://zq.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ge.haigaiapp.cn

[R50] awk 求和
来源：http://rs.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xz.muxihuayi.cn

[R51] 排序去重取前几
来源：http://lk.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eg.hnjuh.cn

[R52] 统计行数
来源：http://rt.yuexingan06.cn

wc -l a.txt
来源：http://ur.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://uy.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://es.jctech888.com.cn

[R54] 比较两个文件
来源：http://zx.wgjwhj.cn

diff a.txt b.txt
来源：http://rz.muxihuayi.cn

[R55] 压缩与解压
来源：http://gl.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yo.bookmarksfly.cn

[R56] 远程拷贝
来源：http://be.nicolike.cn

scp file user@host:/path/
来源：http://pq.shxzukj.cn

[R57] 远程执行命令
来源：http://ua.shxzskj.cn

ssh user@host 'uptime'
来源：http://eo.shtwfgs.cn

[R58] 下载文件
来源：http://rd.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gl.shxzukj.cn

[R59] 发 POST JSON
来源：http://nr.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rc.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://yt.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://db.asd995.cn

[R61] 磁盘占用
来源：http://ql.yuntaijiaju.cn

df -h;  du -sh *
来源：http://az.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://es.colortex.cn

du -ah . | sort -rh | head -10
来源：http://jn.chemitech.net.cn

[R63] 内存与进程
来源：http://ds.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://hp.bookmarksfly.cn

[R64] 结束进程
来源：http://ii.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://ic.szsharing.cn

[R65] 查看端口占用
来源：http://vf.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uh.panjiajie.cn

[R66] 定时任务
来源：http://pb.huixiangedu.cn

crontab -e;  crontab -l
来源：http://uu.521024.cn

[R67] 生成随机十六进制串
来源：http://jk.nicolike.cn

openssl rand -hex 16
来源：http://hb.hahajie.cn

[R68] 计算文件校验值
来源：http://zl.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rk.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://ha.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://rt.shxzskj.cn

[R70] 时间戳与互转
来源：http://el.newstarts.cn

date +%s;  date -d @1700000000
来源：http://io.hahajie.cn

[R71] 日期格式化
来源：http://qo.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ng.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://pv.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pc.shxzukj.cn

[R73] 分割大日志
来源：http://jv.lnxyls.cn

split -l 1000 big.log part_
来源：http://fb.lnxyls.cn

[R74] 批量重命名
来源：http://ii.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bw.huanxung.cn

[R75] 导出环境变量
来源：http://sb.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://rx.haigaiapp.cn

[R76] 使用临时文件
来源：http://ux.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yk.hnjuh.cn

[R77] 读取用户输入
来源：http://bb.gzmigu.cn

read -rp "请输入: " ans
来源：http://pf.hnjuh.cn

[R78] 交互式菜单
来源：http://mx.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dw.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://ir.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://be.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://hv.jctech888.com.cn

time ./run.sh
来源：http://vw.nszjky.cn

================================================================================
来源：http://ry.9csxet.cn

S. C / C++ 专题
来源：http://th.panjiajie.cn

================================================================================
来源：http://kr.yuexingan06.cn

[S01] C：Hello World
来源：http://sq.huixinmuqiang.cn

#include <stdio.h>
来源：http://kx.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rc.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://gu.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://te.nicolike.cn

[S03] C：读入整数
来源：http://jj.colortex.cn

int x; scanf("%d", &x);
来源：http://la.colortex.cn

[S04] C：字符串复制
来源：http://kw.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ho.bookmarksfly.cn

[S05] C：字符串长度
来源：http://dp.jianghongdianzi.cn

strlen(s)
来源：http://qe.hnjuh.cn

[S06] C：字符串比较
来源：http://jd.shxzukj.cn

strcmp(a, b) == 0
来源：http://um.panjiajie.cn

[S07] C：数组遍历求和
来源：http://ab.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cn.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://kr.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wt.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://ar.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wt.nicolike.cn

[S10] C：指针与解引用
来源：http://us.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://kd.huanxung.cn

[S11] C：逐行读文件
来源：http://xc.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://pm.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oz.gzmigu.cn

fclose(f);
来源：http://ro.gzmigu.cn

[S12] C：写文件
来源：http://wr.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hd.bjjhwx.cn

[S13] C：宏定义
来源：http://mb.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ae.jianghongdianzi.cn

[S14] C：枚举
来源：http://rg.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://tr.yuexingan06.cn

[S15] C：类型转换
来源：http://ms.asd995.cn

(double) a / b
来源：http://lg.szsharing.cn

[S16] C：位操作置位
来源：http://yx.nicolike.cn

x |= (1 << 3);
来源：http://to.colortex.cn

[S17] C：安全拼接字符串
来源：http://ny.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ep.huixiangedu.cn

[S18] C：命令行参数
来源：http://ed.haigaiapp.cn

int main(int argc, char **argv)
来源：http://pi.jianghongdianzi.cn

[S19] C：快速排序
来源：http://bd.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ne.hnjuh.cn

[S20] C：二分查找
来源：http://cl.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gx.yuexingan06.cn

[S21] C：字符类别判断
来源：http://na.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sl.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://mq.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rn.bjjhwx.cn

[S23] C：随机数
来源：http://ki.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://by.szxytkj.cn

[S24] C：获取本地时间
来源：http://cn.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hp.wgjwhj.cn

[S25] C：内存拷贝
来源：http://we.yuexingan06.cn

memcpy(dst, src, n);
来源：http://gg.hahajie.cn

[S26] C：内存清零
来源：http://un.huanxung.cn

memset(a, 0, sizeof a);
来源：http://id.muxihuayi.cn

[S27] C：定义常量
来源：http://ww.haigaiapp.cn

const double PI = 3.14159;
来源：http://ud.521024.cn

[S28] C：静态变量
来源：http://tr.huixinmuqiang.cn

static int counter = 0;
来源：http://gk.szxytkj.cn

[S29] C：变参函数
来源：http://lw.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ss.521024.cn

[S30] C：头文件保护
来源：http://tr.muxihuayi.cn

#ifndef X_H
来源：http://mx.huixinmuqiang.cn

#define X_H
来源：http://vl.shtwfgs.cn

#endif
来源：http://ry.bookmarksfly.cn

[S31] C++：Hello World
来源：http://tc.hahajie.cn

#include <iostream>
来源：http://vq.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ck.jianghongdianzi.cn

[S32] C++：字符串
来源：http://ek.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://im.asd995.cn

[S33] C++：vector 增删
来源：http://wp.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zk.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://ze.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://tq.jctech888.com.cn

[S35] C++：map
来源：http://nj.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ms.lnxyls.cn

[S36] C++：unordered_map
来源：http://hm.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ij.shxzskj.cn

[S37] C++：set
来源：http://tm.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yn.panjiajie.cn

[S38] C++：排序
来源：http://vi.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://vi.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://hi.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://da.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://bf.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cb.521024.cn

[S41] C++：类与构造函数
来源：http://wo.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zh.hahajie.cn

[S42] C++：继承与虚函数
来源：http://pr.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://ob.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://bq.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://jd.nicolike.cn

[S44] C++：引用传参
来源：http://hz.9csxet.cn

void inc(int &x) { ++x; }
来源：http://jv.szxytkj.cn

[S45] C++：lambda
来源：http://rc.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ws.shxzskj.cn

[S46] C++：函数模板
来源：http://pq.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vm.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://jq.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ub.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://ap.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qe.nicolike.cn

while (std::getline(in, line)) { }
来源：http://oc.szxytkj.cn

[S49] C++：写文件
来源：http://lh.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ak.newstarts.cn

[S50] C++：格式化数字
来源：http://ux.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jo.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://bn.haigaiapp.cn

static_cast<double>(a) / b
来源：http://hu.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://ze.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://nr.521024.cn

[S53] C++：移动语义
来源：http://qn.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://xq.panjiajie.cn

[S54] C++：异常处理
来源：http://mi.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ap.newstarts.cn

[S55] C++：结构化绑定
来源：http://kx.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ei.lnxyls.cn

[S56] C++：optional
来源：http://dr.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uv.nszjky.cn

[S57] C++：编译期常量
来源：http://jp.chemitech.net.cn

constexpr int N = 10;
来源：http://mt.gzmigu.cn

[S58] C++：命名空间
来源：http://vl.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://lu.shtwfgs.cn

[S59] C++：静态断言
来源：http://zk.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zg.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://xj.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oq.9csxet.cn

================================================================================
来源：http://ag.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ka.panjiajie.cn

================================================================================
来源：http://na.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://hj.szxytkj.cn

println("Hello")
来源：http://sg.szsharing.cn

[T02] Kotlin：变量
来源：http://qs.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dl.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://jj.hnjuh.cn

"值: $b"
来源：http://zj.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://ey.nicolike.cn

val n: String? = null;  n?.length
来源：http://bj.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://ru.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dl.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://ar.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jb.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://ax.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qo.colortex.cn

[T08] Kotlin：数据类
来源：http://cg.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://hs.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://kz.asd995.cn

fun String.exclaim() = this + "!"
来源：http://rp.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://lk.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ji.huanxung.cn


<!-- 参考信息 -->