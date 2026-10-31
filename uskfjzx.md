代发 wailian999

[Q67] 设置隔离级别
来源：http://gh.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rx.bjjhwx.cn

[Q68] 保存点
来源：http://ic.szsharing.cn

SAVEPOINT sp1;
来源：http://fi.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://pr.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://bg.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vw.huixiangedu.cn

[Q70] 更新统计信息
来源：http://gj.haigaiapp.cn

ANALYZE TABLE users;
来源：http://xl.shxzukj.cn

[Q71] 查看建表语句
来源：http://ew.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eb.521024.cn

[Q72] 查看索引
来源：http://pm.panjiajie.cn

SHOW INDEX FROM users;
来源：http://ej.chemitech.net.cn

[Q73] 查看表状态
来源：http://vo.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hb.gzmigu.cn

[Q74] 强制使用索引
来源：http://mw.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://le.lnxyls.cn

[Q75] 日期格式化
来源：http://lk.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ps.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://il.huixinmuqiang.cn

[Q76] 按天统计
来源：http://rg.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kp.hnjuh.cn

[Q77] 时间加减
来源：http://dt.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vt.bjjhwx.cn

[Q78] 当前时间
来源：http://zi.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cw.shxzskj.cn

[Q79] 字符串拼接
来源：http://qx.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gx.shtwfgs.cn

[Q80] 字符串截取
来源：http://rd.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ab.lnxyls.cn

[Q81] 字符串替换
来源：http://ho.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nx.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://zk.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://su.haigaiapp.cn

[Q83] 大小写转换
来源：http://vd.szsharing.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://au.521024.cn

[Q84] 去除首尾空格
来源：http://la.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://ot.lnxyls.cn

[Q85] 数值取整
来源：http://za.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wp.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://kn.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wn.nicolike.cn

[Q87] JSON 字段做条件
来源：http://pk.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ez.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://fp.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pe.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pt.szsharing.cn

[Q89] 判断表是否存在
来源：http://fo.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ap.shtwfgs.cn

[Q90] 生成序号列
来源：http://dy.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cf.shxzskj.cn

================================================================================
来源：http://on.shtwfgs.cn

R. Bash 专题
来源：http://ii.nszjky.cn

================================================================================
来源：http://qg.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://uc.jctech888.com.cn

#!/usr/bin/env bash
来源：http://ix.bookmarksfly.cn

set -euo pipefail
来源：http://df.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://ju.gzmigu.cn

name="Tom"; echo "$name"
来源：http://nm.colortex.cn

[R03] 只读变量
来源：http://ye.muxihuayi.cn

readonly PI=3.14
来源：http://bu.jctech888.com.cn

[R04] 位置参数
来源：http://xi.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ch.colortex.cn

[R05] 参数默认值
来源：http://oo.huixiangedu.cn

name="${1:-default}"
来源：http://aw.shxzskj.cn

[R06] 判断命令是否存在
来源：http://ns.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kk.haigaiapp.cn

[R07] if 判断文件
来源：http://co.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://up.wgjwhj.cn

[R08] 数值比较
来源：http://fz.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qg.huixinmuqiang.cn

[R09] 字符串比较
来源：http://yn.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jf.521024.cn

[R10] 正则匹配
来源：http://dz.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pj.haigaiapp.cn

[R11] case 多分支
来源：http://cz.newstarts.cn

case "$1" in
来源：http://ln.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://vk.asd995.cn

stop)  echo "停止" ;;
来源：http://cs.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://dh.huixinmuqiang.cn

esac
来源：http://xb.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://ev.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://hh.shxzukj.cn

[R13] for 计数循环
来源：http://ye.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://yx.wgjwhj.cn

[R14] C 风格 for
来源：http://qq.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://is.hnjuh.cn

[R15] while 逐行读文件
来源：http://km.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wv.nicolike.cn

[R16] until 等待条件
来源：http://uh.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ie.gzmigu.cn

[R17] 数组定义与取值
来源：http://nl.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rj.yuntaijiaju.cn

[R18] 遍历数组
来源：http://ns.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mh.yuntaijiaju.cn

[R19] 数组长度
来源：http://fx.szxytkj.cn

echo "${#arr[@]}"
来源：http://du.huanxung.cn

[R20] 关联数组（字典）
来源：http://og.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gh.hahajie.cn

[R21] 字符串长度
来源：http://an.jctech888.com.cn

echo "${#s}"
来源：http://tt.shxzukj.cn

[R22] 截取子串
来源：http://wu.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://vz.szxytkj.cn

