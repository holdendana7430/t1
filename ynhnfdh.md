代发 wailian999

name="${1:-default}"
来源：http://wj.nszjky.cn

[R06] 判断命令是否存在
来源：http://vd.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gc.bookmarksfly.cn

[R07] if 判断文件
来源：http://vh.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xt.nicolike.cn

[R08] 数值比较
来源：http://ya.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fa.yuexingan06.cn

[R09] 字符串比较
来源：http://hg.nszjky.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://is.huanxung.cn

[R10] 正则匹配
来源：http://jt.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cu.shtwfgs.cn

[R11] case 多分支
来源：http://zi.asd995.cn

case "$1" in
来源：http://fx.shxzukj.cn

start) echo "启动" ;;
来源：http://iu.nszjky.cn

stop)  echo "停止" ;;
来源：http://tt.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://gq.lnxyls.cn

esac
来源：http://ju.9csxet.cn

[R12] for 遍历文件
来源：http://ap.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://xl.yuntaijiaju.cn

[R13] for 计数循环
来源：http://hi.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://xj.huixiangedu.cn

[R14] C 风格 for
来源：http://eu.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bu.szsharing.cn

[R15] while 逐行读文件
来源：http://ya.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://un.panjiajie.cn

[R16] until 等待条件
来源：http://qd.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wo.bjjhwx.cn

[R17] 数组定义与取值
来源：http://fa.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zw.newstarts.cn

[R18] 遍历数组
来源：http://vl.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ba.muxihuayi.cn

[R19] 数组长度
来源：http://jj.hahajie.cn

echo "${#arr[@]}"
来源：http://pq.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://me.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ql.hnjuh.cn

[R21] 字符串长度
来源：http://nj.szsharing.cn

echo "${#s}"
来源：http://yh.haigaiapp.cn

[R22] 截取子串
来源：http://pj.huixiangedu.cn

echo "${s:0:5}"
来源：http://gy.bookmarksfly.cn

[R23] 字符串替换
来源：http://vo.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wu.shtwfgs.cn

[R24] 大小写转换
来源：http://ww.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hk.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://rt.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wh.szxytkj.cn

[R26] 命令替换
来源：http://xh.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://vg.bookmarksfly.cn

[R27] 算术展开
来源：http://qm.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://ih.521024.cn

[R28] 浮点运算
来源：http://yt.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://cg.jianghongdianzi.cn

[R29] 定义函数
来源：http://hf.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mm.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://gg.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://fm.521024.cn

[R31] 局部变量
来源：http://nu.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://xa.shxzukj.cn

[R32] 参数个数校验
来源：http://ze.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oo.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://wh.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lk.huixinmuqiang.cn

[R34] 退出时清理
来源：http://hm.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qr.hahajie.cn

[R35] 后台执行并等待
来源：http://zi.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zq.hnjuh.cn

[R36] 并发执行多个任务
来源：http://yn.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gw.nicolike.cn

[R37] 把输出赋给变量
来源：http://gz.huixiangedu.cn

files=$(ls -1)
来源：http://vk.lnxyls.cn

[R38] 管道串联
来源：http://pq.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://ay.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://ql.muxihuayi.cn

cmd > out.log 2>&1
来源：http://gw.huixiangedu.cn

[R40] 追加写日志
来源：http://on.panjiajie.cn

echo "log" >> out.log
来源：http://rk.muxihuayi.cn

[R41] 丢弃输出
来源：http://zu.newstarts.cn

cmd >/dev/null 2>&1
来源：http://ww.jianghongdianzi.cn

[R42] 输入重定向
来源：http://zp.nszjky.cn

wc -l < a.txt
来源：http://yi.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://ha.muxihuayi.cn

find . -name "*.log" -type f
来源：http://ld.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://bu.haigaiapp.cn

find . -mtime -7 -type f
来源：http://jr.nszjky.cn

[R45] 批量删除
来源：http://zx.nszjky.cn

find . -name "*.tmp" -delete
来源：http://ek.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://jb.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://db.hahajie.cn

[R47] sed 单行替换
来源：http://qt.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ex.lnxyls.cn

[R48] awk 取指定列
来源：http://re.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://wn.yuntaijiaju.cn

[R49] awk 带条件
来源：http://rr.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tz.shtwfgs.cn

[R50] awk 求和
来源：http://pq.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cw.shxzskj.cn

[R51] 排序去重取前几
来源：http://sv.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ug.huixinmuqiang.cn

