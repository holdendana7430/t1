代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cq.9csxet.cn

[Q52] 删除指定行
来源：http://me.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://am.huanxung.cn

[Q53] 按条件删除
来源：http://mc.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eu.bjjhwx.cn

[Q54] 清空表
来源：http://nz.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://vz.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://df.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ax.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://xb.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vs.huanxung.cn

[Q57] 行号
来源：http://hv.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vp.nicolike.cn

[Q58] 累计求和
来源：http://ze.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dp.shxzskj.cn

[Q59] 分组内累计
来源：http://oi.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jz.bookmarksfly.cn

[Q60] 取上一行 / 下一行
来源：http://tr.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cl.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tf.asd995.cn

[Q61] 移动平均
来源：http://dj.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ee.haigaiapp.cn

[Q62] 分组占比
来源：http://cb.shtwfgs.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://op.bjjhwx.cn

[Q63] 开启事务
来源：http://ec.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ia.jianghongdianzi.cn

[Q64] 提交事务
来源：http://ng.szsharing.cn

COMMIT;
来源：http://kv.newstarts.cn

[Q65] 回滚事务
来源：http://vl.colortex.cn

ROLLBACK;
来源：http://ck.bjjhwx.cn

[Q66] 行锁查询
来源：http://op.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ni.gzmigu.cn

[Q67] 设置隔离级别
来源：http://zp.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ro.bookmarksfly.cn

[Q68] 保存点
来源：http://ok.521024.cn

SAVEPOINT sp1;
来源：http://zd.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://lj.yuexingan06.cn

[Q69] 查看执行计划
来源：http://sq.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wg.gzmigu.cn

[Q70] 更新统计信息
来源：http://zz.colortex.cn

ANALYZE TABLE users;
来源：http://pr.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://uw.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zs.wgjwhj.cn

[Q72] 查看索引
来源：http://dm.haigaiapp.cn

SHOW INDEX FROM users;
来源：http://cf.chemitech.net.cn

[Q73] 查看表状态
来源：http://nq.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zh.asd995.cn

[Q74] 强制使用索引
来源：http://kh.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zo.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://fd.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://va.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qw.lnxyls.cn

[Q76] 按天统计
来源：http://wl.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nn.wgjwhj.cn

[Q77] 时间加减
来源：http://dx.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nk.shxzskj.cn

[Q78] 当前时间
来源：http://wr.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wt.newstarts.cn

[Q79] 字符串拼接
来源：http://wt.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tm.shxzskj.cn

[Q80] 字符串截取
来源：http://gj.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cb.szsharing.cn

[Q81] 字符串替换
来源：http://jl.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cf.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://ga.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eb.nszjky.cn

[Q83] 大小写转换
来源：http://wg.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dg.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://pw.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://hi.colortex.cn

[Q85] 数值取整
来源：http://bu.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zj.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://zm.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zv.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://mq.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fm.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://ls.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lv.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ip.newstarts.cn

[Q89] 判断表是否存在
来源：http://vr.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tk.muxihuayi.cn

[Q90] 生成序号列
来源：http://fo.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://in.bjjhwx.cn

================================================================================
来源：http://zu.colortex.cn

R. Bash 专题
来源：http://ol.bookmarksfly.cn

================================================================================
来源：http://ww.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://od.panjiajie.cn

#!/usr/bin/env bash
来源：http://dx.bjjhwx.cn

set -euo pipefail
来源：http://ve.gzmigu.cn

[R02] 变量赋值与使用
来源：http://gg.lnxyls.cn

name="Tom"; echo "$name"
来源：http://kz.shtwfgs.cn

[R03] 只读变量
来源：http://ui.shxzukj.cn

readonly PI=3.14
来源：http://pq.gzmigu.cn

[R04] 位置参数
来源：http://tp.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nn.yuexingan06.cn

[R05] 参数默认值
来源：http://jc.hahajie.cn

name="${1:-default}"
来源：http://ui.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://ga.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qq.newstarts.cn

[R07] if 判断文件
来源：http://yn.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vw.gzmigu.cn

[R08] 数值比较
来源：http://kf.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rm.huixiangedu.cn

[R09] 字符串比较
来源：http://th.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ox.muxihuayi.cn

[R10] 正则匹配
来源：http://ci.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lz.shtwfgs.cn

