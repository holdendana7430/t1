代发 wailian999

[Q61] 移动平均
来源：http://xl.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jn.wgjwhj.cn

[Q62] 分组占比
来源：http://et.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ll.colortex.cn

[Q63] 开启事务
来源：http://hw.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wq.huixinmuqiang.cn

[Q64] 提交事务
来源：http://eu.asd995.cn

COMMIT;
来源：http://qw.huanxung.cn

[Q65] 回滚事务
来源：http://sy.shtwfgs.cn

ROLLBACK;
来源：http://yr.wgjwhj.cn

[Q66] 行锁查询
来源：http://eu.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zh.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://ah.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pa.huanxung.cn

[Q68] 保存点
来源：http://qx.panjiajie.cn

SAVEPOINT sp1;
来源：http://xf.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://ty.haigaiapp.cn

[Q69] 查看执行计划
来源：http://ys.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tf.521024.cn

[Q70] 更新统计信息
来源：http://kf.gzmigu.cn

ANALYZE TABLE users;
来源：http://dg.yuexingan06.cn

[Q71] 查看建表语句
来源：http://sd.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fs.szsharing.cn

[Q72] 查看索引
来源：http://ph.huanxung.cn

SHOW INDEX FROM users;
来源：http://fa.haigaiapp.cn

[Q73] 查看表状态
来源：http://ud.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vs.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://nl.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fn.lnxyls.cn

[Q75] 日期格式化
来源：http://bi.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ew.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zi.colortex.cn

[Q76] 按天统计
来源：http://gp.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tw.huixiangedu.cn

[Q77] 时间加减
来源：http://pk.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mj.521024.cn

[Q78] 当前时间
来源：http://az.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://go.shtwfgs.cn

[Q79] 字符串拼接
来源：http://aw.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ud.shxzukj.cn

[Q80] 字符串截取
来源：http://kd.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ez.shxzukj.cn

[Q81] 字符串替换
来源：http://ba.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vb.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://vd.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gr.lnxyls.cn

[Q83] 大小写转换
来源：http://ur.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ue.szsharing.cn

[Q84] 去除首尾空格
来源：http://bj.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://zr.asd995.cn

[Q85] 数值取整
来源：http://vf.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://va.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://lk.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nu.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://ek.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yn.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://fn.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qe.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fx.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://pk.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ez.panjiajie.cn

[Q90] 生成序号列
来源：http://qh.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vh.shxzukj.cn

================================================================================
来源：http://co.gzmigu.cn

R. Bash 专题
来源：http://ch.nicolike.cn

================================================================================
来源：http://gt.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://ns.gzmigu.cn

#!/usr/bin/env bash
来源：http://fa.521024.cn

set -euo pipefail
来源：http://nb.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://po.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://pp.9csxet.cn

[R03] 只读变量
来源：http://eq.wgjwhj.cn

readonly PI=3.14
来源：http://gy.huixinmuqiang.cn

[R04] 位置参数
来源：http://xy.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://no.asd995.cn

[R05] 参数默认值
来源：http://vc.szsharing.cn

name="${1:-default}"
来源：http://nk.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://ky.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rv.yuexingan06.cn

[R07] if 判断文件
来源：http://kx.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wv.huixiangedu.cn

[R08] 数值比较
来源：http://lh.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sv.szxytkj.cn

[R09] 字符串比较
来源：http://pq.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kg.521024.cn

[R10] 正则匹配
来源：http://jz.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hc.hnjuh.cn

[R11] case 多分支
来源：http://js.newstarts.cn

case "$1" in
来源：http://xg.shtwfgs.cn

start) echo "启动" ;;
来源：http://yq.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://yy.colortex.cn

*)     echo "未知命令" ;;
来源：http://jz.shtwfgs.cn

esac
来源：http://ay.nicolike.cn

[R12] for 遍历文件
来源：http://ti.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://be.bookmarksfly.cn

[R13] for 计数循环
来源：http://dm.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://cg.521024.cn

[R14] C 风格 for
来源：http://qp.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yk.shxzukj.cn

[R15] while 逐行读文件
来源：http://dh.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dr.panjiajie.cn

[R16] until 等待条件
来源：http://kt.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eg.nicolike.cn

[R17] 数组定义与取值
来源：http://uf.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jc.9csxet.cn

[R18] 遍历数组
来源：http://wp.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ri.lnxyls.cn

[R19] 数组长度
来源：http://fs.asd995.cn

echo "${#arr[@]}"
来源：http://yb.asd995.cn

