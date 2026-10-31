代发 wailian999

set -euo pipefail
来源：http://dx.colortex.cn

[R02] 变量赋值与使用
来源：http://is.lnxyls.cn

name="Tom"; echo "$name"
来源：http://vo.yuntaijiaju.cn

[R03] 只读变量
来源：http://ag.hahajie.cn

readonly PI=3.14
来源：http://aa.haigaiapp.cn

[R04] 位置参数
来源：http://fh.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ox.hnjuh.cn

[R05] 参数默认值
来源：http://qo.huixinmuqiang.cn

name="${1:-default}"
来源：http://zt.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://un.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ez.huanxung.cn

[R07] if 判断文件
来源：http://ng.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gt.521024.cn

[R08] 数值比较
来源：http://vh.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vp.asd995.cn

[R09] 字符串比较
来源：http://xr.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ge.huixiangedu.cn

[R10] 正则匹配
来源：http://bx.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fg.shxzukj.cn

[R11] case 多分支
来源：http://jm.huixiangedu.cn

case "$1" in
来源：http://iq.shtwfgs.cn

start) echo "启动" ;;
来源：http://dd.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://to.huanxung.cn

*)     echo "未知命令" ;;
来源：http://zt.szxytkj.cn

esac
来源：http://fa.colortex.cn

[R12] for 遍历文件
来源：http://ul.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://my.nszjky.cn

[R13] for 计数循环
来源：http://xr.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://bu.asd995.cn

[R14] C 风格 for
来源：http://ji.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nr.shxzukj.cn

[R15] while 逐行读文件
来源：http://ct.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lu.hahajie.cn

[R16] until 等待条件
来源：http://gl.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tf.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://oj.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nw.bjjhwx.cn

[R18] 遍历数组
来源：http://bc.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hh.jianghongdianzi.cn

[R19] 数组长度
来源：http://ke.shtwfgs.cn

echo "${#arr[@]}"
来源：http://vs.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://ez.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zi.szxytkj.cn

[R21] 字符串长度
来源：http://us.chemitech.net.cn

echo "${#s}"
来源：http://ku.huixinmuqiang.cn

[R22] 截取子串
来源：http://jn.huanxung.cn

echo "${s:0:5}"
来源：http://zd.jctech888.com.cn

[R23] 字符串替换
来源：http://yu.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://db.gzmigu.cn

[R24] 大小写转换
来源：http://cn.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bm.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://up.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jj.szsharing.cn

[R26] 命令替换
来源：http://gn.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://mh.colortex.cn

[R27] 算术展开
来源：http://om.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://he.panjiajie.cn

[R28] 浮点运算
来源：http://md.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://km.jctech888.com.cn

[R29] 定义函数
来源：http://ws.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ei.asd995.cn

[R30] 函数返回状态码
来源：http://uv.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://vb.huanxung.cn

[R31] 局部变量
来源：http://ii.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://sw.muxihuayi.cn

[R32] 参数个数校验
来源：http://wp.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kc.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://km.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oa.nicolike.cn

[R34] 退出时清理
来源：http://ai.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mf.lnxyls.cn

[R35] 后台执行并等待
来源：http://pl.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ih.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://gw.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://se.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://ty.nicolike.cn

files=$(ls -1)
来源：http://hs.panjiajie.cn

[R38] 管道串联
来源：http://ul.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://cj.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://yy.wgjwhj.cn

cmd > out.log 2>&1
来源：http://jx.szxytkj.cn

[R40] 追加写日志
来源：http://te.yuexingan06.cn

echo "log" >> out.log
来源：http://eo.panjiajie.cn

[R41] 丢弃输出
来源：http://jg.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://ur.hnjuh.cn

[R42] 输入重定向
来源：http://rm.hahajie.cn

wc -l < a.txt
来源：http://dk.chemitech.net.cn

[R43] 按名字查找文件
来源：http://bx.jctech888.com.cn

find . -name "*.log" -type f
来源：http://ma.asd995.cn

[R44] 按修改时间查找
来源：http://dp.chemitech.net.cn

find . -mtime -7 -type f
来源：http://ba.hnjuh.cn

[R45] 批量删除
来源：http://tn.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://dc.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://id.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lb.haigaiapp.cn

[R47] sed 单行替换
来源：http://oj.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yj.gzmigu.cn

[R48] awk 取指定列
来源：http://bg.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://uk.jianghongdianzi.cn

