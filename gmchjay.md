代发 wailian999

[Q65] 回滚事务
来源：http://dy.lnxyls.cn

ROLLBACK;
来源：http://bg.haigaiapp.cn

[Q66] 行锁查询
来源：http://av.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vl.newstarts.cn

[Q67] 设置隔离级别
来源：http://xl.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qx.lnxyls.cn

[Q68] 保存点
来源：http://gk.yuexingan06.cn

SAVEPOINT sp1;
来源：http://fy.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://fc.huanxung.cn

[Q69] 查看执行计划
来源：http://nm.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gt.chemitech.net.cn

[Q70] 更新统计信息
来源：http://jo.yuexingan06.cn

ANALYZE TABLE users;
来源：http://ae.haigaiapp.cn

[Q71] 查看建表语句
来源：http://pi.huanxung.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dv.jianghongdianzi.cn

[Q72] 查看索引
来源：http://qv.shxzukj.cn

SHOW INDEX FROM users;
来源：http://vc.colortex.cn

[Q73] 查看表状态
来源：http://zx.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://la.wgjwhj.cn

[Q74] 强制使用索引
来源：http://tw.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ig.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://jc.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ui.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ii.panjiajie.cn

[Q76] 按天统计
来源：http://zw.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kv.newstarts.cn

[Q77] 时间加减
来源：http://be.huanxung.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ci.huanxung.cn

[Q78] 当前时间
来源：http://ia.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zu.yuexingan06.cn

[Q79] 字符串拼接
来源：http://ql.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vf.nszjky.cn

[Q80] 字符串截取
来源：http://pu.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qf.szxytkj.cn

[Q81] 字符串替换
来源：http://fb.bookmarksfly.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xn.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://oo.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pc.huanxung.cn

[Q83] 大小写转换
来源：http://fv.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cp.asd995.cn

[Q84] 去除首尾空格
来源：http://bb.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://pk.9csxet.cn

[Q85] 数值取整
来源：http://wf.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lh.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://zo.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xx.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://is.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ps.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://hr.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ip.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tl.nszjky.cn

[Q89] 判断表是否存在
来源：http://de.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ym.nszjky.cn

[Q90] 生成序号列
来源：http://hl.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sa.bjjhwx.cn

================================================================================
来源：http://dl.muxihuayi.cn

R. Bash 专题
来源：http://ob.9csxet.cn

================================================================================
来源：http://mj.szxytkj.cn

[R01] shebang 与严格模式
来源：http://xw.yuexingan06.cn

#!/usr/bin/env bash
来源：http://pz.jianghongdianzi.cn

set -euo pipefail
来源：http://wc.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://tg.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://nf.lnxyls.cn

[R03] 只读变量
来源：http://ss.hnjuh.cn

readonly PI=3.14
来源：http://hy.9csxet.cn

[R04] 位置参数
来源：http://un.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vp.jctech888.com.cn

[R05] 参数默认值
来源：http://iy.newstarts.cn

name="${1:-default}"
来源：http://vj.szxytkj.cn

[R06] 判断命令是否存在
来源：http://ts.bjjhwx.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bt.huanxung.cn

[R07] if 判断文件
来源：http://po.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://td.nicolike.cn

[R08] 数值比较
来源：http://kx.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tb.shxzukj.cn

[R09] 字符串比较
来源：http://bi.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ih.jctech888.com.cn

[R10] 正则匹配
来源：http://oz.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bu.yuntaijiaju.cn

[R11] case 多分支
来源：http://pv.lnxyls.cn

case "$1" in
来源：http://nc.nicolike.cn

start) echo "启动" ;;
来源：http://ls.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://xh.huanxung.cn

*)     echo "未知命令" ;;
来源：http://wv.bookmarksfly.cn

esac
来源：http://sg.newstarts.cn

[R12] for 遍历文件
来源：http://ud.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://yl.hahajie.cn

[R13] for 计数循环
来源：http://ew.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://vw.lnxyls.cn

[R14] C 风格 for
来源：http://mx.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ao.colortex.cn

[R15] while 逐行读文件
来源：http://gf.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ur.yuntaijiaju.cn

[R16] until 等待条件
来源：http://ja.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bb.shxzskj.cn

[R17] 数组定义与取值
来源：http://ig.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nv.shxzskj.cn

[R18] 遍历数组
来源：http://lo.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cf.colortex.cn

[R19] 数组长度
来源：http://qj.shxzskj.cn

echo "${#arr[@]}"
来源：http://tk.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://wh.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ci.nicolike.cn

