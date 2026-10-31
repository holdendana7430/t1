代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://ur.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xw.9csxet.cn

[Q13] 忽略重复插入
来源：http://vz.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bq.521024.cn

[Q14] 存在则更新（upsert）
来源：http://kt.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://up.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dl.nszjky.cn

[Q15] 查询全部
来源：http://nt.asd995.cn

SELECT * FROM users;
来源：http://zt.521024.cn

[Q16] 查询指定列
来源：http://lz.szsharing.cn

SELECT id, name FROM users;
来源：http://fl.huanxung.cn

[Q17] 条件查询
来源：http://ko.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ki.huixiangedu.cn

[Q18] 模糊匹配
来源：http://ke.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wp.gzmigu.cn

[Q19] 范围查询
来源：http://gp.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qr.jctech888.com.cn

[Q20] IN 列表
来源：http://mo.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://we.jianghongdianzi.cn

[Q21] 空值判断
来源：http://vo.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fp.yuexingan06.cn

[Q22] 排序
来源：http://hx.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qv.szxytkj.cn

[Q23] 分页
来源：http://ik.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cb.huanxung.cn

[Q24] 去重
来源：http://pl.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://fm.asd995.cn

[Q25] 只取前 N 条
来源：http://mx.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://im.wgjwhj.cn

[Q26] 计数
来源：http://xk.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://tr.wgjwhj.cn

[Q27] 条件计数
来源：http://il.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bi.bookmarksfly.cn

[Q28] 求和与平均
来源：http://is.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zp.gzmigu.cn

[Q29] 最大最小值
来源：http://wt.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lc.shtwfgs.cn

[Q30] 分组统计
来源：http://xm.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://us.nszjky.cn

[Q31] 分组后过滤
来源：http://dv.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wf.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://tu.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lm.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://as.nicolike.cn

[Q33] 多列分组
来源：http://aj.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dc.muxihuayi.cn

[Q34] 每组取第一条
来源：http://gt.muxihuayi.cn

SELECT * FROM (
来源：http://sx.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cv.shxzukj.cn

) t WHERE rn = 1;
来源：http://bn.jianghongdianzi.cn

[Q35] 内连接
来源：http://fj.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ea.newstarts.cn

[Q36] 左连接
来源：http://wg.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uw.szsharing.cn

[Q37] 右连接
来源：http://yv.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ii.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zh.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bc.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://iw.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ji.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jr.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pf.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ak.shxzskj.cn

[Q41] 多表连接
来源：http://if.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dc.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://ql.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://ym.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://ru.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://qo.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qc.wgjwhj.cn

[Q43] 标量子查询
来源：http://bg.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jn.shtwfgs.cn

[Q44] IN 子查询
来源：http://my.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zz.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://tm.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hs.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fz.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://as.asd995.cn

[Q47] 与平均值比较
来源：http://bb.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ba.colortex.cn

[Q48] CTE 公用表表达式
来源：http://yb.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ry.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://pw.huixiangedu.cn

[Q49] 更新单行
来源：http://dz.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dv.wgjwhj.cn

[Q50] 批量更新
来源：http://hh.newstarts.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zw.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://ke.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cn.bjjhwx.cn

[Q52] 删除指定行
来源：http://ls.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://sp.huanxung.cn

[Q53] 按条件删除
来源：http://tf.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ux.huanxung.cn

[Q54] 清空表
来源：http://nn.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://sa.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://mf.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rj.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://jl.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bu.wgjwhj.cn

[Q57] 行号
来源：http://xz.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gg.newstarts.cn

[Q58] 累计求和
来源：http://ri.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uk.panjiajie.cn

[Q59] 分组内累计
来源：http://eq.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nm.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://rn.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eb.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qd.huixiangedu.cn

[Q61] 移动平均
来源：http://vr.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ej.shxzskj.cn

[Q62] 分组占比
来源：http://cg.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sk.jianghongdianzi.cn

[Q63] 开启事务
来源：http://ee.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gl.521024.cn

[Q64] 提交事务
来源：http://yh.huanxung.cn

COMMIT;
来源：http://um.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://ya.szsharing.cn

