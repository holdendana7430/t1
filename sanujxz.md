代发 wailian999

SELECT * FROM users;
来源：http://iw.lnxyls.cn

[Q16] 查询指定列
来源：http://jd.wgjwhj.cn

SELECT id, name FROM users;
来源：http://sn.jctech888.com.cn

[Q17] 条件查询
来源：http://tl.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cw.huixiangedu.cn

[Q18] 模糊匹配
来源：http://ob.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yz.panjiajie.cn

[Q19] 范围查询
来源：http://jj.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ph.lnxyls.cn

[Q20] IN 列表
来源：http://zi.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bh.muxihuayi.cn

[Q21] 空值判断
来源：http://mr.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://iy.shtwfgs.cn

[Q22] 排序
来源：http://ey.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wy.lnxyls.cn

[Q23] 分页
来源：http://in.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bq.panjiajie.cn

[Q24] 去重
来源：http://px.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://jt.9csxet.cn

[Q25] 只取前 N 条
来源：http://hs.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ny.asd995.cn

[Q26] 计数
来源：http://fb.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://oj.asd995.cn

[Q27] 条件计数
来源：http://cm.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jl.521024.cn

[Q28] 求和与平均
来源：http://wu.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://go.521024.cn

[Q29] 最大最小值
来源：http://nr.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zf.shxzskj.cn

[Q30] 分组统计
来源：http://xk.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cx.hahajie.cn

[Q31] 分组后过滤
来源：http://nm.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oy.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://kh.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kc.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hj.huixinmuqiang.cn

[Q33] 多列分组
来源：http://cm.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mz.haigaiapp.cn

[Q34] 每组取第一条
来源：http://kw.bookmarksfly.cn

SELECT * FROM (
来源：http://sw.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xk.huanxung.cn

) t WHERE rn = 1;
来源：http://iq.shxzukj.cn

[Q35] 内连接
来源：http://ky.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pb.muxihuayi.cn

[Q36] 左连接
来源：http://pk.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ix.jianghongdianzi.cn

[Q37] 右连接
来源：http://ro.panjiajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://af.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jm.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ui.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://ea.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gl.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dg.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bo.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://og.asd995.cn

[Q41] 多表连接
来源：http://tn.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kq.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://vy.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://df.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://vs.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://tl.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zx.huixiangedu.cn

[Q43] 标量子查询
来源：http://yo.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hd.muxihuayi.cn

[Q44] IN 子查询
来源：http://ia.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wb.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://fn.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xp.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cb.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mh.muxihuayi.cn

[Q47] 与平均值比较
来源：http://jm.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bf.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://tx.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lp.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://hs.szsharing.cn

[Q49] 更新单行
来源：http://cm.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://up.yuexingan06.cn

[Q50] 批量更新
来源：http://oz.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gj.muxihuayi.cn

[Q51] 用子查询更新
来源：http://da.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ox.hahajie.cn

[Q52] 删除指定行
来源：http://kn.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://zk.521024.cn

[Q53] 按条件删除
来源：http://gy.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mp.nszjky.cn

[Q54] 清空表
来源：http://sd.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://px.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://km.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://km.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://fd.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oe.szsharing.cn

[Q57] 行号
来源：http://ta.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ay.chemitech.net.cn

[Q58] 累计求和
来源：http://nf.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cm.bjjhwx.cn

[Q59] 分组内累计
来源：http://yy.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ls.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://uj.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mu.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tz.colortex.cn

[Q61] 移动平均
来源：http://lm.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mi.nicolike.cn

[Q62] 分组占比
来源：http://eu.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vb.shtwfgs.cn

[Q63] 开启事务
来源：http://ij.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fu.huixiangedu.cn

[Q64] 提交事务
来源：http://wk.hahajie.cn

COMMIT;
来源：http://jk.chemitech.net.cn

[Q65] 回滚事务
来源：http://aq.szxytkj.cn

ROLLBACK;
来源：http://km.huanxung.cn

[Q66] 行锁查询
来源：http://tc.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bu.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://ms.lnxyls.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tv.newstarts.cn

