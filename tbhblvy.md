代发 wailian999

================================================================================
来源：http://up.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gi.521024.cn

================================================================================
来源：http://mr.shxzskj.cn

[Q01] 创建表
来源：http://jc.haigaiapp.cn

CREATE TABLE users (
来源：http://th.nszjky.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wi.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://zo.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://zr.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yv.huanxung.cn

);
来源：http://sx.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://gw.bjjhwx.cn

CREATE TABLE orders (
来源：http://zz.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ea.colortex.cn

user_id INT NOT NULL,
来源：http://um.huanxung.cn

amount DECIMAL(10, 2),
来源：http://by.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fz.jctech888.com.cn

);
来源：http://rg.muxihuayi.cn

[Q03] 增加列
来源：http://hq.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wy.szxytkj.cn

[Q04] 修改列类型
来源：http://in.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yq.huanxung.cn

[Q05] 重命名列
来源：http://lb.asd995.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ui.panjiajie.cn

[Q06] 删除列
来源：http://cu.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vv.hahajie.cn

[Q07] 删除表
来源：http://hm.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://cn.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://ms.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ea.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://iy.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.9csxet.cn

[Q10] 插入单行
来源：http://fi.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eb.hnjuh.cn

[Q11] 一次插入多行
来源：http://db.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xd.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://xn.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dm.nszjky.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jt.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://sc.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uu.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://fo.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ef.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sy.haigaiapp.cn

[Q15] 查询全部
来源：http://iu.521024.cn

SELECT * FROM users;
来源：http://uj.haigaiapp.cn

[Q16] 查询指定列
来源：http://xi.szxytkj.cn

SELECT id, name FROM users;
来源：http://dv.bookmarksfly.cn

[Q17] 条件查询
来源：http://qo.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rn.shxzskj.cn

[Q18] 模糊匹配
来源：http://iy.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ew.521024.cn

[Q19] 范围查询
来源：http://pc.9csxet.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ut.bjjhwx.cn

[Q20] IN 列表
来源：http://up.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tk.wgjwhj.cn

[Q21] 空值判断
来源：http://ws.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hr.bookmarksfly.cn

[Q22] 排序
来源：http://ur.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kp.chemitech.net.cn

[Q23] 分页
来源：http://ix.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jn.shxzukj.cn

[Q24] 去重
来源：http://fo.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://wj.newstarts.cn

[Q25] 只取前 N 条
来源：http://zh.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zv.shxzukj.cn

[Q26] 计数
来源：http://kc.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://vp.colortex.cn

[Q27] 条件计数
来源：http://gw.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ko.hahajie.cn

[Q28] 求和与平均
来源：http://hn.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ec.szxytkj.cn

[Q29] 最大最小值
来源：http://lm.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gv.jianghongdianzi.cn

[Q30] 分组统计
来源：http://bu.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nd.shxzskj.cn

[Q31] 分组后过滤
来源：http://mh.jctech888.com.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kx.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://qz.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vm.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://px.yuexingan06.cn

[Q33] 多列分组
来源：http://by.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pb.nicolike.cn

[Q34] 每组取第一条
来源：http://vb.nszjky.cn

SELECT * FROM (
来源：http://by.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mz.hahajie.cn

) t WHERE rn = 1;
来源：http://hx.bookmarksfly.cn

[Q35] 内连接
来源：http://kp.bookmarksfly.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vn.szxytkj.cn

[Q36] 左连接
来源：http://mq.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ky.hahajie.cn

[Q37] 右连接
来源：http://gq.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://az.muxihuayi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hp.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ad.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://ef.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lg.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://as.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://le.shxzukj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dg.wgjwhj.cn

[Q41] 多表连接
来源：http://dp.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wy.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://pv.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://ht.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://mu.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://np.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wp.hnjuh.cn

[Q43] 标量子查询
来源：http://cr.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://te.nicolike.cn

[Q44] IN 子查询
来源：http://qe.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ig.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://ls.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ce.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dt.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ll.chemitech.net.cn

