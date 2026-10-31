代发 wailian999

[Q82] 字符长度与字节长度
来源：http://mt.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ic.9csxet.cn

[Q83] 大小写转换
来源：http://bx.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bb.nicolike.cn

[Q84] 去除首尾空格
来源：http://ku.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://xp.nszjky.cn

[Q85] 数值取整
来源：http://go.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vj.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://ri.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wu.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://xi.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zr.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://ek.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rf.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pb.huanxung.cn

[Q89] 判断表是否存在
来源：http://zv.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ln.hahajie.cn

[Q90] 生成序号列
来源：http://nm.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bv.szxytkj.cn

================================================================================
来源：http://my.muxihuayi.cn

R. Bash 专题
来源：http://fh.huixiangedu.cn

================================================================================
来源：http://dz.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://nx.nszjky.cn

#!/usr/bin/env bash
来源：http://fx.huixinmuqiang.cn

set -euo pipefail
来源：http://dp.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://og.gzmigu.cn

name="Tom"; echo "$name"
来源：http://wb.shxzukj.cn

[R03] 只读变量
来源：http://xf.szxytkj.cn

readonly PI=3.14
来源：http://mh.bookmarksfly.cn

[R04] 位置参数
来源：http://wa.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fb.huixiangedu.cn

[R05] 参数默认值
来源：http://vl.muxihuayi.cn

name="${1:-default}"
来源：http://yn.9csxet.cn

[R06] 判断命令是否存在
来源：http://jc.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://un.nicolike.cn

[R07] if 判断文件
来源：http://vl.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wq.huixinmuqiang.cn

[R08] 数值比较
来源：http://ix.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ed.bookmarksfly.cn

[R09] 字符串比较
来源：http://cg.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ba.panjiajie.cn

[R10] 正则匹配
来源：http://cf.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xx.bookmarksfly.cn

[R11] case 多分支
来源：http://sk.wgjwhj.cn

case "$1" in
来源：http://fb.shtwfgs.cn

start) echo "启动" ;;
来源：http://yg.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://dv.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://zm.bjjhwx.cn

esac
来源：http://jt.newstarts.cn

[R12] for 遍历文件
来源：http://kd.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://an.panjiajie.cn

[R13] for 计数循环
来源：http://fy.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://bc.9csxet.cn

[R14] C 风格 for
来源：http://pj.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://br.nicolike.cn

[R15] while 逐行读文件
来源：http://hp.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ro.bookmarksfly.cn

[R16] until 等待条件
来源：http://kq.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kt.wgjwhj.cn

[R17] 数组定义与取值
来源：http://fb.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lk.bjjhwx.cn

[R18] 遍历数组
来源：http://sm.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zt.hnjuh.cn

[R19] 数组长度
来源：http://cm.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://xi.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://ip.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vz.hahajie.cn

[R21] 字符串长度
来源：http://kb.lnxyls.cn

echo "${#s}"
来源：http://jl.jianghongdianzi.cn

[R22] 截取子串
来源：http://wq.chemitech.net.cn

echo "${s:0:5}"
来源：http://tk.521024.cn

[R23] 字符串替换
来源：http://eu.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cy.huixiangedu.cn

[R24] 大小写转换
来源：http://id.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ak.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://lx.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ay.gzmigu.cn

[R26] 命令替换
来源：http://ah.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://zr.newstarts.cn

[R27] 算术展开
来源：http://tl.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://aq.shxzskj.cn

[R28] 浮点运算
来源：http://sw.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://ud.szxytkj.cn

[R29] 定义函数
来源：http://ye.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ce.huanxung.cn

[R30] 函数返回状态码
来源：http://xk.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://dm.wgjwhj.cn

[R31] 局部变量
来源：http://oy.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://dv.9csxet.cn

[R32] 参数个数校验
来源：http://fw.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ac.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://ou.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jc.nszjky.cn

[R34] 退出时清理
来源：http://li.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qy.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://kw.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://os.hahajie.cn

[R36] 并发执行多个任务
来源：http://fj.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bj.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://fn.asd995.cn

files=$(ls -1)
来源：http://ga.huixinmuqiang.cn

[R38] 管道串联
来源：http://gy.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://mj.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://qj.shxzukj.cn

cmd > out.log 2>&1
来源：http://an.shxzukj.cn

