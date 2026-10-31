代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://px.huanxung.cn

[Q75] 日期格式化
来源：http://gx.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fh.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ux.bookmarksfly.cn

[Q76] 按天统计
来源：http://ky.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wd.bjjhwx.cn

[Q77] 时间加减
来源：http://xc.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aa.gzmigu.cn

[Q78] 当前时间
来源：http://nz.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://to.haigaiapp.cn

[Q79] 字符串拼接
来源：http://le.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://du.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://yn.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ka.bookmarksfly.cn

[Q81] 字符串替换
来源：http://mm.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oy.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://vd.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://av.shtwfgs.cn

[Q83] 大小写转换
来源：http://vx.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://um.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://fo.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://fp.asd995.cn

[Q85] 数值取整
来源：http://zi.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://of.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://qa.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cx.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://ku.panjiajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ja.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://pp.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rp.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sz.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://qf.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lj.panjiajie.cn

[Q90] 生成序号列
来源：http://cx.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://of.bookmarksfly.cn

================================================================================
来源：http://ao.yuntaijiaju.cn

R. Bash 专题
来源：http://bk.nicolike.cn

================================================================================
来源：http://bd.asd995.cn

[R01] shebang 与严格模式
来源：http://lk.haigaiapp.cn

#!/usr/bin/env bash
来源：http://xb.colortex.cn

set -euo pipefail
来源：http://ca.shxzskj.cn

[R02] 变量赋值与使用
来源：http://kz.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://ym.shxzskj.cn

[R03] 只读变量
来源：http://jl.szxytkj.cn

readonly PI=3.14
来源：http://cn.colortex.cn

[R04] 位置参数
来源：http://ev.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://js.haigaiapp.cn

[R05] 参数默认值
来源：http://jc.chemitech.net.cn

name="${1:-default}"
来源：http://ba.panjiajie.cn

[R06] 判断命令是否存在
来源：http://st.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jb.muxihuayi.cn

[R07] if 判断文件
来源：http://sw.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tk.muxihuayi.cn

[R08] 数值比较
来源：http://md.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dg.huixinmuqiang.cn

[R09] 字符串比较
来源：http://ji.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vu.jianghongdianzi.cn

[R10] 正则匹配
来源：http://ra.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mf.jianghongdianzi.cn

[R11] case 多分支
来源：http://hy.asd995.cn

case "$1" in
来源：http://ts.bookmarksfly.cn

start) echo "启动" ;;
来源：http://zy.panjiajie.cn

stop)  echo "停止" ;;
来源：http://pj.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://gz.521024.cn

esac
来源：http://kx.muxihuayi.cn

[R12] for 遍历文件
来源：http://ts.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://sg.yuntaijiaju.cn

[R13] for 计数循环
来源：http://vu.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://xc.shtwfgs.cn

[R14] C 风格 for
来源：http://wa.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uc.huixiangedu.cn

[R15] while 逐行读文件
来源：http://yt.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cu.haigaiapp.cn

[R16] until 等待条件
来源：http://vq.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gd.9csxet.cn

[R17] 数组定义与取值
来源：http://cq.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dk.nszjky.cn

[R18] 遍历数组
来源：http://ir.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nc.muxihuayi.cn

[R19] 数组长度
来源：http://wl.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://lh.panjiajie.cn

[R20] 关联数组（字典）
来源：http://wr.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jx.asd995.cn

[R21] 字符串长度
来源：http://na.newstarts.cn

echo "${#s}"
来源：http://oq.chemitech.net.cn

[R22] 截取子串
来源：http://al.bookmarksfly.cn

echo "${s:0:5}"
来源：http://ro.chemitech.net.cn

[R23] 字符串替换
来源：http://gp.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vy.nicolike.cn

[R24] 大小写转换
来源：http://fk.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bj.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://jn.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rk.nicolike.cn

[R26] 命令替换
来源：http://tu.colortex.cn

now=$(date +%F); echo "$now"
来源：http://es.szxytkj.cn

[R27] 算术展开
来源：http://uc.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://ea.bookmarksfly.cn

[R28] 浮点运算
来源：http://we.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://nr.newstarts.cn

[R29] 定义函数
来源：http://yg.jctech888.com.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hd.nicolike.cn

[R30] 函数返回状态码
来源：http://of.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://lh.huanxung.cn

[R31] 局部变量
来源：http://xj.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://at.521024.cn

