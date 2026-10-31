代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://gq.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dt.9csxet.cn

[Q43] 标量子查询
来源：http://iy.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ty.shxzskj.cn

[Q44] IN 子查询
来源：http://oi.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ew.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://da.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lb.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rp.wgjwhj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fl.hnjuh.cn

[Q47] 与平均值比较
来源：http://nm.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cj.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://kq.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yd.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://vf.wgjwhj.cn

[Q49] 更新单行
来源：http://oh.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fo.gzmigu.cn

[Q50] 批量更新
来源：http://cf.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ix.haigaiapp.cn

[Q51] 用子查询更新
来源：http://iw.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rb.521024.cn

[Q52] 删除指定行
来源：http://jf.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://jc.huixiangedu.cn

[Q53] 按条件删除
来源：http://sa.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xl.huixiangedu.cn

[Q54] 清空表
来源：http://ne.nszjky.cn

TRUNCATE TABLE logs;
来源：http://kx.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://kw.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ov.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://cq.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qw.bjjhwx.cn

[Q57] 行号
来源：http://wo.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://li.asd995.cn

[Q58] 累计求和
来源：http://lf.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://he.panjiajie.cn

[Q59] 分组内累计
来源：http://od.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eq.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://gm.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vx.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ly.9csxet.cn

[Q61] 移动平均
来源：http://eo.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bm.szsharing.cn

[Q62] 分组占比
来源：http://ir.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tq.nszjky.cn

[Q63] 开启事务
来源：http://ts.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://me.gzmigu.cn

[Q64] 提交事务
来源：http://cr.colortex.cn

COMMIT;
来源：http://cc.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://hy.shxzukj.cn

ROLLBACK;
来源：http://qu.asd995.cn

[Q66] 行锁查询
来源：http://mz.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zg.panjiajie.cn

[Q67] 设置隔离级别
来源：http://qf.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wx.9csxet.cn

[Q68] 保存点
来源：http://mw.jctech888.com.cn

SAVEPOINT sp1;
来源：http://ay.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://ym.muxihuayi.cn

[Q69] 查看执行计划
来源：http://dc.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kl.bjjhwx.cn

[Q70] 更新统计信息
来源：http://iz.lnxyls.cn

ANALYZE TABLE users;
来源：http://zr.asd995.cn

[Q71] 查看建表语句
来源：http://aa.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bn.shxzukj.cn

[Q72] 查看索引
来源：http://sc.hnjuh.cn

SHOW INDEX FROM users;
来源：http://bw.hnjuh.cn

[Q73] 查看表状态
来源：http://fh.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fe.521024.cn

[Q74] 强制使用索引
来源：http://xz.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ks.nicolike.cn

[Q75] 日期格式化
来源：http://br.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sp.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lo.panjiajie.cn

[Q76] 按天统计
来源：http://hd.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sn.huanxung.cn

[Q77] 时间加减
来源：http://if.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kx.hnjuh.cn

[Q78] 当前时间
来源：http://io.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lr.nicolike.cn

[Q79] 字符串拼接
来源：http://hb.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ub.panjiajie.cn

[Q80] 字符串截取
来源：http://jv.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://df.yuexingan06.cn

[Q81] 字符串替换
来源：http://si.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kz.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://zx.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ch.521024.cn

[Q83] 大小写转换
来源：http://pl.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kv.asd995.cn

[Q84] 去除首尾空格
来源：http://at.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://wm.521024.cn

[Q85] 数值取整
来源：http://eq.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pl.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://xk.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ke.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://oj.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ue.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://fn.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ev.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://il.szxytkj.cn

[Q89] 判断表是否存在
来源：http://mh.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mu.haigaiapp.cn

[Q90] 生成序号列
来源：http://lt.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fk.huixiangedu.cn

================================================================================
来源：http://bx.chemitech.net.cn

R. Bash 专题
来源：http://zu.bookmarksfly.cn

================================================================================
来源：http://nz.panjiajie.cn

[R01] shebang 与严格模式
来源：http://mx.hnjuh.cn

#!/usr/bin/env bash
来源：http://ru.nszjky.cn

set -euo pipefail
来源：http://gs.panjiajie.cn

[R02] 变量赋值与使用
来源：http://pf.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://xm.lnxyls.cn

