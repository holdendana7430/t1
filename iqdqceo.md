代发 wailian999

[Q61] 移动平均
来源：http://dq.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qr.wgjwhj.cn

[Q62] 分组占比
来源：http://ji.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://os.yuntaijiaju.cn

[Q63] 开启事务
来源：http://gw.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rg.shxzskj.cn

[Q64] 提交事务
来源：http://ei.shtwfgs.cn

COMMIT;
来源：http://aa.bookmarksfly.cn

[Q65] 回滚事务
来源：http://py.huixinmuqiang.cn

ROLLBACK;
来源：http://dz.colortex.cn

[Q66] 行锁查询
来源：http://km.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wz.nszjky.cn

[Q67] 设置隔离级别
来源：http://dj.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uz.muxihuayi.cn

[Q68] 保存点
来源：http://qt.szsharing.cn

SAVEPOINT sp1;
来源：http://be.521024.cn

ROLLBACK TO sp1;
来源：http://rg.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://zm.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wk.colortex.cn

[Q70] 更新统计信息
来源：http://xi.newstarts.cn

ANALYZE TABLE users;
来源：http://vz.panjiajie.cn

[Q71] 查看建表语句
来源：http://yw.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bp.9csxet.cn

[Q72] 查看索引
来源：http://db.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://wd.newstarts.cn

[Q73] 查看表状态
来源：http://be.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xu.yuntaijiaju.cn

[Q74] 强制使用索引
来源：http://yv.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zr.szxytkj.cn

[Q75] 日期格式化
来源：http://pa.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wr.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://os.shxzukj.cn

[Q76] 按天统计
来源：http://xw.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qq.bookmarksfly.cn

[Q77] 时间加减
来源：http://ss.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iy.asd995.cn

[Q78] 当前时间
来源：http://ug.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://li.haigaiapp.cn

[Q79] 字符串拼接
来源：http://az.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vy.jctech888.com.cn

[Q80] 字符串截取
来源：http://aq.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ad.hnjuh.cn

[Q81] 字符串替换
来源：http://or.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ze.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://pj.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ab.chemitech.net.cn

[Q83] 大小写转换
来源：http://ry.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rv.asd995.cn

[Q84] 去除首尾空格
来源：http://fn.521024.cn

SELECT TRIM(name) FROM users;
来源：http://dy.haigaiapp.cn

[Q85] 数值取整
来源：http://jf.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kr.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://md.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ls.nicolike.cn

[Q87] JSON 字段做条件
来源：http://so.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gj.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://pv.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zj.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jm.shxzskj.cn

[Q89] 判断表是否存在
来源：http://jy.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oj.colortex.cn

[Q90] 生成序号列
来源：http://mk.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vj.yuntaijiaju.cn

================================================================================
来源：http://sb.shxzukj.cn

R. Bash 专题
来源：http://fz.nszjky.cn

================================================================================
来源：http://sc.shxzukj.cn

[R01] shebang 与严格模式
来源：http://ko.huanxung.cn

#!/usr/bin/env bash
来源：http://xo.gzmigu.cn

set -euo pipefail
来源：http://pe.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://jj.newstarts.cn

name="Tom"; echo "$name"
来源：http://al.nicolike.cn

[R03] 只读变量
来源：http://vs.yuntaijiaju.cn

readonly PI=3.14
来源：http://yl.colortex.cn

[R04] 位置参数
来源：http://su.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ot.muxihuayi.cn

[R05] 参数默认值
来源：http://fy.yuexingan06.cn

name="${1:-default}"
来源：http://iu.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://ez.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gg.yuexingan06.cn

[R07] if 判断文件
来源：http://pi.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cb.colortex.cn

[R08] 数值比较
来源：http://qc.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lf.lnxyls.cn

[R09] 字符串比较
来源：http://jz.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cd.muxihuayi.cn

[R10] 正则匹配
来源：http://fb.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xo.gzmigu.cn

[R11] case 多分支
来源：http://mc.hahajie.cn

case "$1" in
来源：http://dh.nszjky.cn

start) echo "启动" ;;
来源：http://au.gzmigu.cn

stop)  echo "停止" ;;
来源：http://ry.asd995.cn

*)     echo "未知命令" ;;
来源：http://dk.shxzukj.cn

esac
来源：http://el.hahajie.cn

[R12] for 遍历文件
来源：http://sq.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://so.chemitech.net.cn

[R13] for 计数循环
来源：http://rp.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://fd.huixiangedu.cn

[R14] C 风格 for
来源：http://ou.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qz.asd995.cn

[R15] while 逐行读文件
来源：http://wd.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bk.hnjuh.cn

