代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lp.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://fb.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ch.shxzskj.cn

[Q19] 范围查询
来源：http://ij.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kt.huixiangedu.cn

[Q20] IN 列表
来源：http://tb.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oe.wgjwhj.cn

[Q21] 空值判断
来源：http://qe.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xe.colortex.cn

[Q22] 排序
来源：http://jv.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://it.haigaiapp.cn

[Q23] 分页
来源：http://eh.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gd.nszjky.cn

[Q24] 去重
来源：http://yr.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://db.hnjuh.cn

[Q25] 只取前 N 条
来源：http://mu.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sj.shxzukj.cn

[Q26] 计数
来源：http://bk.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://lw.nicolike.cn

[Q27] 条件计数
来源：http://io.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zg.521024.cn

[Q28] 求和与平均
来源：http://rf.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wf.muxihuayi.cn

[Q29] 最大最小值
来源：http://wo.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pc.gzmigu.cn

[Q30] 分组统计
来源：http://oa.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dy.jctech888.com.cn

[Q31] 分组后过滤
来源：http://nk.haigaiapp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ko.9csxet.cn

[Q32] 分组拼接字符串
来源：http://dk.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ea.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ph.nszjky.cn

[Q33] 多列分组
来源：http://hy.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gy.newstarts.cn

[Q34] 每组取第一条
来源：http://mj.nszjky.cn

SELECT * FROM (
来源：http://bz.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ek.nicolike.cn

) t WHERE rn = 1;
来源：http://ax.huanxung.cn

[Q35] 内连接
来源：http://th.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mo.szsharing.cn

[Q36] 左连接
来源：http://db.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://up.lnxyls.cn

[Q37] 右连接
来源：http://jl.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ky.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ig.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://km.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://at.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nr.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oz.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ir.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mi.chemitech.net.cn

[Q41] 多表连接
来源：http://lq.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cx.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://sw.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://hn.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://km.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://re.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ys.shtwfgs.cn

[Q43] 标量子查询
来源：http://tn.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://it.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://oc.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zo.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://xb.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mu.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pe.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ai.szxytkj.cn

[Q47] 与平均值比较
来源：http://in.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qe.bjjhwx.cn

[Q48] CTE 公用表表达式
来源：http://do.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cq.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://zw.chemitech.net.cn

[Q49] 更新单行
来源：http://tf.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://js.wgjwhj.cn

[Q50] 批量更新
来源：http://ii.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tm.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://wf.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://we.shxzukj.cn

[Q52] 删除指定行
来源：http://ws.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://ro.bookmarksfly.cn

[Q53] 按条件删除
来源：http://lw.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eb.bookmarksfly.cn

[Q54] 清空表
来源：http://tz.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://lz.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://vm.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://md.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://km.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://up.huanxung.cn

[Q57] 行号
来源：http://at.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zv.521024.cn

[Q58] 累计求和
来源：http://xj.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lw.lnxyls.cn

[Q59] 分组内累计
来源：http://pv.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mz.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://ji.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fk.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hu.shtwfgs.cn

[Q61] 移动平均
来源：http://zk.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ve.shxzukj.cn

[Q62] 分组占比
来源：http://wh.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kd.panjiajie.cn

[Q63] 开启事务
来源：http://hu.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oq.yuntaijiaju.cn

[Q64] 提交事务
来源：http://yu.bookmarksfly.cn

COMMIT;
来源：http://ay.9csxet.cn

[Q65] 回滚事务
来源：http://vu.bookmarksfly.cn

ROLLBACK;
来源：http://nd.hahajie.cn

[Q66] 行锁查询
来源：http://ct.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vg.asd995.cn

[Q67] 设置隔离级别
来源：http://up.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lr.chemitech.net.cn

[Q68] 保存点
来源：http://wd.shtwfgs.cn

SAVEPOINT sp1;
来源：http://sq.shxzukj.cn

ROLLBACK TO sp1;
来源：http://fy.521024.cn

[Q69] 查看执行计划
来源：http://wp.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yi.wgjwhj.cn