[R49] awk 带条件
来源：http://ms.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fc.jianghongdianzi.cn

[R50] awk 求和
来源：http://xu.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ms.asd995.cn

[R51] 排序去重取前几
来源：http://fq.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kw.bookmarksfly.cn

[R52] 统计行数
来源：http://yg.lnxyls.cn

wc -l a.txt
来源：http://hf.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://zm.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rn.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://tx.chemitech.net.cn

diff a.txt b.txt
来源：http://sd.hnjuh.cn

[R55] 压缩与解压
来源：http://wv.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kh.szsharing.cn

[R56] 远程拷贝
来源：http://ff.panjiajie.cn

scp file user@host:/path/
来源：http://tk.newstarts.cn

[R57] 远程执行命令
来源：http://rb.nszjky.cn

ssh user@host 'uptime'
来源：http://cg.9csxet.cn

[R58] 下载文件
来源：http://in.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wf.colortex.cn

[R59] 发 POST JSON
来源：http://uf.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xf.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://hw.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vl.shtwfgs.cn

[R61] 磁盘占用
来源：http://jb.nszjky.cn

df -h;  du -sh *
来源：http://kw.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://ag.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://cw.huanxung.cn

[R63] 内存与进程
来源：http://ag.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://ao.nszjky.cn

[R64] 结束进程
来源：http://rd.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://xo.hahajie.cn

[R65] 查看端口占用
来源：http://fk.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gf.jianghongdianzi.cn

[R66] 定时任务
来源：http://hb.wgjwhj.cn

crontab -e;  crontab -l
来源：http://gy.asd995.cn

[R67] 生成随机十六进制串
来源：http://fl.huanxung.cn

openssl rand -hex 16
来源：http://st.jctech888.com.cn

[R68] 计算文件校验值
来源：http://vr.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ye.521024.cn

[R69] 生成随机密码
来源：http://hu.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://ei.haigaiapp.cn

[R70] 时间戳与互转
来源：http://qa.colortex.cn

date +%s;  date -d @1700000000
来源：http://py.nszjky.cn

[R71] 日期格式化
来源：http://tq.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mg.jctech888.com.cn

[R72] 等待端口就绪
来源：http://ux.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pc.huixinmuqiang.cn

[R73] 分割大日志
来源：http://fi.hahajie.cn

split -l 1000 big.log part_
来源：http://wc.yuexingan06.cn

[R74] 批量重命名
来源：http://zw.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rs.hnjuh.cn

[R75] 导出环境变量
来源：http://kf.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://nx.gzmigu.cn

[R76] 使用临时文件
来源：http://ab.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pe.szxytkj.cn

[R77] 读取用户输入
来源：http://xf.wgjwhj.cn

read -rp "请输入: " ans
来源：http://ug.szsharing.cn

[R78] 交互式菜单
来源：http://ql.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://in.szxytkj.cn

[R79] 解析命令行选项
来源：http://oi.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wj.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://zr.panjiajie.cn

time ./run.sh
来源：http://qv.9csxet.cn

================================================================================
来源：http://pa.hnjuh.cn

S. C / C++ 专题
来源：http://tq.jianghongdianzi.cn

================================================================================
来源：http://vc.521024.cn

[S01] C：Hello World
来源：http://xr.hahajie.cn

#include <stdio.h>
来源：http://wn.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ld.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://vx.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://jh.9csxet.cn

[S03] C：读入整数
来源：http://in.hahajie.cn

int x; scanf("%d", &x);
来源：http://us.nicolike.cn

[S04] C：字符串复制
来源：http://qb.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://af.wgjwhj.cn

[S05] C：字符串长度
来源：http://zn.szxytkj.cn

strlen(s)
来源：http://tn.bjjhwx.cn

[S06] C：字符串比较
来源：http://wk.newstarts.cn

strcmp(a, b) == 0
来源：http://on.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://lx.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vg.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://pj.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xh.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://gr.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qo.asd995.cn

[S10] C：指针与解引用
来源：http://gj.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://dd.hahajie.cn

[S11] C：逐行读文件
来源：http://kf.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://aw.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fr.huixinmuqiang.cn

fclose(f);
来源：http://hx.muxihuayi.cn

[S12] C：写文件
来源：http://it.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hd.bookmarksfly.cn

[S13] C：宏定义
来源：http://ux.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rp.chemitech.net.cn

[S14] C：枚举
来源：http://nc.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://kh.chemitech.net.cn

