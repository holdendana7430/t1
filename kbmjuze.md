代发 wailian999

ANALYZE TABLE users;
来源：http://vv.gzmigu.cn

[Q71] 查看建表语句
来源：http://va.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ux.lnxyls.cn

[Q72] 查看索引
来源：http://ue.panjiajie.cn

SHOW INDEX FROM users;
来源：http://wa.szsharing.cn

[Q73] 查看表状态
来源：http://ui.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ii.yuexingan06.cn

[Q74] 强制使用索引
来源：http://iu.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kl.asd995.cn

[Q75] 日期格式化
来源：http://lq.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nh.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hr.wgjwhj.cn

[Q76] 按天统计
来源：http://hb.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lm.chemitech.net.cn

[Q77] 时间加减
来源：http://dm.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cu.nszjky.cn

[Q78] 当前时间
来源：http://lv.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sr.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://cn.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jp.szxytkj.cn

[Q80] 字符串截取
来源：http://km.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ef.hahajie.cn

[Q81] 字符串替换
来源：http://gc.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://za.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://wo.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lh.huanxung.cn

[Q83] 大小写转换
来源：http://ov.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fh.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://na.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://kw.huixinmuqiang.cn

[Q85] 数值取整
来源：http://nb.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://td.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://ln.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sx.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://vu.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rh.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://yb.hnjuh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cl.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tk.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://zh.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yo.gzmigu.cn

[Q90] 生成序号列
来源：http://cs.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://on.newstarts.cn

================================================================================
来源：http://jm.muxihuayi.cn

R. Bash 专题
来源：http://fq.lnxyls.cn

================================================================================
来源：http://ep.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://mw.nszjky.cn

#!/usr/bin/env bash
来源：http://ui.huanxung.cn

set -euo pipefail
来源：http://oe.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://ex.shxzukj.cn

name="Tom"; echo "$name"
来源：http://uu.huixinmuqiang.cn

[R03] 只读变量
来源：http://si.panjiajie.cn

readonly PI=3.14
来源：http://nv.nicolike.cn

[R04] 位置参数
来源：http://zl.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://da.chemitech.net.cn

[R05] 参数默认值
来源：http://ps.shxzukj.cn

name="${1:-default}"
来源：http://yj.newstarts.cn

[R06] 判断命令是否存在
来源：http://ky.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bu.asd995.cn

[R07] if 判断文件
来源：http://pp.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bx.panjiajie.cn

[R08] 数值比较
来源：http://ld.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bu.huixiangedu.cn

[R09] 字符串比较
来源：http://iz.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dv.szsharing.cn

[R10] 正则匹配
来源：http://dw.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ek.szxytkj.cn

[R11] case 多分支
来源：http://yo.hnjuh.cn

case "$1" in
来源：http://pb.bjjhwx.cn

start) echo "启动" ;;
来源：http://ay.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://mb.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://oi.haigaiapp.cn

esac
来源：http://si.wgjwhj.cn

[R12] for 遍历文件
来源：http://bg.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://sy.newstarts.cn

[R13] for 计数循环
来源：http://dk.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://wo.muxihuayi.cn

[R14] C 风格 for
来源：http://hi.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ax.huanxung.cn

[R15] while 逐行读文件
来源：http://uy.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xv.9csxet.cn

[R16] until 等待条件
来源：http://ae.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wl.lnxyls.cn

[R17] 数组定义与取值
来源：http://ig.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://au.chemitech.net.cn

[R18] 遍历数组
来源：http://fh.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://al.bookmarksfly.cn

[R19] 数组长度
来源：http://ug.hahajie.cn

echo "${#arr[@]}"
来源：http://ju.hahajie.cn

[R20] 关联数组（字典）
来源：http://cn.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://om.shtwfgs.cn

[R21] 字符串长度
来源：http://ii.shtwfgs.cn

echo "${#s}"
来源：http://ib.colortex.cn

[R22] 截取子串
来源：http://az.haigaiapp.cn

echo "${s:0:5}"
来源：http://xq.haigaiapp.cn

[R23] 字符串替换
来源：http://mt.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ef.huixinmuqiang.cn

[R24] 大小写转换
来源：http://lm.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mo.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://ps.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sn.wgjwhj.cn

[R26] 命令替换
来源：http://me.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://vm.yuexingan06.cn

[R27] 算术展开
来源：http://ba.521024.cn

echo $((1 + 2 * 3))
来源：http://yn.lnxyls.cn

