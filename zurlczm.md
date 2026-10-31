代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://ts.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ry.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gc.newstarts.cn

[Q89] 判断表是否存在
来源：http://dw.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bd.gzmigu.cn

[Q90] 生成序号列
来源：http://dk.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bs.wgjwhj.cn

================================================================================
来源：http://yt.nszjky.cn

R. Bash 专题
来源：http://zf.asd995.cn

================================================================================
来源：http://bs.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://yn.bjjhwx.cn

#!/usr/bin/env bash
来源：http://zb.wgjwhj.cn

set -euo pipefail
来源：http://tz.szsharing.cn

[R02] 变量赋值与使用
来源：http://ww.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://nz.hahajie.cn

[R03] 只读变量
来源：http://zl.huanxung.cn

readonly PI=3.14
来源：http://az.colortex.cn

[R04] 位置参数
来源：http://od.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xo.asd995.cn

[R05] 参数默认值
来源：http://io.bjjhwx.cn

name="${1:-default}"
来源：http://xp.szsharing.cn

[R06] 判断命令是否存在
来源：http://pb.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://br.muxihuayi.cn

[R07] if 判断文件
来源：http://cj.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tz.haigaiapp.cn

[R08] 数值比较
来源：http://uy.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ns.huixiangedu.cn

[R09] 字符串比较
来源：http://bz.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ow.jctech888.com.cn

[R10] 正则匹配
来源：http://oy.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mo.wgjwhj.cn

[R11] case 多分支
来源：http://uy.huanxung.cn

case "$1" in
来源：http://sr.jctech888.com.cn

start) echo "启动" ;;
来源：http://an.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://cc.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://cz.huanxung.cn

esac
来源：http://zp.chemitech.net.cn

[R12] for 遍历文件
来源：http://su.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://sw.shxzskj.cn

[R13] for 计数循环
来源：http://vd.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://of.huixinmuqiang.cn

[R14] C 风格 for
来源：http://gn.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ns.haigaiapp.cn

[R15] while 逐行读文件
来源：http://ym.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kr.bookmarksfly.cn

[R16] until 等待条件
来源：http://xw.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vu.asd995.cn

[R17] 数组定义与取值
来源：http://qc.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cz.huixinmuqiang.cn

[R18] 遍历数组
来源：http://ux.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ex.nicolike.cn

[R19] 数组长度
来源：http://ut.521024.cn

echo "${#arr[@]}"
来源：http://bg.bookmarksfly.cn

[R20] 关联数组（字典）
来源：http://rp.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wh.asd995.cn

[R21] 字符串长度
来源：http://wj.wgjwhj.cn

echo "${#s}"
来源：http://qa.panjiajie.cn

[R22] 截取子串
来源：http://bv.gzmigu.cn

echo "${s:0:5}"
来源：http://cw.gzmigu.cn

[R23] 字符串替换
来源：http://ss.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jv.haigaiapp.cn

[R24] 大小写转换
来源：http://jq.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qo.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://ir.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jc.bjjhwx.cn

[R26] 命令替换
来源：http://ns.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://au.asd995.cn

[R27] 算术展开
来源：http://ls.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://no.shtwfgs.cn

[R28] 浮点运算
来源：http://sv.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://xc.gzmigu.cn

[R29] 定义函数
来源：http://dq.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sj.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://pq.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://ow.gzmigu.cn

[R31] 局部变量
来源：http://jk.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://gl.huanxung.cn

[R32] 参数个数校验
来源：http://xz.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cv.colortex.cn

[R33] 捕获错误并提示行号
来源：http://ki.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lw.chemitech.net.cn

[R34] 退出时清理
来源：http://bd.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jc.nszjky.cn

[R35] 后台执行并等待
来源：http://di.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vw.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://ri.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ih.hahajie.cn

[R37] 把输出赋给变量
来源：http://si.bjjhwx.cn

files=$(ls -1)
来源：http://bg.szsharing.cn

[R38] 管道串联
来源：http://io.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://yf.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://if.shxzskj.cn

cmd > out.log 2>&1
来源：http://pk.wgjwhj.cn

[R40] 追加写日志
来源：http://ne.hahajie.cn

echo "log" >> out.log
来源：http://ze.wgjwhj.cn

[R41] 丢弃输出
来源：http://ux.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://bp.gzmigu.cn

[R42] 输入重定向
来源：http://rh.hnjuh.cn

wc -l < a.txt
来源：http://hu.521024.cn

