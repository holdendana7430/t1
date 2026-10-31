代发 wailian999

CREATE TABLE users (
来源：http://ob.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fe.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://yx.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://ba.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zr.shtwfgs.cn

);
来源：http://xp.asd995.cn

[Q02] 创建带外键的表
来源：http://qd.huixiangedu.cn

CREATE TABLE orders (
来源：http://zl.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cm.jctech888.com.cn

user_id INT NOT NULL,
来源：http://dh.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://lv.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ci.hnjuh.cn

);
来源：http://ir.bookmarksfly.cn

[Q03] 增加列
来源：http://bl.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mf.shtwfgs.cn

[Q04] 修改列类型
来源：http://ju.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xs.wgjwhj.cn

[Q05] 重命名列
来源：http://nn.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pu.colortex.cn

[Q06] 删除列
来源：http://ot.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yd.jctech888.com.cn

[Q07] 删除表
来源：http://yu.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://nr.gzmigu.cn

[Q08] 创建普通索引
来源：http://tn.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ca.nszjky.cn

[Q09] 创建唯一索引
来源：http://ji.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://on.hnjuh.cn

[Q10] 插入单行
来源：http://ta.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ta.szxytkj.cn

[Q11] 一次插入多行
来源：http://zv.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://az.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://rw.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nd.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wc.nszjky.cn

[Q13] 忽略重复插入
来源：http://vt.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zo.gzmigu.cn

[Q14] 存在则更新（upsert）
来源：http://xf.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eq.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yz.haigaiapp.cn

[Q15] 查询全部
来源：http://gl.521024.cn

SELECT * FROM users;
来源：http://cd.szsharing.cn

[Q16] 查询指定列
来源：http://so.huixiangedu.cn

SELECT id, name FROM users;
来源：http://df.jianghongdianzi.cn

[Q17] 条件查询
来源：http://hb.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mb.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://cj.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dq.huanxung.cn

[Q19] 范围查询
来源：http://at.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mj.shxzukj.cn

[Q20] IN 列表
来源：http://rx.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dg.jctech888.com.cn

[Q21] 空值判断
来源：http://ff.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tx.gzmigu.cn

[Q22] 排序
来源：http://xi.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rd.jctech888.com.cn

[Q23] 分页
来源：http://wq.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sr.huanxung.cn

[Q24] 去重
来源：http://yt.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://lk.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://my.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://up.shxzukj.cn

[Q26] 计数
来源：http://le.chemitech.net.cn

SELECT COUNT(*) FROM users;
来源：http://kx.bookmarksfly.cn

[Q27] 条件计数
来源：http://hd.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xj.shtwfgs.cn

[Q28] 求和与平均
来源：http://xa.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wh.haigaiapp.cn

[Q29] 最大最小值
来源：http://px.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ic.bjjhwx.cn

[Q30] 分组统计
来源：http://zy.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eq.lnxyls.cn

[Q31] 分组后过滤
来源：http://xb.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fd.szsharing.cn

[Q32] 分组拼接字符串
来源：http://en.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ta.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yn.nicolike.cn

[Q33] 多列分组
来源：http://dx.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dp.szsharing.cn

[Q34] 每组取第一条
来源：http://hs.shxzskj.cn

SELECT * FROM (
来源：http://fp.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ci.huixiangedu.cn

) t WHERE rn = 1;
来源：http://kc.wgjwhj.cn

[Q35] 内连接
来源：http://hp.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mb.muxihuayi.cn

[Q36] 左连接
来源：http://rb.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qm.szsharing.cn

[Q37] 右连接
来源：http://gy.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wh.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ic.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ds.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://sf.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://em.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pe.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kt.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pk.jctech888.com.cn

[Q41] 多表连接
来源：http://tz.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vd.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://uj.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://ea.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://qz.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://rz.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ia.hahajie.cn

[Q43] 标量子查询
来源：http://kb.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bq.panjiajie.cn

