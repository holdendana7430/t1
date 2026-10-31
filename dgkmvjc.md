代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://wn.lnxyls.cn

[Q07] 删除表
来源：http://iq.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://el.szxytkj.cn

[Q08] 创建普通索引
来源：http://ai.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zw.hnjuh.cn

[Q09] 创建唯一索引
来源：http://ko.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wa.colortex.cn

[Q10] 插入单行
来源：http://cy.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vj.jctech888.com.cn

[Q11] 一次插入多行
来源：http://fn.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qi.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://ft.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gq.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://go.nszjky.cn

[Q13] 忽略重复插入
来源：http://tp.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ug.521024.cn

[Q14] 存在则更新（upsert）
来源：http://ia.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hp.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ih.shtwfgs.cn

[Q15] 查询全部
来源：http://qk.chemitech.net.cn

SELECT * FROM users;
来源：http://wr.huixiangedu.cn

[Q16] 查询指定列
来源：http://cl.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://gf.chemitech.net.cn

[Q17] 条件查询
来源：http://cf.newstarts.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yz.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://sq.jctech888.com.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pn.bjjhwx.cn

[Q19] 范围查询
来源：http://sj.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ik.521024.cn

[Q20] IN 列表
来源：http://xh.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://li.jctech888.com.cn

[Q21] 空值判断
来源：http://sy.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kv.wgjwhj.cn

[Q22] 排序
来源：http://yy.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lh.muxihuayi.cn

[Q23] 分页
来源：http://ey.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zc.nszjky.cn

[Q24] 去重
来源：http://gi.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://gx.huanxung.cn

[Q25] 只取前 N 条
来源：http://dj.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hp.yuntaijiaju.cn

[Q26] 计数
来源：http://ni.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://ev.newstarts.cn

[Q27] 条件计数
来源：http://jo.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fv.9csxet.cn

[Q28] 求和与平均
来源：http://va.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eu.shxzskj.cn

[Q29] 最大最小值
来源：http://wd.asd995.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ed.jctech888.com.cn

[Q30] 分组统计
来源：http://pj.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yn.huanxung.cn

[Q31] 分组后过滤
来源：http://tx.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xm.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://bk.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://le.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://up.jianghongdianzi.cn

[Q33] 多列分组
来源：http://ex.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mg.haigaiapp.cn

[Q34] 每组取第一条
来源：http://af.asd995.cn

SELECT * FROM (
来源：http://cj.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ut.chemitech.net.cn

) t WHERE rn = 1;
来源：http://we.nszjky.cn

[Q35] 内连接
来源：http://ss.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gl.chemitech.net.cn

[Q36] 左连接
来源：http://gp.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bk.nszjky.cn

[Q37] 右连接
来源：http://zs.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tm.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kv.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cs.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://bq.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ge.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://on.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://he.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xa.nszjky.cn

[Q41] 多表连接
来源：http://vq.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ij.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://bg.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://ng.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://cu.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://en.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://et.wgjwhj.cn

[Q43] 标量子查询
来源：http://iq.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cx.nszjky.cn

[Q44] IN 子查询
来源：http://dg.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ng.haigaiapp.cn

[Q45] EXISTS 判断存在
来源：http://vj.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ym.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ib.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fa.9csxet.cn

[Q47] 与平均值比较
来源：http://bp.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hh.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://mv.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ov.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://wc.wgjwhj.cn

[Q49] 更新单行
来源：http://ne.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oe.jianghongdianzi.cn

[Q50] 批量更新
来源：http://ux.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nw.newstarts.cn

[Q51] 用子查询更新
来源：http://vz.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ei.bookmarksfly.cn

[Q52] 删除指定行
来源：http://ti.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://wc.bjjhwx.cn

[Q53] 按条件删除
来源：http://nf.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lh.shtwfgs.cn

[Q54] 清空表
来源：http://wi.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://bx.nszjky.cn

[Q55] 排名（并列占位）
来源：http://mr.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lu.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://iz.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ty.szsharing.cn

[Q57] 行号
来源：http://kn.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vl.nicolike.cn

[Q58] 累计求和
来源：http://qe.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://su.huixiangedu.cn

