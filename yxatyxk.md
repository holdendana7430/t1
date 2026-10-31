代发 wailian999

================================================================================
来源：http://cy.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oi.shxzskj.cn

================================================================================
来源：http://zf.nicolike.cn

[Q01] 创建表
来源：http://xg.yuexingan06.cn

CREATE TABLE users (
来源：http://zo.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bn.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://mo.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://ve.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ko.bookmarksfly.cn

);
来源：http://cq.shxzskj.cn

[Q02] 创建带外键的表
来源：http://td.nicolike.cn

CREATE TABLE orders (
来源：http://et.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ec.gzmigu.cn

user_id INT NOT NULL,
来源：http://ac.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://jc.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ay.muxihuayi.cn

);
来源：http://vm.yuexingan06.cn

[Q03] 增加列
来源：http://bo.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hw.shtwfgs.cn

[Q04] 修改列类型
来源：http://ph.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zn.muxihuayi.cn

[Q05] 重命名列
来源：http://tf.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wa.shtwfgs.cn

[Q06] 删除列
来源：http://vu.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sn.shxzskj.cn

[Q07] 删除表
来源：http://if.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://ng.hahajie.cn

[Q08] 创建普通索引
来源：http://ur.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gw.huanxung.cn

[Q09] 创建唯一索引
来源：http://zh.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ew.huanxung.cn

[Q10] 插入单行
来源：http://hx.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cv.hahajie.cn

[Q11] 一次插入多行
来源：http://yt.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gb.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://mv.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gi.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ji.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://ix.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vv.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://nj.panjiajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ow.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://po.nszjky.cn

[Q15] 查询全部
来源：http://ze.muxihuayi.cn

SELECT * FROM users;
来源：http://wp.bjjhwx.cn

[Q16] 查询指定列
来源：http://fb.nszjky.cn

SELECT id, name FROM users;
来源：http://td.colortex.cn

[Q17] 条件查询
来源：http://yj.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://we.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://fg.szsharing.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://em.muxihuayi.cn

[Q19] 范围查询
来源：http://bm.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cy.wgjwhj.cn

[Q20] IN 列表
来源：http://rv.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yo.muxihuayi.cn

[Q21] 空值判断
来源：http://uy.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dz.shxzskj.cn

[Q22] 排序
来源：http://ln.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kv.wgjwhj.cn

[Q23] 分页
来源：http://ij.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pe.shxzukj.cn

[Q24] 去重
来源：http://cs.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://lc.szxytkj.cn

[Q25] 只取前 N 条
来源：http://wa.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yh.muxihuayi.cn

[Q26] 计数
来源：http://ej.gzmigu.cn

SELECT COUNT(*) FROM users;
来源：http://oo.lnxyls.cn

[Q27] 条件计数
来源：http://es.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nm.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://lb.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tx.shxzukj.cn

[Q29] 最大最小值
来源：http://nw.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ze.huanxung.cn

[Q30] 分组统计
来源：http://ql.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gz.asd995.cn

[Q31] 分组后过滤
来源：http://jt.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jg.nszjky.cn

[Q32] 分组拼接字符串
来源：http://cs.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ea.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gc.yuntaijiaju.cn

[Q33] 多列分组
来源：http://jy.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ao.haigaiapp.cn

[Q34] 每组取第一条
来源：http://ce.521024.cn

