代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mg.521024.cn

[Q32] 分组拼接字符串
来源：http://uj.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ci.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oi.chemitech.net.cn

[Q33] 多列分组
来源：http://lu.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wu.gzmigu.cn

[Q34] 每组取第一条
来源：http://ee.nicolike.cn

SELECT * FROM (
来源：http://em.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ug.yuexingan06.cn

) t WHERE rn = 1;
来源：http://im.bookmarksfly.cn

[Q35] 内连接
来源：http://yn.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fe.chemitech.net.cn

[Q36] 左连接
来源：http://ll.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hw.bookmarksfly.cn

[Q37] 右连接
来源：http://xy.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nv.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ph.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ri.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://qi.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://br.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hm.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uf.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kr.shxzskj.cn

[Q41] 多表连接
来源：http://ym.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jr.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://ev.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://so.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://tj.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://jc.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lf.huanxung.cn

[Q43] 标量子查询
来源：http://um.lnxyls.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ny.huanxung.cn

[Q44] IN 子查询
来源：http://jx.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://af.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://su.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ir.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ni.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gt.colortex.cn

[Q47] 与平均值比较
来源：http://mw.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qr.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://kz.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gv.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://uk.muxihuayi.cn

[Q49] 更新单行
来源：http://lg.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ea.nicolike.cn

[Q50] 批量更新
来源：http://ac.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mb.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://je.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ye.wgjwhj.cn

[Q52] 删除指定行
来源：http://ze.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://sx.gzmigu.cn

[Q53] 按条件删除
来源：http://bx.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hr.newstarts.cn

[Q54] 清空表
来源：http://py.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://sg.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://hb.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nc.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://nl.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gt.wgjwhj.cn

[Q57] 行号
来源：http://ue.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bp.yuexingan06.cn

[Q58] 累计求和
来源：http://hr.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gd.newstarts.cn

[Q59] 分组内累计
来源：http://wp.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cy.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://sp.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kf.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://im.shtwfgs.cn

[Q61] 移动平均
来源：http://xi.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sy.szsharing.cn

[Q62] 分组占比
来源：http://ad.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://br.szxytkj.cn

[Q63] 开启事务
来源：http://az.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://be.szxytkj.cn

[Q64] 提交事务
来源：http://vg.shxzukj.cn

COMMIT;
来源：http://ud.shxzukj.cn

[Q65] 回滚事务
来源：http://ws.jianghongdianzi.cn

ROLLBACK;
来源：http://zi.panjiajie.cn

[Q66] 行锁查询
来源：http://ja.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gg.shxzskj.cn

[Q67] 设置隔离级别
来源：http://bb.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://as.nszjky.cn

[Q68] 保存点
来源：http://ar.shxzskj.cn

SAVEPOINT sp1;
来源：http://jw.szsharing.cn

ROLLBACK TO sp1;
来源：http://hj.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://lg.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tp.hahajie.cn

[Q70] 更新统计信息
来源：http://xo.bjjhwx.cn

ANALYZE TABLE users;
来源：http://xj.lnxyls.cn

[Q71] 查看建表语句
来源：http://qz.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rp.hahajie.cn

[Q72] 查看索引
来源：http://gl.hahajie.cn

SHOW INDEX FROM users;
来源：http://zi.panjiajie.cn

[Q73] 查看表状态
来源：http://zi.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jk.szxytkj.cn

[Q74] 强制使用索引
来源：http://dw.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sz.9csxet.cn

[Q75] 日期格式化
来源：http://lu.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ok.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oq.szxytkj.cn

[Q76] 按天统计
来源：http://ny.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ch.nszjky.cn

[Q77] 时间加减
来源：http://qn.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dm.asd995.cn

[Q78] 当前时间
来源：http://af.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ld.shtwfgs.cn

[Q79] 字符串拼接
来源：http://vk.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gi.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://jy.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eq.jctech888.com.cn

[Q81] 字符串替换
来源：http://hs.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fw.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://bp.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xc.9csxet.cn

[Q83] 大小写转换
来源：http://bh.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gq.nszjky.cn

