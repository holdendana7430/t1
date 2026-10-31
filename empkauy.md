代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rc.nszjky.cn

[Q18] 模糊匹配
来源：http://lp.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ki.hnjuh.cn

[Q19] 范围查询
来源：http://jt.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sk.colortex.cn

[Q20] IN 列表
来源：http://cl.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hd.muxihuayi.cn

[Q21] 空值判断
来源：http://rt.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jq.jctech888.com.cn

[Q22] 排序
来源：http://ll.newstarts.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aa.shxzukj.cn

[Q23] 分页
来源：http://zi.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dx.yuexingan06.cn

[Q24] 去重
来源：http://tg.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://zr.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://ws.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wk.9csxet.cn

[Q26] 计数
来源：http://vy.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://gq.haigaiapp.cn

[Q27] 条件计数
来源：http://rd.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aq.shtwfgs.cn

[Q28] 求和与平均
来源：http://ll.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mr.lnxyls.cn

[Q29] 最大最小值
来源：http://xr.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vn.lnxyls.cn

[Q30] 分组统计
来源：http://jo.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ru.bjjhwx.cn

[Q31] 分组后过滤
来源：http://ns.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vr.colortex.cn

[Q32] 分组拼接字符串
来源：http://qs.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xd.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fq.jctech888.com.cn

[Q33] 多列分组
来源：http://ck.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fc.nicolike.cn

[Q34] 每组取第一条
来源：http://rc.colortex.cn

SELECT * FROM (
来源：http://ro.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tp.shxzukj.cn

) t WHERE rn = 1;
来源：http://du.huixiangedu.cn

[Q35] 内连接
来源：http://me.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vn.chemitech.net.cn

[Q36] 左连接
来源：http://hr.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jx.gzmigu.cn

[Q37] 右连接
来源：http://ry.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nh.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zb.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ov.yuntaijiaju.cn

[Q39] 自连接（查上下级）
来源：http://cz.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://et.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vg.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mb.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lu.wgjwhj.cn

[Q41] 多表连接
来源：http://lh.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kd.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://wr.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://rm.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://pp.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://jh.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tj.lnxyls.cn

[Q43] 标量子查询
来源：http://rg.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ds.521024.cn

[Q44] IN 子查询
来源：http://sy.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qb.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://up.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mx.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://he.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ux.newstarts.cn

[Q47] 与平均值比较
来源：http://jn.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yt.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://vr.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vc.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://yh.panjiajie.cn

[Q49] 更新单行
来源：http://ol.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://im.lnxyls.cn

[Q50] 批量更新
来源：http://by.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://da.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://ii.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oi.chemitech.net.cn

[Q52] 删除指定行
来源：http://qi.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://hp.szsharing.cn

[Q53] 按条件删除
来源：http://dh.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dy.nicolike.cn

[Q54] 清空表
来源：http://sn.nszjky.cn

TRUNCATE TABLE logs;
来源：http://py.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://qu.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xq.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://zw.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://js.jctech888.com.cn

[Q57] 行号
来源：http://fg.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ap.huixiangedu.cn

[Q58] 累计求和
来源：http://dx.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ur.shtwfgs.cn

[Q59] 分组内累计
来源：http://mj.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oz.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://ch.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rj.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zt.lnxyls.cn

[Q61] 移动平均
来源：http://bl.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mv.bookmarksfly.cn

[Q62] 分组占比
来源：http://vj.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nq.shxzskj.cn

[Q63] 开启事务
来源：http://ym.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yr.shxzukj.cn

[Q64] 提交事务
来源：http://rm.bjjhwx.cn

COMMIT;
来源：http://nt.panjiajie.cn

[Q65] 回滚事务
来源：http://ka.huixinmuqiang.cn

ROLLBACK;
来源：http://fr.nszjky.cn

[Q66] 行锁查询
来源：http://ph.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zx.gzmigu.cn

[Q67] 设置隔离级别
来源：http://ws.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jq.panjiajie.cn

[Q68] 保存点
来源：http://gd.lnxyls.cn

SAVEPOINT sp1;
来源：http://af.lnxyls.cn

ROLLBACK TO sp1;
来源：http://er.szsharing.cn

