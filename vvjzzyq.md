代发 wailian999

================================================================================
来源：http://rl.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eb.asd995.cn

================================================================================
来源：http://jc.shxzskj.cn

[Q01] 创建表
来源：http://mx.colortex.cn

CREATE TABLE users (
来源：http://pg.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://em.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://wb.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://qt.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kj.jctech888.com.cn

);
来源：http://ys.asd995.cn

[Q02] 创建带外键的表
来源：http://or.newstarts.cn

CREATE TABLE orders (
来源：http://yv.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kf.nicolike.cn

user_id INT NOT NULL,
来源：http://kk.colortex.cn

amount DECIMAL(10, 2),
来源：http://ec.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ai.shxzskj.cn

);
来源：http://lh.yuntaijiaju.cn

[Q03] 增加列
来源：http://sh.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ar.9csxet.cn

[Q04] 修改列类型
来源：http://ol.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tg.nicolike.cn

[Q05] 重命名列
来源：http://fa.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wm.shxzukj.cn

[Q06] 删除列
来源：http://dg.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tf.huixinmuqiang.cn

[Q07] 删除表
来源：http://qb.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://ji.nszjky.cn

[Q08] 创建普通索引
来源：http://so.huixinmuqiang.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xo.shxzukj.cn

[Q09] 创建唯一索引
来源：http://bv.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ql.nszjky.cn

[Q10] 插入单行
来源：http://vf.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oy.asd995.cn

[Q11] 一次插入多行
来源：http://py.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cz.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://sl.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://aj.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pq.hnjuh.cn

[Q13] 忽略重复插入
来源：http://ew.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://je.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://wz.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rz.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ao.asd995.cn

[Q15] 查询全部
来源：http://ry.9csxet.cn

SELECT * FROM users;
来源：http://ym.panjiajie.cn

[Q16] 查询指定列
来源：http://aa.chemitech.net.cn

SELECT id, name FROM users;
来源：http://ql.nicolike.cn

[Q17] 条件查询
来源：http://rq.wgjwhj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ly.shxzukj.cn

[Q18] 模糊匹配
来源：http://xl.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qq.gzmigu.cn

[Q19] 范围查询
来源：http://ja.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uw.shxzukj.cn

[Q20] IN 列表
来源：http://tf.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dq.yuexingan06.cn

[Q21] 空值判断
来源：http://sy.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qj.9csxet.cn

[Q22] 排序
来源：http://od.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jy.szsharing.cn

[Q23] 分页
来源：http://bk.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zo.szsharing.cn

[Q24] 去重
来源：http://ap.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://ni.hnjuh.cn

[Q25] 只取前 N 条
来源：http://yy.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iw.bjjhwx.cn

[Q26] 计数
来源：http://vv.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://vq.jianghongdianzi.cn

[Q27] 条件计数
来源：http://xg.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hl.yuexingan06.cn

[Q28] 求和与平均
来源：http://xa.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yt.muxihuayi.cn

[Q29] 最大最小值
来源：http://jq.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ys.jianghongdianzi.cn

[Q30] 分组统计
来源：http://hf.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jw.hahajie.cn

[Q31] 分组后过滤
来源：http://is.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mx.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://li.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mc.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fa.szsharing.cn

[Q33] 多列分组
来源：http://fn.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kf.9csxet.cn

[Q34] 每组取第一条
来源：http://or.shxzukj.cn

SELECT * FROM (
来源：http://yc.hahajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mx.nicolike.cn

) t WHERE rn = 1;
来源：http://rr.szxytkj.cn

[Q35] 内连接
来源：http://xx.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qv.nszjky.cn

[Q36] 左连接
来源：http://jh.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dp.hahajie.cn

[Q37] 右连接
来源：http://xr.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sb.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zd.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mm.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://am.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gb.9csxet.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ih.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uw.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://na.yuexingan06.cn

[Q41] 多表连接
来源：http://sj.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vz.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://od.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://zq.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://gu.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://vf.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fm.bjjhwx.cn

[Q43] 标量子查询
来源：http://yf.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://we.bjjhwx.cn

