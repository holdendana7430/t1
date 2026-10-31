代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rj.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://ul.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xu.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fl.wgjwhj.cn

[Q61] 移动平均
来源：http://ww.hnjuh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dl.hnjuh.cn

[Q62] 分组占比
来源：http://cr.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dq.hnjuh.cn

[Q63] 开启事务
来源：http://py.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mj.panjiajie.cn

[Q64] 提交事务
来源：http://fi.haigaiapp.cn

COMMIT;
来源：http://kv.shxzukj.cn

[Q65] 回滚事务
来源：http://je.szsharing.cn

ROLLBACK;
来源：http://fl.shtwfgs.cn

[Q66] 行锁查询
来源：http://gp.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bk.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://zq.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://df.9csxet.cn

[Q68] 保存点
来源：http://ds.wgjwhj.cn

SAVEPOINT sp1;
来源：http://uw.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://yj.hnjuh.cn

[Q69] 查看执行计划
来源：http://ll.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pl.lnxyls.cn

[Q70] 更新统计信息
来源：http://ta.hnjuh.cn

ANALYZE TABLE users;
来源：http://xr.panjiajie.cn

[Q71] 查看建表语句
来源：http://vi.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wb.huixiangedu.cn

[Q72] 查看索引
来源：http://ig.hnjuh.cn

SHOW INDEX FROM users;
来源：http://fl.gzmigu.cn

[Q73] 查看表状态
来源：http://uj.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ck.szsharing.cn

[Q74] 强制使用索引
来源：http://kk.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rh.chemitech.net.cn

[Q75] 日期格式化
来源：http://sj.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rl.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kw.panjiajie.cn

[Q76] 按天统计
来源：http://ly.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uk.bjjhwx.cn

[Q77] 时间加减
来源：http://ig.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vh.yuexingan06.cn

[Q78] 当前时间
来源：http://ml.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lj.huixiangedu.cn

[Q79] 字符串拼接
来源：http://ep.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rr.yuexingan06.cn

[Q80] 字符串截取
来源：http://rx.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jp.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://mz.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pw.colortex.cn

[Q82] 字符长度与字节长度
来源：http://lf.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://on.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://rm.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xs.shxzukj.cn

[Q84] 去除首尾空格
来源：http://on.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://el.jianghongdianzi.cn

[Q85] 数值取整
来源：http://ha.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ol.colortex.cn

[Q86] 读取 JSON 字段
来源：http://wb.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hg.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://we.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kd.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://wn.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sp.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lz.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://ml.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lw.hahajie.cn

[Q90] 生成序号列
来源：http://so.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fa.521024.cn

================================================================================
来源：http://eg.hahajie.cn

R. Bash 专题
来源：http://tg.521024.cn

================================================================================
来源：http://nl.panjiajie.cn

[R01] shebang 与严格模式
来源：http://tu.hahajie.cn

#!/usr/bin/env bash
来源：http://dy.asd995.cn

set -euo pipefail
来源：http://jz.521024.cn

[R02] 变量赋值与使用
来源：http://cb.hnjuh.cn

name="Tom"; echo "$name"
来源：http://ss.shxzskj.cn

[R03] 只读变量
来源：http://md.szxytkj.cn

readonly PI=3.14
来源：http://pc.wgjwhj.cn

[R04] 位置参数
来源：http://xs.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qe.yuexingan06.cn

[R05] 参数默认值
来源：http://ov.nicolike.cn

name="${1:-default}"
来源：http://xd.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://af.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lv.9csxet.cn

[R07] if 判断文件
来源：http://xw.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sv.huixiangedu.cn

[R08] 数值比较
来源：http://gv.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vn.lnxyls.cn

[R09] 字符串比较
来源：http://lj.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rv.yuntaijiaju.cn

[R10] 正则匹配
来源：http://aa.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ju.huixinmuqiang.cn

[R11] case 多分支
来源：http://rm.bjjhwx.cn

case "$1" in
来源：http://hf.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://ch.521024.cn

stop)  echo "停止" ;;
来源：http://qa.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://pm.colortex.cn

esac
来源：http://tw.shxzukj.cn

[R12] for 遍历文件
来源：http://sw.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://tz.gzmigu.cn

[R13] for 计数循环
来源：http://cc.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://ab.hnjuh.cn

[R14] C 风格 for
来源：http://aq.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pq.521024.cn

