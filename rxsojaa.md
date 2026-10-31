代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ub.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://df.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ds.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://al.asd995.cn

================================================================================
来源：http://rh.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gd.chemitech.net.cn

================================================================================
来源：http://fy.haigaiapp.cn

[Q01] 创建表
来源：http://no.panjiajie.cn

CREATE TABLE users (
来源：http://rv.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vs.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://wo.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://vf.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iw.bookmarksfly.cn

);
来源：http://lq.hnjuh.cn

[Q02] 创建带外键的表
来源：http://jt.muxihuayi.cn

CREATE TABLE orders (
来源：http://jc.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qv.bjjhwx.cn

user_id INT NOT NULL,
来源：http://iu.hahajie.cn

amount DECIMAL(10, 2),
来源：http://lr.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mt.hnjuh.cn

);
来源：http://cg.yuexingan06.cn

[Q03] 增加列
来源：http://xs.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kz.chemitech.net.cn

[Q04] 修改列类型
来源：http://il.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mo.gzmigu.cn

[Q05] 重命名列
来源：http://je.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sb.lnxyls.cn

[Q06] 删除列
来源：http://ws.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gz.chemitech.net.cn

[Q07] 删除表
来源：http://ik.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://ve.lnxyls.cn

[Q08] 创建普通索引
来源：http://gp.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lw.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://sl.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://am.asd995.cn

[Q10] 插入单行
来源：http://do.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ew.huixiangedu.cn

[Q11] 一次插入多行
来源：http://ny.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kp.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://oq.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rz.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xd.shxzskj.cn

[Q13] 忽略重复插入
来源：http://ag.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rj.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://tk.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fh.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yk.huanxung.cn

[Q15] 查询全部
来源：http://ce.haigaiapp.cn

SELECT * FROM users;
来源：http://nn.panjiajie.cn

[Q16] 查询指定列
来源：http://no.lnxyls.cn

SELECT id, name FROM users;
来源：http://tj.newstarts.cn

[Q17] 条件查询
来源：http://eo.wgjwhj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gt.panjiajie.cn

[Q18] 模糊匹配
来源：http://ci.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://on.9csxet.cn

[Q19] 范围查询
来源：http://hb.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://al.jctech888.com.cn

[Q20] IN 列表
来源：http://nv.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gr.szxytkj.cn

[Q21] 空值判断
来源：http://sw.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dy.colortex.cn

[Q22] 排序
来源：http://fz.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wj.bookmarksfly.cn

[Q23] 分页
来源：http://cl.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wr.nicolike.cn

[Q24] 去重
来源：http://pc.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://dn.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://yc.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tz.colortex.cn

[Q26] 计数
来源：http://bg.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://px.shxzskj.cn

[Q27] 条件计数
来源：http://ft.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bf.yuexingan06.cn

[Q28] 求和与平均
来源：http://jn.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zo.wgjwhj.cn

[Q29] 最大最小值
来源：http://ry.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://iw.521024.cn

[Q30] 分组统计
来源：http://as.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ou.muxihuayi.cn

[Q31] 分组后过滤
来源：http://py.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://se.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://lw.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pg.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://os.huanxung.cn

[Q33] 多列分组
来源：http://ht.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://su.yuexingan06.cn

[Q34] 每组取第一条
来源：http://lx.jianghongdianzi.cn

SELECT * FROM (
来源：http://iz.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kw.wgjwhj.cn

) t WHERE rn = 1;
来源：http://pv.asd995.cn

[Q35] 内连接
来源：http://iv.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://op.nszjky.cn

[Q36] 左连接
来源：http://ad.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ov.szsharing.cn

[Q37] 右连接
来源：http://jw.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pa.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qs.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cc.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://bb.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sq.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jz.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ql.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hr.wgjwhj.cn

[Q41] 多表连接
来源：http://ak.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kr.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://lp.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://bj.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://dn.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://ct.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lu.muxihuayi.cn

[Q43] 标量子查询
来源：http://cv.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lm.shxzukj.cn

