代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://fo.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nh.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ti.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://sd.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vk.chemitech.net.cn

[Q90] 生成序号列
来源：http://xs.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cn.521024.cn

================================================================================
来源：http://lq.nszjky.cn

R. Bash 专题
来源：http://mr.9csxet.cn

================================================================================
来源：http://nu.hnjuh.cn

[R01] shebang 与严格模式
来源：http://mf.521024.cn

#!/usr/bin/env bash
来源：http://di.wgjwhj.cn

set -euo pipefail
来源：http://pd.shxzukj.cn

[R02] 变量赋值与使用
来源：http://gc.szsharing.cn

name="Tom"; echo "$name"
来源：http://ee.yuexingan06.cn

[R03] 只读变量
来源：http://xu.bjjhwx.cn

readonly PI=3.14
来源：http://aj.bjjhwx.cn

[R04] 位置参数
来源：http://kv.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dp.shxzskj.cn

[R05] 参数默认值
来源：http://px.nicolike.cn

name="${1:-default}"
来源：http://ar.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://xa.bjjhwx.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sp.huixiangedu.cn

[R07] if 判断文件
来源：http://za.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dl.szsharing.cn

[R08] 数值比较
来源：http://vp.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hq.newstarts.cn

[R09] 字符串比较
来源：http://im.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://al.nszjky.cn

[R10] 正则匹配
来源：http://iz.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://la.yuexingan06.cn

[R11] case 多分支
来源：http://ez.jianghongdianzi.cn

case "$1" in
来源：http://ds.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://lj.shxzukj.cn

stop)  echo "停止" ;;
来源：http://tp.huanxung.cn

*)     echo "未知命令" ;;
来源：http://xx.9csxet.cn

esac
来源：http://nq.asd995.cn

[R12] for 遍历文件
来源：http://ui.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://qm.shxzukj.cn

[R13] for 计数循环
来源：http://jl.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://da.colortex.cn

[R14] C 风格 for
来源：http://xi.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://og.huanxung.cn

[R15] while 逐行读文件
来源：http://uv.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pz.huixiangedu.cn

[R16] until 等待条件
来源：http://hp.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kc.huanxung.cn

[R17] 数组定义与取值
来源：http://xy.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ga.huanxung.cn

[R18] 遍历数组
来源：http://bb.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ek.shxzukj.cn

[R19] 数组长度
来源：http://ax.lnxyls.cn

echo "${#arr[@]}"
来源：http://zp.szxytkj.cn

[R20] 关联数组（字典）
来源：http://px.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jq.hnjuh.cn

[R21] 字符串长度
来源：http://rk.huixinmuqiang.cn

echo "${#s}"
来源：http://kr.yuntaijiaju.cn

[R22] 截取子串
来源：http://zb.shxzskj.cn

echo "${s:0:5}"
来源：http://iu.haigaiapp.cn

[R23] 字符串替换
来源：http://lc.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://er.asd995.cn

[R24] 大小写转换
来源：http://hq.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ek.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://hb.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vx.muxihuayi.cn

[R26] 命令替换
来源：http://hh.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://mn.jianghongdianzi.cn

[R27] 算术展开
来源：http://zc.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://no.shxzskj.cn

[R28] 浮点运算
来源：http://xv.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://ut.szsharing.cn

[R29] 定义函数
来源：http://me.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ss.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://td.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://dq.hnjuh.cn

[R31] 局部变量
来源：http://mv.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://lk.hahajie.cn

[R32] 参数个数校验
来源：http://oh.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bz.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://gt.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xl.gzmigu.cn

[R34] 退出时清理
来源：http://tu.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pg.521024.cn

[R35] 后台执行并等待
来源：http://lv.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sb.panjiajie.cn

[R36] 并发执行多个任务
来源：http://aj.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iq.9csxet.cn

[R37] 把输出赋给变量
来源：http://ed.lnxyls.cn

files=$(ls -1)
来源：http://ck.jctech888.com.cn

[R38] 管道串联
来源：http://di.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://se.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://yn.shtwfgs.cn

cmd > out.log 2>&1
来源：http://qq.nicolike.cn

[R40] 追加写日志
来源：http://gm.shtwfgs.cn

echo "log" >> out.log
来源：http://lh.haigaiapp.cn

[R41] 丢弃输出
来源：http://sj.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://ik.szxytkj.cn

[R42] 输入重定向
来源：http://at.asd995.cn

