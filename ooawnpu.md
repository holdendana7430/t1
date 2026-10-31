代发 wailian999

[Q61] 移动平均
来源：http://fc.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hf.huixinmuqiang.cn

[Q62] 分组占比
来源：http://tf.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fn.panjiajie.cn

[Q63] 开启事务
来源：http://zj.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nq.jianghongdianzi.cn

[Q64] 提交事务
来源：http://jr.yuexingan06.cn

COMMIT;
来源：http://bv.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://us.yuexingan06.cn

ROLLBACK;
来源：http://ss.muxihuayi.cn

[Q66] 行锁查询
来源：http://aw.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dm.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://nc.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zs.huanxung.cn

[Q68] 保存点
来源：http://tx.chemitech.net.cn

SAVEPOINT sp1;
来源：http://lw.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://xs.gzmigu.cn

[Q69] 查看执行计划
来源：http://rf.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sf.panjiajie.cn

[Q70] 更新统计信息
来源：http://gx.lnxyls.cn

ANALYZE TABLE users;
来源：http://zc.colortex.cn

[Q71] 查看建表语句
来源：http://cm.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iw.chemitech.net.cn

[Q72] 查看索引
来源：http://dc.panjiajie.cn

SHOW INDEX FROM users;
来源：http://iq.huanxung.cn

[Q73] 查看表状态
来源：http://or.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ro.szxytkj.cn

[Q74] 强制使用索引
来源：http://aq.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rr.chemitech.net.cn

[Q75] 日期格式化
来源：http://we.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kz.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xg.jctech888.com.cn

[Q76] 按天统计
来源：http://ig.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yw.bjjhwx.cn

[Q77] 时间加减
来源：http://es.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aq.yuexingan06.cn

[Q78] 当前时间
来源：http://ur.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://up.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://ps.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hs.shxzskj.cn

[Q80] 字符串截取
来源：http://tm.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qa.bjjhwx.cn

[Q81] 字符串替换
来源：http://wo.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vm.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://af.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rn.jctech888.com.cn

[Q83] 大小写转换
来源：http://hp.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://du.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://px.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://rp.shxzskj.cn

[Q85] 数值取整
来源：http://nu.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hn.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://fe.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bc.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://pq.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iy.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://ef.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bu.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mq.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://bk.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://im.newstarts.cn

[Q90] 生成序号列
来源：http://qk.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wp.szxytkj.cn

================================================================================
来源：http://sm.bjjhwx.cn

R. Bash 专题
来源：http://wk.yuexingan06.cn

================================================================================
来源：http://yf.hahajie.cn

[R01] shebang 与严格模式
来源：http://sh.hahajie.cn

#!/usr/bin/env bash
来源：http://mi.wgjwhj.cn

set -euo pipefail
来源：http://xq.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://px.hnjuh.cn

name="Tom"; echo "$name"
来源：http://sx.shxzskj.cn

[R03] 只读变量
来源：http://jo.chemitech.net.cn

readonly PI=3.14
来源：http://qo.huanxung.cn

[R04] 位置参数
来源：http://ht.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bo.shtwfgs.cn

[R05] 参数默认值
来源：http://ep.nszjky.cn

name="${1:-default}"
来源：http://fn.hahajie.cn

[R06] 判断命令是否存在
来源：http://py.bjjhwx.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pr.hahajie.cn

[R07] if 判断文件
来源：http://wu.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ds.huixinmuqiang.cn

[R08] 数值比较
来源：http://dd.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jf.szsharing.cn

[R09] 字符串比较
来源：http://wi.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lf.szsharing.cn

[R10] 正则匹配
来源：http://de.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tz.panjiajie.cn

[R11] case 多分支
来源：http://sr.muxihuayi.cn

case "$1" in
来源：http://ba.nszjky.cn

start) echo "启动" ;;
来源：http://ga.9csxet.cn

stop)  echo "停止" ;;
来源：http://sa.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://zt.lnxyls.cn

esac
来源：http://us.shxzukj.cn

[R12] for 遍历文件
来源：http://ar.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://ll.chemitech.net.cn

[R13] for 计数循环
来源：http://iw.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://mk.haigaiapp.cn

[R14] C 风格 for
来源：http://th.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vr.szxytkj.cn

[R15] while 逐行读文件
来源：http://do.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dp.hahajie.cn

[R16] until 等待条件
来源：http://ox.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://my.shtwfgs.cn

[R17] 数组定义与取值
来源：http://zw.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bm.huixiangedu.cn

