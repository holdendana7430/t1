代发 wailian999

[Q80] 字符串截取
来源：http://ha.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xv.panjiajie.cn

[Q81] 字符串替换
来源：http://gh.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ur.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://ue.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ch.szsharing.cn

[Q83] 大小写转换
来源：http://ke.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ro.hahajie.cn

[Q84] 去除首尾空格
来源：http://uj.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://mc.shxzukj.cn

[Q85] 数值取整
来源：http://xz.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wf.colortex.cn

[Q86] 读取 JSON 字段
来源：http://qv.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kr.9csxet.cn

[Q87] JSON 字段做条件
来源：http://ea.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mr.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://ww.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yh.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ap.lnxyls.cn

[Q89] 判断表是否存在
来源：http://uq.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yk.szsharing.cn

[Q90] 生成序号列
来源：http://oa.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ee.shxzskj.cn

================================================================================
来源：http://eb.9csxet.cn

R. Bash 专题
来源：http://pq.jctech888.com.cn

================================================================================
来源：http://no.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://iq.nicolike.cn

#!/usr/bin/env bash
来源：http://zv.wgjwhj.cn

set -euo pipefail
来源：http://ez.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://ta.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://zr.szxytkj.cn

[R03] 只读变量
来源：http://lg.hahajie.cn

readonly PI=3.14
来源：http://lq.huixiangedu.cn

[R04] 位置参数
来源：http://yo.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cl.szsharing.cn

[R05] 参数默认值
来源：http://ev.huixiangedu.cn

name="${1:-default}"
来源：http://xs.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://es.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rs.colortex.cn

[R07] if 判断文件
来源：http://dp.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yr.shxzskj.cn

[R08] 数值比较
来源：http://nk.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ng.shxzskj.cn

[R09] 字符串比较
来源：http://fx.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fu.bjjhwx.cn

[R10] 正则匹配
来源：http://yu.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wq.yuntaijiaju.cn

[R11] case 多分支
来源：http://xb.chemitech.net.cn

case "$1" in
来源：http://oi.hnjuh.cn

start) echo "启动" ;;
来源：http://oo.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://en.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://qc.shtwfgs.cn

esac
来源：http://gs.haigaiapp.cn

[R12] for 遍历文件
来源：http://kb.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://ag.newstarts.cn

[R13] for 计数循环
来源：http://eb.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://cd.panjiajie.cn

[R14] C 风格 for
来源：http://yj.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lx.szxytkj.cn

[R15] while 逐行读文件
来源：http://gi.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wg.chemitech.net.cn

[R16] until 等待条件
来源：http://sz.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eb.9csxet.cn

[R17] 数组定义与取值
来源：http://sy.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xm.hahajie.cn

[R18] 遍历数组
来源：http://mm.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pk.muxihuayi.cn

[R19] 数组长度
来源：http://yr.nszjky.cn

echo "${#arr[@]}"
来源：http://hx.gzmigu.cn

[R20] 关联数组（字典）
来源：http://sc.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ys.newstarts.cn

[R21] 字符串长度
来源：http://cn.szxytkj.cn

echo "${#s}"
来源：http://wn.lnxyls.cn

[R22] 截取子串
来源：http://xz.huixiangedu.cn

echo "${s:0:5}"
来源：http://vd.szxytkj.cn

[R23] 字符串替换
来源：http://dw.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nm.wgjwhj.cn

[R24] 大小写转换
来源：http://vz.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zc.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://dp.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bm.szsharing.cn

[R26] 命令替换
来源：http://ao.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://sj.panjiajie.cn

[R27] 算术展开
来源：http://hr.colortex.cn

echo $((1 + 2 * 3))
来源：http://xo.nszjky.cn

[R28] 浮点运算
来源：http://ri.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://zc.gzmigu.cn

[R29] 定义函数
来源：http://dl.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yq.szxytkj.cn

[R30] 函数返回状态码
来源：http://he.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://qo.chemitech.net.cn

[R31] 局部变量
来源：http://pq.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://mg.haigaiapp.cn

[R32] 参数个数校验
来源：http://bc.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://da.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://uq.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aa.haigaiapp.cn

[R34] 退出时清理
来源：http://wk.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://re.nszjky.cn

[R35] 后台执行并等待
来源：http://su.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dd.521024.cn

[R36] 并发执行多个任务
来源：http://mu.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yh.asd995.cn