[R52] 统计行数
来源：http://sz.yuexingan06.cn

wc -l a.txt
来源：http://oq.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://ni.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sg.gzmigu.cn

[R54] 比较两个文件
来源：http://cm.bjjhwx.cn

diff a.txt b.txt
来源：http://mc.huanxung.cn

[R55] 压缩与解压
来源：http://nh.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://we.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://qw.muxihuayi.cn

scp file user@host:/path/
来源：http://dd.wgjwhj.cn

[R57] 远程执行命令
来源：http://fx.9csxet.cn

ssh user@host 'uptime'
来源：http://ho.chemitech.net.cn

[R58] 下载文件
来源：http://os.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rq.chemitech.net.cn

[R59] 发 POST JSON
来源：http://it.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zw.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://oi.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hl.gzmigu.cn

[R61] 磁盘占用
来源：http://bo.huixiangedu.cn

df -h;  du -sh *
来源：http://vh.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://cj.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://kn.szsharing.cn

[R63] 内存与进程
来源：http://ob.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://jq.nszjky.cn

[R64] 结束进程
来源：http://yh.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://le.9csxet.cn

[R65] 查看端口占用
来源：http://fr.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dz.huixinmuqiang.cn

[R66] 定时任务
来源：http://nd.huanxung.cn

crontab -e;  crontab -l
来源：http://ap.szsharing.cn

[R67] 生成随机十六进制串
来源：http://jx.colortex.cn

openssl rand -hex 16
来源：http://gw.szsharing.cn

[R68] 计算文件校验值
来源：http://fr.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pe.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://qj.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://as.hahajie.cn

[R70] 时间戳与互转
来源：http://hc.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://dm.bjjhwx.cn

[R71] 日期格式化
来源：http://hh.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ky.szxytkj.cn

[R72] 等待端口就绪
来源：http://hb.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hi.asd995.cn

[R73] 分割大日志
来源：http://qq.szxytkj.cn

split -l 1000 big.log part_
来源：http://au.9csxet.cn

[R74] 批量重命名
来源：http://va.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jy.yuexingan06.cn

[R75] 导出环境变量
来源：http://el.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://of.haigaiapp.cn

[R76] 使用临时文件
来源：http://sj.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bt.asd995.cn

[R77] 读取用户输入
来源：http://sd.colortex.cn

read -rp "请输入: " ans
来源：http://kn.colortex.cn

[R78] 交互式菜单
来源：http://gx.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://br.nicolike.cn

[R79] 解析命令行选项
来源：http://mp.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cu.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://kr.szsharing.cn

time ./run.sh
来源：http://rm.shtwfgs.cn

================================================================================
来源：http://yb.hahajie.cn

S. C / C++ 专题
来源：http://fg.chemitech.net.cn

================================================================================
来源：http://zr.bjjhwx.cn

[S01] C：Hello World
来源：http://yi.huanxung.cn

#include <stdio.h>
来源：http://tt.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cl.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://bt.shxzukj.cn

int a = 10; printf("%d\n", a);
来源：http://ko.panjiajie.cn

[S03] C：读入整数
来源：http://li.shxzskj.cn

int x; scanf("%d", &x);
来源：http://jc.bookmarksfly.cn

[S04] C：字符串复制
来源：http://cp.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xx.shxzskj.cn

[S05] C：字符串长度
来源：http://jo.nicolike.cn

strlen(s)
来源：http://ev.shxzukj.cn

[S06] C：字符串比较
来源：http://gb.shxzskj.cn

strcmp(a, b) == 0
来源：http://pr.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://kk.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ok.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://mu.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://be.521024.cn

[S09] C：结构体定义与初始化
来源：http://sp.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zu.haigaiapp.cn

[S10] C：指针与解引用
来源：http://ku.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://gv.9csxet.cn

[S11] C：逐行读文件
来源：http://xt.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://so.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kf.shtwfgs.cn

fclose(f);
来源：http://th.huixiangedu.cn

[S12] C：写文件
来源：http://rd.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ie.huixiangedu.cn

[S13] C：宏定义
来源：http://hh.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hm.shxzukj.cn

[S14] C：枚举
来源：http://no.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://mp.newstarts.cn

[S15] C：类型转换
来源：http://vt.muxihuayi.cn

(double) a / b
来源：http://md.bjjhwx.cn

[S16] C：位操作置位
来源：http://ba.huanxung.cn