[Q69] 查看执行计划
来源：http://sl.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ys.szsharing.cn

[Q70] 更新统计信息
来源：http://ti.hnjuh.cn

ANALYZE TABLE users;
来源：http://xb.shtwfgs.cn

[Q71] 查看建表语句
来源：http://io.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fk.gzmigu.cn

[Q72] 查看索引
来源：http://gp.szsharing.cn

SHOW INDEX FROM users;
来源：http://ih.szsharing.cn

[Q73] 查看表状态
来源：http://uq.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sm.wgjwhj.cn

[Q74] 强制使用索引
来源：http://fp.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rx.nszjky.cn

[Q75] 日期格式化
来源：http://iy.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://en.huanxung.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ae.colortex.cn

[Q76] 按天统计
来源：http://ao.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://el.asd995.cn

[Q77] 时间加减
来源：http://ij.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://as.9csxet.cn

[Q78] 当前时间
来源：http://pc.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vo.hnjuh.cn

[Q79] 字符串拼接
来源：http://mb.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lw.haigaiapp.cn

[Q80] 字符串截取
来源：http://lc.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iz.521024.cn

[Q81] 字符串替换
来源：http://am.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xc.521024.cn

[Q82] 字符长度与字节长度
来源：http://lg.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ci.huixiangedu.cn

[Q83] 大小写转换
来源：http://tm.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hf.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://mt.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://fe.gzmigu.cn

[Q85] 数值取整
来源：http://iw.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xk.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://jc.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xp.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://oc.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yw.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://fa.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gk.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jj.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://vo.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://df.bjjhwx.cn

[Q90] 生成序号列
来源：http://ls.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mo.colortex.cn

================================================================================
来源：http://dn.szsharing.cn

R. Bash 专题
来源：http://jo.huixinmuqiang.cn

================================================================================
来源：http://na.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://ag.chemitech.net.cn

#!/usr/bin/env bash
来源：http://lf.lnxyls.cn

set -euo pipefail
来源：http://bj.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://xo.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://sj.nszjky.cn

[R03] 只读变量
来源：http://ei.muxihuayi.cn

readonly PI=3.14
来源：http://jd.jianghongdianzi.cn

[R04] 位置参数
来源：http://oy.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cg.nicolike.cn

[R05] 参数默认值
来源：http://lt.newstarts.cn

name="${1:-default}"
来源：http://tu.newstarts.cn

[R06] 判断命令是否存在
来源：http://oi.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ig.wgjwhj.cn

[R07] if 判断文件
来源：http://gd.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://td.shxzskj.cn

[R08] 数值比较
来源：http://nl.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yb.haigaiapp.cn

[R09] 字符串比较
来源：http://pt.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zr.szxytkj.cn

[R10] 正则匹配
来源：http://ft.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vp.shxzukj.cn

[R11] case 多分支
来源：http://ao.wgjwhj.cn

case "$1" in
来源：http://os.chemitech.net.cn

start) echo "启动" ;;
来源：http://ej.hnjuh.cn

stop)  echo "停止" ;;
来源：http://vg.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://ad.shxzukj.cn

esac
来源：http://pq.asd995.cn

[R12] for 遍历文件
来源：http://xz.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://bb.lnxyls.cn

[R13] for 计数循环
来源：http://dj.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://lt.gzmigu.cn

[R14] C 风格 for
来源：http://xt.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yb.panjiajie.cn

[R15] while 逐行读文件
来源：http://hw.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pf.nicolike.cn

[R16] until 等待条件
来源：http://zl.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zj.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://yk.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://td.szsharing.cn

[R18] 遍历数组
来源：http://sv.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kl.nicolike.cn

[R19] 数组长度
来源：http://ks.huixiangedu.cn

echo "${#arr[@]}"
来源：http://zu.colortex.cn

[R20] 关联数组（字典）
来源：http://ao.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fk.shtwfgs.cn

[R21] 字符串长度
来源：http://ko.haigaiapp.cn

echo "${#s}"
来源：http://fr.muxihuayi.cn

[R22] 截取子串
来源：http://du.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://sa.bookmarksfly.cn

[R23] 字符串替换
来源：http://lm.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cm.gzmigu.cn