[Q44] IN 子查询
来源：http://he.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xl.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://rw.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ym.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ss.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://be.shxzskj.cn

[Q47] 与平均值比较
来源：http://mu.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bx.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://an.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uj.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://vw.jianghongdianzi.cn

[Q49] 更新单行
来源：http://yf.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ji.muxihuayi.cn

[Q50] 批量更新
来源：http://uk.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tx.panjiajie.cn

[Q51] 用子查询更新
来源：http://ic.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yj.szxytkj.cn

[Q52] 删除指定行
来源：http://dk.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://gs.szsharing.cn

[Q53] 按条件删除
来源：http://zt.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gl.haigaiapp.cn

[Q54] 清空表
来源：http://fg.asd995.cn

TRUNCATE TABLE logs;
来源：http://bg.nszjky.cn

[Q55] 排名（并列占位）
来源：http://ik.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bs.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://dp.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fb.muxihuayi.cn

[Q57] 行号
来源：http://hp.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ff.jianghongdianzi.cn

[Q58] 累计求和
来源：http://rl.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nv.szsharing.cn

[Q59] 分组内累计
来源：http://kv.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zd.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://kf.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ax.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uq.szsharing.cn

[Q61] 移动平均
来源：http://oq.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mh.panjiajie.cn

[Q62] 分组占比
来源：http://hy.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lz.chemitech.net.cn

[Q63] 开启事务
来源：http://so.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gf.shtwfgs.cn

[Q64] 提交事务
来源：http://xr.yuexingan06.cn

COMMIT;
来源：http://rp.szxytkj.cn

[Q65] 回滚事务
来源：http://yl.haigaiapp.cn

ROLLBACK;
来源：http://fj.huixinmuqiang.cn

[Q66] 行锁查询
来源：http://ad.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://es.hnjuh.cn

[Q67] 设置隔离级别
来源：http://ml.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://th.huixiangedu.cn

[Q68] 保存点
来源：http://ch.chemitech.net.cn

SAVEPOINT sp1;
来源：http://zq.panjiajie.cn

ROLLBACK TO sp1;
来源：http://cu.huanxung.cn

[Q69] 查看执行计划
来源：http://vd.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hd.wgjwhj.cn

[Q70] 更新统计信息
来源：http://dl.huixiangedu.cn

ANALYZE TABLE users;
来源：http://zl.huixiangedu.cn

[Q71] 查看建表语句
来源：http://rx.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dx.haigaiapp.cn

[Q72] 查看索引
来源：http://uf.newstarts.cn

SHOW INDEX FROM users;
来源：http://tm.bookmarksfly.cn

[Q73] 查看表状态
来源：http://yg.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://em.szxytkj.cn

[Q74] 强制使用索引
来源：http://uh.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://as.jctech888.com.cn

[Q75] 日期格式化
来源：http://am.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kd.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xs.bjjhwx.cn

[Q76] 按天统计
来源：http://zf.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fm.huanxung.cn

[Q77] 时间加减
来源：http://rv.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rp.shtwfgs.cn

[Q78] 当前时间
来源：http://em.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xl.haigaiapp.cn

[Q79] 字符串拼接
来源：http://da.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cc.521024.cn

[Q80] 字符串截取
来源：http://ht.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zo.szsharing.cn

[Q81] 字符串替换
来源：http://hd.bjjhwx.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yu.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://ei.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gx.newstarts.cn

[Q83] 大小写转换
来源：http://vj.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mx.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://zx.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://kg.hahajie.cn

[Q85] 数值取整
来源：http://jj.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mq.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://wg.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://if.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://mb.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rv.521024.cn

[Q88] 行转列（条件聚合）
来源：http://uf.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hp.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nq.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://wl.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qb.hnjuh.cn

[Q90] 生成序号列
来源：http://oh.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rx.shxzskj.cn

================================================================================
来源：http://hw.shxzukj.cn

R. Bash 专题
来源：http://em.shxzukj.cn

================================================================================
来源：http://dm.colortex.cn

