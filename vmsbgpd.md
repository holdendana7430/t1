代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ot.szxytkj.cn

[Q90] 生成序号列
来源：http://cv.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ti.muxihuayi.cn

================================================================================
来源：http://wd.yuntaijiaju.cn

R. Bash 专题
来源：http://fx.panjiajie.cn

================================================================================
来源：http://zg.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://ma.haigaiapp.cn

#!/usr/bin/env bash
来源：http://op.colortex.cn

set -euo pipefail
来源：http://bx.shxzukj.cn

[R02] 变量赋值与使用
来源：http://fs.shxzskj.cn

name="Tom"; echo "$name"
来源：http://mp.gzmigu.cn

[R03] 只读变量
来源：http://nw.szsharing.cn

readonly PI=3.14
来源：http://ui.newstarts.cn

[R04] 位置参数
来源：http://sa.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vn.shxzskj.cn

[R05] 参数默认值
来源：http://er.jctech888.com.cn

name="${1:-default}"
来源：http://vp.newstarts.cn

[R06] 判断命令是否存在
来源：http://ys.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fw.szxytkj.cn

[R07] if 判断文件
来源：http://sl.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dc.haigaiapp.cn

[R08] 数值比较
来源：http://zu.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gd.szxytkj.cn

[R09] 字符串比较
来源：http://hb.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ko.yuntaijiaju.cn

[R10] 正则匹配
来源：http://xo.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qq.newstarts.cn

[R11] case 多分支
来源：http://fq.szxytkj.cn

case "$1" in
来源：http://vl.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://jm.9csxet.cn

stop)  echo "停止" ;;
来源：http://zj.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://dv.lnxyls.cn

esac
来源：http://lp.jctech888.com.cn

[R12] for 遍历文件
来源：http://je.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://qd.huixinmuqiang.cn

[R13] for 计数循环
来源：http://ox.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://uk.bjjhwx.cn

[R14] C 风格 for
来源：http://sh.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qq.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://kj.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bb.huixiangedu.cn

[R16] until 等待条件
来源：http://ff.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xi.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://lj.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nn.lnxyls.cn

[R18] 遍历数组
来源：http://ri.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fh.huixiangedu.cn

[R19] 数组长度
来源：http://sb.shxzukj.cn

echo "${#arr[@]}"
来源：http://zp.gzmigu.cn

[R20] 关联数组（字典）
来源：http://ux.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://by.jctech888.com.cn

[R21] 字符串长度
来源：http://xe.nicolike.cn

echo "${#s}"
来源：http://fm.nszjky.cn

[R22] 截取子串
来源：http://ae.chemitech.net.cn

echo "${s:0:5}"
来源：http://ne.shtwfgs.cn

[R23] 字符串替换
来源：http://zy.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gf.hnjuh.cn

[R24] 大小写转换
来源：http://ra.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mx.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://nq.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ay.bjjhwx.cn

[R26] 命令替换
来源：http://iq.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://gq.jianghongdianzi.cn

[R27] 算术展开
来源：http://ox.asd995.cn

echo $((1 + 2 * 3))
来源：http://oq.panjiajie.cn

[R28] 浮点运算
来源：http://tl.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://lo.521024.cn

[R29] 定义函数
来源：http://wy.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eb.huixiangedu.cn

[R30] 函数返回状态码
来源：http://rt.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://tk.haigaiapp.cn

[R31] 局部变量
来源：http://ez.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://rg.szxytkj.cn

[R32] 参数个数校验
来源：http://iz.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zw.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://qa.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ov.huanxung.cn

[R34] 退出时清理
来源：http://re.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qu.hahajie.cn

[R35] 后台执行并等待
来源：http://xx.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bq.szxytkj.cn

[R36] 并发执行多个任务
来源：http://id.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bk.szxytkj.cn

[R37] 把输出赋给变量
来源：http://fy.gzmigu.cn

files=$(ls -1)
来源：http://cz.muxihuayi.cn

[R38] 管道串联
来源：http://yl.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://qt.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://vq.shtwfgs.cn

cmd > out.log 2>&1
来源：http://vh.nicolike.cn

[R40] 追加写日志
来源：http://aw.hahajie.cn

echo "log" >> out.log
来源：http://yk.wgjwhj.cn

[R41] 丢弃输出
来源：http://xo.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://xk.colortex.cn

[R42] 输入重定向
来源：http://fx.asd995.cn