[R23] 字符串替换
来源：http://ab.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://or.lnxyls.cn

[R24] 大小写转换
来源：http://ec.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fz.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://en.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fi.521024.cn

[R26] 命令替换
来源：http://iw.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://sy.9csxet.cn

[R27] 算术展开
来源：http://hg.521024.cn

echo $((1 + 2 * 3))
来源：http://xr.lnxyls.cn

[R28] 浮点运算
来源：http://yv.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://md.haigaiapp.cn

[R29] 定义函数
来源：http://vi.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hp.521024.cn

[R30] 函数返回状态码
来源：http://lf.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://bz.bjjhwx.cn

[R31] 局部变量
来源：http://ol.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://cb.hnjuh.cn

[R32] 参数个数校验
来源：http://pt.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sl.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://ky.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ji.wgjwhj.cn

[R34] 退出时清理
来源：http://sy.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fi.asd995.cn

[R35] 后台执行并等待
来源：http://kd.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sj.szsharing.cn

[R36] 并发执行多个任务
来源：http://rq.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vt.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://eg.hnjuh.cn

files=$(ls -1)
来源：http://cy.huixinmuqiang.cn

[R38] 管道串联
来源：http://fs.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://nv.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://ff.newstarts.cn

cmd > out.log 2>&1
来源：http://ej.asd995.cn

[R40] 追加写日志
来源：http://rn.yuntaijiaju.cn

echo "log" >> out.log
来源：http://le.szsharing.cn

[R41] 丢弃输出
来源：http://tv.colortex.cn

cmd >/dev/null 2>&1
来源：http://mw.gzmigu.cn

[R42] 输入重定向
来源：http://ho.shtwfgs.cn

wc -l < a.txt
来源：http://ax.szsharing.cn

[R43] 按名字查找文件
来源：http://gi.chemitech.net.cn

find . -name "*.log" -type f
来源：http://ez.nszjky.cn

[R44] 按修改时间查找
来源：http://cy.hahajie.cn

find . -mtime -7 -type f
来源：http://qu.szsharing.cn

[R45] 批量删除
来源：http://gr.colortex.cn

find . -name "*.tmp" -delete
来源：http://lr.gzmigu.cn

[R46] 递归替换文件内容
来源：http://sv.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eg.wgjwhj.cn

[R47] sed 单行替换
来源：http://gj.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pr.colortex.cn

[R48] awk 取指定列
来源：http://mp.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://ef.haigaiapp.cn

[R49] awk 带条件
来源：http://op.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://de.colortex.cn

[R50] awk 求和
来源：http://cv.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tq.yuexingan06.cn

[R51] 排序去重取前几
来源：http://dv.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gs.jctech888.com.cn

[R52] 统计行数
来源：http://xs.bjjhwx.cn

wc -l a.txt
来源：http://ug.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://ns.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ng.bjjhwx.cn

[R54] 比较两个文件
来源：http://yc.haigaiapp.cn

diff a.txt b.txt
来源：http://pj.wgjwhj.cn

[R55] 压缩与解压
来源：http://ar.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gw.bjjhwx.cn

[R56] 远程拷贝
来源：http://yr.wgjwhj.cn

scp file user@host:/path/
来源：http://fa.shtwfgs.cn

[R57] 远程执行命令
来源：http://yj.haigaiapp.cn

ssh user@host 'uptime'
来源：http://mh.panjiajie.cn

[R58] 下载文件
来源：http://oa.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qo.huanxung.cn

[R59] 发 POST JSON
来源：http://xm.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vb.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://wm.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bk.muxihuayi.cn

[R61] 磁盘占用
来源：http://uf.hnjuh.cn

df -h;  du -sh *
来源：http://id.hahajie.cn

[R62] 找最占空间的文件
来源：http://ua.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://xx.szsharing.cn

[R63] 内存与进程
来源：http://ga.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://pi.szxytkj.cn

[R64] 结束进程
来源：http://bw.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://dm.hnjuh.cn

[R65] 查看端口占用
来源：http://fp.shtwfgs.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://th.wgjwhj.cn

[R66] 定时任务
来源：http://rf.huanxung.cn

crontab -e;  crontab -l
来源：http://cu.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://kw.panjiajie.cn

openssl rand -hex 16
来源：http://jk.shxzskj.cn

[R68] 计算文件校验值
来源：http://zt.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mn.panjiajie.cn

[R69] 生成随机密码
来源：http://gp.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://km.shtwfgs.cn