[R32] 参数个数校验
来源：http://sc.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uy.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://av.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pn.huixinmuqiang.cn

[R34] 退出时清理
来源：http://cm.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bj.jctech888.com.cn

[R35] 后台执行并等待
来源：http://hh.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zb.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://ui.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ad.huanxung.cn

[R37] 把输出赋给变量
来源：http://ne.huixinmuqiang.cn

files=$(ls -1)
来源：http://jf.521024.cn

[R38] 管道串联
来源：http://ax.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://fi.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://fv.9csxet.cn

cmd > out.log 2>&1
来源：http://jq.colortex.cn

[R40] 追加写日志
来源：http://lw.huixinmuqiang.cn

echo "log" >> out.log
来源：http://bm.haigaiapp.cn

[R41] 丢弃输出
来源：http://nr.nicolike.cn

cmd >/dev/null 2>&1
来源：http://fo.hahajie.cn

[R42] 输入重定向
来源：http://hn.huanxung.cn

wc -l < a.txt
来源：http://sz.hahajie.cn

[R43] 按名字查找文件
来源：http://lb.nszjky.cn

find . -name "*.log" -type f
来源：http://do.nicolike.cn

[R44] 按修改时间查找
来源：http://hc.lnxyls.cn

find . -mtime -7 -type f
来源：http://ce.huixinmuqiang.cn

[R45] 批量删除
来源：http://dv.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://sr.hahajie.cn

[R46] 递归替换文件内容
来源：http://br.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ev.521024.cn

[R47] sed 单行替换
来源：http://ew.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yc.huixiangedu.cn

[R48] awk 取指定列
来源：http://vv.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://if.521024.cn

[R49] awk 带条件
来源：http://nz.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gl.asd995.cn

[R50] awk 求和
来源：http://mu.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ka.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://qa.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ki.szsharing.cn

[R52] 统计行数
来源：http://vv.panjiajie.cn

wc -l a.txt
来源：http://wi.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://tz.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ix.newstarts.cn

[R54] 比较两个文件
来源：http://zi.jianghongdianzi.cn

diff a.txt b.txt
来源：http://io.shxzukj.cn

[R55] 压缩与解压
来源：http://yn.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vu.yuexingan06.cn

[R56] 远程拷贝
来源：http://lt.bjjhwx.cn

scp file user@host:/path/
来源：http://qv.haigaiapp.cn

[R57] 远程执行命令
来源：http://mm.gzmigu.cn

ssh user@host 'uptime'
来源：http://pz.huixiangedu.cn

[R58] 下载文件
来源：http://tj.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gb.yuexingan06.cn

[R59] 发 POST JSON
来源：http://zr.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hh.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://zu.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zt.521024.cn

[R61] 磁盘占用
来源：http://jn.bjjhwx.cn

df -h;  du -sh *
来源：http://uq.newstarts.cn

[R62] 找最占空间的文件
来源：http://mw.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://ys.yuexingan06.cn

[R63] 内存与进程
来源：http://vf.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://ml.asd995.cn

[R64] 结束进程
来源：http://xs.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://zm.hahajie.cn

[R65] 查看端口占用
来源：http://au.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pg.chemitech.net.cn

[R66] 定时任务
来源：http://mk.gzmigu.cn

crontab -e;  crontab -l
来源：http://cf.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://vd.shtwfgs.cn

openssl rand -hex 16
来源：http://tz.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://zv.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xa.haigaiapp.cn

[R69] 生成随机密码
来源：http://kp.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://xa.shxzukj.cn

[R70] 时间戳与互转
来源：http://qx.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://ai.lnxyls.cn

[R71] 日期格式化
来源：http://pc.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wj.huixiangedu.cn

[R72] 等待端口就绪
来源：http://lv.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lm.jctech888.com.cn

[R73] 分割大日志
来源：http://uf.hnjuh.cn

split -l 1000 big.log part_
来源：http://lr.lnxyls.cn

[R74] 批量重命名
来源：http://ht.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gj.jctech888.com.cn

[R75] 导出环境变量
来源：http://vk.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://kf.chemitech.net.cn

[R76] 使用临时文件
来源：http://ij.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mb.bjjhwx.cn

[R77] 读取用户输入
来源：http://am.newstarts.cn

read -rp "请输入: " ans
来源：http://lk.wgjwhj.cn

[R78] 交互式菜单
来源：http://fg.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ar.huanxung.cn

[R79] 解析命令行选项
来源：http://yb.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tw.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://kb.jctech888.com.cn

