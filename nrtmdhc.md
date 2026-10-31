代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://wl.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nl.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qg.hnjuh.cn

[Q89] 判断表是否存在
来源：http://vb.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://df.haigaiapp.cn

[Q90] 生成序号列
来源：http://qb.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://io.szsharing.cn

================================================================================
来源：http://rd.huixiangedu.cn

R. Bash 专题
来源：http://hz.newstarts.cn

================================================================================
来源：http://dr.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://ox.hahajie.cn

#!/usr/bin/env bash
来源：http://xu.colortex.cn

set -euo pipefail
来源：http://pi.asd995.cn

[R02] 变量赋值与使用
来源：http://le.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://da.colortex.cn

[R03] 只读变量
来源：http://ql.jianghongdianzi.cn

readonly PI=3.14
来源：http://xj.huanxung.cn

[R04] 位置参数
来源：http://fl.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jm.521024.cn

[R05] 参数默认值
来源：http://or.chemitech.net.cn

name="${1:-default}"
来源：http://ef.nicolike.cn

[R06] 判断命令是否存在
来源：http://ri.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xf.bjjhwx.cn

[R07] if 判断文件
来源：http://sh.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pt.haigaiapp.cn

[R08] 数值比较
来源：http://gg.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qj.szsharing.cn

[R09] 字符串比较
来源：http://iw.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lh.huixinmuqiang.cn

[R10] 正则匹配
来源：http://vw.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ch.haigaiapp.cn

[R11] case 多分支
来源：http://hv.haigaiapp.cn

case "$1" in
来源：http://jy.jctech888.com.cn

start) echo "启动" ;;
来源：http://hw.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://ra.nszjky.cn

*)     echo "未知命令" ;;
来源：http://tv.colortex.cn

esac
来源：http://ug.huixiangedu.cn

[R12] for 遍历文件
来源：http://so.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://vs.yuexingan06.cn

[R13] for 计数循环
来源：http://oh.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://dp.huixinmuqiang.cn

[R14] C 风格 for
来源：http://jt.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lq.asd995.cn

[R15] while 逐行读文件
来源：http://hr.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ly.yuntaijiaju.cn

[R16] until 等待条件
来源：http://ym.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zx.szxytkj.cn

[R17] 数组定义与取值
来源：http://fd.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ko.szsharing.cn

[R18] 遍历数组
来源：http://pw.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vi.hahajie.cn

[R19] 数组长度
来源：http://pi.9csxet.cn

echo "${#arr[@]}"
来源：http://cq.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://gw.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dg.wgjwhj.cn

[R21] 字符串长度
来源：http://zb.huanxung.cn

echo "${#s}"
来源：http://sd.nicolike.cn

[R22] 截取子串
来源：http://ta.huixiangedu.cn

echo "${s:0:5}"
来源：http://xe.colortex.cn

[R23] 字符串替换
来源：http://yr.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gh.9csxet.cn

[R24] 大小写转换
来源：http://vq.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ef.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://sp.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://um.newstarts.cn

[R26] 命令替换
来源：http://zu.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://vf.wgjwhj.cn

[R27] 算术展开
来源：http://fe.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://md.huanxung.cn

[R28] 浮点运算
来源：http://pr.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://mu.yuexingan06.cn

[R29] 定义函数
来源：http://hv.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ye.nicolike.cn

[R30] 函数返回状态码
来源：http://lp.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://qg.chemitech.net.cn

[R31] 局部变量
来源：http://rd.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://ne.panjiajie.cn

[R32] 参数个数校验
来源：http://wj.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ca.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://ma.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nl.bjjhwx.cn

[R34] 退出时清理
来源：http://fb.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vl.nszjky.cn

[R35] 后台执行并等待
来源：http://ae.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xf.nicolike.cn

[R36] 并发执行多个任务
来源：http://zr.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lk.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://kx.chemitech.net.cn

files=$(ls -1)
来源：http://hn.lnxyls.cn

[R38] 管道串联
来源：http://ln.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://rr.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://ns.panjiajie.cn

cmd > out.log 2>&1
来源：http://uc.szxytkj.cn

[R40] 追加写日志
来源：http://co.huixiangedu.cn

echo "log" >> out.log
来源：http://vp.bjjhwx.cn

[R41] 丢弃输出
来源：http://ck.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://ug.nszjky.cn

[R42] 输入重定向
来源：http://wu.bjjhwx.cn