[R20] 关联数组（字典）
来源：http://oz.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fh.huixinmuqiang.cn

[R21] 字符串长度
来源：http://ve.szxytkj.cn

echo "${#s}"
来源：http://cw.szxytkj.cn

[R22] 截取子串
来源：http://du.colortex.cn

echo "${s:0:5}"
来源：http://ug.jianghongdianzi.cn

[R23] 字符串替换
来源：http://lj.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oi.asd995.cn

[R24] 大小写转换
来源：http://ur.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uc.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://wi.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wo.nszjky.cn

[R26] 命令替换
来源：http://kd.521024.cn

now=$(date +%F); echo "$now"
来源：http://gn.haigaiapp.cn

[R27] 算术展开
来源：http://wc.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://rn.shtwfgs.cn

[R28] 浮点运算
来源：http://an.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://fm.jianghongdianzi.cn

[R29] 定义函数
来源：http://gs.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qj.szxytkj.cn

[R30] 函数返回状态码
来源：http://uo.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://vb.hahajie.cn

[R31] 局部变量
来源：http://wg.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://ur.shxzskj.cn

[R32] 参数个数校验
来源：http://gv.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aw.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://jn.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ax.shtwfgs.cn

[R34] 退出时清理
来源：http://km.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://za.hnjuh.cn

[R35] 后台执行并等待
来源：http://sv.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cv.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://hj.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ou.521024.cn

[R37] 把输出赋给变量
来源：http://gy.huixinmuqiang.cn

files=$(ls -1)
来源：http://jf.newstarts.cn

[R38] 管道串联
来源：http://ae.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://ci.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://ax.bjjhwx.cn

cmd > out.log 2>&1
来源：http://tv.haigaiapp.cn

[R40] 追加写日志
来源：http://iv.asd995.cn

echo "log" >> out.log
来源：http://ci.shxzskj.cn

[R41] 丢弃输出
来源：http://fh.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://qk.szxytkj.cn

[R42] 输入重定向
来源：http://pw.colortex.cn

wc -l < a.txt
来源：http://bk.nszjky.cn

[R43] 按名字查找文件
来源：http://br.nszjky.cn

find . -name "*.log" -type f
来源：http://wx.huanxung.cn

[R44] 按修改时间查找
来源：http://ua.haigaiapp.cn

find . -mtime -7 -type f
来源：http://kc.yuexingan06.cn

[R45] 批量删除
来源：http://xi.colortex.cn

find . -name "*.tmp" -delete
来源：http://wp.9csxet.cn

[R46] 递归替换文件内容
来源：http://cn.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lr.wgjwhj.cn

[R47] sed 单行替换
来源：http://vc.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ci.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://jr.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://zz.lnxyls.cn

[R49] awk 带条件
来源：http://wp.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://py.bjjhwx.cn

[R50] awk 求和
来源：http://tq.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vm.lnxyls.cn

[R51] 排序去重取前几
来源：http://db.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lh.521024.cn

[R52] 统计行数
来源：http://tl.9csxet.cn

wc -l a.txt
来源：http://ie.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://ma.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jj.szxytkj.cn

[R54] 比较两个文件
来源：http://em.jctech888.com.cn

diff a.txt b.txt
来源：http://vb.muxihuayi.cn

[R55] 压缩与解压
来源：http://zq.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cd.hnjuh.cn

[R56] 远程拷贝
来源：http://nv.lnxyls.cn

scp file user@host:/path/
来源：http://ax.huixiangedu.cn

[R57] 远程执行命令
来源：http://uj.yuexingan06.cn

ssh user@host 'uptime'
来源：http://hw.newstarts.cn

[R58] 下载文件
来源：http://tn.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vu.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://ui.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cq.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://ha.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ah.szsharing.cn

[R61] 磁盘占用
来源：http://vc.gzmigu.cn

df -h;  du -sh *
来源：http://uh.panjiajie.cn

[R62] 找最占空间的文件
来源：http://kc.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://hw.yuntaijiaju.cn

[R63] 内存与进程
来源：http://tn.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://fm.huixinmuqiang.cn

[R64] 结束进程
来源：http://ek.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://ko.chemitech.net.cn

[R65] 查看端口占用
来源：http://ur.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wr.gzmigu.cn

[R66] 定时任务
来源：http://dy.bjjhwx.cn

crontab -e;  crontab -l
来源：http://qc.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://ww.nicolike.cn

openssl rand -hex 16
来源：http://mo.muxihuayi.cn

[R68] 计算文件校验值
来源：http://xb.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tj.colortex.cn

