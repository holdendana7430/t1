代发 wailian999

[Q78] 当前时间
来源：http://gy.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ek.panjiajie.cn

[Q79] 字符串拼接
来源：http://ks.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rw.nszjky.cn

[Q80] 字符串截取
来源：http://hk.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://px.shxzskj.cn

[Q81] 字符串替换
来源：http://fe.bookmarksfly.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sc.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://ro.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yf.panjiajie.cn

[Q83] 大小写转换
来源：http://hu.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vm.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://rx.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://yi.jianghongdianzi.cn

[Q85] 数值取整
来源：http://sz.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://tt.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tk.hahajie.cn

[Q87] JSON 字段做条件
来源：http://bi.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tx.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://du.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rg.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hu.gzmigu.cn

[Q89] 判断表是否存在
来源：http://oy.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cf.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://my.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://op.shxzukj.cn

================================================================================
来源：http://xs.colortex.cn

R. Bash 专题
来源：http://gp.jianghongdianzi.cn

================================================================================
来源：http://jn.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://xs.hahajie.cn

#!/usr/bin/env bash
来源：http://pk.asd995.cn

set -euo pipefail
来源：http://rv.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://is.gzmigu.cn

name="Tom"; echo "$name"
来源：http://lu.jctech888.com.cn

[R03] 只读变量
来源：http://ty.jctech888.com.cn

readonly PI=3.14
来源：http://aa.szsharing.cn

[R04] 位置参数
来源：http://rf.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ex.haigaiapp.cn

[R05] 参数默认值
来源：http://lb.hahajie.cn

name="${1:-default}"
来源：http://sz.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://iy.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jx.nszjky.cn

[R07] if 判断文件
来源：http://ld.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ok.huanxung.cn

[R08] 数值比较
来源：http://ry.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wu.hahajie.cn

[R09] 字符串比较
来源：http://zw.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gd.nszjky.cn

[R10] 正则匹配
来源：http://aw.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hg.szsharing.cn

[R11] case 多分支
来源：http://mx.shtwfgs.cn

case "$1" in
来源：http://mr.9csxet.cn

start) echo "启动" ;;
来源：http://yn.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://ta.521024.cn

*)     echo "未知命令" ;;
来源：http://qd.shxzskj.cn

esac
来源：http://kh.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://gg.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://pt.chemitech.net.cn

[R13] for 计数循环
来源：http://mf.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://fd.lnxyls.cn

[R14] C 风格 for
来源：http://dl.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wi.haigaiapp.cn

[R15] while 逐行读文件
来源：http://ny.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pg.lnxyls.cn

[R16] until 等待条件
来源：http://nt.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ln.nszjky.cn

[R17] 数组定义与取值
来源：http://hv.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lc.newstarts.cn

[R18] 遍历数组
来源：http://zv.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ku.shxzukj.cn

[R19] 数组长度
来源：http://tv.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://oe.szxytkj.cn

[R20] 关联数组（字典）
来源：http://zo.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wn.gzmigu.cn

[R21] 字符串长度
来源：http://tp.colortex.cn

echo "${#s}"
来源：http://hw.hnjuh.cn

[R22] 截取子串
来源：http://ol.nicolike.cn

echo "${s:0:5}"
来源：http://nz.hahajie.cn

[R23] 字符串替换
来源：http://cg.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ju.szsharing.cn

[R24] 大小写转换
来源：http://dw.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rf.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://gu.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jn.shxzukj.cn

[R26] 命令替换
来源：http://wv.colortex.cn

now=$(date +%F); echo "$now"
来源：http://xm.szxytkj.cn

[R27] 算术展开
来源：http://gj.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://pn.shtwfgs.cn

[R28] 浮点运算
来源：http://mo.huixiangedu.cn

echo "scale=2; 10/3" | bc
来源：http://oq.panjiajie.cn

[R29] 定义函数
来源：http://ii.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bp.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://hz.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://ye.nicolike.cn

[R31] 局部变量
来源：http://xn.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://yq.nszjky.cn

[R32] 参数个数校验
来源：http://fo.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fw.521024.cn

[R33] 捕获错误并提示行号
来源：http://mt.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wz.bookmarksfly.cn

[R34] 退出时清理
来源：http://gl.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yx.haigaiapp.cn

