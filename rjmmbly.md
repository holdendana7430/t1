代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tc.huanxung.cn

[Q50] 批量更新
来源：http://hp.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tk.nszjky.cn

[Q51] 用子查询更新
来源：http://sc.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xc.shtwfgs.cn

[Q52] 删除指定行
来源：http://mp.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://fb.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://nv.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ir.panjiajie.cn

[Q54] 清空表
来源：http://ao.szsharing.cn

TRUNCATE TABLE logs;
来源：http://ey.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://ht.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tn.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://nc.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ks.chemitech.net.cn

[Q57] 行号
来源：http://js.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://un.jctech888.com.cn

[Q58] 累计求和
来源：http://wr.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sp.nszjky.cn

[Q59] 分组内累计
来源：http://vp.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wl.jianghongdianzi.cn

[Q60] 取上一行 / 下一行
来源：http://sw.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pt.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tf.szxytkj.cn

[Q61] 移动平均
来源：http://da.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ri.yuexingan06.cn

[Q62] 分组占比
来源：http://kf.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kd.lnxyls.cn

[Q63] 开启事务
来源：http://tc.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://om.wgjwhj.cn

[Q64] 提交事务
来源：http://td.hahajie.cn

COMMIT;
来源：http://iu.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://aq.muxihuayi.cn

ROLLBACK;
来源：http://qj.gzmigu.cn

[Q66] 行锁查询
来源：http://wd.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wb.gzmigu.cn

[Q67] 设置隔离级别
来源：http://vb.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rw.colortex.cn

[Q68] 保存点
来源：http://wi.muxihuayi.cn

SAVEPOINT sp1;
来源：http://wd.shxzukj.cn

ROLLBACK TO sp1;
来源：http://oh.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://lq.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zo.gzmigu.cn

[Q70] 更新统计信息
来源：http://lv.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://so.jctech888.com.cn

[Q71] 查看建表语句
来源：http://ld.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mr.szxytkj.cn

[Q72] 查看索引
来源：http://tz.asd995.cn

SHOW INDEX FROM users;
来源：http://ak.wgjwhj.cn

[Q73] 查看表状态
来源：http://dw.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wo.hahajie.cn

[Q74] 强制使用索引
来源：http://qc.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nl.asd995.cn

[Q75] 日期格式化
来源：http://ze.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wn.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ek.shxzukj.cn

[Q76] 按天统计
来源：http://qz.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ua.yuntaijiaju.cn

[Q77] 时间加减
来源：http://ea.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://df.jianghongdianzi.cn

[Q78] 当前时间
来源：http://aw.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bh.szxytkj.cn

[Q79] 字符串拼接
来源：http://xw.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nv.nszjky.cn

[Q80] 字符串截取
来源：http://pu.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://od.szxytkj.cn

[Q81] 字符串替换
来源：http://ht.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zc.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://oj.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hi.bjjhwx.cn

[Q83] 大小写转换
来源：http://wm.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oq.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://kg.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://nk.nszjky.cn

[Q85] 数值取整
来源：http://gt.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jt.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://wa.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cj.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://dm.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zl.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://jd.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hl.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bh.hnjuh.cn

[Q89] 判断表是否存在
来源：http://eo.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://js.nicolike.cn

[Q90] 生成序号列
来源：http://ax.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jd.asd995.cn

================================================================================
来源：http://cw.chemitech.net.cn

R. Bash 专题
来源：http://mp.9csxet.cn

================================================================================
来源：http://ij.shxzukj.cn

[R01] shebang 与严格模式
来源：http://mf.newstarts.cn

#!/usr/bin/env bash
来源：http://ta.asd995.cn

set -euo pipefail
来源：http://jk.colortex.cn

[R02] 变量赋值与使用
来源：http://nl.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://rz.nszjky.cn

[R03] 只读变量
来源：http://ba.bookmarksfly.cn

readonly PI=3.14
来源：http://uw.wgjwhj.cn

[R04] 位置参数
来源：http://et.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cx.yuexingan06.cn

[R05] 参数默认值
来源：http://nk.lnxyls.cn

name="${1:-default}"
来源：http://zk.shxzukj.cn

[R06] 判断命令是否存在
来源：http://ru.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bd.wgjwhj.cn

[R07] if 判断文件
来源：http://lg.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://my.bookmarksfly.cn