[R37] 把输出赋给变量
来源：http://oj.lnxyls.cn

files=$(ls -1)
来源：http://uh.yuexingan06.cn

[R38] 管道串联
来源：http://sp.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://rz.asd995.cn

[R39] 重定向标准输出与错误
来源：http://ka.hnjuh.cn

cmd > out.log 2>&1
来源：http://jz.9csxet.cn

[R40] 追加写日志
来源：http://fq.nicolike.cn

echo "log" >> out.log
来源：http://mn.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://ie.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://ye.nicolike.cn

[R42] 输入重定向
来源：http://uk.lnxyls.cn

wc -l < a.txt
来源：http://ye.newstarts.cn

[R43] 按名字查找文件
来源：http://za.shxzskj.cn

find . -name "*.log" -type f
来源：http://vs.shxzukj.cn

[R44] 按修改时间查找
来源：http://yj.haigaiapp.cn

find . -mtime -7 -type f
来源：http://gd.hahajie.cn

[R45] 批量删除
来源：http://uc.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://mo.521024.cn

[R46] 递归替换文件内容
来源：http://eb.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xp.nszjky.cn

[R47] sed 单行替换
来源：http://iv.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yq.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://ub.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://fa.szxytkj.cn

[R49] awk 带条件
来源：http://gg.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bn.muxihuayi.cn

[R50] awk 求和
来源：http://xh.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://su.jctech888.com.cn

[R51] 排序去重取前几
来源：http://kl.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xl.nszjky.cn

[R52] 统计行数
来源：http://xc.huanxung.cn

wc -l a.txt
来源：http://qz.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://fu.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gl.9csxet.cn

[R54] 比较两个文件
来源：http://nz.shxzskj.cn

diff a.txt b.txt
来源：http://bt.bookmarksfly.cn

[R55] 压缩与解压
来源：http://zh.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sm.wgjwhj.cn

[R56] 远程拷贝
来源：http://lt.huanxung.cn

scp file user@host:/path/
来源：http://br.gzmigu.cn

[R57] 远程执行命令
来源：http://lx.colortex.cn

ssh user@host 'uptime'
来源：http://ql.panjiajie.cn

[R58] 下载文件
来源：http://la.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pt.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://fz.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ei.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://or.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wp.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://fh.yuntaijiaju.cn

df -h;  du -sh *
来源：http://us.nszjky.cn

[R62] 找最占空间的文件
来源：http://ot.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://ed.lnxyls.cn

[R63] 内存与进程
来源：http://jg.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://ga.521024.cn

[R64] 结束进程
来源：http://jp.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://lr.521024.cn

[R65] 查看端口占用
来源：http://oe.nicolike.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qp.asd995.cn

[R66] 定时任务
来源：http://tw.hahajie.cn

crontab -e;  crontab -l
来源：http://fp.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://ek.huixinmuqiang.cn

openssl rand -hex 16
来源：http://ww.szsharing.cn

[R68] 计算文件校验值
来源：http://pt.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xo.chemitech.net.cn

[R69] 生成随机密码
来源：http://ev.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://hm.asd995.cn

[R70] 时间戳与互转
来源：http://re.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://mj.lnxyls.cn

[R71] 日期格式化
来源：http://iy.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cv.yuexingan06.cn

[R72] 等待端口就绪
来源：http://ga.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tw.shxzskj.cn

[R73] 分割大日志
来源：http://zy.panjiajie.cn

split -l 1000 big.log part_
来源：http://kb.jctech888.com.cn

[R74] 批量重命名
来源：http://rn.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://op.jianghongdianzi.cn

[R75] 导出环境变量
来源：http://ml.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://qp.hahajie.cn

[R76] 使用临时文件
来源：http://be.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mt.asd995.cn

[R77] 读取用户输入
来源：http://eq.nszjky.cn

read -rp "请输入: " ans
来源：http://st.szsharing.cn

[R78] 交互式菜单
来源：http://kz.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wo.jctech888.com.cn

[R79] 解析命令行选项
来源：http://aw.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wz.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://xw.gzmigu.cn

time ./run.sh
来源：http://jx.muxihuayi.cn

================================================================================
来源：http://vp.shxzukj.cn

S. C / C++ 专题
来源：http://cd.huixinmuqiang.cn

================================================================================
来源：http://cj.colortex.cn

[S01] C：Hello World
来源：http://oe.lnxyls.cn