[R18] 遍历数组
来源：http://zt.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ux.jianghongdianzi.cn

[R19] 数组长度
来源：http://op.huixiangedu.cn

echo "${#arr[@]}"
来源：http://fy.asd995.cn

[R20] 关联数组（字典）
来源：http://vp.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bt.hnjuh.cn

[R21] 字符串长度
来源：http://nw.asd995.cn

echo "${#s}"
来源：http://qw.shxzukj.cn

[R22] 截取子串
来源：http://ry.huixiangedu.cn

echo "${s:0:5}"
来源：http://vp.colortex.cn

[R23] 字符串替换
来源：http://hg.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ko.9csxet.cn

[R24] 大小写转换
来源：http://vm.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://su.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://vz.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jb.hahajie.cn

[R26] 命令替换
来源：http://cx.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://nk.lnxyls.cn

[R27] 算术展开
来源：http://kx.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://xh.asd995.cn

[R28] 浮点运算
来源：http://id.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://pz.shxzukj.cn

[R29] 定义函数
来源：http://ec.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dt.shxzukj.cn

[R30] 函数返回状态码
来源：http://xz.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://jk.521024.cn

[R31] 局部变量
来源：http://qw.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://wd.huixiangedu.cn

[R32] 参数个数校验
来源：http://wk.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kw.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://uf.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://he.haigaiapp.cn

[R34] 退出时清理
来源：http://jl.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sg.hahajie.cn

[R35] 后台执行并等待
来源：http://um.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pk.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://sf.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sq.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://wr.jianghongdianzi.cn

files=$(ls -1)
来源：http://va.colortex.cn

[R38] 管道串联
来源：http://sb.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://xi.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://qo.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://ui.haigaiapp.cn

[R40] 追加写日志
来源：http://jr.jctech888.com.cn

echo "log" >> out.log
来源：http://aj.lnxyls.cn

[R41] 丢弃输出
来源：http://ld.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://lw.jctech888.com.cn

[R42] 输入重定向
来源：http://qr.chemitech.net.cn

wc -l < a.txt
来源：http://zs.nszjky.cn

[R43] 按名字查找文件
来源：http://de.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://aj.9csxet.cn

[R44] 按修改时间查找
来源：http://el.shtwfgs.cn

find . -mtime -7 -type f
来源：http://id.9csxet.cn

[R45] 批量删除
来源：http://ei.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://ea.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://kr.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oc.lnxyls.cn

[R47] sed 单行替换
来源：http://pn.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jn.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://vs.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://gy.haigaiapp.cn

[R49] awk 带条件
来源：http://sa.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yw.9csxet.cn

[R50] awk 求和
来源：http://iv.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xe.chemitech.net.cn

[R51] 排序去重取前几
来源：http://cm.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vw.huixinmuqiang.cn

[R52] 统计行数
来源：http://ej.lnxyls.cn

wc -l a.txt
来源：http://pn.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://ug.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://al.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://af.bookmarksfly.cn

diff a.txt b.txt
来源：http://hn.shxzskj.cn

[R55] 压缩与解压
来源：http://dw.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vm.colortex.cn

[R56] 远程拷贝
来源：http://um.muxihuayi.cn

scp file user@host:/path/
来源：http://ir.hahajie.cn

[R57] 远程执行命令
来源：http://xw.newstarts.cn

ssh user@host 'uptime'
来源：http://ku.9csxet.cn

[R58] 下载文件
来源：http://ak.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cg.panjiajie.cn

[R59] 发 POST JSON
来源：http://ac.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jd.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://fv.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ik.yuexingan06.cn

[R61] 磁盘占用
来源：http://iy.haigaiapp.cn

df -h;  du -sh *
来源：http://sl.shxzskj.cn

[R62] 找最占空间的文件
来源：http://xy.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://xw.hahajie.cn

[R63] 内存与进程
来源：http://xf.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://ty.chemitech.net.cn

[R64] 结束进程
来源：http://sz.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://bo.yuexingan06.cn

[R65] 查看端口占用
来源：http://yt.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qc.huixiangedu.cn

[R66] 定时任务
来源：http://xu.hnjuh.cn

crontab -e;  crontab -l
来源：http://mt.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://gy.szsharing.cn

openssl rand -hex 16
来源：http://lz.asd995.cn

[R68] 计算文件校验值
来源：http://fs.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qk.9csxet.cn

[R69] 生成随机密码
来源：http://ut.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://vx.yuexingan06.cn