[Q44] IN 子查询
来源：http://ms.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ya.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://qo.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lt.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kf.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iz.9csxet.cn

[Q47] 与平均值比较
来源：http://zj.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dh.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://ts.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vg.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://jf.lnxyls.cn

[Q49] 更新单行
来源：http://zc.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ud.huixiangedu.cn

[Q50] 批量更新
来源：http://lf.newstarts.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ia.chemitech.net.cn

[Q51] 用子查询更新
来源：http://bj.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hj.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://nq.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://dh.gzmigu.cn

[Q53] 按条件删除
来源：http://el.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nq.asd995.cn

[Q54] 清空表
来源：http://xs.nszjky.cn

TRUNCATE TABLE logs;
来源：http://jo.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://rk.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xg.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://th.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mr.shxzukj.cn

[Q57] 行号
来源：http://ck.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gf.haigaiapp.cn

[Q58] 累计求和
来源：http://ma.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://no.yuexingan06.cn

[Q59] 分组内累计
来源：http://mo.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aq.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://ov.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ey.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vl.jianghongdianzi.cn

[Q61] 移动平均
来源：http://cb.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gx.newstarts.cn

[Q62] 分组占比
来源：http://cs.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yy.yuntaijiaju.cn

[Q63] 开启事务
来源：http://op.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vr.szsharing.cn

[Q64] 提交事务
来源：http://ho.9csxet.cn

COMMIT;
来源：http://ze.shtwfgs.cn

[Q65] 回滚事务
来源：http://fk.shtwfgs.cn

ROLLBACK;
来源：http://xy.szsharing.cn

[Q66] 行锁查询
来源：http://oi.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://av.hnjuh.cn

[Q67] 设置隔离级别
来源：http://df.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pj.shtwfgs.cn

[Q68] 保存点
来源：http://ak.colortex.cn

SAVEPOINT sp1;
来源：http://ii.shxzukj.cn

ROLLBACK TO sp1;
来源：http://yf.bjjhwx.cn

[Q69] 查看执行计划
来源：http://br.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mq.521024.cn

[Q70] 更新统计信息
来源：http://fl.muxihuayi.cn

ANALYZE TABLE users;
来源：http://ar.shtwfgs.cn

[Q71] 查看建表语句
来源：http://kx.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ba.hahajie.cn

[Q72] 查看索引
来源：http://xx.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://of.nicolike.cn

[Q73] 查看表状态
来源：http://qn.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xt.newstarts.cn

[Q74] 强制使用索引
来源：http://xa.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ql.panjiajie.cn

[Q75] 日期格式化
来源：http://qt.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kw.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jv.newstarts.cn

[Q76] 按天统计
来源：http://mr.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ud.huixiangedu.cn

[Q77] 时间加减
来源：http://yw.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ro.lnxyls.cn

[Q78] 当前时间
来源：http://tg.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zv.hnjuh.cn

[Q79] 字符串拼接
来源：http://ln.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pt.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://er.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hd.haigaiapp.cn

[Q81] 字符串替换
来源：http://ui.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tw.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://ke.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dq.szsharing.cn

[Q83] 大小写转换
来源：http://bd.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cl.jctech888.com.cn

[Q84] 去除首尾空格
来源：http://ip.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://mf.lnxyls.cn

[Q85] 数值取整
来源：http://iq.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lf.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://kt.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ff.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://hp.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ub.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://rd.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xz.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qc.nicolike.cn

[Q89] 判断表是否存在
来源：http://ea.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dl.newstarts.cn

[Q90] 生成序号列
来源：http://cs.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xy.panjiajie.cn

================================================================================
来源：http://yu.yuexingan06.cn

R. Bash 专题
来源：http://ac.yuexingan06.cn

================================================================================
来源：http://jr.shxzskj.cn

[R01] shebang 与严格模式
来源：http://es.nicolike.cn

#!/usr/bin/env bash
来源：http://fu.chemitech.net.cn

set -euo pipefail
来源：http://pd.lnxyls.cn

[R02] 变量赋值与使用
来源：http://ac.asd995.cn

