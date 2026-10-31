代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://bn.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xt.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ow.yuexingan06.cn

[Q15] 查询全部
来源：http://tw.bjjhwx.cn

SELECT * FROM users;
来源：http://hj.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://yo.newstarts.cn

SELECT id, name FROM users;
来源：http://yp.szsharing.cn

[Q17] 条件查询
来源：http://qw.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vm.yuexingan06.cn

[Q18] 模糊匹配
来源：http://dg.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mn.muxihuayi.cn

[Q19] 范围查询
来源：http://ns.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ue.9csxet.cn

[Q20] IN 列表
来源：http://px.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tm.chemitech.net.cn

[Q21] 空值判断
来源：http://np.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://oz.bookmarksfly.cn

[Q22] 排序
来源：http://un.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zc.huanxung.cn

[Q23] 分页
来源：http://sc.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uz.521024.cn

[Q24] 去重
来源：http://ph.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://fp.shxzskj.cn

[Q25] 只取前 N 条
来源：http://ay.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cr.asd995.cn

[Q26] 计数
来源：http://cn.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://oo.wgjwhj.cn

[Q27] 条件计数
来源：http://zu.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nm.9csxet.cn

[Q28] 求和与平均
来源：http://yf.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nr.shxzskj.cn

[Q29] 最大最小值
来源：http://qk.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bn.shtwfgs.cn

[Q30] 分组统计
来源：http://xn.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mn.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://vs.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cf.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://su.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hx.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qb.jctech888.com.cn

[Q33] 多列分组
来源：http://ka.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://he.huanxung.cn

[Q34] 每组取第一条
来源：http://wq.muxihuayi.cn

SELECT * FROM (
来源：http://nq.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gi.wgjwhj.cn

) t WHERE rn = 1;
来源：http://ik.colortex.cn

[Q35] 内连接
来源：http://au.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wc.yuntaijiaju.cn

[Q36] 左连接
来源：http://ul.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mg.yuntaijiaju.cn

[Q37] 右连接
来源：http://lr.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://de.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zq.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ir.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://xp.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nv.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mb.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fg.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://et.asd995.cn

[Q41] 多表连接
来源：http://xl.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xa.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://dl.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://fh.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://mf.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://la.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oe.huixiangedu.cn

[Q43] 标量子查询
来源：http://rb.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pj.szsharing.cn

[Q44] IN 子查询
来源：http://eu.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kh.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://ht.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://io.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pu.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ac.9csxet.cn

[Q47] 与平均值比较
来源：http://ei.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ht.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://xm.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lu.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://ar.hahajie.cn

[Q49] 更新单行
来源：http://ii.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jv.9csxet.cn

[Q50] 批量更新
来源：http://po.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wq.521024.cn

[Q51] 用子查询更新
来源：http://yd.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ei.lnxyls.cn

[Q52] 删除指定行
来源：http://jq.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://va.wgjwhj.cn

[Q53] 按条件删除
来源：http://xw.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vx.jianghongdianzi.cn

[Q54] 清空表
来源：http://zy.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://bh.newstarts.cn

[Q55] 排名（并列占位）
来源：http://wh.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jk.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://ps.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xe.haigaiapp.cn

[Q57] 行号
来源：http://lh.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gt.yuntaijiaju.cn

[Q58] 累计求和
来源：http://de.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xm.nicolike.cn

[Q59] 分组内累计
来源：http://ge.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ti.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://cd.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ei.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ha.szsharing.cn

[Q61] 移动平均
来源：http://hk.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fq.gzmigu.cn

[Q62] 分组占比
来源：http://el.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sg.shxzukj.cn

[Q63] 开启事务
来源：http://tu.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bl.newstarts.cn

[Q64] 提交事务
来源：http://ty.nicolike.cn

COMMIT;
来源：http://zu.nszjky.cn

[Q65] 回滚事务
来源：http://hw.shxzukj.cn

ROLLBACK;
来源：http://bn.bjjhwx.cn

