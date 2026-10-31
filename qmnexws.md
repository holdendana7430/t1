代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lr.521024.cn

[Q60] 取上一行 / 下一行
来源：http://hg.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qy.hnjuh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xi.panjiajie.cn

[Q61] 移动平均
来源：http://ns.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wy.nszjky.cn

[Q62] 分组占比
来源：http://xj.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uy.haigaiapp.cn

[Q63] 开启事务
来源：http://bl.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qt.shxzukj.cn

[Q64] 提交事务
来源：http://su.huixiangedu.cn

COMMIT;
来源：http://sm.panjiajie.cn

[Q65] 回滚事务
来源：http://zb.chemitech.net.cn

ROLLBACK;
来源：http://uo.shxzskj.cn

[Q66] 行锁查询
来源：http://ip.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rd.521024.cn

[Q67] 设置隔离级别
来源：http://vt.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kq.muxihuayi.cn

[Q68] 保存点
来源：http://ts.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://js.gzmigu.cn

ROLLBACK TO sp1;
来源：http://xc.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://cq.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rg.lnxyls.cn

[Q70] 更新统计信息
来源：http://wf.hahajie.cn

ANALYZE TABLE users;
来源：http://fi.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://mu.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zw.szxytkj.cn

[Q72] 查看索引
来源：http://qy.hnjuh.cn

SHOW INDEX FROM users;
来源：http://rg.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://nv.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uq.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://bk.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://io.hnjuh.cn

[Q75] 日期格式化
来源：http://nv.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vq.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://de.huixinmuqiang.cn

[Q76] 按天统计
来源：http://ya.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uy.chemitech.net.cn

[Q77] 时间加减
来源：http://su.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gs.yuntaijiaju.cn

[Q78] 当前时间
来源：http://lv.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bj.9csxet.cn

[Q79] 字符串拼接
来源：http://ts.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wg.shxzskj.cn

[Q80] 字符串截取
来源：http://ed.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vy.521024.cn

[Q81] 字符串替换
来源：http://li.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ve.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://aa.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mp.chemitech.net.cn

[Q83] 大小写转换
来源：http://zw.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vn.hnjuh.cn

[Q84] 去除首尾空格
来源：http://gr.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://ym.bjjhwx.cn

[Q85] 数值取整
来源：http://du.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nz.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://bd.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zt.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://wa.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mz.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://uo.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kb.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gg.szsharing.cn

[Q89] 判断表是否存在
来源：http://nj.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hv.hnjuh.cn

[Q90] 生成序号列
来源：http://pe.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nf.yuntaijiaju.cn

================================================================================
来源：http://hw.jianghongdianzi.cn

R. Bash 专题
来源：http://lh.szsharing.cn

================================================================================
来源：http://ex.huanxung.cn

[R01] shebang 与严格模式
来源：http://cc.wgjwhj.cn

#!/usr/bin/env bash
来源：http://ws.szxytkj.cn

set -euo pipefail
来源：http://ga.shxzukj.cn

[R02] 变量赋值与使用
来源：http://wg.asd995.cn

name="Tom"; echo "$name"
来源：http://jw.9csxet.cn

[R03] 只读变量
来源：http://is.9csxet.cn

readonly PI=3.14
来源：http://kn.nszjky.cn

[R04] 位置参数
来源：http://kk.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ro.9csxet.cn

[R05] 参数默认值
来源：http://mt.nicolike.cn

name="${1:-default}"
来源：http://ej.shxzukj.cn

[R06] 判断命令是否存在
来源：http://av.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vc.chemitech.net.cn

[R07] if 判断文件
来源：http://pe.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vf.lnxyls.cn

[R08] 数值比较
来源：http://jg.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dg.nszjky.cn

[R09] 字符串比较
来源：http://do.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iw.haigaiapp.cn

[R10] 正则匹配
来源：http://ue.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ef.huanxung.cn

[R11] case 多分支
来源：http://id.muxihuayi.cn

case "$1" in
来源：http://mi.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://zg.szxytkj.cn

stop)  echo "停止" ;;
来源：http://lf.gzmigu.cn

*)     echo "未知命令" ;;
来源：http://na.shxzskj.cn

esac
来源：http://gi.huixiangedu.cn

[R12] for 遍历文件
来源：http://ms.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://dg.asd995.cn

[R13] for 计数循环
来源：http://yl.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://gy.9csxet.cn

[R14] C 风格 for
来源：http://mb.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tm.yuexingan06.cn

[R15] while 逐行读文件
来源：http://ni.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kh.nicolike.cn

[R16] until 等待条件
来源：http://uq.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ru.chemitech.net.cn