[R70] 时间戳与互转
来源：http://hc.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://mj.521024.cn

[R71] 日期格式化
来源：http://ww.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qh.nicolike.cn

[R72] 等待端口就绪
来源：http://ig.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jr.yuntaijiaju.cn

[R73] 分割大日志
来源：http://cb.9csxet.cn

split -l 1000 big.log part_
来源：http://ak.9csxet.cn

[R74] 批量重命名
来源：http://sb.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mp.gzmigu.cn

[R75] 导出环境变量
来源：http://dz.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://oj.shxzskj.cn

[R76] 使用临时文件
来源：http://hn.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xt.wgjwhj.cn

[R77] 读取用户输入
来源：http://gm.szsharing.cn

read -rp "请输入: " ans
来源：http://jf.wgjwhj.cn

[R78] 交互式菜单
来源：http://ah.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fv.shtwfgs.cn

[R79] 解析命令行选项
来源：http://ps.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ba.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://jd.yuntaijiaju.cn

time ./run.sh
来源：http://rx.nicolike.cn

================================================================================
来源：http://cw.huanxung.cn

S. C / C++ 专题
来源：http://vc.lnxyls.cn

================================================================================
来源：http://mt.haigaiapp.cn

[S01] C：Hello World
来源：http://mu.asd995.cn

#include <stdio.h>
来源：http://qc.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ew.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://qe.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://pj.muxihuayi.cn

[S03] C：读入整数
来源：http://jc.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://uy.shtwfgs.cn

[S04] C：字符串复制
来源：http://we.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gc.newstarts.cn

[S05] C：字符串长度
来源：http://sd.colortex.cn

strlen(s)
来源：http://oj.wgjwhj.cn

[S06] C：字符串比较
来源：http://hr.gzmigu.cn

strcmp(a, b) == 0
来源：http://bn.asd995.cn

[S07] C：数组遍历求和
来源：http://qi.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hx.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://sz.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://te.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://rg.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ex.shtwfgs.cn

[S10] C：指针与解引用
来源：http://yg.huanxung.cn

int *p = &a;  *p = 5;
来源：http://ok.bjjhwx.cn

[S11] C：逐行读文件
来源：http://ic.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://nr.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rl.wgjwhj.cn

fclose(f);
来源：http://wz.asd995.cn

[S12] C：写文件
来源：http://cz.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xx.newstarts.cn

[S13] C：宏定义
来源：http://hk.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yr.huixinmuqiang.cn

[S14] C：枚举
来源：http://ky.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://py.jianghongdianzi.cn

[S15] C：类型转换
来源：http://lz.nicolike.cn

(double) a / b
来源：http://sd.huanxung.cn

[S16] C：位操作置位
来源：http://hc.nicolike.cn

x |= (1 << 3);
来源：http://fw.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://gy.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oq.szxytkj.cn

[S18] C：命令行参数
来源：http://ht.colortex.cn

int main(int argc, char **argv)
来源：http://zj.shxzskj.cn

[S19] C：快速排序
来源：http://sx.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nf.wgjwhj.cn

[S20] C：二分查找
来源：http://ci.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jt.newstarts.cn

[S21] C：字符类别判断
来源：http://my.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uc.shxzukj.cn

[S22] C：字符串转数字
来源：http://ry.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rp.bookmarksfly.cn

[S23] C：随机数
来源：http://em.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rx.szsharing.cn

[S24] C：获取本地时间
来源：http://nb.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ip.asd995.cn

[S25] C：内存拷贝
来源：http://ke.jctech888.com.cn

memcpy(dst, src, n);
来源：http://ru.bookmarksfly.cn

[S26] C：内存清零
来源：http://ws.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://sd.colortex.cn

[S27] C：定义常量
来源：http://tl.wgjwhj.cn

const double PI = 3.14159;
来源：http://pm.chemitech.net.cn

[S28] C：静态变量
来源：http://ms.szxytkj.cn

static int counter = 0;
来源：http://uk.huixinmuqiang.cn

[S29] C：变参函数
来源：http://ef.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xf.szsharing.cn

[S30] C：头文件保护
来源：http://bb.wgjwhj.cn

#ifndef X_H
来源：http://ca.lnxyls.cn

#define X_H
来源：http://hd.nszjky.cn

#endif
来源：http://hm.shxzukj.cn

[S31] C++：Hello World
来源：http://an.yuntaijiaju.cn


<!-- 参考信息 -->