[R16] until 等待条件
来源：http://iz.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://en.newstarts.cn

[R17] 数组定义与取值
来源：http://tt.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://da.lnxyls.cn

[R18] 遍历数组
来源：http://ve.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://je.nicolike.cn

[R19] 数组长度
来源：http://vu.shxzukj.cn

echo "${#arr[@]}"
来源：http://jz.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://mc.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oc.wgjwhj.cn

[R21] 字符串长度
来源：http://ze.muxihuayi.cn

echo "${#s}"
来源：http://ev.9csxet.cn

[R22] 截取子串
来源：http://we.lnxyls.cn

echo "${s:0:5}"
来源：http://ax.wgjwhj.cn

[R23] 字符串替换
来源：http://dt.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tg.huixinmuqiang.cn

[R24] 大小写转换
来源：http://ul.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nv.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://rk.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gg.muxihuayi.cn

[R26] 命令替换
来源：http://gk.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://lj.521024.cn

[R27] 算术展开
来源：http://qj.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://dg.nszjky.cn

[R28] 浮点运算
来源：http://em.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://ah.hnjuh.cn

[R29] 定义函数
来源：http://zf.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mc.muxihuayi.cn

[R30] 函数返回状态码
来源：http://cp.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://rq.nicolike.cn

[R31] 局部变量
来源：http://jj.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://qb.newstarts.cn

[R32] 参数个数校验
来源：http://ob.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hv.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://jj.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://se.shxzskj.cn

[R34] 退出时清理
来源：http://ps.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tv.yuexingan06.cn

[R35] 后台执行并等待
来源：http://fj.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ua.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://gi.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fg.newstarts.cn

[R37] 把输出赋给变量
来源：http://nl.gzmigu.cn

files=$(ls -1)
来源：http://ec.muxihuayi.cn

[R38] 管道串联
来源：http://xf.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://hr.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://ju.yuexingan06.cn

cmd > out.log 2>&1
来源：http://ik.wgjwhj.cn

[R40] 追加写日志
来源：http://et.jianghongdianzi.cn

echo "log" >> out.log
来源：http://nr.muxihuayi.cn

[R41] 丢弃输出
来源：http://ky.szsharing.cn

cmd >/dev/null 2>&1
来源：http://sl.lnxyls.cn

[R42] 输入重定向
来源：http://av.asd995.cn

wc -l < a.txt
来源：http://nr.yuexingan06.cn

[R43] 按名字查找文件
来源：http://fe.wgjwhj.cn

find . -name "*.log" -type f
来源：http://jo.haigaiapp.cn

[R44] 按修改时间查找
来源：http://bv.muxihuayi.cn

find . -mtime -7 -type f
来源：http://km.nicolike.cn

[R45] 批量删除
来源：http://gg.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://qf.nicolike.cn

[R46] 递归替换文件内容
来源：http://cm.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ft.shtwfgs.cn

[R47] sed 单行替换
来源：http://jd.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ko.szsharing.cn

[R48] awk 取指定列
来源：http://rb.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://hk.yuexingan06.cn

[R49] awk 带条件
来源：http://gc.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vp.wgjwhj.cn

[R50] awk 求和
来源：http://gl.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://go.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://sq.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ks.shxzukj.cn

[R52] 统计行数
来源：http://do.wgjwhj.cn

wc -l a.txt
来源：http://zp.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://kj.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gy.shxzskj.cn

[R54] 比较两个文件
来源：http://xk.haigaiapp.cn

diff a.txt b.txt
来源：http://mb.yuexingan06.cn

[R55] 压缩与解压
来源：http://jf.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qw.chemitech.net.cn

[R56] 远程拷贝
来源：http://vf.521024.cn

scp file user@host:/path/
来源：http://bq.shxzskj.cn

[R57] 远程执行命令
来源：http://jn.wgjwhj.cn

ssh user@host 'uptime'
来源：http://hq.szxytkj.cn

[R58] 下载文件
来源：http://lw.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sw.haigaiapp.cn

[R59] 发 POST JSON
来源：http://jp.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ed.521024.cn

[R60] 只看 HTTP 状态码
来源：http://er.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dg.9csxet.cn

[R61] 磁盘占用
来源：http://ml.bjjhwx.cn

df -h;  du -sh *
来源：http://yh.asd995.cn

[R62] 找最占空间的文件
来源：http://il.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://aq.huanxung.cn

[R63] 内存与进程
来源：http://kv.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://va.shxzskj.cn

[R64] 结束进程
来源：http://nb.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://qe.shxzskj.cn

[R65] 查看端口占用
来源：http://yu.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://om.nicolike.cn

