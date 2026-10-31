代发 wailian999

[Q82] 字符长度与字节长度
来源：http://pm.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hj.9csxet.cn

[Q83] 大小写转换
来源：http://nk.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lp.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://nl.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://gj.huanxung.cn

[Q85] 数值取整
来源：http://er.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mi.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://qk.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kz.colortex.cn

[Q87] JSON 字段做条件
来源：http://jh.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mu.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://qy.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fq.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ge.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://oo.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mv.huixiangedu.cn

[Q90] 生成序号列
来源：http://nu.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nf.521024.cn

================================================================================
来源：http://yn.521024.cn

R. Bash 专题
来源：http://rf.hahajie.cn

================================================================================
来源：http://ww.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://ts.521024.cn

#!/usr/bin/env bash
来源：http://pn.huixiangedu.cn

set -euo pipefail
来源：http://sr.hnjuh.cn

[R02] 变量赋值与使用
来源：http://bp.newstarts.cn

name="Tom"; echo "$name"
来源：http://yd.hnjuh.cn

[R03] 只读变量
来源：http://bk.shxzukj.cn

readonly PI=3.14
来源：http://af.hnjuh.cn

[R04] 位置参数
来源：http://yb.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zz.huanxung.cn

[R05] 参数默认值
来源：http://rc.panjiajie.cn

name="${1:-default}"
来源：http://wh.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://hw.bjjhwx.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xv.bjjhwx.cn

[R07] if 判断文件
来源：http://sz.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ct.jctech888.com.cn

[R08] 数值比较
来源：http://xy.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bc.gzmigu.cn

[R09] 字符串比较
来源：http://tc.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ta.colortex.cn

[R10] 正则匹配
来源：http://ym.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gs.asd995.cn

[R11] case 多分支
来源：http://aj.asd995.cn

case "$1" in
来源：http://ij.521024.cn

start) echo "启动" ;;
来源：http://kt.panjiajie.cn

stop)  echo "停止" ;;
来源：http://hy.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://ge.yuntaijiaju.cn

esac
来源：http://pt.newstarts.cn

[R12] for 遍历文件
来源：http://qt.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://ak.9csxet.cn

[R13] for 计数循环
来源：http://cf.asd995.cn

for i in {1..10}; do echo "$i"; done
来源：http://gv.hahajie.cn

[R14] C 风格 for
来源：http://zt.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nf.9csxet.cn

[R15] while 逐行读文件
来源：http://rw.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fp.colortex.cn

[R16] until 等待条件
来源：http://rl.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hh.wgjwhj.cn

[R17] 数组定义与取值
来源：http://uj.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zs.bjjhwx.cn

[R18] 遍历数组
来源：http://fx.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zc.colortex.cn

[R19] 数组长度
来源：http://dy.newstarts.cn

echo "${#arr[@]}"
来源：http://yb.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://ga.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ry.yuntaijiaju.cn

[R21] 字符串长度
来源：http://or.nicolike.cn

echo "${#s}"
来源：http://px.jianghongdianzi.cn

[R22] 截取子串
来源：http://hl.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://xz.panjiajie.cn

[R23] 字符串替换
来源：http://tb.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vd.szxytkj.cn

[R24] 大小写转换
来源：http://fg.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qm.521024.cn

[R25] 去后缀 / 去前缀
来源：http://cg.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ac.szxytkj.cn

[R26] 命令替换
来源：http://vt.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://ue.shxzukj.cn

[R27] 算术展开
来源：http://og.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://rd.huixiangedu.cn

[R28] 浮点运算
来源：http://tk.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://wf.gzmigu.cn

[R29] 定义函数
来源：http://xn.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qd.gzmigu.cn

[R30] 函数返回状态码
来源：http://rj.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ie.colortex.cn

[R31] 局部变量
来源：http://um.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://if.jctech888.com.cn

[R32] 参数个数校验
来源：http://hz.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sy.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://lh.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gt.huanxung.cn

[R34] 退出时清理
来源：http://rf.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qs.shxzukj.cn

[R35] 后台执行并等待
来源：http://nw.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fm.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://ft.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xc.szxytkj.cn

[R37] 把输出赋给变量
来源：http://mx.huixinmuqiang.cn

files=$(ls -1)
来源：http://ia.521024.cn

[R38] 管道串联
来源：http://kg.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://ts.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://nl.huanxung.cn

cmd > out.log 2>&1
来源：http://sb.wgjwhj.cn

