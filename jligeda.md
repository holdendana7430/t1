代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://nz.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://lt.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://pf.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://iw.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://au.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yj.lnxyls.cn

[Q43] 标量子查询
来源：http://yv.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vh.chemitech.net.cn

[Q44] IN 子查询
来源：http://nu.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qv.asd995.cn

[Q45] EXISTS 判断存在
来源：http://vj.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ph.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ub.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nh.muxihuayi.cn

[Q47] 与平均值比较
来源：http://pq.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ys.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://mq.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aw.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://nf.newstarts.cn

[Q49] 更新单行
来源：http://ue.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xi.gzmigu.cn

[Q50] 批量更新
来源：http://wx.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ps.haigaiapp.cn

[Q51] 用子查询更新
来源：http://eh.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mv.wgjwhj.cn

[Q52] 删除指定行
来源：http://pr.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://fi.nszjky.cn

[Q53] 按条件删除
来源：http://yc.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gt.huixiangedu.cn

[Q54] 清空表
来源：http://wx.nszjky.cn

TRUNCATE TABLE logs;
来源：http://ks.521024.cn

[Q55] 排名（并列占位）
来源：http://fn.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dh.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://bb.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vz.szsharing.cn

[Q57] 行号
来源：http://uc.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ys.szxytkj.cn

[Q58] 累计求和
来源：http://qu.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://op.jctech888.com.cn

[Q59] 分组内累计
来源：http://wv.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iv.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://zc.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cv.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ox.wgjwhj.cn

[Q61] 移动平均
来源：http://qk.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fh.szsharing.cn

[Q62] 分组占比
来源：http://oz.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wi.yuntaijiaju.cn

[Q63] 开启事务
来源：http://sm.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xi.hahajie.cn

[Q64] 提交事务
来源：http://ln.gzmigu.cn

COMMIT;
来源：http://ky.panjiajie.cn

[Q65] 回滚事务
来源：http://bu.panjiajie.cn

ROLLBACK;
来源：http://ln.hnjuh.cn

[Q66] 行锁查询
来源：http://ud.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yz.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://fl.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ot.huixinmuqiang.cn

[Q68] 保存点
来源：http://gt.colortex.cn

SAVEPOINT sp1;
来源：http://qr.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://tp.szsharing.cn

[Q69] 查看执行计划
来源：http://au.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tj.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://ae.shtwfgs.cn

ANALYZE TABLE users;
来源：http://aw.shxzukj.cn

[Q71] 查看建表语句
来源：http://pf.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ty.chemitech.net.cn

[Q72] 查看索引
来源：http://ke.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://cm.wgjwhj.cn

[Q73] 查看表状态
来源：http://ts.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bx.hnjuh.cn

[Q74] 强制使用索引
来源：http://tc.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://el.chemitech.net.cn

[Q75] 日期格式化
来源：http://bt.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wj.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rq.hahajie.cn

[Q76] 按天统计
来源：http://go.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kz.bookmarksfly.cn

[Q77] 时间加减
来源：http://ar.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hl.yuexingan06.cn

[Q78] 当前时间
来源：http://oo.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lx.panjiajie.cn

[Q79] 字符串拼接
来源：http://oq.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ir.shtwfgs.cn

[Q80] 字符串截取
来源：http://jj.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wa.lnxyls.cn

[Q81] 字符串替换
来源：http://am.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://em.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://ew.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cg.9csxet.cn

[Q83] 大小写转换
来源：http://bl.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nt.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://pr.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://qq.szsharing.cn

[Q85] 数值取整
来源：http://ma.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vt.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://jb.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oa.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://ps.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pw.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://hr.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://we.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vs.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://ua.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rh.haigaiapp.cn

[Q90] 生成序号列
来源：http://we.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ke.bjjhwx.cn

================================================================================
来源：http://zn.wgjwhj.cn

R. Bash 专题
来源：http://qe.bjjhwx.cn

================================================================================
来源：http://po.521024.cn

[R01] shebang 与严格模式
来源：http://io.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://ys.huixinmuqiang.cn

set -euo pipefail
来源：http://lf.hnjuh.cn

[R02] 变量赋值与使用
来源：http://eh.lnxyls.cn

name="Tom"; echo "$name"
来源：http://za.shtwfgs.cn