[R17] 数组定义与取值
来源：http://pg.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://va.gzmigu.cn

[R18] 遍历数组
来源：http://ze.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xv.shxzukj.cn

[R19] 数组长度
来源：http://ob.chemitech.net.cn

echo "${#arr[@]}"
来源：http://re.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://yy.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qw.szsharing.cn

[R21] 字符串长度
来源：http://ei.colortex.cn

echo "${#s}"
来源：http://rn.shxzukj.cn

[R22] 截取子串
来源：http://xk.colortex.cn

echo "${s:0:5}"
来源：http://eo.yuexingan06.cn

[R23] 字符串替换
来源：http://dc.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kf.wgjwhj.cn

[R24] 大小写转换
来源：http://yi.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://be.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://eb.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fs.bookmarksfly.cn

[R26] 命令替换
来源：http://mj.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://gj.szxytkj.cn

[R27] 算术展开
来源：http://sz.huanxung.cn

echo $((1 + 2 * 3))
来源：http://ih.colortex.cn

[R28] 浮点运算
来源：http://hm.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://el.bjjhwx.cn

[R29] 定义函数
来源：http://fk.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tk.jctech888.com.cn

[R30] 函数返回状态码
来源：http://uw.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://js.nszjky.cn

[R31] 局部变量
来源：http://vu.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://oe.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://kb.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ds.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://yv.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uv.bookmarksfly.cn

[R34] 退出时清理
来源：http://ew.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ds.9csxet.cn

[R35] 后台执行并等待
来源：http://nq.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ad.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://hq.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ry.huanxung.cn

[R37] 把输出赋给变量
来源：http://az.yuntaijiaju.cn

files=$(ls -1)
来源：http://yx.colortex.cn

[R38] 管道串联
来源：http://lv.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://ko.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://lq.szsharing.cn

cmd > out.log 2>&1
来源：http://ca.shxzskj.cn

[R40] 追加写日志
来源：http://af.521024.cn

echo "log" >> out.log
来源：http://is.yuexingan06.cn

[R41] 丢弃输出
来源：http://bx.szsharing.cn

cmd >/dev/null 2>&1
来源：http://qh.gzmigu.cn

[R42] 输入重定向
来源：http://vx.nszjky.cn

wc -l < a.txt
来源：http://iw.panjiajie.cn

[R43] 按名字查找文件
来源：http://yu.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://ev.colortex.cn

[R44] 按修改时间查找
来源：http://pp.szxytkj.cn

find . -mtime -7 -type f
来源：http://hu.jctech888.com.cn

[R45] 批量删除
来源：http://zu.huanxung.cn

find . -name "*.tmp" -delete
来源：http://hj.lnxyls.cn

[R46] 递归替换文件内容
来源：http://yw.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pa.colortex.cn

[R47] sed 单行替换
来源：http://ku.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wa.nicolike.cn

[R48] awk 取指定列
来源：http://hl.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://mq.jianghongdianzi.cn

[R49] awk 带条件
来源：http://ab.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ys.gzmigu.cn

[R50] awk 求和
来源：http://vo.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ru.lnxyls.cn

[R51] 排序去重取前几
来源：http://nw.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yx.huixiangedu.cn

[R52] 统计行数
来源：http://gl.panjiajie.cn

wc -l a.txt
来源：http://xk.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://pv.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mo.9csxet.cn

[R54] 比较两个文件
来源：http://xm.hahajie.cn

diff a.txt b.txt
来源：http://ee.colortex.cn

[R55] 压缩与解压
来源：http://gw.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ap.shxzukj.cn

[R56] 远程拷贝
来源：http://jm.hahajie.cn

scp file user@host:/path/
来源：http://qm.chemitech.net.cn

[R57] 远程执行命令
来源：http://or.gzmigu.cn

ssh user@host 'uptime'
来源：http://gi.lnxyls.cn

[R58] 下载文件
来源：http://gh.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zz.bjjhwx.cn

[R59] 发 POST JSON
来源：http://wv.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zx.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://ho.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yn.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://cj.yuntaijiaju.cn

df -h;  du -sh *
来源：http://qu.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://uo.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://ze.jctech888.com.cn

[R63] 内存与进程
来源：http://cw.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://mp.haigaiapp.cn

[R64] 结束进程
来源：http://aa.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://ha.bookmarksfly.cn

[R65] 查看端口占用
来源：http://ur.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vh.szxytkj.cn

[R66] 定时任务
来源：http://oc.9csxet.cn

crontab -e;  crontab -l
来源：http://ax.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://dp.bookmarksfly.cn