[R43] 按名字查找文件
来源：http://by.asd995.cn

find . -name "*.log" -type f
来源：http://it.asd995.cn

[R44] 按修改时间查找
来源：http://xj.jctech888.com.cn

find . -mtime -7 -type f
来源：http://qs.hnjuh.cn

[R45] 批量删除
来源：http://xd.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://tq.shxzukj.cn

[R46] 递归替换文件内容
来源：http://xy.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wu.muxihuayi.cn

[R47] sed 单行替换
来源：http://lr.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jb.panjiajie.cn

[R48] awk 取指定列
来源：http://kn.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://zp.huixinmuqiang.cn

[R49] awk 带条件
来源：http://xy.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ia.panjiajie.cn

[R50] awk 求和
来源：http://jp.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pq.nicolike.cn

[R51] 排序去重取前几
来源：http://hm.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ew.9csxet.cn

[R52] 统计行数
来源：http://xr.hahajie.cn

wc -l a.txt
来源：http://vq.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://gs.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://or.yuexingan06.cn

[R54] 比较两个文件
来源：http://eh.nicolike.cn

diff a.txt b.txt
来源：http://uq.shtwfgs.cn

[R55] 压缩与解压
来源：http://la.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vi.asd995.cn

[R56] 远程拷贝
来源：http://wb.szsharing.cn

scp file user@host:/path/
来源：http://hs.szsharing.cn

[R57] 远程执行命令
来源：http://tf.hnjuh.cn

ssh user@host 'uptime'
来源：http://mi.shtwfgs.cn

[R58] 下载文件
来源：http://gc.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bt.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://qx.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yr.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://bs.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fv.colortex.cn

[R61] 磁盘占用
来源：http://wv.chemitech.net.cn

df -h;  du -sh *
来源：http://jf.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://ul.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://ng.jianghongdianzi.cn

[R63] 内存与进程
来源：http://gd.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://fi.huixinmuqiang.cn

[R64] 结束进程
来源：http://ej.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://ph.gzmigu.cn

[R65] 查看端口占用
来源：http://ro.nicolike.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sf.haigaiapp.cn

[R66] 定时任务
来源：http://qz.panjiajie.cn

crontab -e;  crontab -l
来源：http://me.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://as.chemitech.net.cn

openssl rand -hex 16
来源：http://ls.hnjuh.cn

[R68] 计算文件校验值
来源：http://ws.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wq.hahajie.cn

[R69] 生成随机密码
来源：http://dv.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://hc.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://dn.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://ta.huixiangedu.cn

[R71] 日期格式化
来源：http://ve.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rf.nszjky.cn

[R72] 等待端口就绪
来源：http://hb.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hw.9csxet.cn

[R73] 分割大日志
来源：http://ka.wgjwhj.cn

split -l 1000 big.log part_
来源：http://bu.bjjhwx.cn

[R74] 批量重命名
来源：http://wf.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://te.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://jt.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://yp.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://zm.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://au.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://uo.521024.cn

read -rp "请输入: " ans
来源：http://pp.szsharing.cn

[R78] 交互式菜单
来源：http://lk.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tv.9csxet.cn

[R79] 解析命令行选项
来源：http://gb.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yx.asd995.cn

[R80] 查看脚本执行耗时
来源：http://ha.yuntaijiaju.cn

time ./run.sh
来源：http://gi.huixiangedu.cn

================================================================================
来源：http://gm.szxytkj.cn

S. C / C++ 专题
来源：http://jp.szsharing.cn

================================================================================
来源：http://vr.muxihuayi.cn

[S01] C：Hello World
来源：http://cy.szxytkj.cn

#include <stdio.h>
来源：http://ba.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nr.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://tf.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://ne.szsharing.cn

[S03] C：读入整数
来源：http://mh.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://qf.newstarts.cn

[S04] C：字符串复制
来源：http://rc.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fg.muxihuayi.cn

[S05] C：字符串长度
来源：http://us.szxytkj.cn

strlen(s)
来源：http://rg.haigaiapp.cn

[S06] C：字符串比较
来源：http://hw.yuexingan06.cn

strcmp(a, b) == 0
来源：http://ka.shxzskj.cn

[S07] C：数组遍历求和
来源：http://uf.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ft.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://ww.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lr.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://lb.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yy.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://eb.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://fw.muxihuayi.cn

[S11] C：逐行读文件
来源：http://ig.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://tr.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://er.newstarts.cn