SELECT * FROM (
来源：http://mq.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nv.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://na.szsharing.cn

[Q35] 内连接
来源：http://yr.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ja.jianghongdianzi.cn

[Q36] 左连接
来源：http://wl.asd995.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mh.nszjky.cn

[Q37] 右连接
来源：http://dj.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://we.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pe.newstarts.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://li.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://vq.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zw.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wq.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://si.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ds.shtwfgs.cn

[Q41] 多表连接
来源：http://tb.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jd.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://lu.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://hc.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://ei.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://cf.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qj.shtwfgs.cn

[Q43] 标量子查询
来源：http://dr.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mr.lnxyls.cn

[Q44] IN 子查询
来源：http://nk.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ba.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://ql.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yn.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bx.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nj.szsharing.cn

[Q47] 与平均值比较
来源：http://pe.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ro.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://hr.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tv.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://ev.yuexingan06.cn

[Q49] 更新单行
来源：http://yt.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://md.gzmigu.cn

[Q50] 批量更新
来源：http://gw.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://du.haigaiapp.cn

[Q51] 用子查询更新
来源：http://ou.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kd.szsharing.cn

[Q52] 删除指定行
来源：http://qz.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://fy.muxihuayi.cn

[Q53] 按条件删除
来源：http://ue.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gj.yuntaijiaju.cn

[Q54] 清空表
来源：http://xk.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://zr.521024.cn

[Q55] 排名（并列占位）
来源：http://vv.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://md.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://hw.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wb.newstarts.cn

[Q57] 行号
来源：http://fd.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gb.muxihuayi.cn

[Q58] 累计求和
来源：http://xx.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ah.gzmigu.cn

[Q59] 分组内累计
来源：http://dg.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fe.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://cr.gzmigu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://py.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uw.jctech888.com.cn

[Q61] 移动平均
来源：http://wb.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hj.nszjky.cn

[Q62] 分组占比
来源：http://jo.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ik.huixinmuqiang.cn

[Q63] 开启事务
来源：http://sy.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ie.9csxet.cn

[Q64] 提交事务
来源：http://qg.yuexingan06.cn

COMMIT;
来源：http://gr.haigaiapp.cn

[Q65] 回滚事务
来源：http://gq.huixiangedu.cn

ROLLBACK;
来源：http://od.hahajie.cn

[Q66] 行锁查询
来源：http://nv.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oh.shxzukj.cn

[Q67] 设置隔离级别
来源：http://ac.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rm.szxytkj.cn

[Q68] 保存点
来源：http://fz.shxzskj.cn

SAVEPOINT sp1;
来源：http://yb.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://gm.muxihuayi.cn

[Q69] 查看执行计划
来源：http://bf.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bl.huanxung.cn

[Q70] 更新统计信息
来源：http://ys.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://wc.nicolike.cn

[Q71] 查看建表语句
来源：http://hd.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ov.lnxyls.cn

[Q72] 查看索引
来源：http://od.9csxet.cn

SHOW INDEX FROM users;
来源：http://xs.shxzskj.cn

[Q73] 查看表状态
来源：http://nf.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://re.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://mx.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xg.gzmigu.cn

[Q75] 日期格式化
来源：http://xe.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ju.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pk.haigaiapp.cn

[Q76] 按天统计
来源：http://ye.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://px.jctech888.com.cn

[Q77] 时间加减
来源：http://uy.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yq.asd995.cn

[Q78] 当前时间
来源：http://rt.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kc.bjjhwx.cn

[Q79] 字符串拼接
来源：http://io.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ed.huanxung.cn

[Q80] 字符串截取
来源：http://rc.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rm.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://od.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lq.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://po.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gj.haigaiapp.cn

[Q83] 大小写转换
来源：http://ae.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zu.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://ld.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://fa.yuexingan06.cn

[Q85] 数值取整
来源：http://bk.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://an.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://sn.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kv.colortex.cn

[Q87] JSON 字段做条件
来源：http://dx.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ln.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://hm.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iu.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sv.nicolike.cn

[Q89] 判断表是否存在
来源：http://cd.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://un.haigaiapp.cn

[Q90] 生成序号列
来源：http://av.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kl.lnxyls.cn

================================================================================
来源：http://ql.shtwfgs.cn

R. Bash 专题
来源：http://vp.gzmigu.cn

================================================================================
来源：http://jq.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://bh.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://ym.panjiajie.cn

set -euo pipefail
来源：http://ut.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://lb.asd995.cn

name="Tom"; echo "$name"
来源：http://xq.hahajie.cn

[R03] 只读变量
来源：http://aa.bjjhwx.cn

readonly PI=3.14
来源：http://xy.chemitech.net.cn

[R04] 位置参数
来源：http://tm.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://us.szxytkj.cn

[R05] 参数默认值
来源：http://fn.nicolike.cn

name="${1:-default}"
来源：http://mg.shxzukj.cn

[R06] 判断命令是否存在
来源：http://zo.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ar.yuexingan06.cn

[R07] if 判断文件
来源：http://dx.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qa.wgjwhj.cn

[R08] 数值比较
来源：http://zu.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ts.bjjhwx.cn

[R09] 字符串比较
来源：http://ep.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ly.shtwfgs.cn

[R10] 正则匹配
来源：http://al.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vb.shxzskj.cn

[R11] case 多分支
来源：http://rw.bookmarksfly.cn

case "$1" in
来源：http://uq.gzmigu.cn

start) echo "启动" ;;
来源：http://nj.asd995.cn

