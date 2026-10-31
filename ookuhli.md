代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://to.nicolike.cn

);
来源：http://vl.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://we.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://yq.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wv.asd995.cn

user_id INT NOT NULL,
来源：http://si.colortex.cn

amount DECIMAL(10, 2),
来源：http://sz.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pj.yuntaijiaju.cn

);
来源：http://st.shxzskj.cn

[Q03] 增加列
来源：http://zf.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mp.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://jz.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dx.shxzukj.cn

[Q05] 重命名列
来源：http://zz.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yh.nicolike.cn

[Q06] 删除列
来源：http://gc.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wl.shxzskj.cn

[Q07] 删除表
来源：http://iz.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://fh.szsharing.cn

[Q08] 创建普通索引
来源：http://ee.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://em.hnjuh.cn

[Q09] 创建唯一索引
来源：http://iy.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tm.shxzukj.cn

[Q10] 插入单行
来源：http://ko.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dk.panjiajie.cn

[Q11] 一次插入多行
来源：http://qy.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xi.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://cu.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sh.nicolike.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jd.nicolike.cn

[Q13] 忽略重复插入
来源：http://dj.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ul.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://zy.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vt.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xu.huixinmuqiang.cn

[Q15] 查询全部
来源：http://zo.wgjwhj.cn

SELECT * FROM users;
来源：http://hi.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://rn.shxzukj.cn

SELECT id, name FROM users;
来源：http://gz.szsharing.cn

[Q17] 条件查询
来源：http://bw.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ek.hnjuh.cn

[Q18] 模糊匹配
来源：http://ld.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yr.muxihuayi.cn

[Q19] 范围查询
来源：http://hu.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nn.panjiajie.cn

[Q20] IN 列表
来源：http://dj.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hv.muxihuayi.cn

[Q21] 空值判断
来源：http://dx.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aa.yuntaijiaju.cn

[Q22] 排序
来源：http://bq.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ej.lnxyls.cn

[Q23] 分页
来源：http://zy.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nj.shxzskj.cn

[Q24] 去重
来源：http://pc.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://sh.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://ar.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ka.bookmarksfly.cn

[Q26] 计数
来源：http://xd.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://zw.yuexingan06.cn

[Q27] 条件计数
来源：http://et.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dj.chemitech.net.cn

[Q28] 求和与平均
来源：http://is.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dt.shxzukj.cn

[Q29] 最大最小值
来源：http://cr.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zx.shxzukj.cn

[Q30] 分组统计
来源：http://qi.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dx.huixiangedu.cn

[Q31] 分组后过滤
来源：http://hv.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mv.colortex.cn

[Q32] 分组拼接字符串
来源：http://ay.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://di.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qn.shxzukj.cn

[Q33] 多列分组
来源：http://lh.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ap.wgjwhj.cn

[Q34] 每组取第一条
来源：http://kd.lnxyls.cn

SELECT * FROM (
来源：http://qt.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hw.szsharing.cn

) t WHERE rn = 1;
来源：http://im.shxzskj.cn

[Q35] 内连接
来源：http://nz.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oc.bjjhwx.cn

[Q36] 左连接
来源：http://ot.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ma.nszjky.cn

[Q37] 右连接
来源：http://ny.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sw.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rb.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vz.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://es.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ws.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mg.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lp.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cw.szxytkj.cn

[Q41] 多表连接
来源：http://sb.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yg.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://tw.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://to.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://gj.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://ma.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yh.szsharing.cn

[Q43] 标量子查询
来源：http://on.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xc.lnxyls.cn

[Q44] IN 子查询
来源：http://em.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kz.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://ze.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cp.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bv.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ti.szsharing.cn

[Q47] 与平均值比较
来源：http://qz.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qd.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://by.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nf.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://jc.chemitech.net.cn

[Q49] 更新单行
来源：http://ot.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cc.jianghongdianzi.cn

[Q50] 批量更新
来源：http://bz.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yb.colortex.cn

[Q51] 用子查询更新
来源：http://nw.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gf.9csxet.cn

[Q52] 删除指定行
来源：http://qp.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://gp.jctech888.com.cn

[Q53] 按条件删除
来源：http://zk.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bh.hahajie.cn

[Q54] 清空表
来源：http://le.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://uk.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://dr.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ps.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://rw.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zd.shtwfgs.cn

[Q57] 行号
来源：http://ag.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sa.wgjwhj.cn

[Q58] 累计求和
来源：http://mv.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bv.szsharing.cn

[Q59] 分组内累计
来源：http://rt.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cz.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://te.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ji.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hn.shxzukj.cn

[Q61] 移动平均
来源：http://ir.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kp.jctech888.com.cn

[Q62] 分组占比
来源：http://lb.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uj.huanxung.cn

[Q63] 开启事务
来源：http://ir.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gc.bjjhwx.cn

[Q64] 提交事务
来源：http://pt.yuntaijiaju.cn

COMMIT;
来源：http://sh.szsharing.cn

[Q65] 回滚事务
来源：http://rg.nicolike.cn

ROLLBACK;
来源：http://tq.gzmigu.cn

[Q66] 行锁查询
来源：http://uu.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rs.9csxet.cn

[Q67] 设置隔离级别
来源：http://rc.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ot.shxzukj.cn

[Q68] 保存点
来源：http://ay.bjjhwx.cn

SAVEPOINT sp1;
来源：http://ox.nszjky.cn

ROLLBACK TO sp1;
来源：http://sf.bjjhwx.cn

[Q69] 查看执行计划
来源：http://hw.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://or.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://ur.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://ed.shxzukj.cn

[Q71] 查看建表语句
来源：http://yp.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://la.jctech888.com.cn

[Q72] 查看索引
来源：http://pw.huanxung.cn