name="Tom"; echo "$name"
来源：http://wt.bookmarksfly.cn

[R03] 只读变量
来源：http://lv.shxzskj.cn

readonly PI=3.14
来源：http://cd.szxytkj.cn

[R04] 位置参数
来源：http://vd.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ye.yuntaijiaju.cn

[R05] 参数默认值
来源：http://ri.lnxyls.cn

name="${1:-default}"
来源：http://on.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://iq.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uq.yuexingan06.cn

[R07] if 判断文件
来源：http://fo.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dw.yuexingan06.cn

[R08] 数值比较
来源：http://kp.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gn.huanxung.cn

[R09] 字符串比较
来源：http://zw.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vz.bjjhwx.cn

[R10] 正则匹配
来源：http://io.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tg.szsharing.cn

[R11] case 多分支
来源：http://jy.szxytkj.cn

case "$1" in
来源：http://xe.shtwfgs.cn

start) echo "启动" ;;
来源：http://ia.lnxyls.cn

stop)  echo "停止" ;;
来源：http://xz.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://jc.nicolike.cn

esac
来源：http://hl.colortex.cn

[R12] for 遍历文件
来源：http://xu.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://sa.shxzskj.cn

[R13] for 计数循环
来源：http://fg.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://rn.lnxyls.cn

[R14] C 风格 for
来源：http://zg.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ix.yuexingan06.cn

[R15] while 逐行读文件
来源：http://qe.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lx.bookmarksfly.cn

[R16] until 等待条件
来源：http://gd.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rr.haigaiapp.cn

[R17] 数组定义与取值
来源：http://xm.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jx.panjiajie.cn

[R18] 遍历数组
来源：http://xl.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gh.jianghongdianzi.cn

[R19] 数组长度
来源：http://fa.9csxet.cn

echo "${#arr[@]}"
来源：http://ef.lnxyls.cn

[R20] 关联数组（字典）
来源：http://wp.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rp.huixiangedu.cn

[R21] 字符串长度
来源：http://pd.chemitech.net.cn

echo "${#s}"
来源：http://qh.jctech888.com.cn

[R22] 截取子串
来源：http://zn.yuexingan06.cn

echo "${s:0:5}"
来源：http://cn.chemitech.net.cn

[R23] 字符串替换
来源：http://lx.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rp.jianghongdianzi.cn

[R24] 大小写转换
来源：http://cy.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pz.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://rb.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fd.jianghongdianzi.cn

[R26] 命令替换
来源：http://mf.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://gc.nicolike.cn

[R27] 算术展开
来源：http://cv.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://sh.colortex.cn

[R28] 浮点运算
来源：http://ok.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://hp.shxzukj.cn

[R29] 定义函数
来源：http://cz.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kc.muxihuayi.cn

[R30] 函数返回状态码
来源：http://er.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://ld.shtwfgs.cn

[R31] 局部变量
来源：http://xv.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://dg.shxzskj.cn

[R32] 参数个数校验
来源：http://nh.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bo.colortex.cn

[R33] 捕获错误并提示行号
来源：http://wg.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sy.szxytkj.cn

[R34] 退出时清理
来源：http://vj.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hv.521024.cn

[R35] 后台执行并等待
来源：http://qv.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nm.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://dd.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ym.nicolike.cn

[R37] 把输出赋给变量
来源：http://yl.chemitech.net.cn

files=$(ls -1)
来源：http://on.shxzskj.cn

[R38] 管道串联
来源：http://kb.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://tn.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://ol.521024.cn

cmd > out.log 2>&1
来源：http://jr.hahajie.cn

[R40] 追加写日志
来源：http://du.bookmarksfly.cn

echo "log" >> out.log
来源：http://sm.shxzukj.cn

[R41] 丢弃输出
来源：http://jz.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://oq.panjiajie.cn

[R42] 输入重定向
来源：http://pr.huixiangedu.cn

wc -l < a.txt
来源：http://ia.haigaiapp.cn

[R43] 按名字查找文件
来源：http://qy.nszjky.cn


<!-- 参考信息 -->