wc -l < a.txt
来源：http://kh.asd995.cn

[R43] 按名字查找文件
来源：http://fl.nicolike.cn

find . -name "*.log" -type f
来源：http://bb.lnxyls.cn

[R44] 按修改时间查找
来源：http://yd.szsharing.cn

find . -mtime -7 -type f
来源：http://ab.szxytkj.cn

[R45] 批量删除
来源：http://fh.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://vt.hahajie.cn

[R46] 递归替换文件内容
来源：http://zl.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xv.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://gw.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://of.521024.cn

[R48] awk 取指定列
来源：http://ur.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://tw.hnjuh.cn

[R49] awk 带条件
来源：http://pl.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tw.colortex.cn

[R50] awk 求和
来源：http://yo.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bo.shxzukj.cn

[R51] 排序去重取前几
来源：http://oj.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nj.haigaiapp.cn

[R52] 统计行数
来源：http://an.hahajie.cn

wc -l a.txt
来源：http://wl.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://dj.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://da.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://ed.newstarts.cn

diff a.txt b.txt
来源：http://te.huanxung.cn

[R55] 压缩与解压
来源：http://zo.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cw.bookmarksfly.cn

[R56] 远程拷贝
来源：http://nx.huixiangedu.cn

scp file user@host:/path/
来源：http://yb.9csxet.cn

[R57] 远程执行命令
来源：http://dt.shxzskj.cn

ssh user@host 'uptime'
来源：http://kv.newstarts.cn

[R58] 下载文件
来源：http://ve.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jb.huanxung.cn

[R59] 发 POST JSON
来源：http://hp.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fb.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://jp.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qw.newstarts.cn

[R61] 磁盘占用
来源：http://zn.bjjhwx.cn

df -h;  du -sh *
来源：http://jf.asd995.cn

[R62] 找最占空间的文件
来源：http://lk.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://nn.huixinmuqiang.cn

[R63] 内存与进程
来源：http://su.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://qo.colortex.cn

[R64] 结束进程
来源：http://lv.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://mg.bjjhwx.cn

[R65] 查看端口占用
来源：http://jb.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bi.muxihuayi.cn

[R66] 定时任务
来源：http://fx.muxihuayi.cn

crontab -e;  crontab -l
来源：http://aq.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://vl.haigaiapp.cn

openssl rand -hex 16
来源：http://gy.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://aq.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mg.panjiajie.cn

[R69] 生成随机密码
来源：http://ee.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://uk.hnjuh.cn

[R70] 时间戳与互转
来源：http://vl.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://xu.gzmigu.cn

[R71] 日期格式化
来源：http://vi.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gl.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://os.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xi.shtwfgs.cn

[R73] 分割大日志
来源：http://mp.panjiajie.cn

split -l 1000 big.log part_
来源：http://gd.hnjuh.cn

[R74] 批量重命名
来源：http://wv.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zl.shxzukj.cn

[R75] 导出环境变量
来源：http://vn.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://cf.hahajie.cn

[R76] 使用临时文件
来源：http://ry.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cu.colortex.cn

[R77] 读取用户输入
来源：http://qe.yuexingan06.cn

read -rp "请输入: " ans
来源：http://gr.panjiajie.cn

[R78] 交互式菜单
来源：http://to.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zq.gzmigu.cn

[R79] 解析命令行选项
来源：http://md.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cv.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://ea.colortex.cn

time ./run.sh
来源：http://tx.newstarts.cn

================================================================================
来源：http://ir.colortex.cn

S. C / C++ 专题
来源：http://ir.szsharing.cn

================================================================================
来源：http://ki.huanxung.cn

[S01] C：Hello World
来源：http://co.yuntaijiaju.cn

#include <stdio.h>
来源：http://mw.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://at.asd995.cn

[S02] C：变量与格式化输出
来源：http://ei.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://hl.chemitech.net.cn

[S03] C：读入整数
来源：http://wr.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://ku.wgjwhj.cn

[S04] C：字符串复制
来源：http://fs.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rs.newstarts.cn

[S05] C：字符串长度
来源：http://vc.newstarts.cn

strlen(s)
来源：http://fa.huanxung.cn

[S06] C：字符串比较
来源：http://qw.nszjky.cn

strcmp(a, b) == 0
来源：http://sc.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://jo.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ha.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://ho.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yj.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://vq.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dw.huixiangedu.cn

