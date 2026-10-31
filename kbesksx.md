代发 wailian999

name="${1:-default}"
来源：http://rr.nicolike.cn

[R06] 判断命令是否存在
来源：http://sf.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yh.gzmigu.cn

[R07] if 判断文件
来源：http://uh.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qt.panjiajie.cn

[R08] 数值比较
来源：http://tg.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zk.jianghongdianzi.cn

[R09] 字符串比较
来源：http://gr.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yk.jctech888.com.cn

[R10] 正则匹配
来源：http://pv.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oi.huanxung.cn

[R11] case 多分支
来源：http://ie.huanxung.cn

case "$1" in
来源：http://rc.lnxyls.cn

start) echo "启动" ;;
来源：http://km.nszjky.cn

stop)  echo "停止" ;;
来源：http://fn.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://nj.lnxyls.cn

esac
来源：http://jt.muxihuayi.cn

[R12] for 遍历文件
来源：http://zn.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://if.bookmarksfly.cn

[R13] for 计数循环
来源：http://vb.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://xi.bookmarksfly.cn

[R14] C 风格 for
来源：http://nn.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mi.nszjky.cn

[R15] while 逐行读文件
来源：http://an.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wr.521024.cn

[R16] until 等待条件
来源：http://pu.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sh.szsharing.cn

[R17] 数组定义与取值
来源：http://lk.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ms.521024.cn

[R18] 遍历数组
来源：http://lj.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://te.huixiangedu.cn

[R19] 数组长度
来源：http://lt.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://pa.szsharing.cn

[R20] 关联数组（字典）
来源：http://ff.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ug.nszjky.cn

[R21] 字符串长度
来源：http://up.yuexingan06.cn

echo "${#s}"
来源：http://nz.nszjky.cn

[R22] 截取子串
来源：http://sa.colortex.cn

echo "${s:0:5}"
来源：http://nt.szxytkj.cn

[R23] 字符串替换
来源：http://ni.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pt.bjjhwx.cn

[R24] 大小写转换
来源：http://wi.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bf.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://wf.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://up.szxytkj.cn

[R26] 命令替换
来源：http://js.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://us.nicolike.cn

[R27] 算术展开
来源：http://hi.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://ku.asd995.cn

[R28] 浮点运算
来源：http://tw.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://uh.nicolike.cn

[R29] 定义函数
来源：http://zq.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sl.nicolike.cn

[R30] 函数返回状态码
来源：http://ix.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://ui.bookmarksfly.cn

[R31] 局部变量
来源：http://pg.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://la.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://ae.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mb.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://ot.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nj.gzmigu.cn

[R34] 退出时清理
来源：http://hc.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dm.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://am.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://do.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://ib.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lv.panjiajie.cn

[R37] 把输出赋给变量
来源：http://pq.hahajie.cn

files=$(ls -1)
来源：http://kb.huixinmuqiang.cn

[R38] 管道串联
来源：http://uk.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://tg.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://kj.muxihuayi.cn

cmd > out.log 2>&1
来源：http://qv.huanxung.cn

[R40] 追加写日志
来源：http://dw.colortex.cn

echo "log" >> out.log
来源：http://du.chemitech.net.cn

[R41] 丢弃输出
来源：http://hg.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://lt.521024.cn

[R42] 输入重定向
来源：http://cc.asd995.cn

wc -l < a.txt
来源：http://tf.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://ky.shtwfgs.cn

find . -name "*.log" -type f
来源：http://us.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://os.jctech888.com.cn

find . -mtime -7 -type f
来源：http://mr.shxzskj.cn

[R45] 批量删除
来源：http://sx.szsharing.cn

find . -name "*.tmp" -delete
来源：http://mt.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://sx.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mv.szxytkj.cn

[R47] sed 单行替换
来源：http://en.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jd.shtwfgs.cn

[R48] awk 取指定列
来源：http://ql.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://ut.nicolike.cn

[R49] awk 带条件
来源：http://wn.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tw.9csxet.cn

[R50] awk 求和
来源：http://ie.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wo.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://ve.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tz.yuexingan06.cn

[R52] 统计行数
来源：http://jk.panjiajie.cn

wc -l a.txt
来源：http://bi.asd995.cn

[R53] 查看文件头与实时尾
来源：http://xt.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gc.lnxyls.cn