[R69] 生成随机密码
来源：http://xh.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://zu.newstarts.cn

[R70] 时间戳与互转
来源：http://sy.colortex.cn

date +%s;  date -d @1700000000
来源：http://fm.szsharing.cn

[R71] 日期格式化
来源：http://kq.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dn.gzmigu.cn

[R72] 等待端口就绪
来源：http://fd.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zr.newstarts.cn

[R73] 分割大日志
来源：http://mo.521024.cn

split -l 1000 big.log part_
来源：http://wc.shxzukj.cn

[R74] 批量重命名
来源：http://fh.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mf.hnjuh.cn

[R75] 导出环境变量
来源：http://wr.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://fg.wgjwhj.cn

[R76] 使用临时文件
来源：http://jy.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ud.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://ye.asd995.cn

read -rp "请输入: " ans
来源：http://yj.bookmarksfly.cn

[R78] 交互式菜单
来源：http://ps.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nq.colortex.cn

[R79] 解析命令行选项
来源：http://yx.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rb.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://oy.nicolike.cn

time ./run.sh
来源：http://jk.colortex.cn

================================================================================
来源：http://ji.nicolike.cn

S. C / C++ 专题
来源：http://mh.newstarts.cn

================================================================================
来源：http://jk.haigaiapp.cn

[S01] C：Hello World
来源：http://vq.hahajie.cn

#include <stdio.h>
来源：http://gr.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ud.9csxet.cn

[S02] C：变量与格式化输出
来源：http://be.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://by.szxytkj.cn

[S03] C：读入整数
来源：http://un.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://sd.panjiajie.cn

[S04] C：字符串复制
来源：http://yl.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sf.nszjky.cn

[S05] C：字符串长度
来源：http://uv.shxzskj.cn

strlen(s)
来源：http://ns.wgjwhj.cn

[S06] C：字符串比较
来源：http://jq.shxzukj.cn

strcmp(a, b) == 0
来源：http://ue.huanxung.cn

[S07] C：数组遍历求和
来源：http://le.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wc.colortex.cn

[S08] C：动态内存分配与释放
来源：http://ul.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ic.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://zh.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qs.newstarts.cn

[S10] C：指针与解引用
来源：http://aq.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://le.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://jt.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://li.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dl.yuntaijiaju.cn

fclose(f);
来源：http://ob.chemitech.net.cn

[S12] C：写文件
来源：http://ei.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vc.chemitech.net.cn

[S13] C：宏定义
来源：http://dq.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tb.huixinmuqiang.cn

[S14] C：枚举
来源：http://ew.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://vr.szsharing.cn

[S15] C：类型转换
来源：http://zt.gzmigu.cn

(double) a / b
来源：http://eo.lnxyls.cn

[S16] C：位操作置位
来源：http://rn.wgjwhj.cn

x |= (1 << 3);
来源：http://bf.newstarts.cn

[S17] C：安全拼接字符串
来源：http://dk.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cb.huixiangedu.cn

[S18] C：命令行参数
来源：http://in.hnjuh.cn

int main(int argc, char **argv)
来源：http://oh.chemitech.net.cn

[S19] C：快速排序
来源：http://oh.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lp.panjiajie.cn

[S20] C：二分查找
来源：http://dm.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cn.nicolike.cn

[S21] C：字符类别判断
来源：http://cg.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://di.wgjwhj.cn

[S22] C：字符串转数字
来源：http://og.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wp.shtwfgs.cn

[S23] C：随机数
来源：http://ow.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dc.521024.cn

[S24] C：获取本地时间
来源：http://ju.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://om.lnxyls.cn

[S25] C：内存拷贝
来源：http://ew.newstarts.cn

memcpy(dst, src, n);
来源：http://gi.jctech888.com.cn

[S26] C：内存清零
来源：http://sm.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://ce.muxihuayi.cn

[S27] C：定义常量
来源：http://mr.jctech888.com.cn

const double PI = 3.14159;
来源：http://zw.chemitech.net.cn

[S28] C：静态变量
来源：http://ko.lnxyls.cn

static int counter = 0;
来源：http://fp.9csxet.cn

[S29] C：变参函数
来源：http://ay.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ej.yuexingan06.cn

[S30] C：头文件保护
来源：http://to.jctech888.com.cn

#ifndef X_H
来源：http://av.chemitech.net.cn

#define X_H
来源：http://vh.muxihuayi.cn

#endif
来源：http://ut.huixiangedu.cn

[S31] C++：Hello World
来源：http://wd.wgjwhj.cn


<!-- 参考信息 -->