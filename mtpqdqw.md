代发 wailian999

[Q80] 字符串截取
来源：http://ng.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kf.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://ve.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nc.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://rd.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dp.shxzskj.cn

[Q83] 大小写转换
来源：http://bg.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ov.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://ej.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://cy.9csxet.cn

[Q85] 数值取整
来源：http://zx.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qz.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://rv.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tz.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://bw.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vu.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://lc.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vs.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mk.colortex.cn

[Q89] 判断表是否存在
来源：http://ul.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hh.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://hf.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://al.szsharing.cn

================================================================================
来源：http://pm.huixinmuqiang.cn

R. Bash 专题
来源：http://vn.huanxung.cn

================================================================================
来源：http://do.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://ex.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://ip.bjjhwx.cn

set -euo pipefail
来源：http://il.hnjuh.cn

[R02] 变量赋值与使用
来源：http://zw.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://js.521024.cn

[R03] 只读变量
来源：http://zz.shtwfgs.cn

readonly PI=3.14
来源：http://kq.lnxyls.cn

[R04] 位置参数
来源：http://cl.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ky.huanxung.cn

[R05] 参数默认值
来源：http://oi.jctech888.com.cn

name="${1:-default}"
来源：http://oi.hnjuh.cn

[R06] 判断命令是否存在
来源：http://aa.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jy.lnxyls.cn

[R07] if 判断文件
来源：http://ph.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lr.huixinmuqiang.cn

[R08] 数值比较
来源：http://vn.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yk.yuexingan06.cn

[R09] 字符串比较
来源：http://hr.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ge.colortex.cn

[R10] 正则匹配
来源：http://vi.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zu.huanxung.cn

[R11] case 多分支
来源：http://ym.huanxung.cn

case "$1" in
来源：http://to.szxytkj.cn

start) echo "启动" ;;
来源：http://tv.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://ti.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://rd.nszjky.cn

esac
来源：http://gm.chemitech.net.cn

[R12] for 遍历文件
来源：http://js.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://ex.521024.cn

[R13] for 计数循环
来源：http://tx.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://xn.gzmigu.cn

[R14] C 风格 for
来源：http://gf.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sd.asd995.cn

[R15] while 逐行读文件
来源：http://xr.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gi.asd995.cn

[R16] until 等待条件
来源：http://aw.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bs.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://ej.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vd.bjjhwx.cn

[R18] 遍历数组
来源：http://hx.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zx.jctech888.com.cn

[R19] 数组长度
来源：http://pf.asd995.cn

echo "${#arr[@]}"
来源：http://zn.nicolike.cn

[R20] 关联数组（字典）
来源：http://wp.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wv.lnxyls.cn

[R21] 字符串长度
来源：http://bt.shxzukj.cn

echo "${#s}"
来源：http://on.colortex.cn

[R22] 截取子串
来源：http://fo.lnxyls.cn

echo "${s:0:5}"
来源：http://tk.lnxyls.cn

[R23] 字符串替换
来源：http://qj.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mx.shtwfgs.cn

[R24] 大小写转换
来源：http://ig.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wr.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://dt.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nw.wgjwhj.cn

[R26] 命令替换
来源：http://cm.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://er.shxzukj.cn

[R27] 算术展开
来源：http://sa.newstarts.cn

echo $((1 + 2 * 3))
来源：http://bs.szxytkj.cn

[R28] 浮点运算
来源：http://tv.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://ia.yuntaijiaju.cn

[R29] 定义函数
来源：http://px.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://up.521024.cn

[R30] 函数返回状态码
来源：http://po.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://fw.hnjuh.cn

[R31] 局部变量
来源：http://jk.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://jv.hahajie.cn

[R32] 参数个数校验
来源：http://ld.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bt.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://oz.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rm.shxzskj.cn

[R34] 退出时清理
来源：http://cu.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kd.huixiangedu.cn

[R35] 后台执行并等待
来源：http://xp.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://px.521024.cn

[R36] 并发执行多个任务
来源：http://dv.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hu.newstarts.cn

[R37] 把输出赋给变量
来源：http://ic.colortex.cn

files=$(ls -1)
来源：http://aq.shxzukj.cn