[S10] C：指针与解引用
来源：http://da.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://fo.wgjwhj.cn

[S11] C：逐行读文件
来源：http://iv.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://sh.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dt.szsharing.cn

fclose(f);
来源：http://mw.shxzukj.cn

[S12] C：写文件
来源：http://if.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zt.asd995.cn

[S13] C：宏定义
来源：http://gg.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zc.hahajie.cn

[S14] C：枚举
来源：http://tp.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://yk.yuntaijiaju.cn

[S15] C：类型转换
来源：http://oq.chemitech.net.cn

(double) a / b
来源：http://ik.shxzukj.cn

[S16] C：位操作置位
来源：http://yt.yuntaijiaju.cn

x |= (1 << 3);
来源：http://au.colortex.cn

[S17] C：安全拼接字符串
来源：http://xf.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ua.huixiangedu.cn

[S18] C：命令行参数
来源：http://pz.asd995.cn

int main(int argc, char **argv)
来源：http://pb.huixinmuqiang.cn

[S19] C：快速排序
来源：http://fq.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dv.yuexingan06.cn

[S20] C：二分查找
来源：http://qb.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lu.szxytkj.cn

[S21] C：字符类别判断
来源：http://eq.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ki.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://ym.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gr.bjjhwx.cn

[S23] C：随机数
来源：http://mk.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bd.jctech888.com.cn

[S24] C：获取本地时间
来源：http://gs.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fi.asd995.cn

[S25] C：内存拷贝
来源：http://fd.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://qp.szxytkj.cn

[S26] C：内存清零
来源：http://pt.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://dj.9csxet.cn

[S27] C：定义常量
来源：http://de.muxihuayi.cn

const double PI = 3.14159;
来源：http://yf.newstarts.cn

[S28] C：静态变量
来源：http://jx.yuexingan06.cn

static int counter = 0;
来源：http://ou.shxzukj.cn

[S29] C：变参函数
来源：http://qe.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mr.huixiangedu.cn

[S30] C：头文件保护
来源：http://er.bjjhwx.cn

#ifndef X_H
来源：http://ge.nszjky.cn

#define X_H
来源：http://lb.haigaiapp.cn

#endif
来源：http://qs.asd995.cn

[S31] C++：Hello World
来源：http://eg.yuexingan06.cn

#include <iostream>
来源：http://ic.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://wp.shtwfgs.cn

[S32] C++：字符串
来源：http://sb.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://yy.asd995.cn

[S33] C++：vector 增删
来源：http://ei.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ks.hnjuh.cn

[S34] C++：遍历 vector
来源：http://ib.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://xu.jctech888.com.cn

[S35] C++：map
来源：http://lw.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bn.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://ik.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://do.huixinmuqiang.cn

[S37] C++：set
来源：http://lk.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fm.huanxung.cn

[S38] C++：排序
来源：http://tz.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://mz.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://ts.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vm.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://ws.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tb.shxzukj.cn

[S41] C++：类与构造函数
来源：http://gi.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xa.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://tj.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://bw.hahajie.cn

[S43] C++：智能指针
来源：http://mj.521024.cn

auto p = std::make_unique<int>(5);
来源：http://fm.shtwfgs.cn

[S44] C++：引用传参
来源：http://qy.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://tt.bjjhwx.cn

[S45] C++：lambda
来源：http://tx.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://as.huanxung.cn

[S46] C++：函数模板
来源：http://pw.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xn.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://it.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fo.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://ro.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hi.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://qn.nicolike.cn

[S49] C++：写文件
来源：http://oe.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aj.jctech888.com.cn

[S50] C++：格式化数字
来源：http://fp.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bv.shxzskj.cn

[S51] C++：显式类型转换
来源：http://pq.szxytkj.cn

static_cast<double>(a) / b
来源：http://ls.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://rd.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://eo.521024.cn

[S53] C++：移动语义
来源：http://hg.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://dh.hahajie.cn

[S54] C++：异常处理
来源：http://an.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gl.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://gv.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ll.huixiangedu.cn

[S56] C++：optional
来源：http://ok.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ki.colortex.cn

[S57] C++：编译期常量
来源：http://pf.jianghongdianzi.cn

constexpr int N = 10;
来源：http://ex.haigaiapp.cn

[S58] C++：命名空间
来源：http://wo.szsharing.cn


<!-- 参考信息 -->