[Q44] IN 子查询
来源：http://bh.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kb.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://pr.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ud.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mu.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hb.szxytkj.cn

[Q47] 与平均值比较
来源：http://qe.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fj.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://hs.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sj.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://gh.wgjwhj.cn

[Q49] 更新单行
来源：http://kq.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fx.colortex.cn

[Q50] 批量更新
来源：http://nf.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yn.haigaiapp.cn

[Q51] 用子查询更新
来源：http://vb.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xa.bjjhwx.cn

[Q52] 删除指定行
来源：http://do.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://zd.lnxyls.cn

[Q53] 按条件删除
来源：http://en.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zi.huixiangedu.cn

[Q54] 清空表
来源：http://vp.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://dc.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://qm.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qt.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://xe.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bd.yuntaijiaju.cn

[Q57] 行号
来源：http://ou.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yi.hnjuh.cn

[Q58] 累计求和
来源：http://yx.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gj.hnjuh.cn

[Q59] 分组内累计
来源：http://dg.yuntaijiaju.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kx.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://ey.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bb.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tc.9csxet.cn

[Q61] 移动平均
来源：http://yr.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iy.hnjuh.cn

[Q62] 分组占比
来源：http://ti.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://de.hahajie.cn

[Q63] 开启事务
来源：http://hr.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cd.muxihuayi.cn

[Q64] 提交事务
来源：http://fj.bjjhwx.cn

COMMIT;
来源：http://gk.wgjwhj.cn

[Q65] 回滚事务
来源：http://yn.hahajie.cn

ROLLBACK;
来源：http://bn.asd995.cn

[Q66] 行锁查询
来源：http://gz.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zv.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://fb.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://af.hnjuh.cn

[Q68] 保存点
来源：http://ef.wgjwhj.cn

SAVEPOINT sp1;
来源：http://cp.gzmigu.cn

ROLLBACK TO sp1;
来源：http://ud.huixiangedu.cn

[Q69] 查看执行计划
来源：http://tc.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ie.shxzskj.cn

[Q70] 更新统计信息
来源：http://lj.huanxung.cn

ANALYZE TABLE users;
来源：http://tn.newstarts.cn

[Q71] 查看建表语句
来源：http://kg.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dm.shxzskj.cn

[Q72] 查看索引
来源：http://oj.hnjuh.cn

SHOW INDEX FROM users;
来源：http://ks.colortex.cn

[Q73] 查看表状态
来源：http://cp.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gr.newstarts.cn

[Q74] 强制使用索引
来源：http://ww.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zc.szsharing.cn

[Q75] 日期格式化
来源：http://or.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xc.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kc.hahajie.cn

[Q76] 按天统计
来源：http://dn.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fk.jianghongdianzi.cn

[Q77] 时间加减
来源：http://fc.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nq.colortex.cn

[Q78] 当前时间
来源：http://ge.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jg.chemitech.net.cn

[Q79] 字符串拼接
来源：http://cn.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fo.gzmigu.cn

[Q80] 字符串截取
来源：http://cx.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cu.asd995.cn

[Q81] 字符串替换
来源：http://gx.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tj.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://qi.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tp.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://gg.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dd.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://bc.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://bs.newstarts.cn

[Q85] 数值取整
来源：http://nb.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ca.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://kf.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cx.nszjky.cn

[Q87] JSON 字段做条件
来源：http://xa.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hg.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://wy.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://co.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eo.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://vj.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vf.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://gg.jctech888.com.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lr.wgjwhj.cn

================================================================================
来源：http://kp.panjiajie.cn

R. Bash 专题
来源：http://yu.haigaiapp.cn

================================================================================
来源：http://by.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://sk.nicolike.cn

#!/usr/bin/env bash
来源：http://ub.yuexingan06.cn

set -euo pipefail
来源：http://kp.hnjuh.cn

[R02] 变量赋值与使用
来源：http://ig.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://xl.newstarts.cn

[R03] 只读变量
来源：http://kr.9csxet.cn

readonly PI=3.14
来源：http://rt.huixinmuqiang.cn