[R38] 管道串联
来源：http://nl.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://tz.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://la.asd995.cn

cmd > out.log 2>&1
来源：http://qr.newstarts.cn

[R40] 追加写日志
来源：http://gm.shtwfgs.cn

echo "log" >> out.log
来源：http://rf.lnxyls.cn

[R41] 丢弃输出
来源：http://cq.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://ye.huixiangedu.cn

[R42] 输入重定向
来源：http://wf.jianghongdianzi.cn

wc -l < a.txt
来源：http://ht.9csxet.cn

[R43] 按名字查找文件
来源：http://rv.muxihuayi.cn

find . -name "*.log" -type f
来源：http://iq.asd995.cn

[R44] 按修改时间查找
来源：http://ts.521024.cn

find . -mtime -7 -type f
来源：http://og.szsharing.cn

[R45] 批量删除
来源：http://ve.newstarts.cn

find . -name "*.tmp" -delete
来源：http://of.szsharing.cn

[R46] 递归替换文件内容
来源：http://dx.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ad.shxzskj.cn

[R47] sed 单行替换
来源：http://ma.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ih.jctech888.com.cn

[R48] awk 取指定列
来源：http://hc.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://cb.huanxung.cn

[R49] awk 带条件
来源：http://fo.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ib.muxihuayi.cn

[R50] awk 求和
来源：http://uh.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wk.szxytkj.cn

[R51] 排序去重取前几
来源：http://ez.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uf.jianghongdianzi.cn

[R52] 统计行数
来源：http://jx.szsharing.cn

wc -l a.txt
来源：http://kq.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://vt.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kr.newstarts.cn

[R54] 比较两个文件
来源：http://gk.lnxyls.cn

diff a.txt b.txt
来源：http://ol.colortex.cn

[R55] 压缩与解压
来源：http://jz.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qz.newstarts.cn

[R56] 远程拷贝
来源：http://fy.huixinmuqiang.cn

scp file user@host:/path/
来源：http://jr.szxytkj.cn

[R57] 远程执行命令
来源：http://ov.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://jb.jianghongdianzi.cn

[R58] 下载文件
来源：http://jb.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://li.asd995.cn

[R59] 发 POST JSON
来源：http://hw.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kx.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://ka.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cw.colortex.cn

[R61] 磁盘占用
来源：http://mi.szxytkj.cn

df -h;  du -sh *
来源：http://ip.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://pm.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://sc.shtwfgs.cn

[R63] 内存与进程
来源：http://na.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://cx.nszjky.cn

[R64] 结束进程
来源：http://gl.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://rw.nszjky.cn

[R65] 查看端口占用
来源：http://sf.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qt.shxzukj.cn

[R66] 定时任务
来源：http://qh.asd995.cn

crontab -e;  crontab -l
来源：http://fr.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://cw.yuntaijiaju.cn

openssl rand -hex 16
来源：http://wc.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://rp.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ch.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://tk.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://bj.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://ya.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://zf.shxzukj.cn

[R71] 日期格式化
来源：http://fv.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yc.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://ze.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vy.huanxung.cn

[R73] 分割大日志
来源：http://lc.haigaiapp.cn

split -l 1000 big.log part_
来源：http://qc.shxzukj.cn

[R74] 批量重命名
来源：http://lm.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fq.szxytkj.cn

[R75] 导出环境变量
来源：http://is.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://xk.hahajie.cn

[R76] 使用临时文件
来源：http://au.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wf.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://dj.hahajie.cn

read -rp "请输入: " ans
来源：http://cb.szxytkj.cn

[R78] 交互式菜单
来源：http://go.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oi.szxytkj.cn

[R79] 解析命令行选项
来源：http://fi.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ds.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://fm.chemitech.net.cn

time ./run.sh
来源：http://tq.huixiangedu.cn

================================================================================
来源：http://gr.haigaiapp.cn

S. C / C++ 专题
来源：http://eb.bjjhwx.cn

================================================================================
来源：http://cg.newstarts.cn

[S01] C：Hello World
来源：http://pg.lnxyls.cn

#include <stdio.h>
来源：http://kt.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yj.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://je.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://tc.huanxung.cn

[S03] C：读入整数
来源：http://og.gzmigu.cn

