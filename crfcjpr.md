代发 wailian999

================================================================================
来源：http://fn.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rl.yuexingan06.cn

================================================================================
来源：http://pj.colortex.cn

[Q01] 创建表
来源：http://pc.521024.cn

CREATE TABLE users (
来源：http://gm.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ht.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://fb.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://ev.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lp.bookmarksfly.cn

);
来源：http://pe.nszjky.cn

[Q02] 创建带外键的表
来源：http://gx.panjiajie.cn

CREATE TABLE orders (
来源：http://mf.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lr.szsharing.cn

user_id INT NOT NULL,
来源：http://bu.szsharing.cn

amount DECIMAL(10, 2),
来源：http://hy.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yv.panjiajie.cn

);
来源：http://zh.hahajie.cn

[Q03] 增加列
来源：http://uv.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jx.huanxung.cn

[Q04] 修改列类型
来源：http://dc.hahajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cl.nicolike.cn

[Q05] 重命名列
来源：http://fd.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ct.9csxet.cn

[Q06] 删除列
来源：http://bk.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://he.szsharing.cn

[Q07] 删除表
来源：http://mw.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://ge.jctech888.com.cn

[Q08] 创建普通索引
来源：http://qj.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://le.shxzskj.cn

[Q09] 创建唯一索引
来源：http://pp.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nw.yuntaijiaju.cn

[Q10] 插入单行
来源：http://cp.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vv.nicolike.cn

[Q11] 一次插入多行
来源：http://fp.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ih.colortex.cn

[Q12] 插入后取自增 ID
来源：http://za.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xt.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aa.gzmigu.cn

[Q13] 忽略重复插入
来源：http://ul.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pb.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://be.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cf.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zl.hnjuh.cn

[Q15] 查询全部
来源：http://oq.asd995.cn

SELECT * FROM users;
来源：http://hi.chemitech.net.cn

[Q16] 查询指定列
来源：http://no.lnxyls.cn

SELECT id, name FROM users;
来源：http://ss.huixinmuqiang.cn

[Q17] 条件查询
来源：http://mz.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lk.nszjky.cn

[Q18] 模糊匹配
来源：http://nq.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bw.wgjwhj.cn

[Q19] 范围查询
来源：http://nc.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dg.colortex.cn

[Q20] IN 列表
来源：http://vi.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vk.hahajie.cn

[Q21] 空值判断
来源：http://dy.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://iw.huanxung.cn

[Q22] 排序
来源：http://oz.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cq.shxzukj.cn

[Q23] 分页
来源：http://pl.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yh.newstarts.cn

[Q24] 去重
来源：http://gq.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://bb.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://xs.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lw.521024.cn

[Q26] 计数
来源：http://to.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://bd.nicolike.cn

[Q27] 条件计数
来源：http://dk.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gm.muxihuayi.cn

[Q28] 求和与平均
来源：http://av.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://um.bookmarksfly.cn

[Q29] 最大最小值
来源：http://xr.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xf.yuexingan06.cn

[Q30] 分组统计
来源：http://oq.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ei.panjiajie.cn

[Q31] 分组后过滤
来源：http://fg.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pd.szsharing.cn

[Q32] 分组拼接字符串
来源：http://lk.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dw.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jc.nicolike.cn

[Q33] 多列分组
来源：http://ma.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sn.nszjky.cn

[Q34] 每组取第一条
来源：http://gi.gzmigu.cn

SELECT * FROM (
来源：http://fb.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://so.hahajie.cn

) t WHERE rn = 1;
来源：http://mo.wgjwhj.cn

[Q35] 内连接
来源：http://yb.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mj.9csxet.cn

[Q36] 左连接
来源：http://pj.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://an.hnjuh.cn

[Q37] 右连接
来源：http://fo.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ja.haigaiapp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zj.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tk.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://jl.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sq.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ze.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fn.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vo.lnxyls.cn

[Q41] 多表连接
来源：http://ia.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cv.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://vz.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://ta.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://fi.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://ad.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ad.colortex.cn