[R70] 时间戳与互转
来源：http://be.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://yg.newstarts.cn

[R71] 日期格式化
来源：http://zn.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ft.chemitech.net.cn

[R72] 等待端口就绪
来源：http://dz.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rr.bookmarksfly.cn

[R73] 分割大日志
来源：http://xj.gzmigu.cn

split -l 1000 big.log part_
来源：http://vz.panjiajie.cn

[R74] 批量重命名
来源：http://iv.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nc.szxytkj.cn

[R75] 导出环境变量
来源：http://sp.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://bj.jctech888.com.cn

[R76] 使用临时文件
来源：http://pe.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jg.lnxyls.cn

[R77] 读取用户输入
来源：http://xc.9csxet.cn

read -rp "请输入: " ans
来源：http://vj.huanxung.cn

[R78] 交互式菜单
来源：http://ks.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xv.hnjuh.cn

[R79] 解析命令行选项
来源：http://ql.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nk.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://sy.yuntaijiaju.cn

time ./run.sh
来源：http://bc.521024.cn

================================================================================
来源：http://sy.wgjwhj.cn

S. C / C++ 专题
来源：http://bu.chemitech.net.cn

================================================================================
来源：http://ou.521024.cn

[S01] C：Hello World
来源：http://qx.hahajie.cn

#include <stdio.h>
来源：http://zm.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pb.huanxung.cn

[S02] C：变量与格式化输出
来源：http://mg.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://hu.9csxet.cn

[S03] C：读入整数
来源：http://uy.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://xq.bjjhwx.cn

[S04] C：字符串复制
来源：http://hv.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hg.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://rh.newstarts.cn

strlen(s)
来源：http://ho.521024.cn

[S06] C：字符串比较
来源：http://la.muxihuayi.cn

strcmp(a, b) == 0
来源：http://bn.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://ua.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fk.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://bn.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ph.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://ua.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kk.9csxet.cn

[S10] C：指针与解引用
来源：http://xy.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://ur.szxytkj.cn

[S11] C：逐行读文件
来源：http://ys.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://je.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eo.hnjuh.cn

fclose(f);
来源：http://ch.huixiangedu.cn

[S12] C：写文件
来源：http://kr.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aw.bjjhwx.cn

[S13] C：宏定义
来源：http://bw.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ip.521024.cn

[S14] C：枚举
来源：http://wm.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://qx.panjiajie.cn

[S15] C：类型转换
来源：http://ih.shtwfgs.cn

(double) a / b
来源：http://nh.newstarts.cn

[S16] C：位操作置位
来源：http://je.nicolike.cn

x |= (1 << 3);
来源：http://nn.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://hm.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ua.nicolike.cn

[S18] C：命令行参数
来源：http://zb.muxihuayi.cn

int main(int argc, char **argv)
来源：http://pm.shxzskj.cn

[S19] C：快速排序
来源：http://iv.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ar.wgjwhj.cn

[S20] C：二分查找
来源：http://jp.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://la.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://bu.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ha.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://im.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nz.huanxung.cn

[S23] C：随机数
来源：http://et.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://is.haigaiapp.cn

[S24] C：获取本地时间
来源：http://eq.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ik.shxzskj.cn

[S25] C：内存拷贝
来源：http://fw.haigaiapp.cn

memcpy(dst, src, n);
来源：http://ce.shtwfgs.cn

[S26] C：内存清零
来源：http://qn.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://nr.huixiangedu.cn

[S27] C：定义常量
来源：http://jm.panjiajie.cn

const double PI = 3.14159;
来源：http://zt.bookmarksfly.cn

[S28] C：静态变量
来源：http://my.bjjhwx.cn

static int counter = 0;
来源：http://of.chemitech.net.cn

[S29] C：变参函数
来源：http://pd.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qo.9csxet.cn

[S30] C：头文件保护
来源：http://hr.jianghongdianzi.cn

#ifndef X_H
来源：http://gh.huixinmuqiang.cn

#define X_H
来源：http://gy.9csxet.cn

#endif
来源：http://sn.newstarts.cn

[S31] C++：Hello World
来源：http://uo.huixiangedu.cn

#include <iostream>
来源：http://vj.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://qv.muxihuayi.cn

[S32] C++：字符串
来源：http://js.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://dx.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://pb.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yy.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://ci.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://ze.huixinmuqiang.cn

[S35] C++：map
来源：http://vo.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sr.9csxet.cn

[S36] C++：unordered_map
来源：http://lo.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rt.521024.cn


<!-- 参考信息 -->