[R11] case 多分支
来源：http://un.bookmarksfly.cn

case "$1" in
来源：http://do.yuexingan06.cn

start) echo "启动" ;;
来源：http://hu.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://uh.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://ua.panjiajie.cn

esac
来源：http://mb.hnjuh.cn

[R12] for 遍历文件
来源：http://ux.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://qp.huixiangedu.cn

[R13] for 计数循环
来源：http://da.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://qc.bjjhwx.cn

[R14] C 风格 for
来源：http://fz.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tk.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://an.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://al.wgjwhj.cn

[R16] until 等待条件
来源：http://cz.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vu.colortex.cn

[R17] 数组定义与取值
来源：http://jk.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://de.hnjuh.cn

[R18] 遍历数组
来源：http://zx.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mv.shxzukj.cn

[R19] 数组长度
来源：http://sj.521024.cn

echo "${#arr[@]}"
来源：http://pi.nicolike.cn

[R20] 关联数组（字典）
来源：http://xb.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://py.chemitech.net.cn

[R21] 字符串长度
来源：http://rd.lnxyls.cn

echo "${#s}"
来源：http://sa.chemitech.net.cn

[R22] 截取子串
来源：http://ht.newstarts.cn

echo "${s:0:5}"
来源：http://pe.huanxung.cn

[R23] 字符串替换
来源：http://vj.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qr.szxytkj.cn

[R24] 大小写转换
来源：http://ha.colortex.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jy.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://ay.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://df.gzmigu.cn

[R26] 命令替换
来源：http://va.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://eg.szxytkj.cn

[R27] 算术展开
来源：http://an.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://hf.hahajie.cn

[R28] 浮点运算
来源：http://vo.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://gc.huixiangedu.cn

[R29] 定义函数
来源：http://bk.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lq.shxzukj.cn

[R30] 函数返回状态码
来源：http://cw.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://sl.haigaiapp.cn

[R31] 局部变量
来源：http://ii.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://yw.shxzukj.cn

[R32] 参数个数校验
来源：http://qk.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aa.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://ve.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wt.haigaiapp.cn

[R34] 退出时清理
来源：http://vj.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vr.shxzukj.cn

[R35] 后台执行并等待
来源：http://uj.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ki.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://ph.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zh.shxzukj.cn

[R37] 把输出赋给变量
来源：http://nk.521024.cn

files=$(ls -1)
来源：http://kz.yuntaijiaju.cn

[R38] 管道串联
来源：http://ew.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://on.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://pp.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://vo.521024.cn

[R40] 追加写日志
来源：http://uy.wgjwhj.cn

echo "log" >> out.log
来源：http://ud.lnxyls.cn

[R41] 丢弃输出
来源：http://vu.huanxung.cn

cmd >/dev/null 2>&1
来源：http://vf.gzmigu.cn

[R42] 输入重定向
来源：http://qd.szsharing.cn

wc -l < a.txt
来源：http://xp.asd995.cn

[R43] 按名字查找文件
来源：http://if.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://fy.huanxung.cn

[R44] 按修改时间查找
来源：http://ph.asd995.cn

find . -mtime -7 -type f
来源：http://us.yuntaijiaju.cn

[R45] 批量删除
来源：http://ya.colortex.cn

find . -name "*.tmp" -delete
来源：http://ti.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://ok.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mb.shxzskj.cn

[R47] sed 单行替换
来源：http://la.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wr.chemitech.net.cn

[R48] awk 取指定列
来源：http://ue.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://fh.gzmigu.cn

[R49] awk 带条件
来源：http://vp.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rn.shxzskj.cn

[R50] awk 求和
来源：http://ea.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bd.chemitech.net.cn

[R51] 排序去重取前几
来源：http://kl.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vy.yuexingan06.cn

[R52] 统计行数
来源：http://zc.gzmigu.cn

wc -l a.txt
来源：http://ae.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://qm.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wc.panjiajie.cn

[R54] 比较两个文件
来源：http://sn.wgjwhj.cn

diff a.txt b.txt
来源：http://mo.wgjwhj.cn

[R55] 压缩与解压
来源：http://fe.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yy.colortex.cn

[R56] 远程拷贝
来源：http://zr.muxihuayi.cn