[R35] 后台执行并等待
来源：http://bw.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ng.szxytkj.cn

[R36] 并发执行多个任务
来源：http://xu.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lb.colortex.cn

[R37] 把输出赋给变量
来源：http://gz.nszjky.cn

files=$(ls -1)
来源：http://wv.jianghongdianzi.cn

[R38] 管道串联
来源：http://vg.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://rr.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://hw.yuexingan06.cn

cmd > out.log 2>&1
来源：http://zj.huanxung.cn

[R40] 追加写日志
来源：http://zf.huixinmuqiang.cn

echo "log" >> out.log
来源：http://yt.hahajie.cn

[R41] 丢弃输出
来源：http://ju.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://jo.shxzskj.cn

[R42] 输入重定向
来源：http://yr.yuntaijiaju.cn

wc -l < a.txt
来源：http://lu.521024.cn

[R43] 按名字查找文件
来源：http://zw.wgjwhj.cn

find . -name "*.log" -type f
来源：http://wl.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://ia.asd995.cn

find . -mtime -7 -type f
来源：http://bp.asd995.cn

[R45] 批量删除
来源：http://jx.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://cx.nszjky.cn

[R46] 递归替换文件内容
来源：http://bs.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ay.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://sl.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pk.muxihuayi.cn

[R48] awk 取指定列
来源：http://ho.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://rd.yuexingan06.cn

[R49] awk 带条件
来源：http://bv.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ks.shxzskj.cn

[R50] awk 求和
来源：http://da.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jw.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://dr.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ar.hnjuh.cn

[R52] 统计行数
来源：http://ww.bookmarksfly.cn

wc -l a.txt
来源：http://wj.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://we.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tz.wgjwhj.cn

[R54] 比较两个文件
来源：http://jh.hnjuh.cn

diff a.txt b.txt
来源：http://yc.521024.cn

[R55] 压缩与解压
来源：http://qd.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gc.yuexingan06.cn

[R56] 远程拷贝
来源：http://wj.panjiajie.cn

scp file user@host:/path/
来源：http://go.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://ex.shxzskj.cn

ssh user@host 'uptime'
来源：http://dp.chemitech.net.cn

[R58] 下载文件
来源：http://xo.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ey.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://nd.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fb.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://an.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gn.nszjky.cn

[R61] 磁盘占用
来源：http://or.shxzskj.cn

df -h;  du -sh *
来源：http://dg.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://zj.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://gl.muxihuayi.cn

[R63] 内存与进程
来源：http://oj.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://dn.szsharing.cn

[R64] 结束进程
来源：http://fu.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://ol.jctech888.com.cn

[R65] 查看端口占用
来源：http://ut.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uy.jctech888.com.cn

[R66] 定时任务
来源：http://cx.bjjhwx.cn

crontab -e;  crontab -l
来源：http://jh.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://pz.shxzskj.cn

openssl rand -hex 16
来源：http://mt.lnxyls.cn

[R68] 计算文件校验值
来源：http://pc.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uv.hahajie.cn

[R69] 生成随机密码
来源：http://wg.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://ck.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://le.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://zw.colortex.cn

[R71] 日期格式化
来源：http://xf.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mz.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://gc.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://el.haigaiapp.cn

[R73] 分割大日志
来源：http://gf.nicolike.cn

split -l 1000 big.log part_
来源：http://ck.muxihuayi.cn

[R74] 批量重命名
来源：http://wh.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uw.szxytkj.cn

[R75] 导出环境变量
来源：http://tt.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://he.shtwfgs.cn

[R76] 使用临时文件
来源：http://cx.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ay.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://bw.hnjuh.cn

read -rp "请输入: " ans
来源：http://qy.shxzskj.cn

[R78] 交互式菜单
来源：http://ml.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pb.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://cq.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vg.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://vh.newstarts.cn

time ./run.sh
来源：http://zj.9csxet.cn

================================================================================
来源：http://so.bjjhwx.cn

S. C / C++ 专题
来源：http://cr.lnxyls.cn

================================================================================
来源：http://ng.shtwfgs.cn

[S01] C：Hello World
来源：http://wa.szsharing.cn

#include <stdio.h>
来源：http://vv.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ez.huanxung.cn

[S02] C：变量与格式化输出
来源：http://hj.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://wp.lnxyls.cn

