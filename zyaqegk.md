代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mr.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://ai.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dx.szxytkj.cn

[Q57] 行号
来源：http://bq.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zw.huixiangedu.cn

[Q58] 累计求和
来源：http://nl.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gn.gzmigu.cn

[Q59] 分组内累计
来源：http://mq.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ax.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://gj.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://db.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fj.huixiangedu.cn

[Q61] 移动平均
来源：http://mq.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cf.jctech888.com.cn

[Q62] 分组占比
来源：http://sq.shxzukj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://he.huanxung.cn

[Q63] 开启事务
来源：http://si.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ds.wgjwhj.cn

[Q64] 提交事务
来源：http://mz.shxzskj.cn

COMMIT;
来源：http://gg.wgjwhj.cn

[Q65] 回滚事务
来源：http://of.szsharing.cn

ROLLBACK;
来源：http://ss.bookmarksfly.cn

[Q66] 行锁查询
来源：http://kc.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ff.shxzskj.cn

[Q67] 设置隔离级别
来源：http://hc.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fw.yuntaijiaju.cn

[Q68] 保存点
来源：http://ig.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://lz.panjiajie.cn

ROLLBACK TO sp1;
来源：http://jp.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://nl.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cf.jctech888.com.cn

[Q70] 更新统计信息
来源：http://vd.9csxet.cn

ANALYZE TABLE users;
来源：http://ni.bjjhwx.cn

[Q71] 查看建表语句
来源：http://qd.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ww.bjjhwx.cn

[Q72] 查看索引
来源：http://mk.lnxyls.cn

SHOW INDEX FROM users;
来源：http://ed.muxihuayi.cn

[Q73] 查看表状态
来源：http://hq.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ht.bjjhwx.cn

[Q74] 强制使用索引
来源：http://bj.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nf.lnxyls.cn

[Q75] 日期格式化
来源：http://pi.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gy.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ar.chemitech.net.cn

[Q76] 按天统计
来源：http://yn.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oi.huixiangedu.cn

[Q77] 时间加减
来源：http://to.huanxung.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gv.panjiajie.cn

[Q78] 当前时间
来源：http://mi.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ne.haigaiapp.cn

[Q79] 字符串拼接
来源：http://ma.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://do.jianghongdianzi.cn

[Q80] 字符串截取
来源：http://rz.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gw.wgjwhj.cn

[Q81] 字符串替换
来源：http://yh.bookmarksfly.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cm.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://fg.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pn.shxzukj.cn

[Q83] 大小写转换
来源：http://tt.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gs.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://tp.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://mh.hnjuh.cn

[Q85] 数值取整
来源：http://nj.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mf.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://oy.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zm.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://xn.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fj.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://gp.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eq.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hy.shxzskj.cn

[Q89] 判断表是否存在
来源：http://jc.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dy.colortex.cn

[Q90] 生成序号列
来源：http://po.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ck.newstarts.cn

================================================================================
来源：http://fc.nicolike.cn

R. Bash 专题
来源：http://en.asd995.cn

================================================================================
来源：http://ze.colortex.cn

[R01] shebang 与严格模式
来源：http://ay.bjjhwx.cn

#!/usr/bin/env bash
来源：http://sh.newstarts.cn

set -euo pipefail
来源：http://ng.lnxyls.cn

[R02] 变量赋值与使用
来源：http://ic.szsharing.cn

name="Tom"; echo "$name"
来源：http://na.jctech888.com.cn

[R03] 只读变量
来源：http://xs.hahajie.cn

readonly PI=3.14
来源：http://tk.521024.cn

[R04] 位置参数
来源：http://ew.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://se.muxihuayi.cn

[R05] 参数默认值
来源：http://nz.521024.cn

name="${1:-default}"
来源：http://sv.nicolike.cn

[R06] 判断命令是否存在
来源：http://fg.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ht.bookmarksfly.cn

[R07] if 判断文件
来源：http://av.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zw.521024.cn

[R08] 数值比较
来源：http://xu.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vl.wgjwhj.cn

[R09] 字符串比较
来源：http://vg.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tj.haigaiapp.cn

[R10] 正则匹配
来源：http://fs.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hp.hahajie.cn

[R11] case 多分支
来源：http://ud.hahajie.cn

case "$1" in
来源：http://kf.haigaiapp.cn

start) echo "启动" ;;
来源：http://xa.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://pz.521024.cn

*)     echo "未知命令" ;;
来源：http://eg.hnjuh.cn

esac
来源：http://xs.lnxyls.cn