scp file user@host:/path/
来源：http://ow.9csxet.cn

[R57] 远程执行命令
来源：http://ti.lnxyls.cn

ssh user@host 'uptime'
来源：http://ce.lnxyls.cn

[R58] 下载文件
来源：http://tc.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xa.gzmigu.cn

[R59] 发 POST JSON
来源：http://rr.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fd.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://no.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vw.bookmarksfly.cn

[R61] 磁盘占用
来源：http://vf.wgjwhj.cn

df -h;  du -sh *
来源：http://ee.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://oj.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://jb.bookmarksfly.cn

[R63] 内存与进程
来源：http://pt.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://yh.jianghongdianzi.cn

[R64] 结束进程
来源：http://yr.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://jl.haigaiapp.cn

[R65] 查看端口占用
来源：http://rp.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mz.jianghongdianzi.cn

[R66] 定时任务
来源：http://pd.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://bc.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://li.colortex.cn

openssl rand -hex 16
来源：http://mo.szsharing.cn

[R68] 计算文件校验值
来源：http://lz.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qp.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://bv.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://zp.szsharing.cn

[R70] 时间戳与互转
来源：http://bj.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://pq.szxytkj.cn

[R71] 日期格式化
来源：http://ha.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uk.gzmigu.cn

[R72] 等待端口就绪
来源：http://mx.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dz.asd995.cn

[R73] 分割大日志
来源：http://zz.521024.cn

split -l 1000 big.log part_
来源：http://tn.lnxyls.cn

[R74] 批量重命名
来源：http://rv.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xe.colortex.cn

[R75] 导出环境变量
来源：http://qs.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://ge.9csxet.cn

[R76] 使用临时文件
来源：http://af.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hi.jctech888.com.cn

[R77] 读取用户输入
来源：http://fc.gzmigu.cn

read -rp "请输入: " ans
来源：http://oz.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://zc.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pe.newstarts.cn

[R79] 解析命令行选项
来源：http://zm.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cq.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://xu.muxihuayi.cn

time ./run.sh
来源：http://ls.asd995.cn

================================================================================
来源：http://ks.shtwfgs.cn

S. C / C++ 专题
来源：http://ov.colortex.cn

================================================================================
来源：http://gy.shxzukj.cn

[S01] C：Hello World
来源：http://fa.shtwfgs.cn

#include <stdio.h>
来源：http://jk.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mz.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://is.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://mn.gzmigu.cn

[S03] C：读入整数
来源：http://vs.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://et.9csxet.cn

[S04] C：字符串复制
来源：http://av.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gw.9csxet.cn

[S05] C：字符串长度
来源：http://kb.jctech888.com.cn

strlen(s)
来源：http://oe.gzmigu.cn

[S06] C：字符串比较
来源：http://jz.huanxung.cn

strcmp(a, b) == 0
来源：http://zv.hahajie.cn

[S07] C：数组遍历求和
来源：http://tz.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uq.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://kp.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hv.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://ag.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nl.newstarts.cn

[S10] C：指针与解引用
来源：http://yv.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://qv.haigaiapp.cn

[S11] C：逐行读文件
来源：http://sf.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://bq.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ho.shxzskj.cn

fclose(f);
来源：http://qu.szsharing.cn

[S12] C：写文件
来源：http://ka.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zi.chemitech.net.cn

[S13] C：宏定义
来源：http://rt.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://de.szsharing.cn

[S14] C：枚举
来源：http://zu.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://bb.jianghongdianzi.cn

[S15] C：类型转换
来源：http://yt.521024.cn

(double) a / b
来源：http://ha.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://jr.haigaiapp.cn

x |= (1 << 3);
来源：http://gf.newstarts.cn

[S17] C：安全拼接字符串
来源：http://vp.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bp.9csxet.cn

[S18] C：命令行参数
来源：http://ck.muxihuayi.cn

int main(int argc, char **argv)
来源：http://ds.shxzskj.cn

[S19] C：快速排序
来源：http://xx.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uu.jianghongdianzi.cn

[S20] C：二分查找
来源：http://ro.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bg.shxzukj.cn

[S21] C：字符类别判断
来源：http://cf.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wy.shtwfgs.cn

[S22] C：字符串转数字
来源：http://dr.nszjky.cn


<!-- 参考信息 -->