[Q84] 去除首尾空格
来源：http://lm.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://ig.jianghongdianzi.cn

[Q85] 数值取整
来源：http://cv.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tp.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://pg.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ha.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://vi.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hh.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://ws.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hq.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gl.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://jt.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tz.huanxung.cn

[Q90] 生成序号列
来源：http://os.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qf.newstarts.cn

================================================================================
来源：http://ee.nicolike.cn

R. Bash 专题
来源：http://fv.nszjky.cn

================================================================================
来源：http://eo.hahajie.cn

[R01] shebang 与严格模式
来源：http://xa.gzmigu.cn

#!/usr/bin/env bash
来源：http://zw.lnxyls.cn

set -euo pipefail
来源：http://lm.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://cu.huanxung.cn

name="Tom"; echo "$name"
来源：http://rw.newstarts.cn

[R03] 只读变量
来源：http://sp.bjjhwx.cn

readonly PI=3.14
来源：http://gm.szxytkj.cn

[R04] 位置参数
来源：http://ob.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rg.gzmigu.cn

[R05] 参数默认值
来源：http://yi.szsharing.cn

name="${1:-default}"
来源：http://mw.newstarts.cn

[R06] 判断命令是否存在
来源：http://fj.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ie.521024.cn

[R07] if 判断文件
来源：http://lb.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ao.nicolike.cn

[R08] 数值比较
来源：http://fn.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ug.huanxung.cn

[R09] 字符串比较
来源：http://ky.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sn.asd995.cn

[R10] 正则匹配
来源：http://eh.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dt.haigaiapp.cn

[R11] case 多分支
来源：http://is.shxzskj.cn

case "$1" in
来源：http://py.szxytkj.cn

start) echo "启动" ;;
来源：http://hl.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://sa.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://eh.lnxyls.cn

esac
来源：http://rp.shxzskj.cn

[R12] for 遍历文件
来源：http://ct.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://ok.lnxyls.cn

[R13] for 计数循环
来源：http://jz.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://sz.9csxet.cn

[R14] C 风格 for
来源：http://mu.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gl.huanxung.cn

[R15] while 逐行读文件
来源：http://ib.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gc.9csxet.cn

[R16] until 等待条件
来源：http://ze.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tv.shxzukj.cn

[R17] 数组定义与取值
来源：http://iy.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://om.muxihuayi.cn

[R18] 遍历数组
来源：http://ca.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eq.gzmigu.cn

[R19] 数组长度
来源：http://ih.huixiangedu.cn

echo "${#arr[@]}"
来源：http://rh.bookmarksfly.cn

[R20] 关联数组（字典）
来源：http://ix.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rl.asd995.cn

[R21] 字符串长度
来源：http://eh.shxzukj.cn

echo "${#s}"
来源：http://xi.szxytkj.cn

[R22] 截取子串
来源：http://xz.shxzskj.cn

echo "${s:0:5}"
来源：http://sf.nszjky.cn

[R23] 字符串替换
来源：http://zf.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dp.521024.cn

[R24] 大小写转换
来源：http://jc.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vy.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://pt.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ld.szxytkj.cn

[R26] 命令替换
来源：http://kf.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://jq.szxytkj.cn

[R27] 算术展开
来源：http://ir.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://wc.panjiajie.cn

[R28] 浮点运算
来源：http://mo.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://ad.nszjky.cn

[R29] 定义函数
来源：http://xx.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nk.haigaiapp.cn

[R30] 函数返回状态码
来源：http://kv.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://jq.shtwfgs.cn

[R31] 局部变量
来源：http://zs.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://pf.jctech888.com.cn

[R32] 参数个数校验
来源：http://dp.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://js.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://pc.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rj.shxzukj.cn

[R34] 退出时清理
来源：http://fz.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ie.wgjwhj.cn

[R35] 后台执行并等待
来源：http://an.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://aj.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://bf.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vb.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://gl.521024.cn

files=$(ls -1)
来源：http://ds.lnxyls.cn

[R38] 管道串联
来源：http://sn.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://mr.colortex.cn