[R01] shebang 与严格模式
来源：http://oz.nicolike.cn

#!/usr/bin/env bash
来源：http://hn.bjjhwx.cn

set -euo pipefail
来源：http://ez.szxytkj.cn

[R02] 变量赋值与使用
来源：http://cs.szsharing.cn

name="Tom"; echo "$name"
来源：http://kl.panjiajie.cn

[R03] 只读变量
来源：http://ed.521024.cn

readonly PI=3.14
来源：http://eq.gzmigu.cn

[R04] 位置参数
来源：http://yo.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lm.szxytkj.cn

[R05] 参数默认值
来源：http://bz.shxzskj.cn

name="${1:-default}"
来源：http://xy.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://hh.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fn.muxihuayi.cn

[R07] if 判断文件
来源：http://rm.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vh.huixiangedu.cn

[R08] 数值比较
来源：http://nh.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uo.szsharing.cn

[R09] 字符串比较
来源：http://xt.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tl.szxytkj.cn

[R10] 正则匹配
来源：http://by.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qy.521024.cn

[R11] case 多分支
来源：http://rw.shxzskj.cn

case "$1" in
来源：http://bt.newstarts.cn

start) echo "启动" ;;
来源：http://uk.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://vr.9csxet.cn

*)     echo "未知命令" ;;
来源：http://td.chemitech.net.cn

esac
来源：http://yp.521024.cn

[R12] for 遍历文件
来源：http://xn.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://co.shtwfgs.cn

[R13] for 计数循环
来源：http://tk.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://zc.muxihuayi.cn

[R14] C 风格 for
来源：http://mv.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nt.shxzskj.cn

[R15] while 逐行读文件
来源：http://vu.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cn.lnxyls.cn

[R16] until 等待条件
来源：http://ok.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vb.hahajie.cn

[R17] 数组定义与取值
来源：http://gs.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bn.colortex.cn

[R18] 遍历数组
来源：http://qo.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ei.bjjhwx.cn

[R19] 数组长度
来源：http://im.521024.cn

echo "${#arr[@]}"
来源：http://pe.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://qf.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oq.newstarts.cn

[R21] 字符串长度
来源：http://gf.hnjuh.cn

echo "${#s}"
来源：http://eo.gzmigu.cn

[R22] 截取子串
来源：http://od.hnjuh.cn

echo "${s:0:5}"
来源：http://xc.huixiangedu.cn

[R23] 字符串替换
来源：http://qz.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ha.lnxyls.cn

[R24] 大小写转换
来源：http://nc.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yu.521024.cn

[R25] 去后缀 / 去前缀
来源：http://rs.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zq.chemitech.net.cn

[R26] 命令替换
来源：http://sa.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://ko.bookmarksfly.cn

[R27] 算术展开
来源：http://ww.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://io.jianghongdianzi.cn

[R28] 浮点运算
来源：http://fj.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://lq.lnxyls.cn

[R29] 定义函数
来源：http://af.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oa.nszjky.cn

[R30] 函数返回状态码
来源：http://ux.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://aq.gzmigu.cn

[R31] 局部变量
来源：http://pl.521024.cn

f() { local x=1; echo "$x"; }
来源：http://na.panjiajie.cn

[R32] 参数个数校验
来源：http://uh.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mm.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://gf.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sa.huixinmuqiang.cn

[R34] 退出时清理
来源：http://la.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vv.huanxung.cn

[R35] 后台执行并等待
来源：http://bv.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uv.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://cc.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nn.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://uc.huixiangedu.cn

files=$(ls -1)
来源：http://aa.nszjky.cn

[R38] 管道串联
来源：http://ia.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://ah.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://po.huanxung.cn

cmd > out.log 2>&1
来源：http://aa.colortex.cn

[R40] 追加写日志
来源：http://pn.lnxyls.cn

echo "log" >> out.log
来源：http://mg.newstarts.cn

[R41] 丢弃输出
来源：http://py.jianghongdianzi.cn


<!-- 参考信息 -->