[Q43] 标量子查询
来源：http://jv.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fw.9csxet.cn

[Q44] IN 子查询
来源：http://tt.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uq.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://ce.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lk.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dg.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sh.521024.cn

[Q47] 与平均值比较
来源：http://bs.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qc.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://zm.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://af.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://db.chemitech.net.cn

[Q49] 更新单行
来源：http://jd.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ad.shxzukj.cn

[Q50] 批量更新
来源：http://qr.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tw.gzmigu.cn

[Q51] 用子查询更新
来源：http://du.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hq.yuexingan06.cn

[Q52] 删除指定行
来源：http://ml.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://nq.shxzskj.cn

[Q53] 按条件删除
来源：http://eg.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rv.hnjuh.cn

[Q54] 清空表
来源：http://vd.colortex.cn

TRUNCATE TABLE logs;
来源：http://ng.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://do.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://il.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://dv.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://on.newstarts.cn

[Q57] 行号
来源：http://mi.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://er.huanxung.cn

[Q58] 累计求和
来源：http://rl.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fb.muxihuayi.cn

[Q59] 分组内累计
来源：http://ty.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://na.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://dv.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ub.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dt.chemitech.net.cn

[Q61] 移动平均
来源：http://wo.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://es.panjiajie.cn

[Q62] 分组占比
来源：http://cs.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ce.hahajie.cn

[Q63] 开启事务
来源：http://zq.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rb.huanxung.cn

[Q64] 提交事务
来源：http://qg.9csxet.cn

COMMIT;
来源：http://tm.shxzskj.cn

[Q65] 回滚事务
来源：http://la.huixiangedu.cn

ROLLBACK;
来源：http://mm.chemitech.net.cn

[Q66] 行锁查询
来源：http://na.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wh.szsharing.cn

[Q67] 设置隔离级别
来源：http://my.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ad.wgjwhj.cn

[Q68] 保存点
来源：http://mu.jctech888.com.cn

SAVEPOINT sp1;
来源：http://np.nszjky.cn

ROLLBACK TO sp1;
来源：http://ql.szsharing.cn

[Q69] 查看执行计划
来源：http://rt.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ub.521024.cn

[Q70] 更新统计信息
来源：http://yp.huixiangedu.cn

ANALYZE TABLE users;
来源：http://pi.9csxet.cn

[Q71] 查看建表语句
来源：http://sg.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ok.bookmarksfly.cn

[Q72] 查看索引
来源：http://yc.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://nk.huixiangedu.cn

[Q73] 查看表状态
来源：http://hd.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dz.colortex.cn

[Q74] 强制使用索引
来源：http://fd.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ul.asd995.cn

[Q75] 日期格式化
来源：http://ji.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vp.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eq.panjiajie.cn

[Q76] 按天统计
来源：http://ff.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ig.hahajie.cn

[Q77] 时间加减
来源：http://ju.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zf.jctech888.com.cn

[Q78] 当前时间
来源：http://fv.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kg.wgjwhj.cn

[Q79] 字符串拼接
来源：http://ad.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ot.newstarts.cn

[Q80] 字符串截取
来源：http://up.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lj.chemitech.net.cn

[Q81] 字符串替换
来源：http://jx.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fi.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://ik.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ko.nszjky.cn

[Q83] 大小写转换
来源：http://ll.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yh.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://ou.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://jq.hahajie.cn

[Q85] 数值取整
来源：http://kd.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lv.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://lb.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pl.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://wt.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dx.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://ji.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sb.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gc.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://wx.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jq.haigaiapp.cn

[Q90] 生成序号列
来源：http://tn.jctech888.com.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://op.nszjky.cn

================================================================================
来源：http://ba.szxytkj.cn

R. Bash 专题
来源：http://ia.asd995.cn

================================================================================
来源：http://ei.hahajie.cn

[R01] shebang 与严格模式
来源：http://rr.hnjuh.cn

#!/usr/bin/env bash
来源：http://vx.chemitech.net.cn