[R39] 重定向标准输出与错误
来源：http://iw.shtwfgs.cn

cmd > out.log 2>&1
来源：http://qv.shtwfgs.cn

[R40] 追加写日志
来源：http://ae.yuntaijiaju.cn

echo "log" >> out.log
来源：http://qe.9csxet.cn

[R41] 丢弃输出
来源：http://vx.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://fr.jianghongdianzi.cn

[R42] 输入重定向
来源：http://fv.colortex.cn

wc -l < a.txt
来源：http://pw.hahajie.cn

[R43] 按名字查找文件
来源：http://ct.huixiangedu.cn

find . -name "*.log" -type f
来源：http://da.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://ei.gzmigu.cn

find . -mtime -7 -type f
来源：http://bj.521024.cn

[R45] 批量删除
来源：http://vj.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://fo.hahajie.cn

[R46] 递归替换文件内容
来源：http://hw.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gg.lnxyls.cn

[R47] sed 单行替换
来源：http://uu.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mo.szxytkj.cn

[R48] awk 取指定列
来源：http://uj.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://il.muxihuayi.cn

[R49] awk 带条件
来源：http://vo.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qi.szsharing.cn

[R50] awk 求和
来源：http://qq.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qx.shxzskj.cn

[R51] 排序去重取前几
来源：http://dj.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ay.hahajie.cn

[R52] 统计行数
来源：http://vx.lnxyls.cn

wc -l a.txt
来源：http://bh.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://cr.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oh.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://qo.wgjwhj.cn

diff a.txt b.txt
来源：http://uq.muxihuayi.cn

[R55] 压缩与解压
来源：http://zo.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jn.shtwfgs.cn

[R56] 远程拷贝
来源：http://zw.lnxyls.cn

scp file user@host:/path/
来源：http://zs.huanxung.cn

[R57] 远程执行命令
来源：http://da.szxytkj.cn

ssh user@host 'uptime'
来源：http://km.szsharing.cn

[R58] 下载文件
来源：http://ic.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ro.szsharing.cn

[R59] 发 POST JSON
来源：http://au.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://af.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://wf.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ut.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://vc.haigaiapp.cn

df -h;  du -sh *
来源：http://lz.nszjky.cn

[R62] 找最占空间的文件
来源：http://hx.colortex.cn

du -ah . | sort -rh | head -10
来源：http://qy.shxzukj.cn

[R63] 内存与进程
来源：http://bd.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://fi.colortex.cn

[R64] 结束进程
来源：http://ux.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://ge.huixiangedu.cn

[R65] 查看端口占用
来源：http://gj.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rg.jianghongdianzi.cn

[R66] 定时任务
来源：http://um.shxzukj.cn

crontab -e;  crontab -l
来源：http://mi.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://cr.szxytkj.cn

openssl rand -hex 16
来源：http://td.szxytkj.cn

[R68] 计算文件校验值
来源：http://vn.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ra.521024.cn

[R69] 生成随机密码
来源：http://is.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://hs.huixiangedu.cn

[R70] 时间戳与互转
来源：http://ry.asd995.cn

date +%s;  date -d @1700000000
来源：http://vc.newstarts.cn

[R71] 日期格式化
来源：http://xm.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ze.chemitech.net.cn

[R72] 等待端口就绪
来源：http://hc.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yi.panjiajie.cn

[R73] 分割大日志
来源：http://nf.hahajie.cn

split -l 1000 big.log part_
来源：http://hh.bjjhwx.cn

[R74] 批量重命名
来源：http://ju.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yu.huixiangedu.cn

[R75] 导出环境变量
来源：http://cp.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://tg.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://oe.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fz.asd995.cn

[R77] 读取用户输入
来源：http://ra.shxzukj.cn

read -rp "请输入: " ans
来源：http://hw.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://lg.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yf.gzmigu.cn

[R79] 解析命令行选项
来源：http://bu.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gp.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://ao.shxzukj.cn

time ./run.sh
来源：http://ox.colortex.cn

================================================================================
来源：http://wr.chemitech.net.cn


<!-- 参考信息 -->