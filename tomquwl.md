代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vb.bookmarksfly.cn

[Q90] 生成序号列
来源：http://nz.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jh.nszjky.cn

================================================================================
来源：http://jh.nszjky.cn

R. Bash 专题
来源：http://ar.muxihuayi.cn

================================================================================
来源：http://vz.9csxet.cn

[R01] shebang 与严格模式
来源：http://go.bjjhwx.cn

#!/usr/bin/env bash
来源：http://fw.bjjhwx.cn

set -euo pipefail
来源：http://ah.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://ez.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://kz.lnxyls.cn

[R03] 只读变量
来源：http://uc.shxzskj.cn

readonly PI=3.14
来源：http://sg.colortex.cn

[R04] 位置参数
来源：http://ik.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ir.haigaiapp.cn

[R05] 参数默认值
来源：http://ec.szsharing.cn

name="${1:-default}"
来源：http://gg.newstarts.cn

[R06] 判断命令是否存在
来源：http://iy.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gq.521024.cn

[R07] if 判断文件
来源：http://qq.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tb.szxytkj.cn

[R08] 数值比较
来源：http://qy.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://or.szsharing.cn

[R09] 字符串比较
来源：http://co.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bt.yuntaijiaju.cn

[R10] 正则匹配
来源：http://pf.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cs.wgjwhj.cn

[R11] case 多分支
来源：http://jk.colortex.cn

case "$1" in
来源：http://wd.szxytkj.cn

start) echo "启动" ;;
来源：http://ij.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://in.9csxet.cn

*)     echo "未知命令" ;;
来源：http://fj.nszjky.cn

esac
来源：http://yd.panjiajie.cn

[R12] for 遍历文件
来源：http://pm.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://xq.yuntaijiaju.cn

[R13] for 计数循环
来源：http://ed.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://qv.wgjwhj.cn

[R14] C 风格 for
来源：http://kd.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mt.huixiangedu.cn

[R15] while 逐行读文件
来源：http://qx.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mu.chemitech.net.cn

[R16] until 等待条件
来源：http://ib.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://co.yuexingan06.cn

[R17] 数组定义与取值
来源：http://ol.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ep.gzmigu.cn

[R18] 遍历数组
来源：http://co.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ac.nicolike.cn

[R19] 数组长度
来源：http://ph.huanxung.cn

echo "${#arr[@]}"
来源：http://sg.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://iz.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gz.panjiajie.cn

[R21] 字符串长度
来源：http://ix.yuntaijiaju.cn

echo "${#s}"
来源：http://en.huanxung.cn

[R22] 截取子串
来源：http://ix.huixiangedu.cn

echo "${s:0:5}"
来源：http://wp.521024.cn

[R23] 字符串替换
来源：http://dl.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://id.muxihuayi.cn

[R24] 大小写转换
来源：http://kg.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zx.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://fc.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yg.nszjky.cn

[R26] 命令替换
来源：http://yt.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://ja.bjjhwx.cn

[R27] 算术展开
来源：http://rt.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://fj.shtwfgs.cn

[R28] 浮点运算
来源：http://rs.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://fx.yuntaijiaju.cn

[R29] 定义函数
来源：http://mp.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qs.shtwfgs.cn

[R30] 函数返回状态码
来源：http://pd.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://kn.lnxyls.cn

[R31] 局部变量
来源：http://mt.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://zu.szsharing.cn

[R32] 参数个数校验
来源：http://vh.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rr.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://kv.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dw.hnjuh.cn

[R34] 退出时清理
来源：http://rd.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://za.nszjky.cn

[R35] 后台执行并等待
来源：http://ve.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bn.9csxet.cn

[R36] 并发执行多个任务
来源：http://al.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pl.shxzskj.cn

[R37] 把输出赋给变量
来源：http://bu.muxihuayi.cn

files=$(ls -1)
来源：http://cb.bjjhwx.cn

[R38] 管道串联
来源：http://mz.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://zw.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://gb.bjjhwx.cn

cmd > out.log 2>&1
来源：http://ik.nicolike.cn

[R40] 追加写日志
来源：http://rt.muxihuayi.cn

echo "log" >> out.log
来源：http://kt.muxihuayi.cn

[R41] 丢弃输出
来源：http://ob.nszjky.cn

cmd >/dev/null 2>&1
来源：http://lq.colortex.cn

[R42] 输入重定向
来源：http://yg.haigaiapp.cn

wc -l < a.txt
来源：http://ui.huixiangedu.cn