[R28] 浮点运算
来源：http://dh.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://mi.huanxung.cn

[R29] 定义函数
来源：http://mt.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bj.nicolike.cn

[R30] 函数返回状态码
来源：http://qe.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://xu.bjjhwx.cn

[R31] 局部变量
来源：http://zc.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://ro.szxytkj.cn

[R32] 参数个数校验
来源：http://vy.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ix.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://iy.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zi.shxzskj.cn

[R34] 退出时清理
来源：http://bb.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qw.szxytkj.cn

[R35] 后台执行并等待
来源：http://sb.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://il.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://er.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kb.9csxet.cn

[R37] 把输出赋给变量
来源：http://tm.yuexingan06.cn

files=$(ls -1)
来源：http://jt.yuexingan06.cn

[R38] 管道串联
来源：http://om.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://qt.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://dm.newstarts.cn

cmd > out.log 2>&1
来源：http://va.panjiajie.cn

[R40] 追加写日志
来源：http://so.panjiajie.cn

echo "log" >> out.log
来源：http://xf.hahajie.cn

[R41] 丢弃输出
来源：http://yn.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://zc.yuntaijiaju.cn

[R42] 输入重定向
来源：http://yq.bjjhwx.cn

wc -l < a.txt
来源：http://fp.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://mm.asd995.cn

find . -name "*.log" -type f
来源：http://wt.asd995.cn

[R44] 按修改时间查找
来源：http://jb.lnxyls.cn

find . -mtime -7 -type f
来源：http://go.bookmarksfly.cn

[R45] 批量删除
来源：http://vy.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://lk.lnxyls.cn

[R46] 递归替换文件内容
来源：http://dm.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fy.jctech888.com.cn

[R47] sed 单行替换
来源：http://fn.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tw.asd995.cn

[R48] awk 取指定列
来源：http://pi.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://fk.yuexingan06.cn

[R49] awk 带条件
来源：http://ha.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wa.shxzukj.cn

[R50] awk 求和
来源：http://wn.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zk.yuexingan06.cn

[R51] 排序去重取前几
来源：http://ki.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sn.yuntaijiaju.cn

[R52] 统计行数
来源：http://ho.wgjwhj.cn

wc -l a.txt
来源：http://ls.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://rl.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xv.hahajie.cn

[R54] 比较两个文件
来源：http://vo.asd995.cn

diff a.txt b.txt
来源：http://sn.521024.cn

[R55] 压缩与解压
来源：http://hq.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ng.szxytkj.cn

[R56] 远程拷贝
来源：http://zy.lnxyls.cn

scp file user@host:/path/
来源：http://rn.gzmigu.cn

[R57] 远程执行命令
来源：http://ao.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://mh.huixiangedu.cn

[R58] 下载文件
来源：http://su.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pk.colortex.cn

[R59] 发 POST JSON
来源：http://es.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dc.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://kw.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dp.shtwfgs.cn

[R61] 磁盘占用
来源：http://tb.gzmigu.cn

df -h;  du -sh *
来源：http://nx.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://iy.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://md.chemitech.net.cn

[R63] 内存与进程
来源：http://wa.521024.cn

free -h;  ps aux | grep nginx
来源：http://gs.bjjhwx.cn

[R64] 结束进程
来源：http://zx.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://zz.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://do.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bi.gzmigu.cn

[R66] 定时任务
来源：http://nd.bjjhwx.cn

crontab -e;  crontab -l
来源：http://na.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://mz.jianghongdianzi.cn

openssl rand -hex 16
来源：http://bw.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://vg.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vq.szxytkj.cn

[R69] 生成随机密码
来源：http://zj.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://es.nicolike.cn

[R70] 时间戳与互转
来源：http://sy.nszjky.cn

date +%s;  date -d @1700000000
来源：http://bg.muxihuayi.cn

[R71] 日期格式化
来源：http://dp.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mg.huixiangedu.cn

[R72] 等待端口就绪
来源：http://ys.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lm.lnxyls.cn

[R73] 分割大日志
来源：http://ya.muxihuayi.cn

split -l 1000 big.log part_
来源：http://pf.bjjhwx.cn

[R74] 批量重命名
来源：http://hi.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ra.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://xd.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://tz.newstarts.cn

[R76] 使用临时文件
来源：http://pu.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://va.asd995.cn

[R77] 读取用户输入
来源：http://zz.hnjuh.cn

read -rp "请输入: " ans
来源：http://ds.asd995.cn