wc -l < a.txt
来源：http://xh.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://aj.huanxung.cn

find . -name "*.log" -type f
来源：http://fj.jctech888.com.cn

[R44] 按修改时间查找
来源：http://po.chemitech.net.cn

find . -mtime -7 -type f
来源：http://zp.bookmarksfly.cn

[R45] 批量删除
来源：http://jy.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://xt.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://fb.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xk.shxzukj.cn

[R47] sed 单行替换
来源：http://ur.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rd.szsharing.cn

[R48] awk 取指定列
来源：http://tg.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://xc.9csxet.cn

[R49] awk 带条件
来源：http://ki.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hi.huixiangedu.cn

[R50] awk 求和
来源：http://eo.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qw.gzmigu.cn

[R51] 排序去重取前几
来源：http://gq.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mf.newstarts.cn

[R52] 统计行数
来源：http://hu.hahajie.cn

wc -l a.txt
来源：http://ov.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://uc.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qe.bjjhwx.cn

[R54] 比较两个文件
来源：http://pe.jctech888.com.cn

diff a.txt b.txt
来源：http://ah.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://cn.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ov.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://qx.hnjuh.cn

scp file user@host:/path/
来源：http://cx.bjjhwx.cn

[R57] 远程执行命令
来源：http://ft.yuexingan06.cn

ssh user@host 'uptime'
来源：http://io.bjjhwx.cn

[R58] 下载文件
来源：http://vm.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sh.haigaiapp.cn

[R59] 发 POST JSON
来源：http://fm.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://on.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://yr.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wt.panjiajie.cn

[R61] 磁盘占用
来源：http://qb.huixiangedu.cn

df -h;  du -sh *
来源：http://gb.huanxung.cn

[R62] 找最占空间的文件
来源：http://dy.521024.cn

du -ah . | sort -rh | head -10
来源：http://rf.shxzukj.cn

[R63] 内存与进程
来源：http://tv.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://ri.nicolike.cn

[R64] 结束进程
来源：http://zs.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://cm.panjiajie.cn

[R65] 查看端口占用
来源：http://uu.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cb.szsharing.cn

[R66] 定时任务
来源：http://jv.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://ql.521024.cn

[R67] 生成随机十六进制串
来源：http://my.shxzukj.cn

openssl rand -hex 16
来源：http://lx.yuexingan06.cn

[R68] 计算文件校验值
来源：http://gt.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hu.asd995.cn

[R69] 生成随机密码
来源：http://mn.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://uj.chemitech.net.cn

[R70] 时间戳与互转
来源：http://pc.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://iw.yuntaijiaju.cn

[R71] 日期格式化
来源：http://lj.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yy.szsharing.cn

[R72] 等待端口就绪
来源：http://vp.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jk.nszjky.cn

[R73] 分割大日志
来源：http://rv.huixiangedu.cn

split -l 1000 big.log part_
来源：http://no.shtwfgs.cn

[R74] 批量重命名
来源：http://zw.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dh.521024.cn

[R75] 导出环境变量
来源：http://bs.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://rf.szxytkj.cn

[R76] 使用临时文件
来源：http://fl.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ka.bookmarksfly.cn

[R77] 读取用户输入
来源：http://td.shxzskj.cn

read -rp "请输入: " ans
来源：http://jx.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://hb.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pe.huanxung.cn

[R79] 解析命令行选项
来源：http://tz.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vy.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://ay.nszjky.cn

time ./run.sh
来源：http://wb.huixinmuqiang.cn

================================================================================
来源：http://ze.newstarts.cn

S. C / C++ 专题
来源：http://xf.hahajie.cn

================================================================================
来源：http://os.nszjky.cn

[S01] C：Hello World
来源：http://jp.huixinmuqiang.cn

#include <stdio.h>
来源：http://ni.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dw.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://xf.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://uo.shtwfgs.cn

[S03] C：读入整数
来源：http://fr.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://zo.chemitech.net.cn

[S04] C：字符串复制
来源：http://cz.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hj.gzmigu.cn

[S05] C：字符串长度
来源：http://tt.chemitech.net.cn

strlen(s)
来源：http://yq.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://tn.szxytkj.cn

strcmp(a, b) == 0
来源：http://md.newstarts.cn

[S07] C：数组遍历求和
来源：http://nt.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xi.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://qg.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://op.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://gs.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tr.gzmigu.cn