ROLLBACK;
来源：http://ar.lnxyls.cn

[Q66] 行锁查询
来源：http://lp.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vc.nicolike.cn

[Q67] 设置隔离级别
来源：http://cn.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oo.shtwfgs.cn

[Q68] 保存点
来源：http://pn.nicolike.cn

SAVEPOINT sp1;
来源：http://mr.huanxung.cn

ROLLBACK TO sp1;
来源：http://ve.szsharing.cn

[Q69] 查看执行计划
来源：http://dr.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ic.hahajie.cn

[Q70] 更新统计信息
来源：http://qn.nszjky.cn

ANALYZE TABLE users;
来源：http://vn.panjiajie.cn

[Q71] 查看建表语句
来源：http://uy.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ux.gzmigu.cn

[Q72] 查看索引
来源：http://te.shxzskj.cn

SHOW INDEX FROM users;
来源：http://fs.nszjky.cn

[Q73] 查看表状态
来源：http://se.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fx.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://cn.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ar.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://ed.szsharing.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sd.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sc.huixinmuqiang.cn

[Q76] 按天统计
来源：http://kr.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rm.asd995.cn

[Q77] 时间加减
来源：http://al.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ud.szsharing.cn

[Q78] 当前时间
来源：http://at.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hq.szxytkj.cn

[Q79] 字符串拼接
来源：http://qy.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://en.bookmarksfly.cn

[Q80] 字符串截取
来源：http://vs.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cx.huanxung.cn

[Q81] 字符串替换
来源：http://nw.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zh.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://ep.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xq.shxzskj.cn

[Q83] 大小写转换
来源：http://le.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ws.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://jj.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://tr.huixinmuqiang.cn

[Q85] 数值取整
来源：http://zo.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xg.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://yj.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://af.newstarts.cn

[Q87] JSON 字段做条件
来源：http://yl.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wn.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://fo.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zx.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zh.szsharing.cn

[Q89] 判断表是否存在
来源：http://oc.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zc.szsharing.cn

[Q90] 生成序号列
来源：http://wf.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wc.huixinmuqiang.cn

================================================================================
来源：http://vs.hahajie.cn

R. Bash 专题
来源：http://rj.szsharing.cn

================================================================================
来源：http://no.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://qc.bjjhwx.cn

#!/usr/bin/env bash
来源：http://ht.newstarts.cn

set -euo pipefail
来源：http://xd.gzmigu.cn

[R02] 变量赋值与使用
来源：http://gm.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://ig.9csxet.cn

[R03] 只读变量
来源：http://pw.shxzukj.cn

readonly PI=3.14
来源：http://ro.521024.cn

[R04] 位置参数
来源：http://fb.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rs.panjiajie.cn

[R05] 参数默认值
来源：http://wh.wgjwhj.cn

name="${1:-default}"
来源：http://zq.521024.cn

[R06] 判断命令是否存在
来源：http://ks.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hv.hnjuh.cn

[R07] if 判断文件
来源：http://mb.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gq.shxzukj.cn

[R08] 数值比较
来源：http://tg.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qb.yuntaijiaju.cn

[R09] 字符串比较
来源：http://wu.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ma.yuntaijiaju.cn

[R10] 正则匹配
来源：http://sn.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vl.newstarts.cn

[R11] case 多分支
来源：http://xa.shxzukj.cn

case "$1" in
来源：http://bx.muxihuayi.cn

start) echo "启动" ;;
来源：http://yb.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://ox.nszjky.cn

*)     echo "未知命令" ;;
来源：http://ip.szsharing.cn

esac
来源：http://kh.panjiajie.cn

[R12] for 遍历文件
来源：http://mz.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://vv.shxzskj.cn

[R13] for 计数循环
来源：http://vr.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://ir.lnxyls.cn

[R14] C 风格 for
来源：http://hi.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oa.szxytkj.cn

[R15] while 逐行读文件
来源：http://xh.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rv.nszjky.cn

[R16] until 等待条件
来源：http://wt.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sc.newstarts.cn

[R17] 数组定义与取值
来源：http://df.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uh.hahajie.cn