[R40] 追加写日志
来源：http://of.lnxyls.cn

echo "log" >> out.log
来源：http://he.muxihuayi.cn

[R41] 丢弃输出
来源：http://gp.newstarts.cn

cmd >/dev/null 2>&1
来源：http://vg.jianghongdianzi.cn

[R42] 输入重定向
来源：http://cz.bookmarksfly.cn

wc -l < a.txt
来源：http://ra.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://gc.9csxet.cn

find . -name "*.log" -type f
来源：http://eu.lnxyls.cn

[R44] 按修改时间查找
来源：http://fu.yuexingan06.cn

find . -mtime -7 -type f
来源：http://qg.hnjuh.cn

[R45] 批量删除
来源：http://il.newstarts.cn

find . -name "*.tmp" -delete
来源：http://kj.hahajie.cn

[R46] 递归替换文件内容
来源：http://mg.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wy.muxihuayi.cn

[R47] sed 单行替换
来源：http://et.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fr.9csxet.cn

[R48] awk 取指定列
来源：http://yb.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://xa.panjiajie.cn

[R49] awk 带条件
来源：http://gn.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cr.haigaiapp.cn

[R50] awk 求和
来源：http://sj.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://el.huanxung.cn

[R51] 排序去重取前几
来源：http://ux.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qt.yuntaijiaju.cn

[R52] 统计行数
来源：http://aq.szsharing.cn

wc -l a.txt
来源：http://xz.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://ft.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ha.521024.cn

[R54] 比较两个文件
来源：http://vw.bookmarksfly.cn

diff a.txt b.txt
来源：http://lb.shxzukj.cn

[R55] 压缩与解压
来源：http://qi.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dw.bjjhwx.cn

[R56] 远程拷贝
来源：http://du.bookmarksfly.cn

scp file user@host:/path/
来源：http://qv.nicolike.cn

[R57] 远程执行命令
来源：http://po.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://il.szsharing.cn

[R58] 下载文件
来源：http://rz.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uo.bjjhwx.cn

[R59] 发 POST JSON
来源：http://ho.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vs.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://dy.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pm.gzmigu.cn

[R61] 磁盘占用
来源：http://xu.bjjhwx.cn

df -h;  du -sh *
来源：http://ga.shxzskj.cn

[R62] 找最占空间的文件
来源：http://vd.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://uz.9csxet.cn

[R63] 内存与进程
来源：http://el.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://tu.wgjwhj.cn

[R64] 结束进程
来源：http://fk.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://cx.asd995.cn

[R65] 查看端口占用
来源：http://cm.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://av.chemitech.net.cn

[R66] 定时任务
来源：http://fw.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://pu.colortex.cn

[R67] 生成随机十六进制串
来源：http://vm.colortex.cn

openssl rand -hex 16
来源：http://jf.shxzskj.cn

[R68] 计算文件校验值
来源：http://yc.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ok.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://gq.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://pc.panjiajie.cn

[R70] 时间戳与互转
来源：http://os.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://ml.nszjky.cn

[R71] 日期格式化
来源：http://xy.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yb.muxihuayi.cn

[R72] 等待端口就绪
来源：http://eb.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xi.521024.cn

[R73] 分割大日志
来源：http://vy.hnjuh.cn

split -l 1000 big.log part_
来源：http://ki.gzmigu.cn

[R74] 批量重命名
来源：http://px.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jv.bookmarksfly.cn

[R75] 导出环境变量
来源：http://yu.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://zf.asd995.cn

[R76] 使用临时文件
来源：http://xf.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wh.yuexingan06.cn

[R77] 读取用户输入
来源：http://fx.yuexingan06.cn

read -rp "请输入: " ans
来源：http://rx.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://ww.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oo.panjiajie.cn

[R79] 解析命令行选项
来源：http://kc.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iu.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://pj.asd995.cn

time ./run.sh
来源：http://vg.huixiangedu.cn

================================================================================
来源：http://yk.panjiajie.cn

S. C / C++ 专题
来源：http://fw.jianghongdianzi.cn

================================================================================
来源：http://wz.panjiajie.cn

[S01] C：Hello World
来源：http://dv.lnxyls.cn

#include <stdio.h>
来源：http://xh.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vc.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://ty.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://sr.yuexingan06.cn

[S03] C：读入整数
来源：http://ao.hnjuh.cn

int x; scanf("%d", &x);
来源：http://lj.shxzukj.cn