[R66] 定时任务
来源：http://hd.wgjwhj.cn

crontab -e;  crontab -l
来源：http://jh.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://nf.huanxung.cn

openssl rand -hex 16
来源：http://ux.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://mu.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nu.szxytkj.cn

[R69] 生成随机密码
来源：http://xn.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://tt.colortex.cn

[R70] 时间戳与互转
来源：http://nz.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://bs.nszjky.cn

[R71] 日期格式化
来源：http://vy.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hh.huanxung.cn

[R72] 等待端口就绪
来源：http://sz.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fv.hnjuh.cn

[R73] 分割大日志
来源：http://pv.bjjhwx.cn

split -l 1000 big.log part_
来源：http://so.huanxung.cn

[R74] 批量重命名
来源：http://og.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oj.shxzskj.cn

[R75] 导出环境变量
来源：http://yv.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://pz.szsharing.cn

[R76] 使用临时文件
来源：http://ts.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ex.lnxyls.cn

[R77] 读取用户输入
来源：http://zn.chemitech.net.cn

read -rp "请输入: " ans
来源：http://mi.huanxung.cn

[R78] 交互式菜单
来源：http://kz.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gs.shxzukj.cn

[R79] 解析命令行选项
来源：http://mf.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fb.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://xz.jianghongdianzi.cn

time ./run.sh
来源：http://zc.newstarts.cn

================================================================================
来源：http://fv.bjjhwx.cn

S. C / C++ 专题
来源：http://do.shtwfgs.cn

================================================================================
来源：http://wo.shtwfgs.cn

[S01] C：Hello World
来源：http://ca.asd995.cn

#include <stdio.h>
来源：http://yj.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vy.colortex.cn

[S02] C：变量与格式化输出
来源：http://kw.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://wi.shtwfgs.cn

[S03] C：读入整数
来源：http://jx.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://gp.panjiajie.cn

[S04] C：字符串复制
来源：http://ss.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tf.bookmarksfly.cn

[S05] C：字符串长度
来源：http://ki.shtwfgs.cn

strlen(s)
来源：http://cg.hnjuh.cn

[S06] C：字符串比较
来源：http://al.wgjwhj.cn

strcmp(a, b) == 0
来源：http://yh.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://zv.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qr.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://ej.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jj.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://rm.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bv.newstarts.cn

[S10] C：指针与解引用
来源：http://ey.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://cl.asd995.cn

[S11] C：逐行读文件
来源：http://vd.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://zj.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qt.jianghongdianzi.cn

fclose(f);
来源：http://tx.bjjhwx.cn

[S12] C：写文件
来源：http://xy.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cq.bjjhwx.cn

[S13] C：宏定义
来源：http://dm.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ev.shxzskj.cn

[S14] C：枚举
来源：http://rp.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://my.gzmigu.cn

[S15] C：类型转换
来源：http://mx.yuexingan06.cn

(double) a / b
来源：http://wo.haigaiapp.cn

[S16] C：位操作置位
来源：http://vh.panjiajie.cn

x |= (1 << 3);
来源：http://at.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://gc.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ur.bookmarksfly.cn

[S18] C：命令行参数
来源：http://ju.nszjky.cn

int main(int argc, char **argv)
来源：http://cm.lnxyls.cn

[S19] C：快速排序
来源：http://uz.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://te.chemitech.net.cn

[S20] C：二分查找
来源：http://kq.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qg.wgjwhj.cn

[S21] C：字符类别判断
来源：http://we.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wk.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://xg.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cu.shxzskj.cn

[S23] C：随机数
来源：http://mx.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ob.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://ue.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xk.9csxet.cn

[S25] C：内存拷贝
来源：http://hw.szxytkj.cn

memcpy(dst, src, n);
来源：http://jj.shxzukj.cn

[S26] C：内存清零
来源：http://xp.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://ss.nszjky.cn

[S27] C：定义常量
来源：http://hd.bjjhwx.cn

const double PI = 3.14159;
来源：http://kr.yuexingan06.cn

[S28] C：静态变量
来源：http://xt.wgjwhj.cn

static int counter = 0;
来源：http://nf.hnjuh.cn

[S29] C：变参函数
来源：http://mc.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ca.huixiangedu.cn

[S30] C：头文件保护
来源：http://jc.shxzukj.cn

#ifndef X_H
来源：http://xt.szsharing.cn

#define X_H
来源：http://wy.hnjuh.cn

#endif
来源：http://qh.9csxet.cn

[S31] C++：Hello World
来源：http://ug.huixinmuqiang.cn


<!-- 参考信息 -->