[R18] 遍历数组
来源：http://dt.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rz.nszjky.cn

[R19] 数组长度
来源：http://xz.chemitech.net.cn

echo "${#arr[@]}"
来源：http://vb.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://rt.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qc.bookmarksfly.cn

[R21] 字符串长度
来源：http://cw.muxihuayi.cn

echo "${#s}"
来源：http://qn.jctech888.com.cn

[R22] 截取子串
来源：http://oh.huanxung.cn

echo "${s:0:5}"
来源：http://nf.521024.cn

[R23] 字符串替换
来源：http://gg.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://en.shxzskj.cn

[R24] 大小写转换
来源：http://le.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gt.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://ui.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yg.shxzukj.cn

[R26] 命令替换
来源：http://gj.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://tc.9csxet.cn

[R27] 算术展开
来源：http://qi.huanxung.cn

echo $((1 + 2 * 3))
来源：http://gr.nszjky.cn

[R28] 浮点运算
来源：http://ik.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://vr.yuexingan06.cn

[R29] 定义函数
来源：http://oo.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pf.lnxyls.cn

[R30] 函数返回状态码
来源：http://sh.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://ql.newstarts.cn

[R31] 局部变量
来源：http://rs.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://ii.shtwfgs.cn

[R32] 参数个数校验
来源：http://ec.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ns.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://qw.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://by.nszjky.cn

[R34] 退出时清理
来源：http://fo.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eo.nicolike.cn

[R35] 后台执行并等待
来源：http://ap.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kd.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://kr.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ot.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://hp.wgjwhj.cn

files=$(ls -1)
来源：http://vd.gzmigu.cn

[R38] 管道串联
来源：http://ac.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://cc.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://ne.521024.cn

cmd > out.log 2>&1
来源：http://pw.hahajie.cn

[R40] 追加写日志
来源：http://jp.shxzukj.cn

echo "log" >> out.log
来源：http://bg.hnjuh.cn

[R41] 丢弃输出
来源：http://mn.nszjky.cn

cmd >/dev/null 2>&1
来源：http://kr.colortex.cn

[R42] 输入重定向
来源：http://ef.bjjhwx.cn

wc -l < a.txt
来源：http://js.szsharing.cn

[R43] 按名字查找文件
来源：http://od.asd995.cn

find . -name "*.log" -type f
来源：http://ah.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://ig.shxzukj.cn

find . -mtime -7 -type f
来源：http://oz.jianghongdianzi.cn

[R45] 批量删除
来源：http://hm.nicolike.cn

find . -name "*.tmp" -delete
来源：http://ls.lnxyls.cn

[R46] 递归替换文件内容
来源：http://ir.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oy.nszjky.cn

[R47] sed 单行替换
来源：http://gu.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uy.haigaiapp.cn

[R48] awk 取指定列
来源：http://ng.521024.cn

awk '{print $1, $3}' a.txt
来源：http://nq.shxzskj.cn

[R49] awk 带条件
来源：http://vr.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eq.shtwfgs.cn

[R50] awk 求和
来源：http://gy.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fz.nicolike.cn

[R51] 排序去重取前几
来源：http://lp.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nc.nszjky.cn

[R52] 统计行数
来源：http://wm.chemitech.net.cn

wc -l a.txt
来源：http://qz.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://er.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ha.nicolike.cn

[R54] 比较两个文件
来源：http://dc.muxihuayi.cn

diff a.txt b.txt
来源：http://sr.huanxung.cn

[R55] 压缩与解压
来源：http://gc.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cx.nicolike.cn

[R56] 远程拷贝
来源：http://ad.hahajie.cn

scp file user@host:/path/
来源：http://ba.nszjky.cn

[R57] 远程执行命令
来源：http://cw.wgjwhj.cn

ssh user@host 'uptime'
来源：http://gg.shtwfgs.cn

[R58] 下载文件
来源：http://ql.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cy.chemitech.net.cn

[R59] 发 POST JSON
来源：http://rc.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eh.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://mi.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zc.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://cz.szsharing.cn


<!-- 参考信息 -->