x |= (1 << 3);
来源：http://gl.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://hu.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yh.szsharing.cn

[S18] C：命令行参数
来源：http://mv.haigaiapp.cn

int main(int argc, char **argv)
来源：http://ee.asd995.cn

[S19] C：快速排序
来源：http://sb.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ch.wgjwhj.cn

[S20] C：二分查找
来源：http://cn.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ec.9csxet.cn

[S21] C：字符类别判断
来源：http://mc.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xs.colortex.cn

[S22] C：字符串转数字
来源：http://za.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ws.yuntaijiaju.cn

[S23] C：随机数
来源：http://xo.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nw.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://fk.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pm.szsharing.cn

[S25] C：内存拷贝
来源：http://ok.gzmigu.cn

memcpy(dst, src, n);
来源：http://zj.shxzukj.cn

[S26] C：内存清零
来源：http://ds.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://nl.nicolike.cn

[S27] C：定义常量
来源：http://lj.bjjhwx.cn

const double PI = 3.14159;
来源：http://ys.nicolike.cn

[S28] C：静态变量
来源：http://wm.nicolike.cn

static int counter = 0;
来源：http://bd.nicolike.cn

[S29] C：变参函数
来源：http://vy.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gd.hnjuh.cn

[S30] C：头文件保护
来源：http://uy.huixinmuqiang.cn

#ifndef X_H
来源：http://mq.muxihuayi.cn

#define X_H
来源：http://el.shxzukj.cn

#endif
来源：http://km.asd995.cn

[S31] C++：Hello World
来源：http://xq.nicolike.cn

#include <iostream>
来源：http://bk.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://yx.hahajie.cn

[S32] C++：字符串
来源：http://ah.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://as.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://bb.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fh.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://vw.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://ww.bookmarksfly.cn

[S35] C++：map
来源：http://bf.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gf.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://vf.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ud.haigaiapp.cn

[S37] C++：set
来源：http://ik.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jp.haigaiapp.cn

[S38] C++：排序
来源：http://nx.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://wz.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://tb.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wm.colortex.cn

[S40] C++：查找元素
来源：http://rq.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gb.nicolike.cn

[S41] C++：类与构造函数
来源：http://xd.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kt.hahajie.cn

[S42] C++：继承与虚函数
来源：http://cc.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://ig.asd995.cn

[S43] C++：智能指针
来源：http://yb.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://um.hnjuh.cn

[S44] C++：引用传参
来源：http://hr.newstarts.cn

void inc(int &x) { ++x; }
来源：http://on.jctech888.com.cn

[S45] C++：lambda
来源：http://sq.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oh.jctech888.com.cn

[S46] C++：函数模板
来源：http://xm.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jw.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://wo.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wo.shxzukj.cn

[S48] C++：逐行读文件
来源：http://az.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oj.huanxung.cn

while (std::getline(in, line)) { }
来源：http://os.huixinmuqiang.cn

[S49] C++：写文件
来源：http://dp.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wn.nszjky.cn

[S50] C++：格式化数字
来源：http://yc.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ol.colortex.cn

[S51] C++：显式类型转换
来源：http://sf.nicolike.cn

static_cast<double>(a) / b
来源：http://zh.colortex.cn

[S52] C++：const 与 noexcept
来源：http://la.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://na.nszjky.cn

[S53] C++：移动语义
来源：http://ae.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://qg.shtwfgs.cn

[S54] C++：异常处理
来源：http://ee.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jy.shxzukj.cn

[S55] C++：结构化绑定
来源：http://iv.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gc.gzmigu.cn

[S56] C++：optional
来源：http://kw.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oa.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://an.jctech888.com.cn

constexpr int N = 10;
来源：http://ov.bookmarksfly.cn

[S58] C++：命名空间
来源：http://oc.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://tx.asd995.cn

[S59] C++：静态断言
来源：http://gz.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wx.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://sg.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pc.shtwfgs.cn

================================================================================
来源：http://nr.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jf.yuexingan06.cn

================================================================================
来源：http://xk.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://ei.9csxet.cn

println("Hello")
来源：http://gr.lnxyls.cn

[T02] Kotlin：变量
来源：http://de.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jx.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://nw.yuexingan06.cn

"值: $b"
来源：http://bn.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://xb.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://ca.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://nq.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qz.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://bn.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kb.huixinmuqiang.cn


<!-- 参考信息 -->