fclose(f);
来源：http://dq.newstarts.cn

[S12] C：写文件
来源：http://yi.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cv.hnjuh.cn

[S13] C：宏定义
来源：http://bt.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tf.gzmigu.cn

[S14] C：枚举
来源：http://vt.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://rq.jctech888.com.cn

[S15] C：类型转换
来源：http://mj.jctech888.com.cn

(double) a / b
来源：http://oy.asd995.cn

[S16] C：位操作置位
来源：http://me.shtwfgs.cn

x |= (1 << 3);
来源：http://bp.nszjky.cn

[S17] C：安全拼接字符串
来源：http://tp.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rc.9csxet.cn

[S18] C：命令行参数
来源：http://va.lnxyls.cn

int main(int argc, char **argv)
来源：http://oh.shtwfgs.cn

[S19] C：快速排序
来源：http://ck.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qv.panjiajie.cn

[S20] C：二分查找
来源：http://wt.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ei.colortex.cn

[S21] C：字符类别判断
来源：http://ma.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eo.chemitech.net.cn

[S22] C：字符串转数字
来源：http://li.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ta.haigaiapp.cn

[S23] C：随机数
来源：http://uh.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ik.szxytkj.cn

[S24] C：获取本地时间
来源：http://qp.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yc.lnxyls.cn

[S25] C：内存拷贝
来源：http://rp.shtwfgs.cn

memcpy(dst, src, n);
来源：http://ju.chemitech.net.cn

[S26] C：内存清零
来源：http://tn.hahajie.cn

memset(a, 0, sizeof a);
来源：http://jh.nicolike.cn

[S27] C：定义常量
来源：http://so.gzmigu.cn

const double PI = 3.14159;
来源：http://ii.shxzukj.cn

[S28] C：静态变量
来源：http://zu.huixiangedu.cn

static int counter = 0;
来源：http://ov.521024.cn

[S29] C：变参函数
来源：http://rl.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://or.hnjuh.cn

[S30] C：头文件保护
来源：http://yn.newstarts.cn

#ifndef X_H
来源：http://ec.bookmarksfly.cn

#define X_H
来源：http://ui.gzmigu.cn

#endif
来源：http://cb.szxytkj.cn

[S31] C++：Hello World
来源：http://ia.wgjwhj.cn

#include <iostream>
来源：http://ov.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://gq.shxzskj.cn

[S32] C++：字符串
来源：http://pr.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://co.huanxung.cn

[S33] C++：vector 增删
来源：http://ma.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ki.gzmigu.cn

[S34] C++：遍历 vector
来源：http://vw.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://dc.muxihuayi.cn

[S35] C++：map
来源：http://ek.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://au.521024.cn

[S36] C++：unordered_map
来源：http://ki.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ef.huixinmuqiang.cn

[S37] C++：set
来源：http://kl.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fi.bookmarksfly.cn

[S38] C++：排序
来源：http://nz.asd995.cn

std::sort(v.begin(), v.end());
来源：http://oo.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://ck.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wd.haigaiapp.cn

[S40] C++：查找元素
来源：http://cs.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ts.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://bb.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sr.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://id.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://gu.huixiangedu.cn

[S43] C++：智能指针
来源：http://hp.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://aw.shxzukj.cn

[S44] C++：引用传参
来源：http://jm.9csxet.cn

void inc(int &x) { ++x; }
来源：http://ly.haigaiapp.cn

[S45] C++：lambda
来源：http://vn.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mv.wgjwhj.cn

[S46] C++：函数模板
来源：http://we.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sr.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://uz.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tk.newstarts.cn

[S48] C++：逐行读文件
来源：http://re.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yc.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://ro.szxytkj.cn

[S49] C++：写文件
来源：http://fa.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cc.wgjwhj.cn

[S50] C++：格式化数字
来源：http://jq.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zs.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://bx.jctech888.com.cn

static_cast<double>(a) / b
来源：http://lb.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://ar.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://zw.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://sx.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://ss.asd995.cn

[S54] C++：异常处理
来源：http://eg.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vz.nicolike.cn

[S55] C++：结构化绑定
来源：http://da.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hw.szsharing.cn

[S56] C++：optional
来源：http://fw.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ma.colortex.cn

[S57] C++：编译期常量
来源：http://qu.nicolike.cn

constexpr int N = 10;
来源：http://ig.huixiangedu.cn

[S58] C++：命名空间
来源：http://ph.bookmarksfly.cn


<!-- 参考信息 -->