[R15] while 逐行读文件
来源：http://sv.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jj.haigaiapp.cn

[R16] until 等待条件
来源：http://mf.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ej.9csxet.cn

[R17] 数组定义与取值
来源：http://oy.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jv.jianghongdianzi.cn

[R18] 遍历数组
来源：http://cz.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jk.muxihuayi.cn

[R19] 数组长度
来源：http://zf.huixiangedu.cn

echo "${#arr[@]}"
来源：http://yp.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://ch.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hd.shtwfgs.cn

[R21] 字符串长度
来源：http://qb.shtwfgs.cn

echo "${#s}"
来源：http://wp.wgjwhj.cn

[R22] 截取子串
来源：http://is.jctech888.com.cn

echo "${s:0:5}"
来源：http://sr.hahajie.cn

[R23] 字符串替换
来源：http://jp.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tu.newstarts.cn

[R24] 大小写转换
来源：http://yb.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fy.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://yy.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://la.nicolike.cn

[R26] 命令替换
来源：http://yo.haigaiapp.cn

now=$(date +%F); echo "$now"
来源：http://ik.bjjhwx.cn

[R27] 算术展开
来源：http://vx.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://zk.shxzskj.cn

[R28] 浮点运算
来源：http://jt.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://vf.huixinmuqiang.cn

[R29] 定义函数
来源：http://tx.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oc.panjiajie.cn

[R30] 函数返回状态码
来源：http://ox.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://fo.chemitech.net.cn

[R31] 局部变量
来源：http://qo.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://hr.asd995.cn

[R32] 参数个数校验
来源：http://dc.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ht.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://dk.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iz.jianghongdianzi.cn

[R34] 退出时清理
来源：http://qq.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mv.huixiangedu.cn

[R35] 后台执行并等待
来源：http://av.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ty.szxytkj.cn

[R36] 并发执行多个任务
来源：http://ld.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cy.nicolike.cn

[R37] 把输出赋给变量
来源：http://vy.szxytkj.cn

files=$(ls -1)
来源：http://rm.521024.cn

[R38] 管道串联
来源：http://an.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://mu.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://tw.lnxyls.cn

cmd > out.log 2>&1
来源：http://rh.shxzukj.cn

[R40] 追加写日志
来源：http://rv.wgjwhj.cn

echo "log" >> out.log
来源：http://xg.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://xj.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://xe.huanxung.cn

[R42] 输入重定向
来源：http://ao.huixinmuqiang.cn

wc -l < a.txt
来源：http://hc.hnjuh.cn

[R43] 按名字查找文件
来源：http://mv.nszjky.cn

find . -name "*.log" -type f
来源：http://ie.521024.cn

[R44] 按修改时间查找
来源：http://fq.huixiangedu.cn

find . -mtime -7 -type f
来源：http://fh.shxzukj.cn

[R45] 批量删除
来源：http://by.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://os.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://mn.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iz.colortex.cn

[R47] sed 单行替换
来源：http://hn.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vh.newstarts.cn

[R48] awk 取指定列
来源：http://fr.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://pc.newstarts.cn

[R49] awk 带条件
来源：http://lh.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nv.panjiajie.cn

[R50] awk 求和
来源：http://xd.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://su.jctech888.com.cn

[R51] 排序去重取前几
来源：http://kv.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tu.shxzskj.cn

[R52] 统计行数
来源：http://zg.colortex.cn

wc -l a.txt
来源：http://pg.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://wh.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tq.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://yb.panjiajie.cn

diff a.txt b.txt
来源：http://ao.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://ez.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wg.muxihuayi.cn

[R56] 远程拷贝
来源：http://ct.521024.cn

scp file user@host:/path/
来源：http://tn.yuexingan06.cn

[R57] 远程执行命令
来源：http://hu.muxihuayi.cn

ssh user@host 'uptime'
来源：http://ct.9csxet.cn

[R58] 下载文件
来源：http://vf.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lk.huanxung.cn

[R59] 发 POST JSON
来源：http://rn.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://in.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://sj.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://af.gzmigu.cn

[R61] 磁盘占用
来源：http://bn.chemitech.net.cn

df -h;  du -sh *
来源：http://qa.asd995.cn

[R62] 找最占空间的文件
来源：http://mc.colortex.cn

du -ah . | sort -rh | head -10
来源：http://ly.muxihuayi.cn

[R63] 内存与进程
来源：http://kx.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://sw.huixinmuqiang.cn