[Q47] 与平均值比较
来源：http://es.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kv.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://it.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jw.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://nu.huanxung.cn

[Q49] 更新单行
来源：http://kb.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wb.bookmarksfly.cn

[Q50] 批量更新
来源：http://eu.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ub.yuexingan06.cn

[Q51] 用子查询更新
来源：http://tp.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://na.nszjky.cn

[Q52] 删除指定行
来源：http://dh.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://cx.chemitech.net.cn

[Q53] 按条件删除
来源：http://ei.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qe.szsharing.cn

[Q54] 清空表
来源：http://ak.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://ax.gzmigu.cn

[Q55] 排名（并列占位）
来源：http://yh.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vc.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://wh.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qx.szxytkj.cn

[Q57] 行号
来源：http://ak.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ox.asd995.cn

[Q58] 累计求和
来源：http://lw.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tx.haigaiapp.cn

[Q59] 分组内累计
来源：http://os.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sd.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://gp.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vp.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fh.lnxyls.cn

[Q61] 移动平均
来源：http://bt.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pa.yuntaijiaju.cn

[Q62] 分组占比
来源：http://na.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dr.521024.cn

[Q63] 开启事务
来源：http://qb.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://us.panjiajie.cn

[Q64] 提交事务
来源：http://hw.yuntaijiaju.cn

COMMIT;
来源：http://hi.lnxyls.cn

[Q65] 回滚事务
来源：http://iy.shxzskj.cn

ROLLBACK;
来源：http://dm.szsharing.cn

[Q66] 行锁查询
来源：http://qv.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jc.9csxet.cn

[Q67] 设置隔离级别
来源：http://bu.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ln.chemitech.net.cn

[Q68] 保存点
来源：http://ho.yuexingan06.cn

SAVEPOINT sp1;
来源：http://fm.szsharing.cn

ROLLBACK TO sp1;
来源：http://qq.panjiajie.cn

[Q69] 查看执行计划
来源：http://gr.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qd.yuexingan06.cn

[Q70] 更新统计信息
来源：http://ru.nicolike.cn

ANALYZE TABLE users;
来源：http://in.nicolike.cn

[Q71] 查看建表语句
来源：http://re.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pq.panjiajie.cn

[Q72] 查看索引
来源：http://lr.hnjuh.cn

SHOW INDEX FROM users;
来源：http://tp.szsharing.cn

[Q73] 查看表状态
来源：http://ee.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tl.nszjky.cn

[Q74] 强制使用索引
来源：http://mx.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qp.hnjuh.cn

[Q75] 日期格式化
来源：http://ev.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rc.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vs.9csxet.cn

[Q76] 按天统计
来源：http://qk.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://er.jctech888.com.cn

[Q77] 时间加减
来源：http://nv.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gx.jctech888.com.cn

[Q78] 当前时间
来源：http://ui.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ow.szxytkj.cn

[Q79] 字符串拼接
来源：http://if.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ho.panjiajie.cn

[Q80] 字符串截取
来源：http://jb.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://df.lnxyls.cn

[Q81] 字符串替换
来源：http://yi.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xc.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://yj.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iq.colortex.cn

[Q83] 大小写转换
来源：http://ts.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uv.newstarts.cn

[Q84] 去除首尾空格
来源：http://ka.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://px.gzmigu.cn

[Q85] 数值取整
来源：http://as.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zq.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://cf.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pb.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://fl.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bo.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://hz.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ps.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iq.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://sl.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tq.nicolike.cn

[Q90] 生成序号列
来源：http://gb.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ic.yuexingan06.cn

================================================================================
来源：http://sk.haigaiapp.cn

R. Bash 专题
来源：http://yy.szsharing.cn

================================================================================
来源：http://cc.shxzskj.cn

[R01] shebang 与严格模式
来源：http://hh.hahajie.cn

#!/usr/bin/env bash
来源：http://pj.huixiangedu.cn