[R04] 位置参数
来源：http://eg.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ac.521024.cn

[R05] 参数默认值
来源：http://ep.yuexingan06.cn

name="${1:-default}"
来源：http://dt.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://zz.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ju.nszjky.cn

[R07] if 判断文件
来源：http://ko.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gv.hnjuh.cn

[R08] 数值比较
来源：http://ts.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oo.shxzukj.cn

[R09] 字符串比较
来源：http://di.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ku.hahajie.cn

[R10] 正则匹配
来源：http://np.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tf.colortex.cn

[R11] case 多分支
来源：http://tg.lnxyls.cn

case "$1" in
来源：http://pe.bjjhwx.cn

start) echo "启动" ;;
来源：http://ov.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://rn.nicolike.cn

*)     echo "未知命令" ;;
来源：http://mw.yuntaijiaju.cn

esac
来源：http://yp.szxytkj.cn

[R12] for 遍历文件
来源：http://pk.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://bn.521024.cn

[R13] for 计数循环
来源：http://em.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://xz.nszjky.cn

[R14] C 风格 for
来源：http://bt.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nu.newstarts.cn

[R15] while 逐行读文件
来源：http://qe.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lt.nszjky.cn

[R16] until 等待条件
来源：http://ku.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uw.newstarts.cn

[R17] 数组定义与取值
来源：http://iz.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://at.asd995.cn

[R18] 遍历数组
来源：http://qi.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gy.shtwfgs.cn

[R19] 数组长度
来源：http://vr.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://sn.521024.cn

[R20] 关联数组（字典）
来源：http://pa.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sp.szxytkj.cn

[R21] 字符串长度
来源：http://fq.newstarts.cn

echo "${#s}"
来源：http://nh.szxytkj.cn

[R22] 截取子串
来源：http://fs.bookmarksfly.cn

echo "${s:0:5}"
来源：http://qo.colortex.cn

[R23] 字符串替换
来源：http://ot.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jy.nicolike.cn

[R24] 大小写转换
来源：http://oi.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zo.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://rx.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gf.shtwfgs.cn

[R26] 命令替换
来源：http://vx.haigaiapp.cn

now=$(date +%F); echo "$now"
来源：http://vy.colortex.cn

[R27] 算术展开
来源：http://ws.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://rx.bookmarksfly.cn

[R28] 浮点运算
来源：http://sf.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://qk.yuntaijiaju.cn

[R29] 定义函数
来源：http://kd.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pz.521024.cn

[R30] 函数返回状态码
来源：http://yw.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://co.bjjhwx.cn

[R31] 局部变量
来源：http://qb.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://ec.colortex.cn

[R32] 参数个数校验
来源：http://fb.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aw.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://qg.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jt.panjiajie.cn

[R34] 退出时清理
来源：http://zq.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rx.9csxet.cn

[R35] 后台执行并等待
来源：http://ik.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gs.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://yo.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kx.asd995.cn

[R37] 把输出赋给变量
来源：http://cy.colortex.cn

files=$(ls -1)
来源：http://mw.huixiangedu.cn

[R38] 管道串联
来源：http://ej.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://pv.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://du.521024.cn

cmd > out.log 2>&1
来源：http://dd.bjjhwx.cn

[R40] 追加写日志
来源：http://rf.nicolike.cn

echo "log" >> out.log
来源：http://am.shtwfgs.cn

[R41] 丢弃输出
来源：http://cu.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://gl.jctech888.com.cn

[R42] 输入重定向
来源：http://fa.huixiangedu.cn

wc -l < a.txt
来源：http://nz.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://zn.wgjwhj.cn

find . -name "*.log" -type f
来源：http://ku.panjiajie.cn

[R44] 按修改时间查找
来源：http://rt.shtwfgs.cn

find . -mtime -7 -type f
来源：http://ev.gzmigu.cn

[R45] 批量删除
来源：http://ea.chemitech.net.cn


<!-- 参考信息 -->