[R03] 只读变量
来源：http://ot.colortex.cn

readonly PI=3.14
来源：http://ax.nszjky.cn

[R04] 位置参数
来源：http://kb.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rh.shtwfgs.cn

[R05] 参数默认值
来源：http://zb.nszjky.cn

name="${1:-default}"
来源：http://qh.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://ti.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ja.huixinmuqiang.cn

[R07] if 判断文件
来源：http://lt.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ge.9csxet.cn

[R08] 数值比较
来源：http://pk.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zb.chemitech.net.cn

[R09] 字符串比较
来源：http://ol.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wj.nszjky.cn

[R10] 正则匹配
来源：http://qn.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pg.chemitech.net.cn

[R11] case 多分支
来源：http://nz.shxzukj.cn

case "$1" in
来源：http://to.gzmigu.cn

start) echo "启动" ;;
来源：http://xl.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://xk.nszjky.cn

*)     echo "未知命令" ;;
来源：http://hx.wgjwhj.cn

esac
来源：http://zy.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://bw.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://xb.bookmarksfly.cn

[R13] for 计数循环
来源：http://si.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://vw.panjiajie.cn

[R14] C 风格 for
来源：http://wa.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://za.szxytkj.cn

[R15] while 逐行读文件
来源：http://mg.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bc.hahajie.cn

[R16] until 等待条件
来源：http://pz.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ic.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://ur.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mq.muxihuayi.cn

[R18] 遍历数组
来源：http://dm.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hg.9csxet.cn

[R19] 数组长度
来源：http://zo.lnxyls.cn

echo "${#arr[@]}"
来源：http://bx.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://gy.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://la.shtwfgs.cn

[R21] 字符串长度
来源：http://fy.bookmarksfly.cn

echo "${#s}"
来源：http://ey.asd995.cn

[R22] 截取子串
来源：http://wq.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://vf.newstarts.cn

[R23] 字符串替换
来源：http://uv.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gd.hnjuh.cn

[R24] 大小写转换
来源：http://bg.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dk.521024.cn

[R25] 去后缀 / 去前缀
来源：http://gb.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ma.wgjwhj.cn

[R26] 命令替换
来源：http://uu.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://ck.lnxyls.cn

[R27] 算术展开
来源：http://qi.huanxung.cn

echo $((1 + 2 * 3))
来源：http://gl.huanxung.cn

[R28] 浮点运算
来源：http://yz.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://xw.521024.cn

[R29] 定义函数
来源：http://sy.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fz.haigaiapp.cn

[R30] 函数返回状态码
来源：http://bi.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://gp.jianghongdianzi.cn

[R31] 局部变量
来源：http://hk.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://ib.muxihuayi.cn

[R32] 参数个数校验
来源：http://sw.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ny.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://qr.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sf.panjiajie.cn

[R34] 退出时清理
来源：http://vk.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gw.gzmigu.cn

[R35] 后台执行并等待
来源：http://ej.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ot.huanxung.cn

[R36] 并发执行多个任务
来源：http://te.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wp.asd995.cn

[R37] 把输出赋给变量
来源：http://km.yuntaijiaju.cn

files=$(ls -1)
来源：http://ir.huixinmuqiang.cn

[R38] 管道串联
来源：http://jw.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://qd.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://gm.muxihuayi.cn

cmd > out.log 2>&1
来源：http://qs.newstarts.cn

[R40] 追加写日志
来源：http://me.bookmarksfly.cn

echo "log" >> out.log
来源：http://zf.szsharing.cn

[R41] 丢弃输出
来源：http://bw.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://vq.hnjuh.cn

[R42] 输入重定向
来源：http://ue.yuntaijiaju.cn

wc -l < a.txt
来源：http://nm.panjiajie.cn

[R43] 按名字查找文件
来源：http://rq.521024.cn

find . -name "*.log" -type f
来源：http://iu.szsharing.cn

[R44] 按修改时间查找
来源：http://lb.yuexingan06.cn

find . -mtime -7 -type f
来源：http://fa.521024.cn

[R45] 批量删除
来源：http://zk.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://qh.szxytkj.cn

[R46] 递归替换文件内容
来源：http://ec.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ym.521024.cn

[R47] sed 单行替换
来源：http://mh.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ld.hnjuh.cn