[R12] for 遍历文件
来源：http://pb.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://bx.haigaiapp.cn

[R13] for 计数循环
来源：http://zh.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://ym.huixinmuqiang.cn

[R14] C 风格 for
来源：http://gg.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ud.9csxet.cn

[R15] while 逐行读文件
来源：http://fo.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://or.bjjhwx.cn

[R16] until 等待条件
来源：http://eu.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xr.haigaiapp.cn

[R17] 数组定义与取值
来源：http://nu.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cc.nszjky.cn

[R18] 遍历数组
来源：http://pi.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ya.lnxyls.cn

[R19] 数组长度
来源：http://jh.muxihuayi.cn

echo "${#arr[@]}"
来源：http://ya.lnxyls.cn

[R20] 关联数组（字典）
来源：http://wf.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://es.szxytkj.cn

[R21] 字符串长度
来源：http://il.jianghongdianzi.cn

echo "${#s}"
来源：http://rc.wgjwhj.cn

[R22] 截取子串
来源：http://dz.lnxyls.cn

echo "${s:0:5}"
来源：http://mp.hnjuh.cn

[R23] 字符串替换
来源：http://qo.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zn.szxytkj.cn

[R24] 大小写转换
来源：http://nr.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://be.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://gh.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qm.hnjuh.cn

[R26] 命令替换
来源：http://ba.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://ji.panjiajie.cn

[R27] 算术展开
来源：http://ij.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://ke.hnjuh.cn

[R28] 浮点运算
来源：http://no.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://fw.szxytkj.cn

[R29] 定义函数
来源：http://cf.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mx.jctech888.com.cn

[R30] 函数返回状态码
来源：http://as.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://iy.shxzskj.cn

[R31] 局部变量
来源：http://yo.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://qr.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://xv.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aa.colortex.cn

[R33] 捕获错误并提示行号
来源：http://mq.bookmarksfly.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yz.panjiajie.cn

[R34] 退出时清理
来源：http://bn.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bp.9csxet.cn

[R35] 后台执行并等待
来源：http://tk.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fe.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://tk.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yp.szxytkj.cn

[R37] 把输出赋给变量
来源：http://ai.bookmarksfly.cn

files=$(ls -1)
来源：http://fu.wgjwhj.cn

[R38] 管道串联
来源：http://zi.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://pm.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://ib.nszjky.cn

cmd > out.log 2>&1
来源：http://ii.9csxet.cn

[R40] 追加写日志
来源：http://yp.shxzukj.cn

echo "log" >> out.log
来源：http://ev.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://xu.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://jt.bookmarksfly.cn

[R42] 输入重定向
来源：http://ic.nszjky.cn

wc -l < a.txt
来源：http://rw.shtwfgs.cn

[R43] 按名字查找文件
来源：http://ta.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://jo.huixiangedu.cn

[R44] 按修改时间查找
来源：http://wb.haigaiapp.cn

find . -mtime -7 -type f
来源：http://wl.szxytkj.cn

[R45] 批量删除
来源：http://rh.huanxung.cn

find . -name "*.tmp" -delete
来源：http://wi.shxzskj.cn

[R46] 递归替换文件内容
来源：http://ry.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://it.haigaiapp.cn

[R47] sed 单行替换
来源：http://ae.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cb.szsharing.cn

[R48] awk 取指定列
来源：http://cl.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://hy.chemitech.net.cn

[R49] awk 带条件
来源：http://sj.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wf.yuexingan06.cn

[R50] awk 求和
来源：http://tk.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vn.hahajie.cn

[R51] 排序去重取前几
来源：http://ob.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cg.muxihuayi.cn

[R52] 统计行数
来源：http://lh.hahajie.cn

wc -l a.txt
来源：http://zs.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://xm.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ll.lnxyls.cn

[R54] 比较两个文件
来源：http://oa.chemitech.net.cn

diff a.txt b.txt
来源：http://te.shtwfgs.cn

[R55] 压缩与解压
来源：http://od.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yt.wgjwhj.cn

[R56] 远程拷贝
来源：http://tj.muxihuayi.cn

scp file user@host:/path/
来源：http://ng.gzmigu.cn

[R57] 远程执行命令
来源：http://bb.bjjhwx.cn

ssh user@host 'uptime'
来源：http://cs.hahajie.cn

[R58] 下载文件
来源：http://rg.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gz.muxihuayi.cn

[R59] 发 POST JSON
来源：http://cm.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oc.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://qo.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sw.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://id.jianghongdianzi.cn