[R64] 结束进程
来源：http://df.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://gf.9csxet.cn

[R65] 查看端口占用
来源：http://tx.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nv.jianghongdianzi.cn

[R66] 定时任务
来源：http://vk.hnjuh.cn

crontab -e;  crontab -l
来源：http://on.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://si.newstarts.cn

openssl rand -hex 16
来源：http://cy.huanxung.cn

[R68] 计算文件校验值
来源：http://jp.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dv.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://vq.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://gs.szsharing.cn

[R70] 时间戳与互转
来源：http://qg.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://ui.jianghongdianzi.cn

[R71] 日期格式化
来源：http://vd.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mk.huixiangedu.cn

[R72] 等待端口就绪
来源：http://qn.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ur.lnxyls.cn

[R73] 分割大日志
来源：http://wz.szsharing.cn

split -l 1000 big.log part_
来源：http://rt.bookmarksfly.cn

[R74] 批量重命名
来源：http://wx.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eq.521024.cn

[R75] 导出环境变量
来源：http://ms.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://fo.huixiangedu.cn

[R76] 使用临时文件
来源：http://ej.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lm.bjjhwx.cn

[R77] 读取用户输入
来源：http://ss.panjiajie.cn

read -rp "请输入: " ans
来源：http://pt.shtwfgs.cn

[R78] 交互式菜单
来源：http://td.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pk.yuexingan06.cn

[R79] 解析命令行选项
来源：http://zk.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dr.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://ur.haigaiapp.cn

time ./run.sh
来源：http://dx.bjjhwx.cn

================================================================================
来源：http://ph.panjiajie.cn

S. C / C++ 专题
来源：http://mt.bookmarksfly.cn

================================================================================
来源：http://ak.yuntaijiaju.cn

[S01] C：Hello World
来源：http://wf.jctech888.com.cn

#include <stdio.h>
来源：http://lu.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ri.521024.cn

[S02] C：变量与格式化输出
来源：http://si.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://sm.521024.cn

[S03] C：读入整数
来源：http://oz.nszjky.cn

int x; scanf("%d", &x);
来源：http://za.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://nj.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jt.shtwfgs.cn

[S05] C：字符串长度
来源：http://am.asd995.cn

strlen(s)
来源：http://ar.shxzskj.cn

[S06] C：字符串比较
来源：http://nz.521024.cn

strcmp(a, b) == 0
来源：http://ne.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://gj.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yf.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://cy.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pq.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://xr.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ca.szxytkj.cn

[S10] C：指针与解引用
来源：http://yj.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://rz.huanxung.cn

[S11] C：逐行读文件
来源：http://he.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://ze.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mh.wgjwhj.cn

fclose(f);
来源：http://vf.newstarts.cn

[S12] C：写文件
来源：http://oh.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xt.wgjwhj.cn

[S13] C：宏定义
来源：http://zo.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ht.hnjuh.cn

[S14] C：枚举
来源：http://wg.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://hx.szsharing.cn

[S15] C：类型转换
来源：http://wp.hnjuh.cn

(double) a / b
来源：http://yo.asd995.cn

[S16] C：位操作置位
来源：http://jh.newstarts.cn

x |= (1 << 3);
来源：http://ya.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://zy.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dw.chemitech.net.cn

[S18] C：命令行参数
来源：http://jj.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://ug.9csxet.cn

[S19] C：快速排序
来源：http://yi.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wc.wgjwhj.cn

[S20] C：二分查找
来源：http://rv.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fi.9csxet.cn

[S21] C：字符类别判断
来源：http://it.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mj.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://eu.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pn.haigaiapp.cn

[S23] C：随机数
来源：http://fk.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://la.chemitech.net.cn

[S24] C：获取本地时间
来源：http://dp.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cq.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://vb.szsharing.cn

memcpy(dst, src, n);
来源：http://hn.yuexingan06.cn

[S26] C：内存清零
来源：http://re.9csxet.cn

memset(a, 0, sizeof a);
来源：http://um.lnxyls.cn

[S27] C：定义常量
来源：http://nt.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://kq.huanxung.cn

[S28] C：静态变量
来源：http://sf.shxzukj.cn

static int counter = 0;
来源：http://dv.hnjuh.cn

[S29] C：变参函数
来源：http://tj.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ik.shxzskj.cn

[S30] C：头文件保护
来源：http://nn.9csxet.cn


<!-- 参考信息 -->