[R24] 大小写转换
来源：http://ol.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pk.521024.cn

[R25] 去后缀 / 去前缀
来源：http://yr.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yz.hnjuh.cn

[R26] 命令替换
来源：http://xw.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://sw.lnxyls.cn

[R27] 算术展开
来源：http://gx.colortex.cn

echo $((1 + 2 * 3))
来源：http://dv.huixinmuqiang.cn

[R28] 浮点运算
来源：http://cz.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://ep.huixiangedu.cn

[R29] 定义函数
来源：http://op.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zr.yuntaijiaju.cn

[R30] 函数返回状态码
来源：http://rq.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://ql.newstarts.cn

[R31] 局部变量
来源：http://th.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://hk.wgjwhj.cn

[R32] 参数个数校验
来源：http://hf.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rh.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://aq.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qm.panjiajie.cn

[R34] 退出时清理
来源：http://uk.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wk.szxytkj.cn

[R35] 后台执行并等待
来源：http://hc.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sw.lnxyls.cn

[R36] 并发执行多个任务
来源：http://ia.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sg.nszjky.cn

[R37] 把输出赋给变量
来源：http://er.bookmarksfly.cn

files=$(ls -1)
来源：http://zp.bookmarksfly.cn

[R38] 管道串联
来源：http://hp.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://td.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://gb.haigaiapp.cn

cmd > out.log 2>&1
来源：http://lb.shxzskj.cn

[R40] 追加写日志
来源：http://nc.gzmigu.cn

echo "log" >> out.log
来源：http://gv.szxytkj.cn

[R41] 丢弃输出
来源：http://wl.huanxung.cn

cmd >/dev/null 2>&1
来源：http://pd.bjjhwx.cn

[R42] 输入重定向
来源：http://eb.panjiajie.cn

wc -l < a.txt
来源：http://sd.szxytkj.cn

[R43] 按名字查找文件
来源：http://fk.asd995.cn

find . -name "*.log" -type f
来源：http://xl.9csxet.cn

[R44] 按修改时间查找
来源：http://fo.huanxung.cn

find . -mtime -7 -type f
来源：http://au.shxzskj.cn

[R45] 批量删除
来源：http://gp.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://fg.colortex.cn

[R46] 递归替换文件内容
来源：http://na.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hd.nszjky.cn

[R47] sed 单行替换
来源：http://es.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yp.szxytkj.cn

[R48] awk 取指定列
来源：http://uv.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://oj.szsharing.cn

[R49] awk 带条件
来源：http://ur.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dj.shxzskj.cn

[R50] awk 求和
来源：http://rk.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qf.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://sk.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vw.nszjky.cn

[R52] 统计行数
来源：http://qs.panjiajie.cn

wc -l a.txt
来源：http://li.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://at.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yj.jctech888.com.cn

[R54] 比较两个文件
来源：http://bw.nszjky.cn

diff a.txt b.txt
来源：http://yz.nicolike.cn

[R55] 压缩与解压
来源：http://no.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sk.szsharing.cn

[R56] 远程拷贝
来源：http://ep.szsharing.cn

scp file user@host:/path/
来源：http://xt.shxzskj.cn

[R57] 远程执行命令
来源：http://vj.shxzukj.cn

ssh user@host 'uptime'
来源：http://vt.jianghongdianzi.cn

[R58] 下载文件
来源：http://xz.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fq.yuexingan06.cn

[R59] 发 POST JSON
来源：http://qo.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oh.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://ym.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mq.yuexingan06.cn

[R61] 磁盘占用
来源：http://wu.jctech888.com.cn

df -h;  du -sh *
来源：http://pj.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://db.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://qm.shxzukj.cn

[R63] 内存与进程
来源：http://dz.521024.cn

free -h;  ps aux | grep nginx
来源：http://xy.521024.cn

[R64] 结束进程
来源：http://ho.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://xp.szxytkj.cn

[R65] 查看端口占用
来源：http://ik.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wz.panjiajie.cn

[R66] 定时任务
来源：http://ta.panjiajie.cn

crontab -e;  crontab -l
来源：http://pe.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://fe.521024.cn


<!-- 参考信息 -->