[R40] 追加写日志
来源：http://it.521024.cn

echo "log" >> out.log
来源：http://mr.szsharing.cn

[R41] 丢弃输出
来源：http://jd.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://ao.bookmarksfly.cn

[R42] 输入重定向
来源：http://le.asd995.cn

wc -l < a.txt
来源：http://yi.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://jk.shtwfgs.cn

find . -name "*.log" -type f
来源：http://lg.huanxung.cn

[R44] 按修改时间查找
来源：http://gb.shxzukj.cn

find . -mtime -7 -type f
来源：http://iv.bookmarksfly.cn

[R45] 批量删除
来源：http://du.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://mi.hahajie.cn

[R46] 递归替换文件内容
来源：http://em.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iq.szxytkj.cn

[R47] sed 单行替换
来源：http://qq.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bz.shtwfgs.cn

[R48] awk 取指定列
来源：http://pd.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://ym.huixiangedu.cn

[R49] awk 带条件
来源：http://qx.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sx.521024.cn

[R50] awk 求和
来源：http://zz.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ji.panjiajie.cn

[R51] 排序去重取前几
来源：http://yu.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://li.yuexingan06.cn

[R52] 统计行数
来源：http://np.wgjwhj.cn

wc -l a.txt
来源：http://mi.521024.cn

[R53] 查看文件头与实时尾
来源：http://qd.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jq.yuexingan06.cn

[R54] 比较两个文件
来源：http://km.lnxyls.cn

diff a.txt b.txt
来源：http://fc.shtwfgs.cn

[R55] 压缩与解压
来源：http://zp.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bp.asd995.cn

[R56] 远程拷贝
来源：http://aq.chemitech.net.cn

scp file user@host:/path/
来源：http://ew.huixiangedu.cn

[R57] 远程执行命令
来源：http://ru.szsharing.cn

ssh user@host 'uptime'
来源：http://dj.nszjky.cn

[R58] 下载文件
来源：http://yy.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fx.lnxyls.cn

[R59] 发 POST JSON
来源：http://sh.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gl.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://qr.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://px.bjjhwx.cn

[R61] 磁盘占用
来源：http://vi.haigaiapp.cn

df -h;  du -sh *
来源：http://ic.panjiajie.cn

[R62] 找最占空间的文件
来源：http://ko.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://vd.szxytkj.cn

[R63] 内存与进程
来源：http://he.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://uv.bjjhwx.cn

[R64] 结束进程
来源：http://bg.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://yr.panjiajie.cn

[R65] 查看端口占用
来源：http://so.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vz.nszjky.cn

[R66] 定时任务
来源：http://xv.szsharing.cn

crontab -e;  crontab -l
来源：http://il.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://bz.gzmigu.cn

openssl rand -hex 16
来源：http://rf.colortex.cn

[R68] 计算文件校验值
来源：http://oo.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qa.colortex.cn

[R69] 生成随机密码
来源：http://sz.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://tn.shtwfgs.cn

[R70] 时间戳与互转
来源：http://no.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://lx.muxihuayi.cn

[R71] 日期格式化
来源：http://fh.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rc.newstarts.cn

[R72] 等待端口就绪
来源：http://ir.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ys.szxytkj.cn

[R73] 分割大日志
来源：http://cn.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://bv.hnjuh.cn

[R74] 批量重命名
来源：http://xw.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hu.bjjhwx.cn

[R75] 导出环境变量
来源：http://ea.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://ae.hnjuh.cn

[R76] 使用临时文件
来源：http://os.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lt.bookmarksfly.cn

[R77] 读取用户输入
来源：http://mt.newstarts.cn

read -rp "请输入: " ans
来源：http://pc.hahajie.cn

[R78] 交互式菜单
来源：http://nq.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bv.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://ub.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kh.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://vg.yuntaijiaju.cn

time ./run.sh
来源：http://vr.yuexingan06.cn

================================================================================
来源：http://pu.haigaiapp.cn

S. C / C++ 专题
来源：http://yh.asd995.cn

================================================================================
来源：http://zv.panjiajie.cn

[S01] C：Hello World
来源：http://tm.shxzskj.cn

#include <stdio.h>
来源：http://sf.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ye.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://rp.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://lu.chemitech.net.cn

[S03] C：读入整数
来源：http://yh.asd995.cn