time ./run.sh
来源：http://qg.bookmarksfly.cn

================================================================================
来源：http://kq.9csxet.cn

S. C / C++ 专题
来源：http://js.jianghongdianzi.cn

================================================================================
来源：http://oc.yuexingan06.cn

[S01] C：Hello World
来源：http://gj.hahajie.cn

#include <stdio.h>
来源：http://yk.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ym.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://eg.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://yk.yuntaijiaju.cn

[S03] C：读入整数
来源：http://px.shxzukj.cn

int x; scanf("%d", &x);
来源：http://ds.jctech888.com.cn

[S04] C：字符串复制
来源：http://sx.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cq.bjjhwx.cn

[S05] C：字符串长度
来源：http://zb.muxihuayi.cn

strlen(s)
来源：http://ui.shxzukj.cn

[S06] C：字符串比较
来源：http://wl.bjjhwx.cn

strcmp(a, b) == 0
来源：http://pz.nszjky.cn

[S07] C：数组遍历求和
来源：http://jh.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cv.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://cy.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lk.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://qh.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xj.nicolike.cn

[S10] C：指针与解引用
来源：http://kq.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://rh.panjiajie.cn

[S11] C：逐行读文件
来源：http://uh.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://iz.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oi.newstarts.cn

fclose(f);
来源：http://yl.hnjuh.cn

[S12] C：写文件
来源：http://hs.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oh.muxihuayi.cn

[S13] C：宏定义
来源：http://zg.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ii.huanxung.cn

[S14] C：枚举
来源：http://mn.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://km.huanxung.cn

[S15] C：类型转换
来源：http://vb.yuexingan06.cn

(double) a / b
来源：http://he.9csxet.cn

[S16] C：位操作置位
来源：http://vf.nicolike.cn

x |= (1 << 3);
来源：http://ey.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://lx.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qj.lnxyls.cn

[S18] C：命令行参数
来源：http://bb.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://eo.newstarts.cn

[S19] C：快速排序
来源：http://ln.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ou.jctech888.com.cn

[S20] C：二分查找
来源：http://hn.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iq.haigaiapp.cn

[S21] C：字符类别判断
来源：http://iw.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fi.chemitech.net.cn

[S22] C：字符串转数字
来源：http://gi.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wa.hnjuh.cn

[S23] C：随机数
来源：http://wd.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fl.jctech888.com.cn

[S24] C：获取本地时间
来源：http://xa.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qh.521024.cn

[S25] C：内存拷贝
来源：http://vs.chemitech.net.cn

memcpy(dst, src, n);
来源：http://qc.szsharing.cn

[S26] C：内存清零
来源：http://mn.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://pu.shxzskj.cn

[S27] C：定义常量
来源：http://vm.huanxung.cn

const double PI = 3.14159;
来源：http://in.521024.cn

[S28] C：静态变量
来源：http://pz.nszjky.cn

static int counter = 0;
来源：http://so.bookmarksfly.cn

[S29] C：变参函数
来源：http://ba.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://er.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://ul.nszjky.cn

#ifndef X_H
来源：http://jw.yuntaijiaju.cn

#define X_H
来源：http://mr.szxytkj.cn

#endif
来源：http://zb.colortex.cn

[S31] C++：Hello World
来源：http://sy.gzmigu.cn

#include <iostream>
来源：http://dv.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://lx.haigaiapp.cn

[S32] C++：字符串
来源：http://dg.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://ey.nicolike.cn

[S33] C++：vector 增删
来源：http://sw.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://na.gzmigu.cn

[S34] C++：遍历 vector
来源：http://or.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://kc.colortex.cn

[S35] C++：map
来源：http://kr.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ll.colortex.cn

[S36] C++：unordered_map
来源：http://mq.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://la.szxytkj.cn

[S37] C++：set
来源：http://ay.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mx.yuexingan06.cn

[S38] C++：排序
来源：http://ft.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://yl.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://dw.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pd.bookmarksfly.cn

[S40] C++：查找元素
来源：http://ga.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ow.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://bd.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fs.nicolike.cn

[S42] C++：继承与虚函数
来源：http://vv.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://pa.haigaiapp.cn

[S43] C++：智能指针
来源：http://mc.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://rz.huanxung.cn

[S44] C++：引用传参
来源：http://xn.colortex.cn

void inc(int &x) { ++x; }
来源：http://jm.chemitech.net.cn


<!-- 参考信息 -->