[Q59] 分组内累计
来源：http://qg.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://us.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://fs.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vo.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ly.521024.cn

[Q61] 移动平均
来源：http://bl.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://us.haigaiapp.cn

[Q62] 分组占比
来源：http://bb.shxzukj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://se.muxihuayi.cn

[Q63] 开启事务
来源：http://yd.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://be.hnjuh.cn

[Q64] 提交事务
来源：http://so.colortex.cn

COMMIT;
来源：http://xx.wgjwhj.cn

[Q65] 回滚事务
来源：http://ks.haigaiapp.cn

ROLLBACK;
来源：http://gz.shxzskj.cn

[Q66] 行锁查询
来源：http://pf.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sc.szxytkj.cn

[Q67] 设置隔离级别
来源：http://gb.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://im.9csxet.cn

[Q68] 保存点
来源：http://hm.521024.cn

SAVEPOINT sp1;
来源：http://ew.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://lq.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://na.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ag.bjjhwx.cn

[Q70] 更新统计信息
来源：http://qg.yuexingan06.cn

ANALYZE TABLE users;
来源：http://ld.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://jz.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ts.shxzskj.cn

[Q72] 查看索引
来源：http://zw.shxzukj.cn

SHOW INDEX FROM users;
来源：http://or.huixiangedu.cn

[Q73] 查看表状态
来源：http://yb.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kc.asd995.cn

[Q74] 强制使用索引
来源：http://ra.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ty.shxzukj.cn

[Q75] 日期格式化
来源：http://qi.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jy.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hg.bookmarksfly.cn

[Q76] 按天统计
来源：http://mr.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hx.yuntaijiaju.cn

[Q77] 时间加减
来源：http://ao.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ks.chemitech.net.cn

[Q78] 当前时间
来源：http://gy.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pq.shxzukj.cn

[Q79] 字符串拼接
来源：http://ob.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cm.jctech888.com.cn

[Q80] 字符串截取
来源：http://ef.9csxet.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qq.lnxyls.cn

[Q81] 字符串替换
来源：http://ek.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hx.521024.cn

[Q82] 字符长度与字节长度
来源：http://sc.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yj.bjjhwx.cn

[Q83] 大小写转换
来源：http://dh.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vi.newstarts.cn

[Q84] 去除首尾空格
来源：http://un.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://ds.szxytkj.cn

[Q85] 数值取整
来源：http://jy.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sr.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://tv.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bw.huanxung.cn

[Q87] JSON 字段做条件
来源：http://er.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sx.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://yj.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sr.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tx.nicolike.cn

[Q89] 判断表是否存在
来源：http://di.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zc.hahajie.cn

[Q90] 生成序号列
来源：http://ox.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tz.shxzskj.cn

================================================================================
来源：http://pm.muxihuayi.cn

R. Bash 专题
来源：http://si.muxihuayi.cn

================================================================================
来源：http://mm.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://jc.yuexingan06.cn

#!/usr/bin/env bash
来源：http://my.szxytkj.cn

set -euo pipefail
来源：http://qk.szxytkj.cn

[R02] 变量赋值与使用
来源：http://xh.hnjuh.cn

name="Tom"; echo "$name"
来源：http://na.jctech888.com.cn

[R03] 只读变量
来源：http://te.wgjwhj.cn

readonly PI=3.14
来源：http://tz.jianghongdianzi.cn

[R04] 位置参数
来源：http://kd.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qf.colortex.cn

[R05] 参数默认值
来源：http://jp.yuexingan06.cn

name="${1:-default}"
来源：http://ah.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://ow.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hx.szxytkj.cn

[R07] if 判断文件
来源：http://ld.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dj.shtwfgs.cn

[R08] 数值比较
来源：http://ns.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fj.panjiajie.cn

[R09] 字符串比较
来源：http://xl.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kc.yuntaijiaju.cn

[R10] 正则匹配
来源：http://mc.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kb.shtwfgs.cn

[R11] case 多分支
来源：http://de.gzmigu.cn

case "$1" in
来源：http://om.muxihuayi.cn