set -euo pipefail
来源：http://qx.shxzskj.cn

[R02] 变量赋值与使用
来源：http://jv.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://is.hahajie.cn

[R03] 只读变量
来源：http://ex.jianghongdianzi.cn

readonly PI=3.14
来源：http://fy.colortex.cn

[R04] 位置参数
来源：http://ll.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fw.szxytkj.cn

[R05] 参数默认值
来源：http://os.newstarts.cn

name="${1:-default}"
来源：http://sa.szsharing.cn

[R06] 判断命令是否存在
来源：http://jd.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zg.hnjuh.cn

[R07] if 判断文件
来源：http://qf.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fe.muxihuayi.cn

[R08] 数值比较
来源：http://ql.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zh.muxihuayi.cn

[R09] 字符串比较
来源：http://bp.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cy.huanxung.cn

[R10] 正则匹配
来源：http://ac.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ra.szsharing.cn

[R11] case 多分支
来源：http://ns.nicolike.cn

case "$1" in
来源：http://vq.chemitech.net.cn

start) echo "启动" ;;
来源：http://pe.hnjuh.cn

stop)  echo "停止" ;;
来源：http://bu.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://lu.lnxyls.cn

esac
来源：http://xy.nicolike.cn

[R12] for 遍历文件
来源：http://bo.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://ak.shtwfgs.cn

[R13] for 计数循环
来源：http://ep.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://he.nicolike.cn

[R14] C 风格 for
来源：http://tu.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lh.szxytkj.cn

[R15] while 逐行读文件
来源：http://pk.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://io.hnjuh.cn

[R16] until 等待条件
来源：http://nm.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qh.jctech888.com.cn

[R17] 数组定义与取值
来源：http://fk.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ym.huixinmuqiang.cn

[R18] 遍历数组
来源：http://sy.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://km.huixiangedu.cn

[R19] 数组长度
来源：http://jc.hnjuh.cn

echo "${#arr[@]}"
来源：http://xi.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://sx.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bk.shxzukj.cn

[R21] 字符串长度
来源：http://wv.szxytkj.cn

echo "${#s}"
来源：http://yp.lnxyls.cn

[R22] 截取子串
来源：http://rf.bookmarksfly.cn

echo "${s:0:5}"
来源：http://nf.huanxung.cn

[R23] 字符串替换
来源：http://dc.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ss.gzmigu.cn

[R24] 大小写转换
来源：http://ed.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qh.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://tw.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uw.shxzukj.cn

[R26] 命令替换
来源：http://xm.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://ha.shtwfgs.cn

[R27] 算术展开
来源：http://ok.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://kb.gzmigu.cn

[R28] 浮点运算
来源：http://di.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://ho.jctech888.com.cn

[R29] 定义函数
来源：http://ps.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ct.shxzskj.cn

[R30] 函数返回状态码
来源：http://ty.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://ht.bjjhwx.cn

[R31] 局部变量
来源：http://xx.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://qi.gzmigu.cn

[R32] 参数个数校验
来源：http://vq.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vr.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://fz.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cm.jianghongdianzi.cn

[R34] 退出时清理
来源：http://cl.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fk.shtwfgs.cn

[R35] 后台执行并等待
来源：http://pv.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zu.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://ri.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jr.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://qq.colortex.cn

files=$(ls -1)
来源：http://vb.huanxung.cn

[R38] 管道串联
来源：http://em.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://oy.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://su.hahajie.cn

cmd > out.log 2>&1
来源：http://tv.gzmigu.cn

[R40] 追加写日志
来源：http://al.szsharing.cn

echo "log" >> out.log
来源：http://ux.colortex.cn

[R41] 丢弃输出
来源：http://sq.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://ti.yuexingan06.cn

[R42] 输入重定向
来源：http://cs.muxihuayi.cn

wc -l < a.txt
来源：http://km.nszjky.cn

[R43] 按名字查找文件
来源：http://qg.bookmarksfly.cn


<!-- 参考信息 -->