wc -l < a.txt
来源：http://jq.gzmigu.cn

[R43] 按名字查找文件
来源：http://sg.shtwfgs.cn

find . -name "*.log" -type f
来源：http://za.gzmigu.cn

[R44] 按修改时间查找
来源：http://jy.hnjuh.cn

find . -mtime -7 -type f
来源：http://qa.huixiangedu.cn

[R45] 批量删除
来源：http://gj.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://ld.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://fs.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yx.haigaiapp.cn

[R47] sed 单行替换
来源：http://ng.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vq.haigaiapp.cn

[R48] awk 取指定列
来源：http://jl.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://es.nicolike.cn

[R49] awk 带条件
来源：http://lz.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pw.9csxet.cn

[R50] awk 求和
来源：http://uj.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gk.nszjky.cn

[R51] 排序去重取前几
来源：http://au.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://og.haigaiapp.cn

[R52] 统计行数
来源：http://aa.bookmarksfly.cn

wc -l a.txt
来源：http://pz.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://gq.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bp.shxzukj.cn

[R54] 比较两个文件
来源：http://bb.huanxung.cn

diff a.txt b.txt
来源：http://ya.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://iz.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mx.huixiangedu.cn

[R56] 远程拷贝
来源：http://xq.huixinmuqiang.cn

scp file user@host:/path/
来源：http://ql.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://ka.shxzskj.cn

ssh user@host 'uptime'
来源：http://cz.9csxet.cn

[R58] 下载文件
来源：http://tw.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vh.hahajie.cn

[R59] 发 POST JSON
来源：http://dp.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://aw.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://fd.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bg.lnxyls.cn

[R61] 磁盘占用
来源：http://cv.haigaiapp.cn

df -h;  du -sh *
来源：http://ay.panjiajie.cn

[R62] 找最占空间的文件
来源：http://cn.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://nr.lnxyls.cn

[R63] 内存与进程
来源：http://bw.asd995.cn

free -h;  ps aux | grep nginx
来源：http://wn.panjiajie.cn

[R64] 结束进程
来源：http://zl.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://az.szxytkj.cn

[R65] 查看端口占用
来源：http://rt.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://py.9csxet.cn

[R66] 定时任务
来源：http://ac.huixiangedu.cn

crontab -e;  crontab -l
来源：http://ly.asd995.cn

[R67] 生成随机十六进制串
来源：http://mi.jianghongdianzi.cn

openssl rand -hex 16
来源：http://ex.nicolike.cn

[R68] 计算文件校验值
来源：http://wc.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mz.nicolike.cn

[R69] 生成随机密码
来源：http://xf.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://in.bjjhwx.cn

[R70] 时间戳与互转
来源：http://rg.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://ts.jianghongdianzi.cn

[R71] 日期格式化
来源：http://sq.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sw.asd995.cn

[R72] 等待端口就绪
来源：http://nt.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kd.nszjky.cn

[R73] 分割大日志
来源：http://lz.huixiangedu.cn

split -l 1000 big.log part_
来源：http://jh.gzmigu.cn

[R74] 批量重命名
来源：http://qc.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mj.colortex.cn

[R75] 导出环境变量
来源：http://ne.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://ps.gzmigu.cn

[R76] 使用临时文件
来源：http://do.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gy.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://yd.nicolike.cn

read -rp "请输入: " ans
来源：http://kt.shtwfgs.cn

[R78] 交互式菜单
来源：http://hz.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hr.hahajie.cn

[R79] 解析命令行选项
来源：http://bw.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://as.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://vb.yuexingan06.cn

time ./run.sh
来源：http://zf.bjjhwx.cn

================================================================================
来源：http://qx.wgjwhj.cn

S. C / C++ 专题
来源：http://ys.521024.cn

================================================================================
来源：http://oh.muxihuayi.cn

[S01] C：Hello World
来源：http://of.jianghongdianzi.cn

#include <stdio.h>
来源：http://xp.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ld.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://qz.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://vh.shtwfgs.cn

[S03] C：读入整数
来源：http://bd.huanxung.cn

int x; scanf("%d", &x);
来源：http://wi.bookmarksfly.cn

[S04] C：字符串复制
来源：http://is.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oj.shtwfgs.cn

[S05] C：字符串长度
来源：http://jp.szxytkj.cn

strlen(s)
来源：http://ug.asd995.cn

[S06] C：字符串比较
来源：http://zo.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://cq.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://iu.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ya.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://oy.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kc.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://lb.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eb.nicolike.cn