[Q68] 保存点
来源：http://ig.haigaiapp.cn

SAVEPOINT sp1;
来源：http://is.panjiajie.cn

ROLLBACK TO sp1;
来源：http://bw.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://xl.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nw.yuexingan06.cn

[Q70] 更新统计信息
来源：http://bb.szsharing.cn

ANALYZE TABLE users;
来源：http://cl.bjjhwx.cn

[Q71] 查看建表语句
来源：http://xj.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ci.nszjky.cn

[Q72] 查看索引
来源：http://xp.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://qt.yuexingan06.cn

[Q73] 查看表状态
来源：http://ay.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wy.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://yb.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lc.gzmigu.cn

[Q75] 日期格式化
来源：http://ft.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xg.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bv.colortex.cn

[Q76] 按天统计
来源：http://wc.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eo.hahajie.cn

[Q77] 时间加减
来源：http://rl.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ec.lnxyls.cn

[Q78] 当前时间
来源：http://qn.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kv.shxzskj.cn

[Q79] 字符串拼接
来源：http://au.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zv.shxzskj.cn

[Q80] 字符串截取
来源：http://us.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kp.shxzskj.cn

[Q81] 字符串替换
来源：http://iz.yuexingan06.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yi.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://bw.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yy.jctech888.com.cn

[Q83] 大小写转换
来源：http://lp.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xv.szsharing.cn

[Q84] 去除首尾空格
来源：http://kj.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://cv.huanxung.cn

[Q85] 数值取整
来源：http://co.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ab.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://ii.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cq.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://wk.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aw.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://zk.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gv.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yi.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://mj.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ii.chemitech.net.cn

[Q90] 生成序号列
来源：http://ho.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jh.colortex.cn

================================================================================
来源：http://gq.shxzukj.cn

R. Bash 专题
来源：http://dg.chemitech.net.cn

================================================================================
来源：http://tb.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://md.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://fw.521024.cn

set -euo pipefail
来源：http://oy.9csxet.cn

[R02] 变量赋值与使用
来源：http://lv.9csxet.cn

name="Tom"; echo "$name"
来源：http://tz.jctech888.com.cn

[R03] 只读变量
来源：http://wq.jctech888.com.cn

readonly PI=3.14
来源：http://th.huixiangedu.cn

[R04] 位置参数
来源：http://lj.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://je.nicolike.cn

[R05] 参数默认值
来源：http://bp.asd995.cn

name="${1:-default}"
来源：http://cw.colortex.cn

[R06] 判断命令是否存在
来源：http://cw.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ms.shxzskj.cn

[R07] if 判断文件
来源：http://om.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://em.bookmarksfly.cn

[R08] 数值比较
来源：http://od.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hc.shtwfgs.cn

[R09] 字符串比较
来源：http://cs.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ze.szxytkj.cn

[R10] 正则匹配
来源：http://re.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ep.asd995.cn

[R11] case 多分支
来源：http://fl.huixiangedu.cn

case "$1" in
来源：http://wd.jctech888.com.cn

start) echo "启动" ;;
来源：http://qm.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://ku.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://fp.shtwfgs.cn

esac
来源：http://zl.colortex.cn

[R12] for 遍历文件
来源：http://ud.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://hr.shxzukj.cn

[R13] for 计数循环
来源：http://ah.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://ua.hahajie.cn

[R14] C 风格 for
来源：http://yn.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bk.gzmigu.cn

[R15] while 逐行读文件
来源：http://uu.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dv.bookmarksfly.cn

[R16] until 等待条件
来源：http://ad.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jx.gzmigu.cn

[R17] 数组定义与取值
来源：http://ya.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zt.yuntaijiaju.cn

[R18] 遍历数组
来源：http://fr.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qh.chemitech.net.cn

[R19] 数组长度
来源：http://yp.chemitech.net.cn

echo "${#arr[@]}"
来源：http://dm.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://lq.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://op.colortex.cn

[R21] 字符串长度
来源：http://yr.wgjwhj.cn

echo "${#s}"
来源：http://uz.shxzukj.cn

[R22] 截取子串
来源：http://jb.huanxung.cn