SHOW INDEX FROM users;
来源：http://vv.lnxyls.cn

[Q73] 查看表状态
来源：http://ny.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ib.hahajie.cn

[Q74] 强制使用索引
来源：http://wa.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dz.shtwfgs.cn

[Q75] 日期格式化
来源：http://kg.szsharing.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mx.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hr.newstarts.cn

[Q76] 按天统计
来源：http://sb.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pn.szxytkj.cn

[Q77] 时间加减
来源：http://jx.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ev.haigaiapp.cn

[Q78] 当前时间
来源：http://rb.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qh.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://bj.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mq.wgjwhj.cn

[Q80] 字符串截取
来源：http://yf.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gj.asd995.cn

[Q81] 字符串替换
来源：http://ma.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kk.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://wn.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aw.yuexingan06.cn

[Q83] 大小写转换
来源：http://fr.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cj.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://hg.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://gz.colortex.cn

[Q85] 数值取整
来源：http://zk.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xr.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://xb.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ww.9csxet.cn

[Q87] JSON 字段做条件
来源：http://ff.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gm.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://ws.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gg.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sn.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://so.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jw.colortex.cn

[Q90] 生成序号列
来源：http://fq.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uq.huixinmuqiang.cn

================================================================================
来源：http://ir.huixinmuqiang.cn

R. Bash 专题
来源：http://ba.gzmigu.cn

================================================================================
来源：http://de.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://ur.chemitech.net.cn

#!/usr/bin/env bash
来源：http://sw.colortex.cn

set -euo pipefail
来源：http://ed.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://cb.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://oi.newstarts.cn

[R03] 只读变量
来源：http://rl.hnjuh.cn

readonly PI=3.14
来源：http://yl.yuntaijiaju.cn

[R04] 位置参数
来源：http://ho.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lk.chemitech.net.cn

[R05] 参数默认值
来源：http://pu.hahajie.cn

name="${1:-default}"
来源：http://ot.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://mu.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pt.haigaiapp.cn

[R07] if 判断文件
来源：http://hd.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yf.huanxung.cn

[R08] 数值比较
来源：http://ri.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dq.bjjhwx.cn

[R09] 字符串比较
来源：http://aa.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lv.nicolike.cn

[R10] 正则匹配
来源：http://rr.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zr.shxzukj.cn

[R11] case 多分支
来源：http://wk.asd995.cn

case "$1" in
来源：http://zi.bookmarksfly.cn

start) echo "启动" ;;
来源：http://pm.szxytkj.cn

stop)  echo "停止" ;;
来源：http://oz.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://ni.yuexingan06.cn

esac
来源：http://te.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://uc.shxzskj.cn

for f in *.txt; do echo "$f"; done
来源：http://oe.lnxyls.cn

[R13] for 计数循环
来源：http://hm.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://ra.yuexingan06.cn

[R14] C 风格 for
来源：http://kh.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ar.521024.cn

[R15] while 逐行读文件
来源：http://ny.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ho.chemitech.net.cn

[R16] until 等待条件
来源：http://vx.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ue.521024.cn

[R17] 数组定义与取值
来源：http://ep.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://iy.muxihuayi.cn

[R18] 遍历数组
来源：http://ag.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://su.shxzukj.cn

[R19] 数组长度
来源：http://ri.hahajie.cn

echo "${#arr[@]}"
来源：http://rk.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://gi.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cg.muxihuayi.cn

[R21] 字符串长度
来源：http://gu.szxytkj.cn

echo "${#s}"
来源：http://bu.bookmarksfly.cn

[R22] 截取子串
来源：http://yn.9csxet.cn

echo "${s:0:5}"
来源：http://lr.haigaiapp.cn

[R23] 字符串替换
来源：http://xe.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vx.panjiajie.cn

[R24] 大小写转换
来源：http://kv.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://my.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://nr.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qu.jianghongdianzi.cn

[R26] 命令替换
来源：http://cq.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://yv.asd995.cn

[R27] 算术展开
来源：http://qj.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://uu.shtwfgs.cn

[R28] 浮点运算
来源：http://er.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://yv.nicolike.cn

[R29] 定义函数
来源：http://or.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xj.nszjky.cn

[R30] 函数返回状态码
来源：http://io.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://cv.asd995.cn

[R31] 局部变量
来源：http://sz.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://sg.bjjhwx.cn

[R32] 参数个数校验
来源：http://bm.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ih.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://xu.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jk.haigaiapp.cn

[R34] 退出时清理
来源：http://dd.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dc.chemitech.net.cn

[R35] 后台执行并等待
来源：http://ye.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zr.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://qd.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ri.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://en.521024.cn

files=$(ls -1)
来源：http://sv.huixiangedu.cn

[R38] 管道串联
来源：http://ns.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://wj.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://xd.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://ek.nszjky.cn

[R40] 追加写日志
来源：http://er.haigaiapp.cn

echo "log" >> out.log
来源：http://vc.521024.cn

[R41] 丢弃输出
来源：http://px.hahajie.cn

cmd >/dev/null 2>&1
来源：http://ql.chemitech.net.cn

[R42] 输入重定向
来源：http://ap.chemitech.net.cn

wc -l < a.txt
来源：http://lu.521024.cn

[R43] 按名字查找文件
来源：http://qa.asd995.cn

find . -name "*.log" -type f
来源：http://ds.muxihuayi.cn

[R44] 按修改时间查找
来源：http://sn.nicolike.cn

find . -mtime -7 -type f
来源：http://mo.haigaiapp.cn

[R45] 批量删除
来源：http://ca.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://og.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://ht.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://et.shxzskj.cn

[R47] sed 单行替换
来源：http://yh.szsharing.cn


<!-- 参考信息 -->