[S10] C：指针与解引用
来源：http://sq.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://ll.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://vn.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://eu.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vg.colortex.cn

fclose(f);
来源：http://dm.hahajie.cn

[S12] C：写文件
来源：http://fb.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iy.jianghongdianzi.cn

[S13] C：宏定义
来源：http://yz.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eb.jianghongdianzi.cn

[S14] C：枚举
来源：http://rq.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://kr.521024.cn

[S15] C：类型转换
来源：http://dp.chemitech.net.cn

(double) a / b
来源：http://hs.szxytkj.cn

[S16] C：位操作置位
来源：http://zy.lnxyls.cn

x |= (1 << 3);
来源：http://do.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://vn.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://is.szsharing.cn

[S18] C：命令行参数
来源：http://cq.huixiangedu.cn

int main(int argc, char **argv)
来源：http://eh.huanxung.cn

[S19] C：快速排序
来源：http://qj.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vm.yuexingan06.cn

[S20] C：二分查找
来源：http://na.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uf.nszjky.cn

[S21] C：字符类别判断
来源：http://sg.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uc.szxytkj.cn

[S22] C：字符串转数字
来源：http://tq.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qe.shtwfgs.cn

[S23] C：随机数
来源：http://lt.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sh.521024.cn

[S24] C：获取本地时间
来源：http://rh.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sg.jctech888.com.cn

[S25] C：内存拷贝
来源：http://rp.jctech888.com.cn

memcpy(dst, src, n);
来源：http://aq.szxytkj.cn

[S26] C：内存清零
来源：http://jf.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://ac.lnxyls.cn

[S27] C：定义常量
来源：http://wz.chemitech.net.cn

const double PI = 3.14159;
来源：http://ke.newstarts.cn

[S28] C：静态变量
来源：http://oz.9csxet.cn

static int counter = 0;
来源：http://qt.bjjhwx.cn

[S29] C：变参函数
来源：http://ae.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ps.lnxyls.cn

[S30] C：头文件保护
来源：http://hd.bjjhwx.cn

#ifndef X_H
来源：http://gx.huixinmuqiang.cn

#define X_H
来源：http://aq.haigaiapp.cn

#endif
来源：http://zy.bookmarksfly.cn

[S31] C++：Hello World
来源：http://ys.huixiangedu.cn

#include <iostream>
来源：http://xh.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://en.9csxet.cn

[S32] C++：字符串
来源：http://km.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://to.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://nb.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qn.shxzukj.cn

[S34] C++：遍历 vector
来源：http://tu.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://lo.hahajie.cn

[S35] C++：map
来源：http://ia.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ty.nicolike.cn

[S36] C++：unordered_map
来源：http://vi.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rm.shxzukj.cn

[S37] C++：set
来源：http://ml.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://da.yuexingan06.cn

[S38] C++：排序
来源：http://ok.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://kk.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://uy.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oi.shtwfgs.cn

[S40] C++：查找元素
来源：http://wb.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gx.521024.cn

[S41] C++：类与构造函数
来源：http://mg.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ur.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://td.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://ur.haigaiapp.cn

[S43] C++：智能指针
来源：http://hr.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://au.newstarts.cn

[S44] C++：引用传参
来源：http://tt.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://qu.chemitech.net.cn

[S45] C++：lambda
来源：http://ge.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sp.hnjuh.cn

[S46] C++：函数模板
来源：http://mr.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qe.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://ci.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lu.nszjky.cn

[S48] C++：逐行读文件
来源：http://wb.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xh.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://aq.wgjwhj.cn

[S49] C++：写文件
来源：http://hn.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sg.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://kk.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xk.huanxung.cn

[S51] C++：显式类型转换
来源：http://gc.haigaiapp.cn

static_cast<double>(a) / b
来源：http://xo.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://ln.huanxung.cn

int size() const noexcept { return n_; }
来源：http://hw.szxytkj.cn

[S53] C++：移动语义
来源：http://ku.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://ea.gzmigu.cn

[S54] C++：异常处理
来源：http://xe.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kt.newstarts.cn

[S55] C++：结构化绑定
来源：http://vd.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nw.huanxung.cn

[S56] C++：optional
来源：http://db.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cc.szxytkj.cn

[S57] C++：编译期常量
来源：http://nx.gzmigu.cn

constexpr int N = 10;
来源：http://ve.haigaiapp.cn

[S58] C++：命名空间
来源：http://rm.chemitech.net.cn


<!-- 参考信息 -->