openssl rand -hex 16
来源：http://ae.nicolike.cn

[R68] 计算文件校验值
来源：http://vp.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dk.hnjuh.cn

[R69] 生成随机密码
来源：http://hm.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://ey.9csxet.cn

[R70] 时间戳与互转
来源：http://qp.nszjky.cn

date +%s;  date -d @1700000000
来源：http://rc.hnjuh.cn

[R71] 日期格式化
来源：http://gy.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ji.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://lu.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tb.huixiangedu.cn

[R73] 分割大日志
来源：http://ia.haigaiapp.cn

split -l 1000 big.log part_
来源：http://tu.wgjwhj.cn

[R74] 批量重命名
来源：http://sv.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hf.hnjuh.cn

[R75] 导出环境变量
来源：http://ld.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ng.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://jp.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hl.hahajie.cn

[R77] 读取用户输入
来源：http://ev.panjiajie.cn

read -rp "请输入: " ans
来源：http://ss.9csxet.cn

[R78] 交互式菜单
来源：http://nb.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rj.colortex.cn

[R79] 解析命令行选项
来源：http://al.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://am.asd995.cn

[R80] 查看脚本执行耗时
来源：http://ss.colortex.cn

time ./run.sh
来源：http://lb.huixiangedu.cn

================================================================================
来源：http://vg.gzmigu.cn

S. C / C++ 专题
来源：http://hn.shxzskj.cn

================================================================================
来源：http://ws.yuntaijiaju.cn

[S01] C：Hello World
来源：http://pa.shxzukj.cn

#include <stdio.h>
来源：http://nr.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bp.nicolike.cn

[S02] C：变量与格式化输出
来源：http://ef.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://hm.szxytkj.cn

[S03] C：读入整数
来源：http://yi.gzmigu.cn

int x; scanf("%d", &x);
来源：http://bl.bjjhwx.cn

[S04] C：字符串复制
来源：http://pj.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gk.haigaiapp.cn

[S05] C：字符串长度
来源：http://jx.bookmarksfly.cn

strlen(s)
来源：http://wa.panjiajie.cn

[S06] C：字符串比较
来源：http://qe.shxzskj.cn

strcmp(a, b) == 0
来源：http://rx.huanxung.cn

[S07] C：数组遍历求和
来源：http://km.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xk.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://hh.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nu.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://bd.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://db.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://iq.nszjky.cn

int *p = &a;  *p = 5;
来源：http://zf.muxihuayi.cn

[S11] C：逐行读文件
来源：http://lw.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ei.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xk.bookmarksfly.cn

fclose(f);
来源：http://xt.lnxyls.cn

[S12] C：写文件
来源：http://hs.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vl.muxihuayi.cn

[S13] C：宏定义
来源：http://dw.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mh.521024.cn

[S14] C：枚举
来源：http://pb.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://dp.chemitech.net.cn

[S15] C：类型转换
来源：http://wt.haigaiapp.cn

(double) a / b
来源：http://tw.gzmigu.cn

[S16] C：位操作置位
来源：http://bf.chemitech.net.cn

x |= (1 << 3);
来源：http://zy.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://xk.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cc.chemitech.net.cn

[S18] C：命令行参数
来源：http://uh.9csxet.cn

int main(int argc, char **argv)
来源：http://fy.jianghongdianzi.cn

[S19] C：快速排序
来源：http://nv.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rl.bookmarksfly.cn

[S20] C：二分查找
来源：http://ry.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vz.shtwfgs.cn

[S21] C：字符类别判断
来源：http://cl.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wm.huixiangedu.cn

[S22] C：字符串转数字
来源：http://qr.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ra.newstarts.cn

[S23] C：随机数
来源：http://vi.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nh.gzmigu.cn

[S24] C：获取本地时间
来源：http://at.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uv.nszjky.cn

[S25] C：内存拷贝
来源：http://hq.nicolike.cn

memcpy(dst, src, n);
来源：http://cs.nicolike.cn

[S26] C：内存清零
来源：http://do.nszjky.cn

memset(a, 0, sizeof a);
来源：http://jk.bjjhwx.cn

[S27] C：定义常量
来源：http://ik.muxihuayi.cn

const double PI = 3.14159;
来源：http://kq.panjiajie.cn

[S28] C：静态变量
来源：http://qw.nicolike.cn

static int counter = 0;
来源：http://gb.shxzskj.cn

[S29] C：变参函数
来源：http://wq.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tu.bjjhwx.cn

[S30] C：头文件保护
来源：http://dg.jctech888.com.cn


<!-- 参考信息 -->