int x; scanf("%d", &x);
来源：http://om.huanxung.cn

[S04] C：字符串复制
来源：http://lj.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ok.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://lj.colortex.cn

strlen(s)
来源：http://vi.panjiajie.cn

[S06] C：字符串比较
来源：http://fn.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://gh.panjiajie.cn

[S07] C：数组遍历求和
来源：http://fs.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eg.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://ie.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jp.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://yt.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ta.jctech888.com.cn

[S10] C：指针与解引用
来源：http://iv.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://uv.huixiangedu.cn

[S11] C：逐行读文件
来源：http://tk.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://fi.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qk.chemitech.net.cn

fclose(f);
来源：http://xd.bookmarksfly.cn

[S12] C：写文件
来源：http://vm.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://st.shxzukj.cn

[S13] C：宏定义
来源：http://nb.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pp.huanxung.cn

[S14] C：枚举
来源：http://io.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://gn.bjjhwx.cn

[S15] C：类型转换
来源：http://kk.colortex.cn

(double) a / b
来源：http://sd.shxzukj.cn

[S16] C：位操作置位
来源：http://ll.colortex.cn

x |= (1 << 3);
来源：http://bq.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://bc.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bn.yuexingan06.cn

[S18] C：命令行参数
来源：http://lw.gzmigu.cn

int main(int argc, char **argv)
来源：http://kk.nicolike.cn

[S19] C：快速排序
来源：http://wh.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qn.szsharing.cn

[S20] C：二分查找
来源：http://kl.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ba.panjiajie.cn

[S21] C：字符类别判断
来源：http://wz.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ml.jctech888.com.cn

[S22] C：字符串转数字
来源：http://px.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cu.newstarts.cn

[S23] C：随机数
来源：http://vz.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uo.wgjwhj.cn

[S24] C：获取本地时间
来源：http://hi.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xf.lnxyls.cn

[S25] C：内存拷贝
来源：http://fu.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://pl.colortex.cn

[S26] C：内存清零
来源：http://xg.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://zh.huixiangedu.cn

[S27] C：定义常量
来源：http://zy.asd995.cn

const double PI = 3.14159;
来源：http://lt.panjiajie.cn

[S28] C：静态变量
来源：http://sw.nicolike.cn

static int counter = 0;
来源：http://dn.huixinmuqiang.cn

[S29] C：变参函数
来源：http://ot.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lq.huixiangedu.cn

[S30] C：头文件保护
来源：http://sq.shtwfgs.cn

#ifndef X_H
来源：http://qf.bookmarksfly.cn

#define X_H
来源：http://tu.chemitech.net.cn

#endif
来源：http://ol.lnxyls.cn

[S31] C++：Hello World
来源：http://oy.nszjky.cn

#include <iostream>
来源：http://eb.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://np.hahajie.cn

[S32] C++：字符串
来源：http://cq.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://ub.shxzukj.cn

[S33] C++：vector 增删
来源：http://xc.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ic.nicolike.cn

[S34] C++：遍历 vector
来源：http://de.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://ui.szxytkj.cn

[S35] C++：map
来源：http://an.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ic.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://vz.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://he.hahajie.cn

[S37] C++：set
来源：http://zh.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jw.bookmarksfly.cn

[S38] C++：排序
来源：http://sh.asd995.cn

std::sort(v.begin(), v.end());
来源：http://ez.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://eq.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vj.521024.cn

[S40] C++：查找元素
来源：http://px.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mk.panjiajie.cn

[S41] C++：类与构造函数
来源：http://so.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://we.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://wb.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://xd.521024.cn

[S43] C++：智能指针
来源：http://wv.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://il.wgjwhj.cn

[S44] C++：引用传参
来源：http://rh.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://qc.shtwfgs.cn

[S45] C++：lambda
来源：http://pu.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rh.huixiangedu.cn

[S46] C++：函数模板
来源：http://iu.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fi.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://zx.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iw.asd995.cn

[S48] C++：逐行读文件
来源：http://ow.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kr.szsharing.cn

while (std::getline(in, line)) { }
来源：http://ii.huixinmuqiang.cn

[S49] C++：写文件
来源：http://rl.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://an.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://qn.nicolike.cn


<!-- 参考信息 -->