[Q70] 更新统计信息
来源：http://ai.lnxyls.cn

ANALYZE TABLE users;
来源：http://en.szsharing.cn

[Q71] 查看建表语句
来源：http://ta.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://il.szxytkj.cn

[Q72] 查看索引
来源：http://kf.hahajie.cn

SHOW INDEX FROM users;
来源：http://hz.chemitech.net.cn

[Q73] 查看表状态
来源：http://so.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rp.9csxet.cn

[Q74] 强制使用索引
来源：http://mq.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gq.colortex.cn

[Q75] 日期格式化
来源：http://nu.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pu.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wh.colortex.cn

[Q76] 按天统计
来源：http://dw.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zl.colortex.cn

[Q77] 时间加减
来源：http://us.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yu.shxzukj.cn

[Q78] 当前时间
来源：http://iy.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ag.chemitech.net.cn

[Q79] 字符串拼接
来源：http://oy.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cb.jctech888.com.cn

[Q80] 字符串截取
来源：http://qh.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nf.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://av.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aw.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://zx.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wu.colortex.cn

[Q83] 大小写转换
来源：http://ug.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cg.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://xc.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://mg.chemitech.net.cn

[Q85] 数值取整
来源：http://et.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xv.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://im.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mr.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://nb.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ch.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://is.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nk.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qo.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://ls.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mb.nicolike.cn

[Q90] 生成序号列
来源：http://kx.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sq.hnjuh.cn

================================================================================
来源：http://so.521024.cn

R. Bash 专题
来源：http://mx.muxihuayi.cn

================================================================================
来源：http://yz.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://ua.newstarts.cn

#!/usr/bin/env bash
来源：http://ly.asd995.cn

set -euo pipefail
来源：http://lh.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://kz.shxzskj.cn

name="Tom"; echo "$name"
来源：http://wa.gzmigu.cn

[R03] 只读变量
来源：http://xn.jctech888.com.cn

readonly PI=3.14
来源：http://ip.521024.cn

[R04] 位置参数
来源：http://ij.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lw.jctech888.com.cn

[R05] 参数默认值
来源：http://ym.huixiangedu.cn

name="${1:-default}"
来源：http://za.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://ao.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cm.nicolike.cn

[R07] if 判断文件
来源：http://il.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yp.shxzukj.cn

[R08] 数值比较
来源：http://af.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vz.hnjuh.cn

[R09] 字符串比较
来源：http://rc.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yq.asd995.cn

[R10] 正则匹配
来源：http://zi.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://on.jianghongdianzi.cn

[R11] case 多分支
来源：http://et.huixinmuqiang.cn

case "$1" in
来源：http://xk.colortex.cn

start) echo "启动" ;;
来源：http://ic.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://oi.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://gw.szxytkj.cn

esac
来源：http://sh.muxihuayi.cn

[R12] for 遍历文件
来源：http://dn.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://nh.haigaiapp.cn

[R13] for 计数循环
来源：http://sb.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://wl.yuntaijiaju.cn

[R14] C 风格 for
来源：http://se.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ep.nicolike.cn

[R15] while 逐行读文件
来源：http://wi.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://en.gzmigu.cn

[R16] until 等待条件
来源：http://wb.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ox.asd995.cn

[R17] 数组定义与取值
来源：http://on.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ll.nszjky.cn

[R18] 遍历数组
来源：http://cr.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xv.newstarts.cn

[R19] 数组长度
来源：http://kk.jctech888.com.cn

echo "${#arr[@]}"
来源：http://bv.huanxung.cn

[R20] 关联数组（字典）
来源：http://wx.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bs.chemitech.net.cn

[R21] 字符串长度
来源：http://tn.haigaiapp.cn

echo "${#s}"
来源：http://id.jctech888.com.cn

[R22] 截取子串
来源：http://sb.521024.cn

echo "${s:0:5}"
来源：http://qg.nicolike.cn

[R23] 字符串替换
来源：http://cp.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yc.newstarts.cn