[R03] 只读变量
来源：http://zr.yuexingan06.cn

readonly PI=3.14
来源：http://bj.muxihuayi.cn

[R04] 位置参数
来源：http://vs.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fy.szxytkj.cn

[R05] 参数默认值
来源：http://so.shxzskj.cn

name="${1:-default}"
来源：http://ii.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://ft.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qg.yuntaijiaju.cn

[R07] if 判断文件
来源：http://ik.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vv.jianghongdianzi.cn

[R08] 数值比较
来源：http://rb.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rj.asd995.cn

[R09] 字符串比较
来源：http://cc.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wd.szsharing.cn

[R10] 正则匹配
来源：http://tg.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://er.521024.cn

[R11] case 多分支
来源：http://di.bjjhwx.cn

case "$1" in
来源：http://mt.newstarts.cn

start) echo "启动" ;;
来源：http://ku.hnjuh.cn

stop)  echo "停止" ;;
来源：http://yk.nszjky.cn

*)     echo "未知命令" ;;
来源：http://kf.shxzukj.cn

esac
来源：http://gg.haigaiapp.cn

[R12] for 遍历文件
来源：http://gx.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://fo.wgjwhj.cn

[R13] for 计数循环
来源：http://ca.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://ee.hahajie.cn

[R14] C 风格 for
来源：http://nu.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cj.yuexingan06.cn

[R15] while 逐行读文件
来源：http://cl.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ne.521024.cn

[R16] until 等待条件
来源：http://xe.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wu.wgjwhj.cn

[R17] 数组定义与取值
来源：http://ab.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nk.nicolike.cn

[R18] 遍历数组
来源：http://ix.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://re.muxihuayi.cn

[R19] 数组长度
来源：http://pi.shtwfgs.cn

echo "${#arr[@]}"
来源：http://vz.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://ov.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://of.muxihuayi.cn

[R21] 字符串长度
来源：http://kp.shxzukj.cn

echo "${#s}"
来源：http://ue.yuntaijiaju.cn

[R22] 截取子串
来源：http://ho.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://li.jctech888.com.cn

[R23] 字符串替换
来源：http://iq.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lu.hahajie.cn

[R24] 大小写转换
来源：http://ih.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zb.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://ip.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sq.lnxyls.cn

[R26] 命令替换
来源：http://bf.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://wf.bjjhwx.cn

[R27] 算术展开
来源：http://oi.colortex.cn

echo $((1 + 2 * 3))
来源：http://cj.lnxyls.cn

[R28] 浮点运算
来源：http://al.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://re.huanxung.cn

[R29] 定义函数
来源：http://pj.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bo.jctech888.com.cn

[R30] 函数返回状态码
来源：http://so.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://pm.szsharing.cn

[R31] 局部变量
来源：http://ij.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://ed.huixiangedu.cn

[R32] 参数个数校验
来源：http://lt.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aq.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://xm.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hn.hahajie.cn

[R34] 退出时清理
来源：http://ln.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qx.gzmigu.cn

[R35] 后台执行并等待
来源：http://ux.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://df.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://dk.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://up.lnxyls.cn

[R37] 把输出赋给变量
来源：http://cp.huanxung.cn

files=$(ls -1)
来源：http://vj.gzmigu.cn

[R38] 管道串联
来源：http://qc.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://fa.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://jv.haigaiapp.cn

cmd > out.log 2>&1
来源：http://mf.bookmarksfly.cn

[R40] 追加写日志
来源：http://yl.jctech888.com.cn

echo "log" >> out.log
来源：http://nv.huixiangedu.cn

[R41] 丢弃输出
来源：http://mo.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://mc.newstarts.cn

[R42] 输入重定向
来源：http://gg.huanxung.cn

wc -l < a.txt
来源：http://wh.muxihuayi.cn

[R43] 按名字查找文件
来源：http://zs.wgjwhj.cn

find . -name "*.log" -type f
来源：http://fk.huixiangedu.cn

[R44] 按修改时间查找
来源：http://dh.521024.cn

find . -mtime -7 -type f
来源：http://rs.asd995.cn

[R45] 批量删除
来源：http://uc.521024.cn

find . -name "*.tmp" -delete
来源：http://dv.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://pw.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hx.wgjwhj.cn

[R47] sed 单行替换
来源：http://kx.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lq.hnjuh.cn

