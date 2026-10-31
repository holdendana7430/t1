代发 wailian999

[Q82] 字符长度与字节长度
来源：http://uj.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ca.shxzukj.cn

[Q83] 大小写转换
来源：http://sg.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ri.szsharing.cn

[Q84] 去除首尾空格
来源：http://nv.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://nh.gzmigu.cn

[Q85] 数值取整
来源：http://lw.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gh.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://oy.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dr.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://wi.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cd.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://gf.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ky.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rp.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://vh.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gb.colortex.cn

[Q90] 生成序号列
来源：http://kd.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vb.chemitech.net.cn

================================================================================
来源：http://be.shxzskj.cn

R. Bash 专题
来源：http://bh.panjiajie.cn

================================================================================
来源：http://rw.shxzukj.cn

[R01] shebang 与严格模式
来源：http://fe.bjjhwx.cn

#!/usr/bin/env bash
来源：http://jk.huanxung.cn

set -euo pipefail
来源：http://uo.nszjky.cn

[R02] 变量赋值与使用
来源：http://nt.shxzukj.cn

name="Tom"; echo "$name"
来源：http://tw.shtwfgs.cn

[R03] 只读变量
来源：http://ej.9csxet.cn

readonly PI=3.14
来源：http://xg.huixiangedu.cn

[R04] 位置参数
来源：http://fa.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gh.colortex.cn

[R05] 参数默认值
来源：http://bl.lnxyls.cn

name="${1:-default}"
来源：http://wj.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://mz.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gp.bjjhwx.cn

[R07] if 判断文件
来源：http://ro.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hk.szsharing.cn

[R08] 数值比较
来源：http://hz.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rr.newstarts.cn

[R09] 字符串比较
来源：http://th.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://da.asd995.cn

[R10] 正则匹配
来源：http://ro.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nm.nicolike.cn

[R11] case 多分支
来源：http://xf.jianghongdianzi.cn

case "$1" in
来源：http://qj.colortex.cn

start) echo "启动" ;;
来源：http://uw.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://mp.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://qr.newstarts.cn

esac
来源：http://dj.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://xi.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://pm.newstarts.cn

[R13] for 计数循环
来源：http://po.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://ie.huanxung.cn

[R14] C 风格 for
来源：http://lj.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ep.nicolike.cn

[R15] while 逐行读文件
来源：http://ub.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ri.newstarts.cn

[R16] until 等待条件
来源：http://pt.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fi.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://ll.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kk.hahajie.cn

[R18] 遍历数组
来源：http://hg.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yf.asd995.cn

[R19] 数组长度
来源：http://ri.panjiajie.cn

echo "${#arr[@]}"
来源：http://lw.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://ui.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ua.shxzukj.cn

[R21] 字符串长度
来源：http://jb.bjjhwx.cn

echo "${#s}"
来源：http://wq.lnxyls.cn

[R22] 截取子串
来源：http://sx.chemitech.net.cn

echo "${s:0:5}"
来源：http://oj.szxytkj.cn

[R23] 字符串替换
来源：http://ir.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qu.chemitech.net.cn

[R24] 大小写转换
来源：http://pl.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dn.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://pg.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ak.asd995.cn

[R26] 命令替换
来源：http://wq.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://wx.521024.cn

[R27] 算术展开
来源：http://dt.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://oy.shxzukj.cn

[R28] 浮点运算
来源：http://pn.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://ch.lnxyls.cn

[R29] 定义函数
来源：http://zy.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sh.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://yd.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://me.hahajie.cn

[R31] 局部变量
来源：http://au.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://ed.huixiangedu.cn

[R32] 参数个数校验
来源：http://ut.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://co.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://qx.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dh.huixiangedu.cn

[R34] 退出时清理
来源：http://lj.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ns.lnxyls.cn

[R35] 后台执行并等待
来源：http://vq.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xw.newstarts.cn

[R36] 并发执行多个任务
来源：http://uj.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ia.hahajie.cn

[R37] 把输出赋给变量
来源：http://ed.chemitech.net.cn

files=$(ls -1)
来源：http://dr.yuntaijiaju.cn

[R38] 管道串联
来源：http://bj.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://km.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://kh.yuexingan06.cn

cmd > out.log 2>&1
来源：http://pg.bjjhwx.cn

[R40] 追加写日志
来源：http://he.shxzskj.cn

echo "log" >> out.log
来源：http://zv.szsharing.cn