[R43] 按名字查找文件
来源：http://rl.yuexingan06.cn

find . -name "*.log" -type f
来源：http://bb.colortex.cn

[R44] 按修改时间查找
来源：http://jp.jctech888.com.cn

find . -mtime -7 -type f
来源：http://ge.gzmigu.cn

[R45] 批量删除
来源：http://hq.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://wv.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://xq.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yz.huixiangedu.cn

[R47] sed 单行替换
来源：http://fp.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dl.panjiajie.cn

[R48] awk 取指定列
来源：http://gh.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://km.muxihuayi.cn

[R49] awk 带条件
来源：http://sy.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xq.jctech888.com.cn

[R50] awk 求和
来源：http://vc.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lb.szxytkj.cn

[R51] 排序去重取前几
来源：http://wq.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://do.chemitech.net.cn

[R52] 统计行数
来源：http://mr.wgjwhj.cn

wc -l a.txt
来源：http://gj.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://lr.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ad.panjiajie.cn

[R54] 比较两个文件
来源：http://fw.nicolike.cn

diff a.txt b.txt
来源：http://cq.nicolike.cn

[R55] 压缩与解压
来源：http://lt.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lv.szsharing.cn

[R56] 远程拷贝
来源：http://ea.lnxyls.cn

scp file user@host:/path/
来源：http://nr.muxihuayi.cn

[R57] 远程执行命令
来源：http://re.huanxung.cn

ssh user@host 'uptime'
来源：http://qi.shtwfgs.cn

[R58] 下载文件
来源：http://te.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dh.nicolike.cn

[R59] 发 POST JSON
来源：http://to.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://we.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://lp.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ti.bookmarksfly.cn

[R61] 磁盘占用
来源：http://nj.9csxet.cn

df -h;  du -sh *
来源：http://xy.asd995.cn

[R62] 找最占空间的文件
来源：http://te.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://dz.bookmarksfly.cn

[R63] 内存与进程
来源：http://dz.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://tn.asd995.cn

[R64] 结束进程
来源：http://dz.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://oy.521024.cn

[R65] 查看端口占用
来源：http://jc.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ue.colortex.cn

[R66] 定时任务
来源：http://qg.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://ou.huanxung.cn

[R67] 生成随机十六进制串
来源：http://su.huixiangedu.cn

openssl rand -hex 16
来源：http://ce.muxihuayi.cn

[R68] 计算文件校验值
来源：http://hv.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ct.szsharing.cn

[R69] 生成随机密码
来源：http://co.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://eq.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://bf.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://km.nicolike.cn

[R71] 日期格式化
来源：http://va.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wi.wgjwhj.cn

[R72] 等待端口就绪
来源：http://ca.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vm.hahajie.cn

[R73] 分割大日志
来源：http://ys.hnjuh.cn

split -l 1000 big.log part_
来源：http://ys.wgjwhj.cn

[R74] 批量重命名
来源：http://eq.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eu.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://ua.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://bk.asd995.cn

[R76] 使用临时文件
来源：http://dm.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yg.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://kg.wgjwhj.cn

read -rp "请输入: " ans
来源：http://kt.huixiangedu.cn

[R78] 交互式菜单
来源：http://qz.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ez.shxzskj.cn

[R79] 解析命令行选项
来源：http://dp.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hd.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://jj.521024.cn

time ./run.sh
来源：http://lc.szsharing.cn

================================================================================
来源：http://xt.bjjhwx.cn

S. C / C++ 专题
来源：http://jv.chemitech.net.cn

================================================================================
来源：http://am.521024.cn

[S01] C：Hello World
来源：http://hl.wgjwhj.cn

#include <stdio.h>
来源：http://gu.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ey.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://jo.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://bp.nicolike.cn

[S03] C：读入整数
来源：http://mc.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://rc.yuexingan06.cn

[S04] C：字符串复制
来源：http://ow.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ed.lnxyls.cn

[S05] C：字符串长度
来源：http://ha.wgjwhj.cn

strlen(s)
来源：http://ke.521024.cn

[S06] C：字符串比较
来源：http://ik.szsharing.cn

strcmp(a, b) == 0
来源：http://yo.9csxet.cn

[S07] C：数组遍历求和
来源：http://fw.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kr.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://lm.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ej.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://ma.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ee.nicolike.cn

[S10] C：指针与解引用
来源：http://yi.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://vi.shxzskj.cn

[S11] C：逐行读文件
来源：http://mo.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://nz.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ky.jctech888.com.cn