[R24] 大小写转换
来源：http://nk.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zw.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://lg.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ry.asd995.cn

[R26] 命令替换
来源：http://zb.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://zb.gzmigu.cn

[R27] 算术展开
来源：http://hh.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://aj.nszjky.cn

[R28] 浮点运算
来源：http://zq.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://kf.bjjhwx.cn

[R29] 定义函数
来源：http://sb.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vz.lnxyls.cn

[R30] 函数返回状态码
来源：http://du.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://nc.szxytkj.cn

[R31] 局部变量
来源：http://po.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://ro.521024.cn

[R32] 参数个数校验
来源：http://ga.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rb.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://sk.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fe.huanxung.cn

[R34] 退出时清理
来源：http://jt.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fp.chemitech.net.cn

[R35] 后台执行并等待
来源：http://lh.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cd.colortex.cn

[R36] 并发执行多个任务
来源：http://la.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ga.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://ht.shxzukj.cn

files=$(ls -1)
来源：http://uk.szxytkj.cn

[R38] 管道串联
来源：http://nu.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://wu.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://wp.bjjhwx.cn

cmd > out.log 2>&1
来源：http://cn.haigaiapp.cn

[R40] 追加写日志
来源：http://lm.colortex.cn

echo "log" >> out.log
来源：http://su.hnjuh.cn

[R41] 丢弃输出
来源：http://ib.huanxung.cn

cmd >/dev/null 2>&1
来源：http://nk.muxihuayi.cn

[R42] 输入重定向
来源：http://mo.hnjuh.cn

wc -l < a.txt
来源：http://yg.huanxung.cn

[R43] 按名字查找文件
来源：http://vn.gzmigu.cn

find . -name "*.log" -type f
来源：http://xz.muxihuayi.cn

[R44] 按修改时间查找
来源：http://ly.szsharing.cn

find . -mtime -7 -type f
来源：http://px.shtwfgs.cn

[R45] 批量删除
来源：http://kk.521024.cn

find . -name "*.tmp" -delete
来源：http://oh.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://iy.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kb.hnjuh.cn

[R47] sed 单行替换
来源：http://di.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://el.jctech888.com.cn

[R48] awk 取指定列
来源：http://fh.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://cu.newstarts.cn

[R49] awk 带条件
来源：http://xu.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kl.lnxyls.cn

[R50] awk 求和
来源：http://ph.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://in.lnxyls.cn

[R51] 排序去重取前几
来源：http://zg.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fb.nicolike.cn

[R52] 统计行数
来源：http://tx.huixiangedu.cn

wc -l a.txt
来源：http://ww.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://zc.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dc.nicolike.cn

[R54] 比较两个文件
来源：http://kt.yuntaijiaju.cn

diff a.txt b.txt
来源：http://il.521024.cn

[R55] 压缩与解压
来源：http://ug.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jz.nszjky.cn

[R56] 远程拷贝
来源：http://al.jianghongdianzi.cn

scp file user@host:/path/
来源：http://hm.gzmigu.cn

[R57] 远程执行命令
来源：http://rk.hahajie.cn

ssh user@host 'uptime'
来源：http://mr.yuexingan06.cn

[R58] 下载文件
来源：http://af.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vf.chemitech.net.cn

[R59] 发 POST JSON
来源：http://ca.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ll.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://yv.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mv.newstarts.cn

[R61] 磁盘占用
来源：http://oa.jctech888.com.cn

df -h;  du -sh *
来源：http://yt.hahajie.cn

[R62] 找最占空间的文件
来源：http://ug.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://yg.nszjky.cn

[R63] 内存与进程
来源：http://tb.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://qg.nicolike.cn

[R64] 结束进程
来源：http://zg.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://ms.szxytkj.cn

[R65] 查看端口占用
来源：http://az.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ty.szsharing.cn

[R66] 定时任务
来源：http://sv.shxzskj.cn

crontab -e;  crontab -l
来源：http://cq.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://tv.newstarts.cn


<!-- 参考信息 -->