[R41] 丢弃输出
来源：http://ug.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://ee.bookmarksfly.cn

[R42] 输入重定向
来源：http://fm.chemitech.net.cn

wc -l < a.txt
来源：http://ad.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://fl.shtwfgs.cn

find . -name "*.log" -type f
来源：http://hl.shxzskj.cn

[R44] 按修改时间查找
来源：http://te.szxytkj.cn

find . -mtime -7 -type f
来源：http://wy.shxzskj.cn

[R45] 批量删除
来源：http://th.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://rq.colortex.cn

[R46] 递归替换文件内容
来源：http://vk.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gd.bookmarksfly.cn

[R47] sed 单行替换
来源：http://hk.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zl.hahajie.cn

[R48] awk 取指定列
来源：http://pl.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://in.gzmigu.cn

[R49] awk 带条件
来源：http://bd.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ey.nicolike.cn

[R50] awk 求和
来源：http://gr.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dg.wgjwhj.cn

[R51] 排序去重取前几
来源：http://mj.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rg.9csxet.cn

[R52] 统计行数
来源：http://cc.muxihuayi.cn

wc -l a.txt
来源：http://kb.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://ad.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fk.gzmigu.cn

[R54] 比较两个文件
来源：http://wz.lnxyls.cn

diff a.txt b.txt
来源：http://hv.9csxet.cn

[R55] 压缩与解压
来源：http://gs.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ej.muxihuayi.cn

[R56] 远程拷贝
来源：http://mc.jianghongdianzi.cn

scp file user@host:/path/
来源：http://br.521024.cn

[R57] 远程执行命令
来源：http://qq.szsharing.cn

ssh user@host 'uptime'
来源：http://nd.9csxet.cn

[R58] 下载文件
来源：http://ej.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fx.wgjwhj.cn

[R59] 发 POST JSON
来源：http://ec.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sx.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://qb.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rz.bookmarksfly.cn

[R61] 磁盘占用
来源：http://hc.shxzukj.cn

df -h;  du -sh *
来源：http://oc.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://cn.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://mv.hnjuh.cn

[R63] 内存与进程
来源：http://ck.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://py.gzmigu.cn

[R64] 结束进程
来源：http://lq.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://rp.shtwfgs.cn

[R65] 查看端口占用
来源：http://wl.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yc.hnjuh.cn

[R66] 定时任务
来源：http://vq.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://ob.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://ns.shxzskj.cn

openssl rand -hex 16
来源：http://ys.9csxet.cn

[R68] 计算文件校验值
来源：http://uh.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dt.gzmigu.cn

[R69] 生成随机密码
来源：http://wi.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://uo.lnxyls.cn

[R70] 时间戳与互转
来源：http://jm.colortex.cn

date +%s;  date -d @1700000000
来源：http://nw.jianghongdianzi.cn

[R71] 日期格式化
来源：http://br.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://by.szsharing.cn

[R72] 等待端口就绪
来源：http://nw.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ug.colortex.cn

[R73] 分割大日志
来源：http://id.hnjuh.cn

split -l 1000 big.log part_
来源：http://ux.bookmarksfly.cn

[R74] 批量重命名
来源：http://ds.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tv.shtwfgs.cn

[R75] 导出环境变量
来源：http://ky.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://nh.hahajie.cn

[R76] 使用临时文件
来源：http://mn.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bn.asd995.cn

[R77] 读取用户输入
来源：http://sa.shtwfgs.cn

read -rp "请输入: " ans
来源：http://qq.hnjuh.cn

[R78] 交互式菜单
来源：http://nu.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xb.nicolike.cn

[R79] 解析命令行选项
来源：http://ht.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mn.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://sb.bookmarksfly.cn

time ./run.sh
来源：http://of.shxzukj.cn

================================================================================
来源：http://sy.szsharing.cn

S. C / C++ 专题
来源：http://in.huanxung.cn

================================================================================
来源：http://lv.szxytkj.cn

[S01] C：Hello World
来源：http://ml.shxzskj.cn

#include <stdio.h>
来源：http://lv.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ly.colortex.cn

[S02] C：变量与格式化输出
来源：http://lw.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://ov.nicolike.cn

[S03] C：读入整数
来源：http://oc.asd995.cn

int x; scanf("%d", &x);
来源：http://ak.hnjuh.cn

[S04] C：字符串复制
来源：http://md.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vn.asd995.cn