df -h;  du -sh *
来源：http://ep.colortex.cn

[R62] 找最占空间的文件
来源：http://mc.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://tj.muxihuayi.cn

[R63] 内存与进程
来源：http://aq.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://vc.521024.cn

[R64] 结束进程
来源：http://wo.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://ko.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://fh.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ys.gzmigu.cn

[R66] 定时任务
来源：http://kx.nicolike.cn

crontab -e;  crontab -l
来源：http://az.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://vx.chemitech.net.cn

openssl rand -hex 16
来源：http://dm.wgjwhj.cn

[R68] 计算文件校验值
来源：http://jc.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qu.hnjuh.cn

[R69] 生成随机密码
来源：http://nf.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://so.wgjwhj.cn

[R70] 时间戳与互转
来源：http://pg.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://af.yuexingan06.cn

[R71] 日期格式化
来源：http://nx.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://av.shxzukj.cn

[R72] 等待端口就绪
来源：http://mx.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ii.shtwfgs.cn

[R73] 分割大日志
来源：http://wy.bjjhwx.cn

split -l 1000 big.log part_
来源：http://gr.gzmigu.cn

[R74] 批量重命名
来源：http://cs.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ly.szsharing.cn

[R75] 导出环境变量
来源：http://qx.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://xw.yuexingan06.cn

[R76] 使用临时文件
来源：http://un.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cd.panjiajie.cn

[R77] 读取用户输入
来源：http://oa.bjjhwx.cn

read -rp "请输入: " ans
来源：http://lq.newstarts.cn

[R78] 交互式菜单
来源：http://yi.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vd.colortex.cn

[R79] 解析命令行选项
来源：http://ph.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fn.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://ld.asd995.cn

time ./run.sh
来源：http://kg.jctech888.com.cn

================================================================================
来源：http://oy.huanxung.cn

S. C / C++ 专题
来源：http://ri.colortex.cn

================================================================================
来源：http://lj.shxzukj.cn

[S01] C：Hello World
来源：http://ss.hnjuh.cn

#include <stdio.h>
来源：http://av.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pu.nszjky.cn

[S02] C：变量与格式化输出
来源：http://ru.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://fm.panjiajie.cn

[S03] C：读入整数
来源：http://ed.newstarts.cn

int x; scanf("%d", &x);
来源：http://ri.521024.cn

[S04] C：字符串复制
来源：http://lt.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ea.panjiajie.cn

[S05] C：字符串长度
来源：http://jr.9csxet.cn

strlen(s)
来源：http://tq.muxihuayi.cn

[S06] C：字符串比较
来源：http://bp.panjiajie.cn

strcmp(a, b) == 0
来源：http://wu.newstarts.cn

[S07] C：数组遍历求和
来源：http://ix.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ne.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://vv.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bo.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://oc.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jm.newstarts.cn

[S10] C：指针与解引用
来源：http://rt.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://gv.yuexingan06.cn

[S11] C：逐行读文件
来源：http://oy.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://oh.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qe.jctech888.com.cn

fclose(f);
来源：http://yx.newstarts.cn

[S12] C：写文件
来源：http://qc.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lp.colortex.cn

[S13] C：宏定义
来源：http://gf.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ah.szsharing.cn

[S14] C：枚举
来源：http://lt.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://lz.nicolike.cn

[S15] C：类型转换
来源：http://io.panjiajie.cn

(double) a / b
来源：http://al.szsharing.cn

[S16] C：位操作置位
来源：http://lv.hahajie.cn

x |= (1 << 3);
来源：http://dp.szsharing.cn

[S17] C：安全拼接字符串
来源：http://tx.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dy.jctech888.com.cn

[S18] C：命令行参数
来源：http://dc.hahajie.cn

int main(int argc, char **argv)
来源：http://fb.521024.cn

[S19] C：快速排序
来源：http://uw.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ik.gzmigu.cn

[S20] C：二分查找
来源：http://iv.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gi.shxzukj.cn

[S21] C：字符类别判断
来源：http://nz.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lf.9csxet.cn

[S22] C：字符串转数字
来源：http://il.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ow.huixiangedu.cn

[S23] C：随机数
来源：http://px.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gp.shxzukj.cn

[S24] C：获取本地时间
来源：http://zy.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vn.muxihuayi.cn

[S25] C：内存拷贝
来源：http://mv.hnjuh.cn

memcpy(dst, src, n);
来源：http://hl.hahajie.cn

[S26] C：内存清零
来源：http://te.nszjky.cn


<!-- 参考信息 -->