[S04] C：字符串复制
来源：http://oo.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ud.9csxet.cn

[S05] C：字符串长度
来源：http://ui.huixiangedu.cn

strlen(s)
来源：http://tj.bjjhwx.cn

[S06] C：字符串比较
来源：http://gv.muxihuayi.cn

strcmp(a, b) == 0
来源：http://lu.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://qf.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xt.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://kk.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gc.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://xq.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yg.colortex.cn

[S10] C：指针与解引用
来源：http://pf.nicolike.cn

int *p = &a;  *p = 5;
来源：http://yu.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://vy.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://nk.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mj.colortex.cn

fclose(f);
来源：http://cl.gzmigu.cn

[S12] C：写文件
来源：http://lb.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rz.wgjwhj.cn

[S13] C：宏定义
来源：http://ab.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ze.9csxet.cn

[S14] C：枚举
来源：http://ui.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://ti.shtwfgs.cn

[S15] C：类型转换
来源：http://ny.asd995.cn

(double) a / b
来源：http://sa.bjjhwx.cn

[S16] C：位操作置位
来源：http://sp.muxihuayi.cn

x |= (1 << 3);
来源：http://ct.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://gp.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cl.shtwfgs.cn

[S18] C：命令行参数
来源：http://cl.521024.cn

int main(int argc, char **argv)
来源：http://tz.yuntaijiaju.cn

[S19] C：快速排序
来源：http://ci.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uq.muxihuayi.cn

[S20] C：二分查找
来源：http://ns.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ya.shxzukj.cn

[S21] C：字符类别判断
来源：http://jr.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qa.wgjwhj.cn

[S22] C：字符串转数字
来源：http://fs.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bg.huixinmuqiang.cn

[S23] C：随机数
来源：http://vb.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://en.nicolike.cn

[S24] C：获取本地时间
来源：http://tv.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yp.bjjhwx.cn

[S25] C：内存拷贝
来源：http://cx.nicolike.cn

memcpy(dst, src, n);
来源：http://nm.chemitech.net.cn

[S26] C：内存清零
来源：http://kj.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://jb.chemitech.net.cn

[S27] C：定义常量
来源：http://qg.chemitech.net.cn

const double PI = 3.14159;
来源：http://sz.521024.cn

[S28] C：静态变量
来源：http://lc.jctech888.com.cn

static int counter = 0;
来源：http://ah.haigaiapp.cn

[S29] C：变参函数
来源：http://kp.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yz.jctech888.com.cn

[S30] C：头文件保护
来源：http://iy.yuexingan06.cn

#ifndef X_H
来源：http://up.wgjwhj.cn

#define X_H
来源：http://mn.panjiajie.cn

#endif
来源：http://hl.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://yd.haigaiapp.cn

#include <iostream>
来源：http://vd.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://am.shxzskj.cn

[S32] C++：字符串
来源：http://hz.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://nf.asd995.cn

[S33] C++：vector 增删
来源：http://wi.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gm.newstarts.cn

[S34] C++：遍历 vector
来源：http://py.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://is.bjjhwx.cn

[S35] C++：map
来源：http://wt.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xa.haigaiapp.cn

[S36] C++：unordered_map
来源：http://jp.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mt.bjjhwx.cn

[S37] C++：set
来源：http://hp.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zn.shxzskj.cn

[S38] C++：排序
来源：http://gc.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://iq.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://ad.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ou.bookmarksfly.cn

[S40] C++：查找元素
来源：http://gs.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fv.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://vo.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ei.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://zb.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://lk.shxzukj.cn

[S43] C++：智能指针
来源：http://ml.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://lp.bjjhwx.cn

[S44] C++：引用传参
来源：http://du.colortex.cn

void inc(int &x) { ++x; }
来源：http://st.bjjhwx.cn

[S45] C++：lambda
来源：http://jf.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mv.jctech888.com.cn

[S46] C++：函数模板
来源：http://dk.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rm.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://fl.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://na.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://aa.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://we.hahajie.cn

while (std::getline(in, line)) { }
来源：http://dl.nicolike.cn

[S49] C++：写文件
来源：http://rq.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zn.jctech888.com.cn

[S50] C++：格式化数字
来源：http://wx.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ie.nicolike.cn

[S51] C++：显式类型转换
来源：http://tk.chemitech.net.cn

static_cast<double>(a) / b
来源：http://fz.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://la.nicolike.cn


<!-- 参考信息 -->