[R21] 字符串长度
来源：http://im.haigaiapp.cn

echo "${#s}"
来源：http://qq.shtwfgs.cn

[R22] 截取子串
来源：http://kw.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://ex.huixiangedu.cn

[R23] 字符串替换
来源：http://xi.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mx.haigaiapp.cn

[R24] 大小写转换
来源：http://kq.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://il.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://sd.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ju.yuntaijiaju.cn

[R26] 命令替换
来源：http://gm.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://hs.bookmarksfly.cn

[R27] 算术展开
来源：http://ow.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://ol.521024.cn

[R28] 浮点运算
来源：http://gk.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://og.shtwfgs.cn

[R29] 定义函数
来源：http://rq.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yt.nicolike.cn

[R30] 函数返回状态码
来源：http://zb.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://tr.jianghongdianzi.cn

[R31] 局部变量
来源：http://aa.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://nr.haigaiapp.cn

[R32] 参数个数校验
来源：http://km.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nr.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://ld.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cy.bookmarksfly.cn

[R34] 退出时清理
来源：http://ft.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rp.shxzskj.cn

[R35] 后台执行并等待
来源：http://pl.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gy.nicolike.cn

[R36] 并发执行多个任务
来源：http://jm.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tb.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://tv.bookmarksfly.cn

files=$(ls -1)
来源：http://ae.shtwfgs.cn

[R38] 管道串联
来源：http://jr.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://rx.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://dm.newstarts.cn

cmd > out.log 2>&1
来源：http://sg.huixinmuqiang.cn

[R40] 追加写日志
来源：http://lm.huixiangedu.cn

echo "log" >> out.log
来源：http://nb.hnjuh.cn

[R41] 丢弃输出
来源：http://cr.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://xy.jianghongdianzi.cn

[R42] 输入重定向
来源：http://zv.lnxyls.cn

wc -l < a.txt
来源：http://od.huanxung.cn

[R43] 按名字查找文件
来源：http://rl.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://ya.shtwfgs.cn

[R44] 按修改时间查找
来源：http://aq.9csxet.cn

find . -mtime -7 -type f
来源：http://mb.nicolike.cn

[R45] 批量删除
来源：http://bd.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://bv.gzmigu.cn

[R46] 递归替换文件内容
来源：http://ya.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kq.muxihuayi.cn

[R47] sed 单行替换
来源：http://nn.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dg.gzmigu.cn

[R48] awk 取指定列
来源：http://ql.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://yx.yuntaijiaju.cn

[R49] awk 带条件
来源：http://hr.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nt.wgjwhj.cn

[R50] awk 求和
来源：http://xr.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bh.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://ce.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jc.szxytkj.cn

[R52] 统计行数
来源：http://bs.colortex.cn

wc -l a.txt
来源：http://qr.asd995.cn

[R53] 查看文件头与实时尾
来源：http://ai.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ct.521024.cn

[R54] 比较两个文件
来源：http://vy.521024.cn

diff a.txt b.txt
来源：http://qs.chemitech.net.cn

[R55] 压缩与解压
来源：http://qa.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vx.wgjwhj.cn

[R56] 远程拷贝
来源：http://cn.newstarts.cn

scp file user@host:/path/
来源：http://pz.muxihuayi.cn

[R57] 远程执行命令
来源：http://yu.shxzskj.cn

ssh user@host 'uptime'
来源：http://eg.newstarts.cn

[R58] 下载文件
来源：http://fz.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lj.chemitech.net.cn

[R59] 发 POST JSON
来源：http://xz.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qg.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://kn.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uc.shxzukj.cn

[R61] 磁盘占用
来源：http://qq.hahajie.cn

df -h;  du -sh *
来源：http://wy.521024.cn

[R62] 找最占空间的文件
来源：http://to.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://gq.hnjuh.cn

[R63] 内存与进程
来源：http://xg.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://ly.huanxung.cn

[R64] 结束进程
来源：http://ep.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://ty.chemitech.net.cn

[R65] 查看端口占用
来源：http://yq.nicolike.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wa.nicolike.cn

[R66] 定时任务
来源：http://ug.nicolike.cn

crontab -e;  crontab -l
来源：http://zf.nszjky.cn

[R67] 生成随机十六进制串
来源：http://lf.shxzukj.cn

openssl rand -hex 16
来源：http://tw.yuexingan06.cn

[R68] 计算文件校验值
来源：http://xz.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wh.yuexingan06.cn

[R69] 生成随机密码
来源：http://mu.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://dx.panjiajie.cn

[R70] 时间戳与互转
来源：http://vp.newstarts.cn