#include <stdio.h>
来源：http://lk.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dz.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://hp.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://dw.jianghongdianzi.cn

[S03] C：读入整数
来源：http://ve.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://os.521024.cn

[S04] C：字符串复制
来源：http://ut.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bo.shtwfgs.cn

[S05] C：字符串长度
来源：http://rx.wgjwhj.cn

strlen(s)
来源：http://yp.shtwfgs.cn

[S06] C：字符串比较
来源：http://vf.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://lv.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://yk.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://is.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://dp.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hy.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://rw.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ij.shtwfgs.cn

[S10] C：指针与解引用
来源：http://dh.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://jo.shtwfgs.cn

[S11] C：逐行读文件
来源：http://gw.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://mk.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://th.yuexingan06.cn

fclose(f);
来源：http://vh.jianghongdianzi.cn

[S12] C：写文件
来源：http://xj.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ly.shtwfgs.cn

[S13] C：宏定义
来源：http://uu.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jy.newstarts.cn

[S14] C：枚举
来源：http://is.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://lg.haigaiapp.cn

[S15] C：类型转换
来源：http://gi.huixiangedu.cn

(double) a / b
来源：http://gx.521024.cn

[S16] C：位操作置位
来源：http://xu.newstarts.cn

x |= (1 << 3);
来源：http://zd.huanxung.cn

[S17] C：安全拼接字符串
来源：http://fi.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mn.panjiajie.cn

[S18] C：命令行参数
来源：http://lu.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://of.lnxyls.cn

[S19] C：快速排序
来源：http://ul.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xg.szxytkj.cn

[S20] C：二分查找
来源：http://ic.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yz.huixiangedu.cn

[S21] C：字符类别判断
来源：http://qv.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nl.yuexingan06.cn

[S22] C：字符串转数字
来源：http://ly.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://al.newstarts.cn

[S23] C：随机数
来源：http://gr.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hb.panjiajie.cn

[S24] C：获取本地时间
来源：http://li.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zg.haigaiapp.cn

[S25] C：内存拷贝
来源：http://ls.lnxyls.cn

memcpy(dst, src, n);
来源：http://di.shtwfgs.cn

[S26] C：内存清零
来源：http://lx.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://kj.lnxyls.cn

[S27] C：定义常量
来源：http://kg.hahajie.cn

const double PI = 3.14159;
来源：http://ba.panjiajie.cn

[S28] C：静态变量
来源：http://ji.bjjhwx.cn

static int counter = 0;
来源：http://ah.gzmigu.cn

[S29] C：变参函数
来源：http://zt.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vt.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://ua.hahajie.cn

#ifndef X_H
来源：http://uo.bjjhwx.cn

#define X_H
来源：http://fy.asd995.cn

#endif
来源：http://lu.gzmigu.cn

[S31] C++：Hello World
来源：http://or.muxihuayi.cn

#include <iostream>
来源：http://bn.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://nk.shxzskj.cn

[S32] C++：字符串
来源：http://ay.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://kr.haigaiapp.cn

[S33] C++：vector 增删
来源：http://zo.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rx.521024.cn

[S34] C++：遍历 vector
来源：http://zu.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://xl.nszjky.cn

[S35] C++：map
来源：http://nm.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lz.hnjuh.cn

[S36] C++：unordered_map
来源：http://yc.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fz.szxytkj.cn

[S37] C++：set
来源：http://zy.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sq.muxihuayi.cn

[S38] C++：排序
来源：http://ot.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://wh.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://yi.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fs.shxzukj.cn

[S40] C++：查找元素
来源：http://cf.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jv.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://zl.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uf.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://yb.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://rm.panjiajie.cn

[S43] C++：智能指针
来源：http://ey.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://ca.gzmigu.cn

[S44] C++：引用传参
来源：http://xv.hahajie.cn

void inc(int &x) { ++x; }
来源：http://no.wgjwhj.cn

[S45] C++：lambda
来源：http://an.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ga.shtwfgs.cn

[S46] C++：函数模板
来源：http://uk.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dl.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://em.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qi.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://ly.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ni.9csxet.cn

while (std::getline(in, line)) { }
来源：http://no.szxytkj.cn

[S49] C++：写文件
来源：http://rp.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://he.lnxyls.cn

[S50] C++：格式化数字
来源：http://vj.gzmigu.cn


<!-- 参考信息 -->