fclose(f);
来源：http://te.asd995.cn

[S12] C：写文件
来源：http://zv.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zb.jianghongdianzi.cn

[S13] C：宏定义
来源：http://ee.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nb.shxzukj.cn

[S14] C：枚举
来源：http://ft.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://uq.jctech888.com.cn

[S15] C：类型转换
来源：http://ic.huixiangedu.cn

(double) a / b
来源：http://nk.chemitech.net.cn

[S16] C：位操作置位
来源：http://aq.9csxet.cn

x |= (1 << 3);
来源：http://rm.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://hl.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ln.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://an.colortex.cn

int main(int argc, char **argv)
来源：http://pv.shxzukj.cn

[S19] C：快速排序
来源：http://al.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ya.bjjhwx.cn

[S20] C：二分查找
来源：http://xv.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iw.asd995.cn

[S21] C：字符类别判断
来源：http://tm.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cd.asd995.cn

[S22] C：字符串转数字
来源：http://yv.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qs.jianghongdianzi.cn

[S23] C：随机数
来源：http://wz.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uv.nszjky.cn

[S24] C：获取本地时间
来源：http://sl.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ld.shxzukj.cn

[S25] C：内存拷贝
来源：http://zy.jctech888.com.cn

memcpy(dst, src, n);
来源：http://ec.bookmarksfly.cn

[S26] C：内存清零
来源：http://jn.nszjky.cn

memset(a, 0, sizeof a);
来源：http://xn.yuexingan06.cn

[S27] C：定义常量
来源：http://qu.shtwfgs.cn

const double PI = 3.14159;
来源：http://yi.huixiangedu.cn

[S28] C：静态变量
来源：http://hr.newstarts.cn

static int counter = 0;
来源：http://xf.haigaiapp.cn

[S29] C：变参函数
来源：http://ks.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mu.panjiajie.cn

[S30] C：头文件保护
来源：http://eb.521024.cn

#ifndef X_H
来源：http://up.521024.cn

#define X_H
来源：http://hf.chemitech.net.cn

#endif
来源：http://uu.hahajie.cn

[S31] C++：Hello World
来源：http://ly.shxzskj.cn

#include <iostream>
来源：http://ta.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://su.nszjky.cn

[S32] C++：字符串
来源：http://rk.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://os.wgjwhj.cn

[S33] C++：vector 增删
来源：http://fy.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zd.panjiajie.cn

[S34] C++：遍历 vector
来源：http://th.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://hf.yuexingan06.cn

[S35] C++：map
来源：http://jz.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fr.shxzskj.cn

[S36] C++：unordered_map
来源：http://zo.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zz.hnjuh.cn

[S37] C++：set
来源：http://xg.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnjuh.cn

[S38] C++：排序
来源：http://eb.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://fo.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://ma.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cj.nicolike.cn

[S40] C++：查找元素
来源：http://xu.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tq.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://cz.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rq.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://ip.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://qh.asd995.cn

[S43] C++：智能指针
来源：http://po.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://uz.hnjuh.cn

[S44] C++：引用传参
来源：http://mx.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://ch.521024.cn

[S45] C++：lambda
来源：http://lw.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xr.lnxyls.cn

[S46] C++：函数模板
来源：http://jf.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://po.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://ns.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gj.panjiajie.cn

[S48] C++：逐行读文件
来源：http://sl.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rm.521024.cn

while (std::getline(in, line)) { }
来源：http://lo.yuexingan06.cn

[S49] C++：写文件
来源：http://sf.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bt.huixiangedu.cn

[S50] C++：格式化数字
来源：http://it.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dl.lnxyls.cn

[S51] C++：显式类型转换
来源：http://my.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://rk.521024.cn

[S52] C++：const 与 noexcept
来源：http://mf.asd995.cn

int size() const noexcept { return n_; }
来源：http://nh.hnjuh.cn

[S53] C++：移动语义
来源：http://nd.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://ki.9csxet.cn

[S54] C++：异常处理
来源：http://oy.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://re.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://ka.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vh.9csxet.cn

[S56] C++：optional
来源：http://rk.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ob.muxihuayi.cn

[S57] C++：编译期常量
来源：http://jq.nicolike.cn

constexpr int N = 10;
来源：http://qw.newstarts.cn

[S58] C++：命名空间
来源：http://st.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://pl.szxytkj.cn

[S59] C++：静态断言
来源：http://fc.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ad.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://mk.nicolike.cn


<!-- 参考信息 -->