stop)  echo "停止" ;;
来源：http://vl.9csxet.cn

*)     echo "未知命令" ;;
来源：http://aa.shtwfgs.cn

esac
来源：http://fo.shxzukj.cn

[R12] for 遍历文件
来源：http://qw.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://so.521024.cn

[R13] for 计数循环
来源：http://ll.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://ko.521024.cn

[R14] C 风格 for
来源：http://jk.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zm.shtwfgs.cn

[R15] while 逐行读文件
来源：http://bk.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uy.shxzskj.cn

[R16] until 等待条件
来源：http://vw.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ln.jctech888.com.cn

[R17] 数组定义与取值
来源：http://sk.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://eo.hahajie.cn

[R18] 遍历数组
来源：http://ct.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sw.gzmigu.cn

[R19] 数组长度
来源：http://ju.colortex.cn

echo "${#arr[@]}"
来源：http://ui.lnxyls.cn

[R20] 关联数组（字典）
来源：http://ks.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gs.nszjky.cn

[R21] 字符串长度
来源：http://db.nszjky.cn

echo "${#s}"
来源：http://px.shxzskj.cn

[R22] 截取子串
来源：http://ln.nicolike.cn

echo "${s:0:5}"
来源：http://cx.gzmigu.cn

[R23] 字符串替换
来源：http://br.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ta.hnjuh.cn

[R24] 大小写转换
来源：http://sf.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://al.521024.cn

[R25] 去后缀 / 去前缀
来源：http://qp.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ri.wgjwhj.cn

[R26] 命令替换
来源：http://br.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://qg.szsharing.cn

[R27] 算术展开
来源：http://ds.nszjky.cn

echo $((1 + 2 * 3))
来源：http://bq.gzmigu.cn

[R28] 浮点运算
来源：http://lq.huixiangedu.cn

echo "scale=2; 10/3" | bc
来源：http://em.hnjuh.cn

[R29] 定义函数
来源：http://uo.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://if.hnjuh.cn

[R30] 函数返回状态码
来源：http://dh.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://kn.huixinmuqiang.cn

[R31] 局部变量
来源：http://je.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://ew.521024.cn

[R32] 参数个数校验
来源：http://lh.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sc.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://oq.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bl.bookmarksfly.cn

[R34] 退出时清理
来源：http://bg.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zg.shxzskj.cn

[R35] 后台执行并等待
来源：http://dy.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xv.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://zd.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sx.nszjky.cn

[R37] 把输出赋给变量
来源：http://xk.yuntaijiaju.cn

files=$(ls -1)
来源：http://hu.nicolike.cn

[R38] 管道串联
来源：http://eo.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://fu.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://bz.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://kw.9csxet.cn

[R40] 追加写日志
来源：http://if.nicolike.cn

echo "log" >> out.log
来源：http://pe.nszjky.cn

[R41] 丢弃输出
来源：http://kh.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://vn.jianghongdianzi.cn

[R42] 输入重定向
来源：http://eb.521024.cn

wc -l < a.txt
来源：http://hj.shxzukj.cn

[R43] 按名字查找文件
来源：http://yk.chemitech.net.cn


<!-- 参考信息 -->