[R48] awk 取指定列
来源：http://bh.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://ll.gzmigu.cn

[R49] awk 带条件
来源：http://nv.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sx.bjjhwx.cn

[R50] awk 求和
来源：http://fh.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://md.hnjuh.cn

[R51] 排序去重取前几
来源：http://pq.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zk.hahajie.cn

[R52] 统计行数
来源：http://yd.newstarts.cn

wc -l a.txt
来源：http://ak.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://cx.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ix.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://ts.haigaiapp.cn

diff a.txt b.txt
来源：http://xu.wgjwhj.cn

[R55] 压缩与解压
来源：http://lb.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bp.gzmigu.cn

[R56] 远程拷贝
来源：http://vh.bookmarksfly.cn

scp file user@host:/path/
来源：http://ve.shxzukj.cn

[R57] 远程执行命令
来源：http://yn.panjiajie.cn

ssh user@host 'uptime'
来源：http://wu.szsharing.cn

[R58] 下载文件
来源：http://cp.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hq.colortex.cn

[R59] 发 POST JSON
来源：http://te.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xs.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://bl.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://do.panjiajie.cn

[R61] 磁盘占用
来源：http://lp.yuntaijiaju.cn

df -h;  du -sh *
来源：http://rj.szsharing.cn

[R62] 找最占空间的文件
来源：http://du.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://qv.bookmarksfly.cn

[R63] 内存与进程
来源：http://mn.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://du.yuexingan06.cn

[R64] 结束进程
来源：http://eb.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://xk.lnxyls.cn

[R65] 查看端口占用
来源：http://jn.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rc.yuexingan06.cn

[R66] 定时任务
来源：http://lx.chemitech.net.cn

crontab -e;  crontab -l
来源：http://yn.colortex.cn

[R67] 生成随机十六进制串
来源：http://pp.asd995.cn

openssl rand -hex 16
来源：http://zc.wgjwhj.cn

[R68] 计算文件校验值
来源：http://tw.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ah.lnxyls.cn

[R69] 生成随机密码
来源：http://wv.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://je.muxihuayi.cn

[R70] 时间戳与互转
来源：http://oo.521024.cn

date +%s;  date -d @1700000000
来源：http://hl.lnxyls.cn

[R71] 日期格式化
来源：http://lq.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tk.nszjky.cn

[R72] 等待端口就绪
来源：http://yq.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tl.asd995.cn

[R73] 分割大日志
来源：http://kw.muxihuayi.cn

split -l 1000 big.log part_
来源：http://xp.huixiangedu.cn

[R74] 批量重命名
来源：http://uk.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yx.jianghongdianzi.cn

[R75] 导出环境变量
来源：http://gu.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://jn.haigaiapp.cn

[R76] 使用临时文件
来源：http://od.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://db.lnxyls.cn

[R77] 读取用户输入
来源：http://mi.bjjhwx.cn

read -rp "请输入: " ans
来源：http://rn.colortex.cn

[R78] 交互式菜单
来源：http://dt.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eo.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://es.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qm.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://jb.521024.cn

time ./run.sh
来源：http://qa.lnxyls.cn

================================================================================
来源：http://sy.wgjwhj.cn

S. C / C++ 专题
来源：http://xg.jianghongdianzi.cn

================================================================================
来源：http://vn.nszjky.cn

[S01] C：Hello World
来源：http://ew.hahajie.cn

#include <stdio.h>
来源：http://ug.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fz.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://se.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://wv.shtwfgs.cn

[S03] C：读入整数
来源：http://gx.521024.cn

int x; scanf("%d", &x);
来源：http://bi.bjjhwx.cn

[S04] C：字符串复制
来源：http://qd.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xy.huixiangedu.cn

[S05] C：字符串长度
来源：http://hl.huanxung.cn

strlen(s)
来源：http://xw.hnjuh.cn

[S06] C：字符串比较
来源：http://sc.lnxyls.cn

strcmp(a, b) == 0
来源：http://bi.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://hm.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zk.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://pl.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://db.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://hv.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://il.wgjwhj.cn

[S10] C：指针与解引用
来源：http://yu.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://lz.panjiajie.cn

[S11] C：逐行读文件
来源：http://ry.hnjuh.cn


<!-- 参考信息 -->