set -euo pipefail
来源：http://uc.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://id.shxzskj.cn

name="Tom"; echo "$name"
来源：http://wl.shxzskj.cn

[R03] 只读变量
来源：http://qm.hnjuh.cn

readonly PI=3.14
来源：http://wz.shtwfgs.cn

[R04] 位置参数
来源：http://qa.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gp.9csxet.cn

[R05] 参数默认值
来源：http://sf.lnxyls.cn

name="${1:-default}"
来源：http://pe.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://ai.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ac.nszjky.cn

[R07] if 判断文件
来源：http://yh.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ib.yuexingan06.cn

[R08] 数值比较
来源：http://qs.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kq.colortex.cn

[R09] 字符串比较
来源：http://lx.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fp.jctech888.com.cn

[R10] 正则匹配
来源：http://cu.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://de.shtwfgs.cn

[R11] case 多分支
来源：http://se.jianghongdianzi.cn

case "$1" in
来源：http://sl.shxzskj.cn

start) echo "启动" ;;
来源：http://mt.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://rd.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://zy.shtwfgs.cn

esac
来源：http://pc.shxzukj.cn

[R12] for 遍历文件
来源：http://kj.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://cm.yuntaijiaju.cn

[R13] for 计数循环
来源：http://yw.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://oa.nszjky.cn

[R14] C 风格 for
来源：http://yl.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bl.nszjky.cn

[R15] while 逐行读文件
来源：http://js.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lr.hahajie.cn

[R16] until 等待条件
来源：http://jy.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ab.gzmigu.cn

[R17] 数组定义与取值
来源：http://jq.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://by.panjiajie.cn

[R18] 遍历数组
来源：http://qg.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sy.jctech888.com.cn

[R19] 数组长度
来源：http://gu.huanxung.cn

echo "${#arr[@]}"
来源：http://sb.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://pj.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yl.shtwfgs.cn

[R21] 字符串长度
来源：http://cf.shtwfgs.cn

echo "${#s}"
来源：http://lp.bjjhwx.cn

[R22] 截取子串
来源：http://jv.shxzskj.cn

echo "${s:0:5}"
来源：http://rh.huixinmuqiang.cn

[R23] 字符串替换
来源：http://ls.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gn.nszjky.cn

[R24] 大小写转换
来源：http://lp.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bp.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://nu.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kx.panjiajie.cn

[R26] 命令替换
来源：http://rb.colortex.cn

now=$(date +%F); echo "$now"
来源：http://st.yuexingan06.cn

[R27] 算术展开
来源：http://zv.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://pm.colortex.cn

[R28] 浮点运算
来源：http://ju.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://ks.hahajie.cn

[R29] 定义函数
来源：http://xr.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ji.szsharing.cn

[R30] 函数返回状态码
来源：http://gu.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://jc.9csxet.cn

[R31] 局部变量
来源：http://qe.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://qe.chemitech.net.cn

[R32] 参数个数校验
来源：http://so.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ar.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://vd.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tz.newstarts.cn

[R34] 退出时清理
来源：http://fu.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nr.jctech888.com.cn

[R35] 后台执行并等待
来源：http://wz.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fi.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://iu.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pr.asd995.cn

[R37] 把输出赋给变量
来源：http://xs.colortex.cn

files=$(ls -1)
来源：http://qw.muxihuayi.cn

[R38] 管道串联
来源：http://qr.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://ht.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://nc.nszjky.cn

cmd > out.log 2>&1
来源：http://uw.huanxung.cn

[R40] 追加写日志
来源：http://qo.bookmarksfly.cn

echo "log" >> out.log
来源：http://mp.gzmigu.cn

[R41] 丢弃输出
来源：http://mx.9csxet.cn

cmd >/dev/null 2>&1
来源：http://os.chemitech.net.cn

[R42] 输入重定向
来源：http://cc.panjiajie.cn

wc -l < a.txt
来源：http://ab.shxzukj.cn

[R43] 按名字查找文件
来源：http://vq.shxzskj.cn


<!-- 参考信息 -->