[S15] C：类型转换
来源：http://ju.muxihuayi.cn

(double) a / b
来源：http://vd.bookmarksfly.cn

[S16] C：位操作置位
来源：http://he.asd995.cn

x |= (1 << 3);
来源：http://nb.nszjky.cn

[S17] C：安全拼接字符串
来源：http://ce.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ob.hahajie.cn

[S18] C：命令行参数
来源：http://ys.wgjwhj.cn

int main(int argc, char **argv)
来源：http://ms.nicolike.cn

[S19] C：快速排序
来源：http://bl.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dy.muxihuayi.cn

[S20] C：二分查找
来源：http://xk.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vt.9csxet.cn

[S21] C：字符类别判断
来源：http://yx.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://id.hahajie.cn

[S22] C：字符串转数字
来源：http://oh.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xu.szsharing.cn

[S23] C：随机数
来源：http://yk.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xw.szxytkj.cn

[S24] C：获取本地时间
来源：http://ko.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jo.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://rp.newstarts.cn

memcpy(dst, src, n);
来源：http://ik.wgjwhj.cn

[S26] C：内存清零
来源：http://li.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://hz.yuexingan06.cn

[S27] C：定义常量
来源：http://be.szsharing.cn

const double PI = 3.14159;
来源：http://tw.asd995.cn

[S28] C：静态变量
来源：http://xb.shtwfgs.cn

static int counter = 0;
来源：http://zi.haigaiapp.cn

[S29] C：变参函数
来源：http://go.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tj.hnjuh.cn

[S30] C：头文件保护
来源：http://wa.muxihuayi.cn

#ifndef X_H
来源：http://pb.szxytkj.cn

#define X_H
来源：http://mc.jctech888.com.cn

#endif
来源：http://xu.nicolike.cn

[S31] C++：Hello World
来源：http://hj.jianghongdianzi.cn

#include <iostream>
来源：http://hx.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://aq.muxihuayi.cn

[S32] C++：字符串
来源：http://fe.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://cn.shxzukj.cn

[S33] C++：vector 增删
来源：http://hz.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wr.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://lz.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://rw.shxzskj.cn

[S35] C++：map
来源：http://fj.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kd.nicolike.cn

[S36] C++：unordered_map
来源：http://tc.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sw.muxihuayi.cn

[S37] C++：set
来源：http://wd.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fn.wgjwhj.cn

[S38] C++：排序
来源：http://ca.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://qz.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://co.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zt.wgjwhj.cn

[S40] C++：查找元素
来源：http://cj.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hm.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://uz.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sg.szsharing.cn

[S42] C++：继承与虚函数
来源：http://xh.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://px.asd995.cn

[S43] C++：智能指针
来源：http://sd.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://eg.colortex.cn

[S44] C++：引用传参
来源：http://qy.9csxet.cn

void inc(int &x) { ++x; }
来源：http://mx.huanxung.cn

[S45] C++：lambda
来源：http://fv.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ex.gzmigu.cn

[S46] C++：函数模板
来源：http://eb.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://we.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://kw.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nm.szxytkj.cn

[S48] C++：逐行读文件
来源：http://la.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mp.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://bj.asd995.cn

[S49] C++：写文件
来源：http://sy.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gc.521024.cn

[S50] C++：格式化数字
来源：http://nv.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xd.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://eu.lnxyls.cn

static_cast<double>(a) / b
来源：http://yy.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://wa.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://pi.szxytkj.cn

[S53] C++：移动语义
来源：http://ud.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://eo.hnjuh.cn

[S54] C++：异常处理
来源：http://ar.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vf.colortex.cn

[S55] C++：结构化绑定
来源：http://az.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vh.gzmigu.cn

[S56] C++：optional
来源：http://eb.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hv.chemitech.net.cn

[S57] C++：编译期常量
来源：http://tx.bjjhwx.cn

constexpr int N = 10;
来源：http://ie.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://xa.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://ic.shxzukj.cn

[S59] C++：静态断言
来源：http://wh.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xa.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://vf.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xl.huanxung.cn

================================================================================
来源：http://uf.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tt.nszjky.cn

================================================================================
来源：http://pk.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://wo.huixinmuqiang.cn

println("Hello")
来源：http://zq.shxzskj.cn

[T02] Kotlin：变量
来源：http://dz.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uq.wgjwhj.cn


<!-- 参考信息 -->