[R78] 交互式菜单
来源：http://um.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zz.newstarts.cn

[R79] 解析命令行选项
来源：http://xq.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dc.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://ge.jctech888.com.cn

time ./run.sh
来源：http://ss.huanxung.cn

================================================================================
来源：http://rb.panjiajie.cn

S. C / C++ 专题
来源：http://de.huanxung.cn

================================================================================
来源：http://ex.521024.cn

[S01] C：Hello World
来源：http://xj.yuexingan06.cn

#include <stdio.h>
来源：http://ap.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ib.colortex.cn

[S02] C：变量与格式化输出
来源：http://dp.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://ea.521024.cn

[S03] C：读入整数
来源：http://xg.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://il.colortex.cn

[S04] C：字符串复制
来源：http://fq.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wx.9csxet.cn

[S05] C：字符串长度
来源：http://uc.asd995.cn

strlen(s)
来源：http://fs.jctech888.com.cn

[S06] C：字符串比较
来源：http://cm.jctech888.com.cn

strcmp(a, b) == 0
来源：http://zw.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://dg.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jk.asd995.cn

[S08] C：动态内存分配与释放
来源：http://mj.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://if.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://ue.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://te.wgjwhj.cn

[S10] C：指针与解引用
来源：http://zv.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://fx.jctech888.com.cn

[S11] C：逐行读文件
来源：http://ue.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://yi.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nm.shtwfgs.cn

fclose(f);
来源：http://dt.9csxet.cn

[S12] C：写文件
来源：http://tg.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vt.colortex.cn

[S13] C：宏定义
来源：http://ux.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://km.shxzukj.cn

[S14] C：枚举
来源：http://yt.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://vo.panjiajie.cn

[S15] C：类型转换
来源：http://bt.jctech888.com.cn

(double) a / b
来源：http://zb.huanxung.cn

[S16] C：位操作置位
来源：http://hh.yuexingan06.cn

x |= (1 << 3);
来源：http://yk.521024.cn

[S17] C：安全拼接字符串
来源：http://id.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qx.nszjky.cn

[S18] C：命令行参数
来源：http://ac.newstarts.cn

int main(int argc, char **argv)
来源：http://df.wgjwhj.cn

[S19] C：快速排序
来源：http://wi.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bv.panjiajie.cn

[S20] C：二分查找
来源：http://yh.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xj.hahajie.cn

[S21] C：字符类别判断
来源：http://dq.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kk.huanxung.cn

[S22] C：字符串转数字
来源：http://fw.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://od.hnjuh.cn

[S23] C：随机数
来源：http://uc.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pf.huanxung.cn

[S24] C：获取本地时间
来源：http://ua.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nn.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://yq.nszjky.cn

memcpy(dst, src, n);
来源：http://do.asd995.cn

[S26] C：内存清零
来源：http://xh.hahajie.cn

memset(a, 0, sizeof a);
来源：http://il.yuexingan06.cn

[S27] C：定义常量
来源：http://jv.hahajie.cn

const double PI = 3.14159;
来源：http://ad.wgjwhj.cn

[S28] C：静态变量
来源：http://nc.yuexingan06.cn

static int counter = 0;
来源：http://ef.wgjwhj.cn

[S29] C：变参函数
来源：http://uz.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fj.chemitech.net.cn

[S30] C：头文件保护
来源：http://wu.wgjwhj.cn

#ifndef X_H
来源：http://qp.yuexingan06.cn

#define X_H
来源：http://nq.yuntaijiaju.cn

#endif
来源：http://qd.asd995.cn

[S31] C++：Hello World
来源：http://hp.shxzukj.cn

#include <iostream>
来源：http://yv.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://pq.lnxyls.cn

[S32] C++：字符串
来源：http://nl.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://qf.muxihuayi.cn

[S33] C++：vector 增删
来源：http://sh.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cm.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://sc.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://af.huanxung.cn

[S35] C++：map
来源：http://bd.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xu.shtwfgs.cn

[S36] C++：unordered_map
来源：http://eo.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qn.bookmarksfly.cn

[S37] C++：set
来源：http://ab.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zi.huixinmuqiang.cn

[S38] C++：排序
来源：http://es.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://ib.521024.cn

[S39] C++：自定义比较器排序
来源：http://cx.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xi.bookmarksfly.cn

[S40] C++：查找元素
来源：http://pp.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rl.shxzukj.cn


<!-- 参考信息 -->