[R54] 比较两个文件
来源：http://jc.jctech888.com.cn

diff a.txt b.txt
来源：http://xw.9csxet.cn

[R55] 压缩与解压
来源：http://bq.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://br.panjiajie.cn

[R56] 远程拷贝
来源：http://pv.521024.cn

scp file user@host:/path/
来源：http://nu.nszjky.cn

[R57] 远程执行命令
来源：http://lk.gzmigu.cn

ssh user@host 'uptime'
来源：http://md.jianghongdianzi.cn

[R58] 下载文件
来源：http://dd.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aw.gzmigu.cn

[R59] 发 POST JSON
来源：http://ff.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gl.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://rt.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zf.haigaiapp.cn

[R61] 磁盘占用
来源：http://aj.shxzskj.cn

df -h;  du -sh *
来源：http://dn.nicolike.cn

[R62] 找最占空间的文件
来源：http://fm.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://my.bjjhwx.cn

[R63] 内存与进程
来源：http://ui.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://gs.newstarts.cn

[R64] 结束进程
来源：http://vj.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://ej.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://lv.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mk.shxzukj.cn

[R66] 定时任务
来源：http://fb.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://zs.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://gw.yuntaijiaju.cn

openssl rand -hex 16
来源：http://vq.yuexingan06.cn

[R68] 计算文件校验值
来源：http://zr.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hj.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://rv.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://kb.nszjky.cn

[R70] 时间戳与互转
来源：http://vz.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://ti.hnjuh.cn

[R71] 日期格式化
来源：http://sz.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fp.nszjky.cn

[R72] 等待端口就绪
来源：http://aq.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://en.jctech888.com.cn

[R73] 分割大日志
来源：http://ko.haigaiapp.cn

split -l 1000 big.log part_
来源：http://va.colortex.cn

[R74] 批量重命名
来源：http://uw.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ky.nszjky.cn

[R75] 导出环境变量
来源：http://te.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://yf.chemitech.net.cn

[R76] 使用临时文件
来源：http://uv.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://id.lnxyls.cn

[R77] 读取用户输入
来源：http://iu.hahajie.cn

read -rp "请输入: " ans
来源：http://te.shxzukj.cn

[R78] 交互式菜单
来源：http://ta.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ul.bjjhwx.cn

[R79] 解析命令行选项
来源：http://nn.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lh.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://is.chemitech.net.cn

time ./run.sh
来源：http://hv.muxihuayi.cn

================================================================================
来源：http://gz.shxzskj.cn

S. C / C++ 专题
来源：http://ug.hnjuh.cn

================================================================================
来源：http://sj.shxzskj.cn

[S01] C：Hello World
来源：http://el.shxzukj.cn

#include <stdio.h>
来源：http://rh.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gp.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://by.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://li.shxzukj.cn

[S03] C：读入整数
来源：http://ho.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://fu.gzmigu.cn

[S04] C：字符串复制
来源：http://zd.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qz.521024.cn

[S05] C：字符串长度
来源：http://oi.9csxet.cn

strlen(s)
来源：http://vt.shxzskj.cn

[S06] C：字符串比较
来源：http://qg.szsharing.cn

strcmp(a, b) == 0
来源：http://ya.huanxung.cn

[S07] C：数组遍历求和
来源：http://gh.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nm.521024.cn

[S08] C：动态内存分配与释放
来源：http://wz.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xq.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://zx.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://an.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://hj.9csxet.cn

int *p = &a;  *p = 5;
来源：http://vq.szxytkj.cn

[S11] C：逐行读文件
来源：http://yv.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://gq.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mj.9csxet.cn

fclose(f);
来源：http://ja.9csxet.cn

[S12] C：写文件
来源：http://rh.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bt.shxzskj.cn

[S13] C：宏定义
来源：http://rn.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://an.jctech888.com.cn

[S14] C：枚举
来源：http://ip.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://rf.nszjky.cn

[S15] C：类型转换
来源：http://nr.shxzukj.cn

(double) a / b
来源：http://gd.huixiangedu.cn

[S16] C：位操作置位
来源：http://np.wgjwhj.cn

x |= (1 << 3);
来源：http://ca.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://ob.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qs.asd995.cn

[S18] C：命令行参数
来源：http://ic.panjiajie.cn

int main(int argc, char **argv)
来源：http://zm.yuexingan06.cn