[R08] 数值比较
来源：http://el.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cc.521024.cn

[R09] 字符串比较
来源：http://ep.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sl.huixiangedu.cn

[R10] 正则匹配
来源：http://lb.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://my.muxihuayi.cn

[R11] case 多分支
来源：http://gd.jctech888.com.cn

case "$1" in
来源：http://ma.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://fr.521024.cn

stop)  echo "停止" ;;
来源：http://ky.huanxung.cn

*)     echo "未知命令" ;;
来源：http://sp.asd995.cn

esac
来源：http://dc.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://ko.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://kv.asd995.cn

[R13] for 计数循环
来源：http://ho.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://mf.newstarts.cn

[R14] C 风格 for
来源：http://ip.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zi.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://sw.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yx.huixiangedu.cn

[R16] until 等待条件
来源：http://ix.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sq.yuexingan06.cn

[R17] 数组定义与取值
来源：http://ia.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ts.huanxung.cn

[R18] 遍历数组
来源：http://ie.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hp.muxihuayi.cn

[R19] 数组长度
来源：http://xm.jctech888.com.cn

echo "${#arr[@]}"
来源：http://wq.asd995.cn

[R20] 关联数组（字典）
来源：http://ts.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xw.nicolike.cn

[R21] 字符串长度
来源：http://lw.jianghongdianzi.cn

echo "${#s}"
来源：http://fw.huanxung.cn

[R22] 截取子串
来源：http://bp.newstarts.cn

echo "${s:0:5}"
来源：http://li.shtwfgs.cn

[R23] 字符串替换
来源：http://no.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ck.asd995.cn

[R24] 大小写转换
来源：http://lk.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ui.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://dq.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ms.9csxet.cn

[R26] 命令替换
来源：http://xk.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://dj.haigaiapp.cn

[R27] 算术展开
来源：http://cc.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://fw.shxzukj.cn

[R28] 浮点运算
来源：http://ya.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://et.shtwfgs.cn

[R29] 定义函数
来源：http://tr.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jb.jctech888.com.cn

[R30] 函数返回状态码
来源：http://ly.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://gd.huixiangedu.cn

[R31] 局部变量
来源：http://rd.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://ge.lnxyls.cn

[R32] 参数个数校验
来源：http://us.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ij.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://xb.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wk.szxytkj.cn

[R34] 退出时清理
来源：http://ua.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sc.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://uz.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lt.asd995.cn

[R36] 并发执行多个任务
来源：http://eu.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gv.lnxyls.cn

[R37] 把输出赋给变量
来源：http://cr.colortex.cn

files=$(ls -1)
来源：http://kc.hnjuh.cn

[R38] 管道串联
来源：http://yp.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://fh.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://iv.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://ny.bookmarksfly.cn

[R40] 追加写日志
来源：http://do.panjiajie.cn

echo "log" >> out.log
来源：http://vm.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://qr.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://qq.szxytkj.cn

[R42] 输入重定向
来源：http://un.bookmarksfly.cn

wc -l < a.txt
来源：http://tc.bjjhwx.cn

[R43] 按名字查找文件
来源：http://ds.gzmigu.cn

find . -name "*.log" -type f
来源：http://bl.bjjhwx.cn

[R44] 按修改时间查找
来源：http://zq.haigaiapp.cn

find . -mtime -7 -type f
来源：http://rr.chemitech.net.cn

[R45] 批量删除
来源：http://fp.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://mv.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://cu.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bn.colortex.cn

[R47] sed 单行替换
来源：http://rf.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wq.wgjwhj.cn

[R48] awk 取指定列
来源：http://yo.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://sh.muxihuayi.cn

[R49] awk 带条件
来源：http://qx.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xk.chemitech.net.cn

[R50] awk 求和
来源：http://up.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://he.jctech888.com.cn

[R51] 排序去重取前几
来源：http://wp.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://se.jctech888.com.cn

[R52] 统计行数
来源：http://ng.shxzskj.cn

wc -l a.txt
来源：http://ds.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://sv.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sz.bjjhwx.cn

[R54] 比较两个文件
来源：http://cd.colortex.cn

diff a.txt b.txt
来源：http://hp.szsharing.cn

[R55] 压缩与解压
来源：http://ur.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oi.chemitech.net.cn