[R48] awk 取指定列
来源：http://dx.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://co.muxihuayi.cn

[R49] awk 带条件
来源：http://my.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kx.9csxet.cn

[R50] awk 求和
来源：http://zg.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://df.hnjuh.cn

[R51] 排序去重取前几
来源：http://fa.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yd.hnjuh.cn

[R52] 统计行数
来源：http://jc.hahajie.cn

wc -l a.txt
来源：http://nd.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://mv.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tx.colortex.cn

[R54] 比较两个文件
来源：http://zf.nicolike.cn

diff a.txt b.txt
来源：http://ql.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://kb.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sk.newstarts.cn

[R56] 远程拷贝
来源：http://yo.muxihuayi.cn

scp file user@host:/path/
来源：http://rr.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://qe.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://pw.shtwfgs.cn

[R58] 下载文件
来源：http://oz.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jm.haigaiapp.cn

[R59] 发 POST JSON
来源：http://mu.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rc.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://uu.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://po.9csxet.cn

[R61] 磁盘占用
来源：http://fw.huanxung.cn

df -h;  du -sh *
来源：http://jv.lnxyls.cn

[R62] 找最占空间的文件
来源：http://wf.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://zw.jianghongdianzi.cn

[R63] 内存与进程
来源：http://bf.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://pk.nicolike.cn

[R64] 结束进程
来源：http://cc.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://yj.haigaiapp.cn

[R65] 查看端口占用
来源：http://uo.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rq.lnxyls.cn

[R66] 定时任务
来源：http://md.hnjuh.cn

crontab -e;  crontab -l
来源：http://jr.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://qd.asd995.cn

openssl rand -hex 16
来源：http://ot.yuexingan06.cn

[R68] 计算文件校验值
来源：http://xk.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mh.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://yg.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://tc.yuexingan06.cn

[R70] 时间戳与互转
来源：http://sb.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://fl.yuexingan06.cn

[R71] 日期格式化
来源：http://ry.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mb.shtwfgs.cn

[R72] 等待端口就绪
来源：http://ba.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mu.nszjky.cn

[R73] 分割大日志
来源：http://rt.szsharing.cn

split -l 1000 big.log part_
来源：http://fr.huixinmuqiang.cn

[R74] 批量重命名
来源：http://ov.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gn.jctech888.com.cn

[R75] 导出环境变量
来源：http://du.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://ur.lnxyls.cn

[R76] 使用临时文件
来源：http://wr.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tu.9csxet.cn

[R77] 读取用户输入
来源：http://vl.521024.cn

read -rp "请输入: " ans
来源：http://re.hnjuh.cn

[R78] 交互式菜单
来源：http://nw.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bh.shxzukj.cn

[R79] 解析命令行选项
来源：http://xm.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kd.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://wm.newstarts.cn

time ./run.sh
来源：http://on.shxzukj.cn

================================================================================
来源：http://lm.huixiangedu.cn

S. C / C++ 专题
来源：http://dn.huanxung.cn

================================================================================
来源：http://pl.chemitech.net.cn

[S01] C：Hello World
来源：http://jb.gzmigu.cn

#include <stdio.h>
来源：http://fb.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cq.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://dq.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://vj.lnxyls.cn

[S03] C：读入整数
来源：http://nh.shxzukj.cn

int x; scanf("%d", &x);
来源：http://kx.nicolike.cn

[S04] C：字符串复制
来源：http://of.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xv.hnjuh.cn

[S05] C：字符串长度
来源：http://tp.chemitech.net.cn

strlen(s)
来源：http://bi.muxihuayi.cn

[S06] C：字符串比较
来源：http://jc.hahajie.cn

strcmp(a, b) == 0
来源：http://jv.hahajie.cn

[S07] C：数组遍历求和
来源：http://fx.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nx.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://ws.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fv.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://ak.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qw.9csxet.cn

[S10] C：指针与解引用
来源：http://nm.newstarts.cn

int *p = &a;  *p = 5;
来源：http://kb.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://rk.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://vi.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ne.jianghongdianzi.cn

fclose(f);
来源：http://ji.shtwfgs.cn

[S12] C：写文件
来源：http://jr.hahajie.cn


<!-- 参考信息 -->