[Q66] 行锁查询
来源：http://xm.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mq.huanxung.cn

[Q67] 设置隔离级别
来源：http://zm.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eb.haigaiapp.cn

[Q68] 保存点
来源：http://ea.panjiajie.cn

SAVEPOINT sp1;
来源：http://uo.shxzskj.cn

ROLLBACK TO sp1;
来源：http://of.hahajie.cn

[Q69] 查看执行计划
来源：http://uy.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mf.hnjuh.cn

[Q70] 更新统计信息
来源：http://gk.hahajie.cn

ANALYZE TABLE users;
来源：http://vm.9csxet.cn

[Q71] 查看建表语句
来源：http://gb.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iy.nszjky.cn

[Q72] 查看索引
来源：http://fw.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://xx.shxzskj.cn

[Q73] 查看表状态
来源：http://ot.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hi.lnxyls.cn

[Q74] 强制使用索引
来源：http://zf.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pw.521024.cn

[Q75] 日期格式化
来源：http://jl.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wz.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ra.huixinmuqiang.cn

[Q76] 按天统计
来源：http://fw.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ex.muxihuayi.cn

[Q77] 时间加减
来源：http://we.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xl.nicolike.cn

[Q78] 当前时间
来源：http://oh.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wn.9csxet.cn

[Q79] 字符串拼接
来源：http://xx.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jr.wgjwhj.cn

[Q80] 字符串截取
来源：http://zn.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ad.colortex.cn

[Q81] 字符串替换
来源：http://tv.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rs.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://dl.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gp.9csxet.cn

[Q83] 大小写转换
来源：http://xf.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gg.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://to.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://la.shxzukj.cn

[Q85] 数值取整
来源：http://zz.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gc.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://yp.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kc.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://lb.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hc.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://pl.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cb.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ms.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://hj.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tt.haigaiapp.cn

[Q90] 生成序号列
来源：http://ug.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qo.nicolike.cn

================================================================================
来源：http://ni.bookmarksfly.cn

R. Bash 专题
来源：http://gw.nszjky.cn

================================================================================
来源：http://ne.shxzukj.cn

[R01] shebang 与严格模式
来源：http://gk.huixiangedu.cn

#!/usr/bin/env bash
来源：http://fo.haigaiapp.cn

set -euo pipefail
来源：http://ak.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://zd.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://ut.yuexingan06.cn

[R03] 只读变量
来源：http://wk.chemitech.net.cn

readonly PI=3.14
来源：http://gf.hahajie.cn

[R04] 位置参数
来源：http://to.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fu.nicolike.cn

[R05] 参数默认值
来源：http://py.gzmigu.cn

name="${1:-default}"
来源：http://zy.huanxung.cn

[R06] 判断命令是否存在
来源：http://sm.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uf.nszjky.cn

[R07] if 判断文件
来源：http://ju.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bb.colortex.cn

[R08] 数值比较
来源：http://ng.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bu.jctech888.com.cn

[R09] 字符串比较
来源：http://nx.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bf.521024.cn

[R10] 正则匹配
来源：http://bj.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dt.yuntaijiaju.cn

[R11] case 多分支
来源：http://bc.muxihuayi.cn

case "$1" in
来源：http://vr.hahajie.cn

start) echo "启动" ;;
来源：http://up.521024.cn

stop)  echo "停止" ;;
来源：http://lb.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://ro.shtwfgs.cn

esac
来源：http://pu.asd995.cn

[R12] for 遍历文件
来源：http://ag.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://fu.yuntaijiaju.cn

[R13] for 计数循环
来源：http://dc.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://ac.nszjky.cn

[R14] C 风格 for
来源：http://sg.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pt.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://zp.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://du.bjjhwx.cn

[R16] until 等待条件
来源：http://ij.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cg.bjjhwx.cn

[R17] 数组定义与取值
来源：http://sq.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rj.jctech888.com.cn

[R18] 遍历数组
来源：http://bq.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cu.shxzskj.cn

[R19] 数组长度
来源：http://hn.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://js.shxzukj.cn