echo "${s:0:5}"
来源：http://xs.yuexingan06.cn

[R23] 字符串替换
来源：http://sd.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ry.huixiangedu.cn

[R24] 大小写转换
来源：http://yt.nszjky.cn

echo "${s^^}"; echo "${s,,}"
来源：http://by.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://xx.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ew.lnxyls.cn

[R26] 命令替换
来源：http://qs.colortex.cn

now=$(date +%F); echo "$now"
来源：http://rp.muxihuayi.cn

[R27] 算术展开
来源：http://cb.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://wh.wgjwhj.cn

[R28] 浮点运算
来源：http://jt.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://hb.shxzskj.cn

[R29] 定义函数
来源：http://fs.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ku.panjiajie.cn

[R30] 函数返回状态码
来源：http://og.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://gp.hahajie.cn

[R31] 局部变量
来源：http://pj.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://vz.bjjhwx.cn

[R32] 参数个数校验
来源：http://yg.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qd.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://re.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sd.521024.cn

[R34] 退出时清理
来源：http://ld.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fu.shxzukj.cn

[R35] 后台执行并等待
来源：http://cd.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jw.shxzukj.cn

[R36] 并发执行多个任务
来源：http://ti.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cw.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://tu.bjjhwx.cn

files=$(ls -1)
来源：http://ts.huixinmuqiang.cn

[R38] 管道串联
来源：http://zu.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://il.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://gv.colortex.cn

cmd > out.log 2>&1
来源：http://ri.jctech888.com.cn

[R40] 追加写日志
来源：http://ir.9csxet.cn

echo "log" >> out.log
来源：http://lf.9csxet.cn

[R41] 丢弃输出
来源：http://uh.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://gy.lnxyls.cn

[R42] 输入重定向
来源：http://ep.shxzukj.cn

wc -l < a.txt
来源：http://ix.jctech888.com.cn

[R43] 按名字查找文件
来源：http://wi.huanxung.cn

find . -name "*.log" -type f
来源：http://ug.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://sy.lnxyls.cn

find . -mtime -7 -type f
来源：http://ng.hahajie.cn

[R45] 批量删除
来源：http://eb.huanxung.cn

find . -name "*.tmp" -delete
来源：http://zg.lnxyls.cn

[R46] 递归替换文件内容
来源：http://by.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xh.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://zd.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gl.hahajie.cn

[R48] awk 取指定列
来源：http://lt.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://fm.jianghongdianzi.cn

[R49] awk 带条件
来源：http://jt.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wz.lnxyls.cn

[R50] awk 求和
来源：http://qd.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bp.szsharing.cn

[R51] 排序去重取前几
来源：http://yz.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://al.shtwfgs.cn

[R52] 统计行数
来源：http://np.nicolike.cn

wc -l a.txt
来源：http://yt.asd995.cn

[R53] 查看文件头与实时尾
来源：http://uj.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ix.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://zx.bookmarksfly.cn

diff a.txt b.txt
来源：http://wd.bookmarksfly.cn

[R55] 压缩与解压
来源：http://qa.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kc.jctech888.com.cn

[R56] 远程拷贝
来源：http://mk.shxzskj.cn

scp file user@host:/path/
来源：http://iz.haigaiapp.cn

[R57] 远程执行命令
来源：http://yx.hahajie.cn

ssh user@host 'uptime'
来源：http://dd.nicolike.cn

[R58] 下载文件
来源：http://ya.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dp.muxihuayi.cn

[R59] 发 POST JSON
来源：http://ml.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qq.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://lc.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ig.panjiajie.cn

[R61] 磁盘占用
来源：http://rq.huixiangedu.cn

df -h;  du -sh *
来源：http://te.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://dn.asd995.cn

du -ah . | sort -rh | head -10
来源：http://jh.colortex.cn

[R63] 内存与进程
来源：http://ub.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://yi.colortex.cn

[R64] 结束进程
来源：http://ku.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://sx.huanxung.cn

[R65] 查看端口占用
来源：http://kz.wgjwhj.cn


<!-- 参考信息 -->