date +%s;  date -d @1700000000
来源：http://aa.newstarts.cn

[R71] 日期格式化
来源：http://iw.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cc.9csxet.cn

[R72] 等待端口就绪
来源：http://fp.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hb.shxzukj.cn

[R73] 分割大日志
来源：http://ps.huanxung.cn

split -l 1000 big.log part_
来源：http://lf.chemitech.net.cn

[R74] 批量重命名
来源：http://sz.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ss.muxihuayi.cn

[R75] 导出环境变量
来源：http://tg.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://vm.chemitech.net.cn

[R76] 使用临时文件
来源：http://iz.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hb.shtwfgs.cn

[R77] 读取用户输入
来源：http://ye.haigaiapp.cn

read -rp "请输入: " ans
来源：http://pk.gzmigu.cn

[R78] 交互式菜单
来源：http://ri.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jb.shtwfgs.cn

[R79] 解析命令行选项
来源：http://ti.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zb.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://xx.jianghongdianzi.cn

time ./run.sh
来源：http://wh.huixinmuqiang.cn

================================================================================
来源：http://ql.jctech888.com.cn

S. C / C++ 专题
来源：http://rr.521024.cn

================================================================================
来源：http://jm.hnjuh.cn

[S01] C：Hello World
来源：http://sz.nicolike.cn

#include <stdio.h>
来源：http://mj.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uo.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://ob.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://xl.9csxet.cn

[S03] C：读入整数
来源：http://ul.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://ii.huixiangedu.cn

[S04] C：字符串复制
来源：http://eg.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://da.hnjuh.cn

[S05] C：字符串长度
来源：http://dr.huanxung.cn

strlen(s)
来源：http://tu.bjjhwx.cn

[S06] C：字符串比较
来源：http://sq.huixiangedu.cn

strcmp(a, b) == 0
来源：http://ie.colortex.cn

[S07] C：数组遍历求和
来源：http://ti.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mk.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://ar.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uc.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://xl.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ql.gzmigu.cn

[S10] C：指针与解引用
来源：http://wn.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://qh.wgjwhj.cn

[S11] C：逐行读文件
来源：http://mh.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://ov.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://np.newstarts.cn

fclose(f);
来源：http://ce.colortex.cn

[S12] C：写文件
来源：http://hv.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://un.huixinmuqiang.cn

[S13] C：宏定义
来源：http://vg.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vo.lnxyls.cn

[S14] C：枚举
来源：http://yz.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://wy.521024.cn

[S15] C：类型转换
来源：http://gn.haigaiapp.cn

(double) a / b
来源：http://xn.shxzukj.cn

[S16] C：位操作置位
来源：http://px.szsharing.cn

x |= (1 << 3);
来源：http://ys.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://bg.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gx.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://rs.chemitech.net.cn

int main(int argc, char **argv)
来源：http://zg.asd995.cn

[S19] C：快速排序
来源：http://fx.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lx.hnjuh.cn

[S20] C：二分查找
来源：http://yp.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eu.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://fp.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ri.huanxung.cn

[S22] C：字符串转数字
来源：http://qc.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nn.chemitech.net.cn

[S23] C：随机数
来源：http://xy.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ox.colortex.cn

[S24] C：获取本地时间
来源：http://dl.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qv.gzmigu.cn

[S25] C：内存拷贝
来源：http://ff.asd995.cn

memcpy(dst, src, n);
来源：http://si.bjjhwx.cn

[S26] C：内存清零
来源：http://af.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://yw.chemitech.net.cn

[S27] C：定义常量
来源：http://vz.hnjuh.cn

const double PI = 3.14159;
来源：http://da.bookmarksfly.cn

[S28] C：静态变量
来源：http://rm.9csxet.cn

static int counter = 0;
来源：http://xb.shtwfgs.cn

[S29] C：变参函数
来源：http://lr.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xo.bjjhwx.cn

[S30] C：头文件保护
来源：http://uz.wgjwhj.cn

#ifndef X_H
来源：http://qj.shxzskj.cn

#define X_H
来源：http://zx.chemitech.net.cn

#endif
来源：http://ac.szsharing.cn

[S31] C++：Hello World
来源：http://my.huixinmuqiang.cn

#include <iostream>
来源：http://zv.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://je.colortex.cn

[S32] C++：字符串
来源：http://lu.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://uh.gzmigu.cn

[S33] C++：vector 增删
来源：http://kn.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bf.panjiajie.cn

[S34] C++：遍历 vector
来源：http://ej.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://ir.shxzukj.cn


<!-- 参考信息 -->