[R20] 关联数组（字典）
来源：http://en.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zk.panjiajie.cn

[R21] 字符串长度
来源：http://rk.muxihuayi.cn

echo "${#s}"
来源：http://hl.huixinmuqiang.cn

[R22] 截取子串
来源：http://dz.colortex.cn

echo "${s:0:5}"
来源：http://jk.yuntaijiaju.cn

[R23] 字符串替换
来源：http://zv.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kx.asd995.cn

[R24] 大小写转换
来源：http://lu.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hh.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://pt.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pb.wgjwhj.cn

[R26] 命令替换
来源：http://pu.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://at.yuexingan06.cn

[R27] 算术展开
来源：http://or.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://ru.bjjhwx.cn

[R28] 浮点运算
来源：http://eb.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://ln.hahajie.cn

[R29] 定义函数
来源：http://ie.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qy.hnjuh.cn

[R30] 函数返回状态码
来源：http://su.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://ax.nicolike.cn

[R31] 局部变量
来源：http://cs.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://wm.haigaiapp.cn

[R32] 参数个数校验
来源：http://gk.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vv.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://nh.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zn.szsharing.cn

[R34] 退出时清理
来源：http://er.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ub.bjjhwx.cn

[R35] 后台执行并等待
来源：http://rq.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lf.panjiajie.cn

[R36] 并发执行多个任务
来源：http://uw.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ig.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://vg.jctech888.com.cn

files=$(ls -1)
来源：http://gd.521024.cn

[R38] 管道串联
来源：http://ek.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://ja.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://bw.wgjwhj.cn

cmd > out.log 2>&1
来源：http://yp.gzmigu.cn

[R40] 追加写日志
来源：http://xx.shxzukj.cn

echo "log" >> out.log
来源：http://kx.panjiajie.cn

[R41] 丢弃输出
来源：http://rc.9csxet.cn

cmd >/dev/null 2>&1
来源：http://mi.huixiangedu.cn

[R42] 输入重定向
来源：http://rg.jctech888.com.cn

wc -l < a.txt
来源：http://fi.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://oz.9csxet.cn

find . -name "*.log" -type f
来源：http://zc.szxytkj.cn

[R44] 按修改时间查找
来源：http://as.shtwfgs.cn

find . -mtime -7 -type f
来源：http://hj.huixinmuqiang.cn

[R45] 批量删除
来源：http://uv.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://rc.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://gb.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vs.asd995.cn

[R47] sed 单行替换
来源：http://yd.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ya.bjjhwx.cn

[R48] awk 取指定列
来源：http://wk.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://sx.nszjky.cn

[R49] awk 带条件
来源：http://tg.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vm.panjiajie.cn

[R50] awk 求和
来源：http://vj.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://eb.lnxyls.cn

[R51] 排序去重取前几
来源：http://ps.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hw.colortex.cn

[R52] 统计行数
来源：http://st.huanxung.cn

wc -l a.txt
来源：http://ep.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://ej.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rf.huanxung.cn

[R54] 比较两个文件
来源：http://cb.newstarts.cn

diff a.txt b.txt
来源：http://ih.panjiajie.cn

[R55] 压缩与解压
来源：http://yj.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ky.panjiajie.cn

[R56] 远程拷贝
来源：http://ye.chemitech.net.cn

scp file user@host:/path/
来源：http://vk.chemitech.net.cn

[R57] 远程执行命令
来源：http://la.hahajie.cn

ssh user@host 'uptime'
来源：http://bj.yuntaijiaju.cn

[R58] 下载文件
来源：http://hk.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zk.newstarts.cn

[R59] 发 POST JSON
来源：http://oq.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qr.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://er.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hw.bjjhwx.cn

[R61] 磁盘占用
来源：http://yc.nicolike.cn

df -h;  du -sh *
来源：http://hm.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://lr.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://pf.yuntaijiaju.cn

[R63] 内存与进程
来源：http://su.muxihuayi.cn


<!-- 参考信息 -->