[S19] C：快速排序
来源：http://cl.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ku.chemitech.net.cn

[S20] C：二分查找
来源：http://hr.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://af.bjjhwx.cn

[S21] C：字符类别判断
来源：http://rz.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://so.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://eb.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qb.bjjhwx.cn

[S23] C：随机数
来源：http://st.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xv.shxzskj.cn

[S24] C：获取本地时间
来源：http://vm.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nv.9csxet.cn

[S25] C：内存拷贝
来源：http://xb.huanxung.cn

memcpy(dst, src, n);
来源：http://sx.9csxet.cn

[S26] C：内存清零
来源：http://cv.newstarts.cn

memset(a, 0, sizeof a);
来源：http://ea.bookmarksfly.cn

[S27] C：定义常量
来源：http://vx.wgjwhj.cn

const double PI = 3.14159;
来源：http://cb.hnjuh.cn

[S28] C：静态变量
来源：http://vi.colortex.cn

static int counter = 0;
来源：http://ad.chemitech.net.cn

[S29] C：变参函数
来源：http://ra.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fp.colortex.cn

[S30] C：头文件保护
来源：http://ep.huanxung.cn

#ifndef X_H
来源：http://xl.haigaiapp.cn

#define X_H
来源：http://dl.lnxyls.cn

#endif
来源：http://gl.szsharing.cn

[S31] C++：Hello World
来源：http://uq.wgjwhj.cn

#include <iostream>
来源：http://mg.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://xl.bjjhwx.cn

[S32] C++：字符串
来源：http://kt.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://vc.asd995.cn

[S33] C++：vector 增删
来源：http://jw.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://me.hahajie.cn

[S34] C++：遍历 vector
来源：http://iz.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://xv.shxzskj.cn

[S35] C++：map
来源：http://re.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wj.nicolike.cn

[S36] C++：unordered_map
来源：http://hk.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uk.gzmigu.cn

[S37] C++：set
来源：http://al.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mv.bookmarksfly.cn

[S38] C++：排序
来源：http://lf.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://lq.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://oa.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xn.nszjky.cn

[S40] C++：查找元素
来源：http://uo.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vu.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://rg.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yu.colortex.cn

[S42] C++：继承与虚函数
来源：http://zc.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://pg.bjjhwx.cn

[S43] C++：智能指针
来源：http://au.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://kd.jctech888.com.cn

[S44] C++：引用传参
来源：http://cn.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://fh.newstarts.cn

[S45] C++：lambda
来源：http://ep.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oy.lnxyls.cn

[S46] C++：函数模板
来源：http://af.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yw.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://vv.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yo.nszjky.cn

[S48] C++：逐行读文件
来源：http://eo.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jq.colortex.cn

while (std::getline(in, line)) { }
来源：http://cu.huixiangedu.cn

[S49] C++：写文件
来源：http://hl.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nr.yuexingan06.cn

[S50] C++：格式化数字
来源：http://ix.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xh.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://xd.jctech888.com.cn

static_cast<double>(a) / b
来源：http://wm.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://sw.hahajie.cn

int size() const noexcept { return n_; }
来源：http://uu.yuexingan06.cn

[S53] C++：移动语义
来源：http://sy.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://pg.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://hg.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ry.shxzskj.cn

[S55] C++：结构化绑定
来源：http://er.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ar.bjjhwx.cn

[S56] C++：optional
来源：http://cb.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wh.lnxyls.cn

[S57] C++：编译期常量
来源：http://zq.hnjuh.cn

constexpr int N = 10;
来源：http://cr.shxzskj.cn

[S58] C++：命名空间
来源：http://pj.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://sd.nicolike.cn

[S59] C++：静态断言
来源：http://jy.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://od.521024.cn

[S60] C++：遍历并删除元素
来源：http://nq.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://us.shxzukj.cn

================================================================================
来源：http://qb.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xw.huixinmuqiang.cn

================================================================================
来源：http://rb.9csxet.cn

[T01] Kotlin：Hello World
来源：http://vk.521024.cn

println("Hello")
来源：http://vi.shtwfgs.cn

[T02] Kotlin：变量
来源：http://wf.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mr.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://am.shtwfgs.cn

"值: $b"
来源：http://xs.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://vo.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://iy.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://ue.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jn.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://ta.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rr.chemitech.net.cn


<!-- 参考信息 -->