start) echo "启动" ;;
来源：http://zq.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://gp.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://fy.nszjky.cn

esac
来源：http://wb.gzmigu.cn

[R12] for 遍历文件
来源：http://ld.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://bx.szsharing.cn

[R13] for 计数循环
来源：http://nc.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://hd.yuntaijiaju.cn

[R14] C 风格 for
来源：http://of.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jx.hahajie.cn

[R15] while 逐行读文件
来源：http://jj.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hg.jianghongdianzi.cn

[R16] until 等待条件
来源：http://xc.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gn.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://oj.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qb.nicolike.cn

[R18] 遍历数组
来源：http://rf.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lv.bookmarksfly.cn

[R19] 数组长度
来源：http://ai.huixiangedu.cn

echo "${#arr[@]}"
来源：http://rv.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://qx.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cq.asd995.cn

[R21] 字符串长度
来源：http://en.bookmarksfly.cn

echo "${#s}"
来源：http://hq.bookmarksfly.cn

[R22] 截取子串
来源：http://zj.yuexingan06.cn

echo "${s:0:5}"
来源：http://an.jianghongdianzi.cn

[R23] 字符串替换
来源：http://qy.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rp.yuexingan06.cn

[R24] 大小写转换
来源：http://hu.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bw.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://vk.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ae.jianghongdianzi.cn

[R26] 命令替换
来源：http://bz.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://pj.szsharing.cn

[R27] 算术展开
来源：http://si.colortex.cn

echo $((1 + 2 * 3))
来源：http://ac.panjiajie.cn

[R28] 浮点运算
来源：http://mu.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://eo.muxihuayi.cn

[R29] 定义函数
来源：http://zp.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fk.szxytkj.cn

[R30] 函数返回状态码
来源：http://qw.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://to.shxzskj.cn

[R31] 局部变量
来源：http://yg.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://kq.shxzskj.cn

[R32] 参数个数校验
来源：http://xo.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tv.asd995.cn

[R33] 捕获错误并提示行号
来源：http://fr.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kw.nszjky.cn

[R34] 退出时清理
来源：http://bz.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fg.nszjky.cn

[R35] 后台执行并等待
来源：http://th.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ff.asd995.cn

[R36] 并发执行多个任务
来源：http://ly.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://za.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://sl.szsharing.cn

files=$(ls -1)
来源：http://ny.nicolike.cn

[R38] 管道串联
来源：http://cz.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://hj.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://ro.yuexingan06.cn

cmd > out.log 2>&1
来源：http://mh.newstarts.cn

[R40] 追加写日志
来源：http://ff.9csxet.cn

echo "log" >> out.log
来源：http://bv.521024.cn

[R41] 丢弃输出
来源：http://zf.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://to.nicolike.cn

[R42] 输入重定向
来源：http://yk.bjjhwx.cn

wc -l < a.txt
来源：http://is.chemitech.net.cn

[R43] 按名字查找文件
来源：http://vq.shtwfgs.cn

find . -name "*.log" -type f
来源：http://jf.shxzskj.cn

[R44] 按修改时间查找
来源：http://ye.bjjhwx.cn

find . -mtime -7 -type f
来源：http://lx.shxzukj.cn

[R45] 批量删除
来源：http://nj.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://co.newstarts.cn

[R46] 递归替换文件内容
来源：http://sz.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://se.szsharing.cn

[R47] sed 单行替换
来源：http://wk.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pu.nszjky.cn

[R48] awk 取指定列
来源：http://zl.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://pd.huanxung.cn

[R49] awk 带条件
来源：http://mg.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bx.jianghongdianzi.cn

[R50] awk 求和
来源：http://og.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://na.wgjwhj.cn

[R51] 排序去重取前几
来源：http://kn.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xl.jctech888.com.cn

[R52] 统计行数
来源：http://om.yuexingan06.cn

wc -l a.txt
来源：http://gp.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://sk.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://al.panjiajie.cn

[R54] 比较两个文件
来源：http://br.bookmarksfly.cn

diff a.txt b.txt
来源：http://kk.hnjuh.cn

[R55] 压缩与解压
来源：http://rq.nicolike.cn


<!-- 参考信息 -->