[S03] C：读入整数
来源：http://gc.shxzukj.cn

int x; scanf("%d", &x);
来源：http://jb.nszjky.cn

[S04] C：字符串复制
来源：http://mo.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nj.shxzskj.cn

[S05] C：字符串长度
来源：http://ap.shxzukj.cn

strlen(s)
来源：http://rc.shxzskj.cn

[S06] C：字符串比较
来源：http://iq.gzmigu.cn

strcmp(a, b) == 0
来源：http://rh.asd995.cn

[S07] C：数组遍历求和
来源：http://ek.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zo.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://ch.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wp.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://xd.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gl.wgjwhj.cn

[S10] C：指针与解引用
来源：http://gh.521024.cn

int *p = &a;  *p = 5;
来源：http://am.huixiangedu.cn

[S11] C：逐行读文件
来源：http://jr.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://sn.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yg.asd995.cn

fclose(f);
来源：http://mz.asd995.cn

[S12] C：写文件
来源：http://fv.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qe.nszjky.cn

[S13] C：宏定义
来源：http://av.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qh.hahajie.cn

[S14] C：枚举
来源：http://io.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://is.huanxung.cn

[S15] C：类型转换
来源：http://if.shxzukj.cn

(double) a / b
来源：http://nw.szxytkj.cn

[S16] C：位操作置位
来源：http://dd.huixinmuqiang.cn

x |= (1 << 3);
来源：http://pa.nszjky.cn

[S17] C：安全拼接字符串
来源：http://ue.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://px.muxihuayi.cn

[S18] C：命令行参数
来源：http://yp.wgjwhj.cn

int main(int argc, char **argv)
来源：http://zl.nszjky.cn

[S19] C：快速排序
来源：http://pc.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vz.szsharing.cn

[S20] C：二分查找
来源：http://zr.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kr.asd995.cn

[S21] C：字符类别判断
来源：http://sl.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jn.shxzukj.cn

[S22] C：字符串转数字
来源：http://uj.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uq.yuexingan06.cn

[S23] C：随机数
来源：http://fl.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qe.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://pf.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lg.muxihuayi.cn

[S25] C：内存拷贝
来源：http://es.shtwfgs.cn

memcpy(dst, src, n);
来源：http://rh.muxihuayi.cn

[S26] C：内存清零
来源：http://ex.nicolike.cn

memset(a, 0, sizeof a);
来源：http://aq.hahajie.cn

[S27] C：定义常量
来源：http://po.panjiajie.cn

const double PI = 3.14159;
来源：http://it.szxytkj.cn

[S28] C：静态变量
来源：http://mu.colortex.cn

static int counter = 0;
来源：http://kw.shxzukj.cn

[S29] C：变参函数
来源：http://nh.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xd.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://fs.newstarts.cn

#ifndef X_H
来源：http://lk.wgjwhj.cn

#define X_H
来源：http://gk.szsharing.cn

#endif
来源：http://nm.shxzukj.cn

[S31] C++：Hello World
来源：http://bc.521024.cn

#include <iostream>
来源：http://va.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://lh.shxzskj.cn

[S32] C++：字符串
来源：http://fs.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://qp.panjiajie.cn

[S33] C++：vector 增删
来源：http://sd.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ar.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://wz.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://vl.haigaiapp.cn

[S35] C++：map
来源：http://zr.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vi.panjiajie.cn

[S36] C++：unordered_map
来源：http://bs.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eb.hnjuh.cn

[S37] C++：set
来源：http://ca.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fb.huanxung.cn

[S38] C++：排序
来源：http://ev.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://uc.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://fa.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://em.hnjuh.cn

[S40] C++：查找元素
来源：http://jj.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fh.gzmigu.cn

[S41] C++：类与构造函数
来源：http://lh.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tq.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://qh.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://nq.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://wk.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://fg.nicolike.cn

[S44] C++：引用传参
来源：http://kd.newstarts.cn

void inc(int &x) { ++x; }
来源：http://cp.muxihuayi.cn

[S45] C++：lambda
来源：http://ed.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://om.nszjky.cn

[S46] C++：函数模板
来源：http://sv.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yn.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://dr.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yv.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://pw.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ok.szsharing.cn


<!-- 参考信息 -->