[S10] C：指针与解引用
来源：http://ll.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://af.nszjky.cn

[S11] C：逐行读文件
来源：http://hr.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://hr.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://er.newstarts.cn

fclose(f);
来源：http://ao.newstarts.cn

[S12] C：写文件
来源：http://nd.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rx.newstarts.cn

[S13] C：宏定义
来源：http://vx.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ol.huixinmuqiang.cn

[S14] C：枚举
来源：http://iy.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://rq.muxihuayi.cn

[S15] C：类型转换
来源：http://om.newstarts.cn

(double) a / b
来源：http://db.szsharing.cn

[S16] C：位操作置位
来源：http://ll.gzmigu.cn

x |= (1 << 3);
来源：http://kp.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://zy.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zm.hahajie.cn

[S18] C：命令行参数
来源：http://ey.haigaiapp.cn

int main(int argc, char **argv)
来源：http://tq.nszjky.cn

[S19] C：快速排序
来源：http://dj.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wi.bookmarksfly.cn

[S20] C：二分查找
来源：http://qt.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oq.9csxet.cn

[S21] C：字符类别判断
来源：http://lg.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yr.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://ml.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kh.bjjhwx.cn

[S23] C：随机数
来源：http://fk.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xo.szsharing.cn

[S24] C：获取本地时间
来源：http://jx.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ok.colortex.cn

[S25] C：内存拷贝
来源：http://yo.shtwfgs.cn

memcpy(dst, src, n);
来源：http://kw.haigaiapp.cn

[S26] C：内存清零
来源：http://du.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://py.panjiajie.cn

[S27] C：定义常量
来源：http://cp.hahajie.cn

const double PI = 3.14159;
来源：http://vl.shxzskj.cn

[S28] C：静态变量
来源：http://ld.muxihuayi.cn

static int counter = 0;
来源：http://ee.chemitech.net.cn

[S29] C：变参函数
来源：http://rc.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fo.shxzskj.cn

[S30] C：头文件保护
来源：http://uk.haigaiapp.cn

#ifndef X_H
来源：http://nj.gzmigu.cn

#define X_H
来源：http://pk.huanxung.cn

#endif
来源：http://vl.nszjky.cn

[S31] C++：Hello World
来源：http://xo.asd995.cn

#include <iostream>
来源：http://ts.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://vh.muxihuayi.cn

[S32] C++：字符串
来源：http://ad.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://fa.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://bo.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nn.panjiajie.cn

[S34] C++：遍历 vector
来源：http://go.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://or.yuexingan06.cn

[S35] C++：map
来源：http://dx.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ih.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://zv.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jy.lnxyls.cn

[S37] C++：set
来源：http://yp.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wt.shxzskj.cn

[S38] C++：排序
来源：http://do.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://ji.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://fh.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rv.9csxet.cn

[S40] C++：查找元素
来源：http://iu.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uf.nicolike.cn

[S41] C++：类与构造函数
来源：http://hr.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ph.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://lu.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://fq.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://vp.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://oi.szsharing.cn

[S44] C++：引用传参
来源：http://it.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://mj.521024.cn

[S45] C++：lambda
来源：http://vn.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://al.huanxung.cn

[S46] C++：函数模板
来源：http://bu.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://at.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://rr.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vs.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://dh.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pr.asd995.cn

while (std::getline(in, line)) { }
来源：http://ow.asd995.cn

[S49] C++：写文件
来源：http://hz.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mk.gzmigu.cn

[S50] C++：格式化数字
来源：http://gu.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ho.shxzukj.cn

[S51] C++：显式类型转换
来源：http://sb.lnxyls.cn

static_cast<double>(a) / b
来源：http://uk.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://kk.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://hb.szxytkj.cn

[S53] C++：移动语义
来源：http://cv.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://vw.shtwfgs.cn

[S54] C++：异常处理
来源：http://fx.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cm.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://vj.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cn.huanxung.cn

[S56] C++：optional
来源：http://ti.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ji.shxzskj.cn

[S57] C++：编译期常量
来源：http://ai.chemitech.net.cn

constexpr int N = 10;
来源：http://tm.wgjwhj.cn

[S58] C++：命名空间
来源：http://is.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://cz.9csxet.cn

[S59] C++：静态断言
来源：http://cv.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qj.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://rz.haigaiapp.cn


<!-- 参考信息 -->