int x; scanf("%d", &x);
来源：http://cy.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://le.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rk.shtwfgs.cn

[S05] C：字符串长度
来源：http://dp.hahajie.cn

strlen(s)
来源：http://bo.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://cj.panjiajie.cn

strcmp(a, b) == 0
来源：http://vr.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://xw.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vj.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://sn.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lz.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://ll.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gi.shtwfgs.cn

[S10] C：指针与解引用
来源：http://qc.nicolike.cn

int *p = &a;  *p = 5;
来源：http://pv.szxytkj.cn

[S11] C：逐行读文件
来源：http://bk.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://as.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://js.huixinmuqiang.cn

fclose(f);
来源：http://gw.panjiajie.cn

[S12] C：写文件
来源：http://wp.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cv.hahajie.cn

[S13] C：宏定义
来源：http://zw.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ag.szsharing.cn

[S14] C：枚举
来源：http://ms.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://vy.jianghongdianzi.cn

[S15] C：类型转换
来源：http://wc.huanxung.cn

(double) a / b
来源：http://ae.colortex.cn

[S16] C：位操作置位
来源：http://dc.newstarts.cn

x |= (1 << 3);
来源：http://jd.asd995.cn

[S17] C：安全拼接字符串
来源：http://dt.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ne.newstarts.cn

[S18] C：命令行参数
来源：http://xg.bjjhwx.cn

int main(int argc, char **argv)
来源：http://oc.szsharing.cn

[S19] C：快速排序
来源：http://yp.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hu.szsharing.cn

[S20] C：二分查找
来源：http://fp.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://it.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://rs.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ui.bjjhwx.cn

[S22] C：字符串转数字
来源：http://sc.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pj.nicolike.cn

[S23] C：随机数
来源：http://pp.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://df.huanxung.cn

[S24] C：获取本地时间
来源：http://be.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yd.yuexingan06.cn

[S25] C：内存拷贝
来源：http://ys.gzmigu.cn

memcpy(dst, src, n);
来源：http://fb.shtwfgs.cn

[S26] C：内存清零
来源：http://on.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://yz.huanxung.cn

[S27] C：定义常量
来源：http://bb.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://xh.huixiangedu.cn

[S28] C：静态变量
来源：http://ef.colortex.cn

static int counter = 0;
来源：http://ce.9csxet.cn

[S29] C：变参函数
来源：http://ec.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ob.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://aj.521024.cn

#ifndef X_H
来源：http://wd.szsharing.cn

#define X_H
来源：http://zb.shtwfgs.cn

#endif
来源：http://lr.hnjuh.cn

[S31] C++：Hello World
来源：http://nw.yuexingan06.cn

#include <iostream>
来源：http://ka.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://ik.jianghongdianzi.cn

[S32] C++：字符串
来源：http://aa.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://gi.hnjuh.cn

[S33] C++：vector 增删
来源：http://bw.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ib.521024.cn

[S34] C++：遍历 vector
来源：http://gg.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://la.newstarts.cn

[S35] C++：map
来源：http://cs.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sx.huixiangedu.cn

[S36] C++：unordered_map
来源：http://bg.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jy.gzmigu.cn

[S37] C++：set
来源：http://sg.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ru.shxzskj.cn

[S38] C++：排序
来源：http://jw.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://lx.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://da.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://se.nszjky.cn

[S40] C++：查找元素
来源：http://dx.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wp.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://we.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oz.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://kx.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://zx.hahajie.cn

[S43] C++：智能指针
来源：http://jz.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://tv.szxytkj.cn

[S44] C++：引用传参
来源：http://ez.asd995.cn

void inc(int &x) { ++x; }
来源：http://lj.muxihuayi.cn

[S45] C++：lambda
来源：http://zm.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mh.bjjhwx.cn

[S46] C++：函数模板
来源：http://yl.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://js.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://zr.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kx.shxzukj.cn

[S48] C++：逐行读文件
来源：http://xf.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vm.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://yf.asd995.cn

[S49] C++：写文件
来源：http://vf.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hw.huixiangedu.cn

[S50] C++：格式化数字
来源：http://eh.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pi.gzmigu.cn

[S51] C++：显式类型转换
来源：http://bc.wgjwhj.cn

static_cast<double>(a) / b
来源：http://qh.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://kn.shxzukj.cn


<!-- 参考信息 -->