[S05] C：字符串长度
来源：http://ze.yuexingan06.cn

strlen(s)
来源：http://gd.yuexingan06.cn

[S06] C：字符串比较
来源：http://pf.gzmigu.cn

strcmp(a, b) == 0
来源：http://ao.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://ek.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rp.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://hh.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xk.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://sh.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qk.jctech888.com.cn

[S10] C：指针与解引用
来源：http://lh.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://vw.chemitech.net.cn

[S11] C：逐行读文件
来源：http://so.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://jg.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ea.wgjwhj.cn

fclose(f);
来源：http://in.szsharing.cn

[S12] C：写文件
来源：http://nt.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qm.huanxung.cn

[S13] C：宏定义
来源：http://hv.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jt.521024.cn

[S14] C：枚举
来源：http://pm.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://yn.wgjwhj.cn

[S15] C：类型转换
来源：http://wi.colortex.cn

(double) a / b
来源：http://jb.nicolike.cn

[S16] C：位操作置位
来源：http://ca.jctech888.com.cn

x |= (1 << 3);
来源：http://lm.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://qb.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lr.huanxung.cn

[S18] C：命令行参数
来源：http://aa.bjjhwx.cn

int main(int argc, char **argv)
来源：http://nx.nicolike.cn

[S19] C：快速排序
来源：http://ov.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mp.chemitech.net.cn

[S20] C：二分查找
来源：http://mo.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wf.szsharing.cn

[S21] C：字符类别判断
来源：http://zp.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qh.szxytkj.cn

[S22] C：字符串转数字
来源：http://lr.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vq.szsharing.cn

[S23] C：随机数
来源：http://vq.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lv.shxzukj.cn

[S24] C：获取本地时间
来源：http://yb.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jh.jctech888.com.cn

[S25] C：内存拷贝
来源：http://dm.szsharing.cn

memcpy(dst, src, n);
来源：http://va.nszjky.cn

[S26] C：内存清零
来源：http://jl.szsharing.cn

memset(a, 0, sizeof a);
来源：http://ul.huanxung.cn

[S27] C：定义常量
来源：http://ge.szsharing.cn

const double PI = 3.14159;
来源：http://tl.haigaiapp.cn

[S28] C：静态变量
来源：http://jj.shtwfgs.cn

static int counter = 0;
来源：http://pi.muxihuayi.cn

[S29] C：变参函数
来源：http://ke.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wj.shxzukj.cn

[S30] C：头文件保护
来源：http://jm.nszjky.cn

#ifndef X_H
来源：http://rw.wgjwhj.cn

#define X_H
来源：http://tm.gzmigu.cn

#endif
来源：http://xg.colortex.cn

[S31] C++：Hello World
来源：http://ie.wgjwhj.cn

#include <iostream>
来源：http://ra.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://po.521024.cn

[S32] C++：字符串
来源：http://rc.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://sj.colortex.cn

[S33] C++：vector 增删
来源：http://hu.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://li.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://fv.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://ce.bookmarksfly.cn

[S35] C++：map
来源：http://ev.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qp.gzmigu.cn

[S36] C++：unordered_map
来源：http://of.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vy.shxzukj.cn

[S37] C++：set
来源：http://hl.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ex.bjjhwx.cn

[S38] C++：排序
来源：http://sl.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://bd.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://dg.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ov.shtwfgs.cn

[S40] C++：查找元素
来源：http://rz.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://os.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://dp.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aj.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://xo.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://xr.colortex.cn

[S43] C++：智能指针
来源：http://oa.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://an.wgjwhj.cn

[S44] C++：引用传参
来源：http://iw.nszjky.cn

void inc(int &x) { ++x; }
来源：http://pl.panjiajie.cn

[S45] C++：lambda
来源：http://wg.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kq.huixiangedu.cn

[S46] C++：函数模板
来源：http://zu.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hj.521024.cn

[S47] C++：结构化绑定遍历
来源：http://qz.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ev.shxzukj.cn

[S48] C++：逐行读文件
来源：http://js.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ao.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://ea.nicolike.cn

[S49] C++：写文件
来源：http://ri.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ck.haigaiapp.cn

[S50] C++：格式化数字
来源：http://cc.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fe.panjiajie.cn

[S51] C++：显式类型转换
来源：http://df.wgjwhj.cn

static_cast<double>(a) / b
来源：http://dv.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://qh.newstarts.cn


<!-- 参考信息 -->