[R56] 远程拷贝
来源：http://od.jianghongdianzi.cn

scp file user@host:/path/
来源：http://ok.nicolike.cn

[R57] 远程执行命令
来源：http://ia.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://ex.huanxung.cn

[R58] 下载文件
来源：http://iy.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gm.huixiangedu.cn

[R59] 发 POST JSON
来源：http://co.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qe.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://mc.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bp.muxihuayi.cn

[R61] 磁盘占用
来源：http://sx.huixinmuqiang.cn

df -h;  du -sh *
来源：http://cs.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://bn.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://ns.huanxung.cn

[R63] 内存与进程
来源：http://fu.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://ed.shxzskj.cn

[R64] 结束进程
来源：http://ts.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://yj.huanxung.cn

[R65] 查看端口占用
来源：http://mc.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rw.wgjwhj.cn

[R66] 定时任务
来源：http://yt.huanxung.cn

crontab -e;  crontab -l
来源：http://im.hahajie.cn

[R67] 生成随机十六进制串
来源：http://bc.asd995.cn

openssl rand -hex 16
来源：http://ak.chemitech.net.cn

[R68] 计算文件校验值
来源：http://ta.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vo.newstarts.cn

[R69] 生成随机密码
来源：http://rq.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://tk.gzmigu.cn

[R70] 时间戳与互转
来源：http://he.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://kj.wgjwhj.cn

[R71] 日期格式化
来源：http://sr.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gh.haigaiapp.cn

[R72] 等待端口就绪
来源：http://oy.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fe.nszjky.cn

[R73] 分割大日志
来源：http://ee.haigaiapp.cn

split -l 1000 big.log part_
来源：http://qz.nicolike.cn

[R74] 批量重命名
来源：http://pq.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vm.newstarts.cn

[R75] 导出环境变量
来源：http://bs.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://af.hnjuh.cn

[R76] 使用临时文件
来源：http://ia.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mp.huixiangedu.cn

[R77] 读取用户输入
来源：http://tf.hahajie.cn

read -rp "请输入: " ans
来源：http://fi.huixiangedu.cn

[R78] 交互式菜单
来源：http://gh.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zi.newstarts.cn

[R79] 解析命令行选项
来源：http://ct.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wf.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://as.jianghongdianzi.cn

time ./run.sh
来源：http://li.9csxet.cn

================================================================================
来源：http://pn.nicolike.cn

S. C / C++ 专题
来源：http://vx.shxzskj.cn

================================================================================
来源：http://qo.hnjuh.cn

[S01] C：Hello World
来源：http://qb.huixinmuqiang.cn

#include <stdio.h>
来源：http://vy.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fe.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://dx.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://le.shxzskj.cn

[S03] C：读入整数
来源：http://rc.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://aw.hnjuh.cn

[S04] C：字符串复制
来源：http://jl.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dc.newstarts.cn

[S05] C：字符串长度
来源：http://oh.shxzukj.cn

strlen(s)
来源：http://om.lnxyls.cn

[S06] C：字符串比较
来源：http://dx.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://np.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://lq.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xl.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://kx.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ie.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://hu.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tb.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://bk.szsharing.cn

int *p = &a;  *p = 5;
来源：http://uh.nszjky.cn

[S11] C：逐行读文件
来源：http://it.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://mo.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zt.shtwfgs.cn

fclose(f);
来源：http://on.9csxet.cn

[S12] C：写文件
来源：http://uu.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ba.chemitech.net.cn

[S13] C：宏定义
来源：http://la.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kw.gzmigu.cn

[S14] C：枚举
来源：http://zn.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://wo.521024.cn

[S15] C：类型转换
来源：http://iy.huanxung.cn

(double) a / b
来源：http://ix.jctech888.com.cn

[S16] C：位操作置位
来源：http://dg.muxihuayi.cn

x |= (1 << 3);
来源：http://pc.huanxung.cn

[S17] C：安全拼接字符串
来源：http://hn.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cv.chemitech.net.cn

[S18] C：命令行参数
来源：http://bh.szxytkj.cn

int main(int argc, char **argv)
来源：http://sp.jianghongdianzi.cn

[S19] C：快速排序
来源：http://zt.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vb.szsharing.cn

[S20] C：二分查找
来源：http://kq.nszjky.cn


<!-- 参考信息 -->