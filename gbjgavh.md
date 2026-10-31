代发 wailian999

================================================================================
来源：http://ce.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sp.panjiajie.cn

================================================================================
来源：http://jm.wgjwhj.cn

[Q01] 创建表
来源：http://tj.yuexingan06.cn

CREATE TABLE users (
来源：http://lo.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hh.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://dn.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://uu.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ve.jianghongdianzi.cn

);
来源：http://ax.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://ko.yuexingan06.cn

CREATE TABLE orders (
来源：http://sv.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tg.newstarts.cn

user_id INT NOT NULL,
来源：http://zj.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://hx.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ql.szxytkj.cn

);
来源：http://hx.hnjuh.cn

[Q03] 增加列
来源：http://ai.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://su.nicolike.cn

[Q04] 修改列类型
来源：http://az.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rm.shxzukj.cn

[Q05] 重命名列
来源：http://zh.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fy.yuexingan06.cn

[Q06] 删除列
来源：http://sl.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://us.shxzskj.cn

[Q07] 删除表
来源：http://iv.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://hz.jctech888.com.cn

[Q08] 创建普通索引
来源：http://mu.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qo.9csxet.cn

[Q09] 创建唯一索引
来源：http://np.huixiangedu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vv.panjiajie.cn

[Q10] 插入单行
来源：http://ee.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yt.nicolike.cn

[Q11] 一次插入多行
来源：http://ur.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rd.521024.cn

[Q12] 插入后取自增 ID
来源：http://vj.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kw.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fm.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://yl.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://th.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://oa.panjiajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ni.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vv.shxzskj.cn

[Q15] 查询全部
来源：http://cb.chemitech.net.cn

SELECT * FROM users;
来源：http://tp.asd995.cn

[Q16] 查询指定列
来源：http://tr.chemitech.net.cn

SELECT id, name FROM users;
来源：http://so.9csxet.cn

[Q17] 条件查询
来源：http://ag.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lu.nicolike.cn

[Q18] 模糊匹配
来源：http://qw.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ty.yuntaijiaju.cn

[Q19] 范围查询
来源：http://kd.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://af.shxzskj.cn

[Q20] IN 列表
来源：http://ik.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pu.haigaiapp.cn

[Q21] 空值判断
来源：http://rv.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gq.huixiangedu.cn

[Q22] 排序
来源：http://eq.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mo.nszjky.cn

[Q23] 分页
来源：http://vk.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sf.hnjuh.cn

[Q24] 去重
来源：http://pu.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://vp.521024.cn

[Q25] 只取前 N 条
来源：http://kw.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yb.bookmarksfly.cn

[Q26] 计数
来源：http://js.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://xb.jianghongdianzi.cn

[Q27] 条件计数
来源：http://nh.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kx.asd995.cn

[Q28] 求和与平均
来源：http://hv.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://of.nicolike.cn

[Q29] 最大最小值
来源：http://ke.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vf.colortex.cn

[Q30] 分组统计
来源：http://cw.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gk.hahajie.cn

[Q31] 分组后过滤
来源：http://pz.haigaiapp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pv.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://qf.hahajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qg.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ay.nszjky.cn

[Q33] 多列分组
来源：http://zx.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fg.nicolike.cn

[Q34] 每组取第一条
来源：http://fg.gzmigu.cn

SELECT * FROM (
来源：http://ra.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uo.bjjhwx.cn

) t WHERE rn = 1;
来源：http://vw.huixinmuqiang.cn

[Q35] 内连接
来源：http://ru.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pi.9csxet.cn

[Q36] 左连接
来源：http://fs.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://su.huanxung.cn

[Q37] 右连接
来源：http://gc.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dn.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dl.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sk.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://me.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qw.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dd.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rh.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xn.jctech888.com.cn

[Q41] 多表连接
来源：http://xc.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://us.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://qq.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://nl.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://zr.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://ag.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://en.chemitech.net.cn

[Q43] 标量子查询
来源：http://vc.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yf.shxzskj.cn

[Q44] IN 子查询
来源：http://da.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://om.asd995.cn

[Q45] EXISTS 判断存在
来源：http://il.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ms.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ws.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://us.bjjhwx.cn

[Q47] 与平均值比较
来源：http://uc.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ol.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://ry.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wq.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://mj.huanxung.cn

[Q49] 更新单行
来源：http://ta.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ak.hahajie.cn

[Q50] 批量更新
来源：http://ri.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qq.shxzskj.cn

[Q51] 用子查询更新
来源：http://kg.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ic.bjjhwx.cn

[Q52] 删除指定行
来源：http://ov.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://wf.shxzukj.cn

[Q53] 按条件删除
来源：http://ug.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yi.wgjwhj.cn

[Q54] 清空表
来源：http://iq.9csxet.cn

TRUNCATE TABLE logs;
来源：http://bc.szsharing.cn

[Q55] 排名（并列占位）
来源：http://ia.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ax.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://zh.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://py.jianghongdianzi.cn

[Q57] 行号
来源：http://ha.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://em.asd995.cn

[Q58] 累计求和
来源：http://zn.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yo.nicolike.cn

[Q59] 分组内累计
来源：http://hu.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uj.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://dk.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pb.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cg.panjiajie.cn

[Q61] 移动平均
来源：http://uy.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ow.szsharing.cn

[Q62] 分组占比
来源：http://mn.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dz.lnxyls.cn

[Q63] 开启事务
来源：http://fd.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uz.jctech888.com.cn

[Q64] 提交事务
来源：http://bz.huixinmuqiang.cn

COMMIT;
来源：http://be.hnjuh.cn

[Q65] 回滚事务
来源：http://gn.jctech888.com.cn

ROLLBACK;
来源：http://gq.chemitech.net.cn

[Q66] 行锁查询
来源：http://wq.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://py.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://yg.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bf.haigaiapp.cn

[Q68] 保存点
来源：http://fv.panjiajie.cn

SAVEPOINT sp1;
来源：http://gx.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://oa.521024.cn

[Q69] 查看执行计划
来源：http://fk.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dj.hahajie.cn

[Q70] 更新统计信息
来源：http://zs.shxzskj.cn

ANALYZE TABLE users;
来源：http://hq.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://ah.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mb.yuexingan06.cn

[Q72] 查看索引
来源：http://kq.hahajie.cn

SHOW INDEX FROM users;
来源：http://mb.9csxet.cn

[Q73] 查看表状态
来源：http://hw.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bp.szsharing.cn

[Q74] 强制使用索引
来源：http://vu.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bk.newstarts.cn

[Q75] 日期格式化
来源：http://fj.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wg.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hs.huixinmuqiang.cn

[Q76] 按天统计
来源：http://qg.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://af.hahajie.cn

[Q77] 时间加减
来源：http://ur.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oj.wgjwhj.cn

[Q78] 当前时间
来源：http://ls.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rg.huixiangedu.cn

[Q79] 字符串拼接
来源：http://zr.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gn.gzmigu.cn

[Q80] 字符串截取
来源：http://xm.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bm.newstarts.cn

[Q81] 字符串替换
来源：http://qn.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vq.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://fd.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qc.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://ob.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ti.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://xe.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://dc.asd995.cn

[Q85] 数值取整
来源：http://km.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bn.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://ar.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wi.huanxung.cn

[Q87] JSON 字段做条件
来源：http://cx.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ya.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://qf.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ft.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ex.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://qt.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sg.nszjky.cn

[Q90] 生成序号列
来源：http://id.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gg.shxzukj.cn

================================================================================
来源：http://wy.bjjhwx.cn

R. Bash 专题
来源：http://ny.chemitech.net.cn

================================================================================
来源：http://qo.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://ug.muxihuayi.cn

#!/usr/bin/env bash
来源：http://na.gzmigu.cn

set -euo pipefail
来源：http://cx.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://qx.asd995.cn

name="Tom"; echo "$name"
来源：http://ai.szsharing.cn

[R03] 只读变量
来源：http://wi.muxihuayi.cn

readonly PI=3.14
来源：http://ff.asd995.cn

[R04] 位置参数
来源：http://yy.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jb.huixiangedu.cn

[R05] 参数默认值
来源：http://kp.lnxyls.cn

name="${1:-default}"
来源：http://ev.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://yj.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wq.9csxet.cn

[R07] if 判断文件
来源：http://zx.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bd.shxzskj.cn

[R08] 数值比较
来源：http://ny.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kp.9csxet.cn

[R09] 字符串比较
来源：http://cr.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uz.gzmigu.cn

[R10] 正则匹配
来源：http://kf.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://te.huixiangedu.cn

[R11] case 多分支
来源：http://yg.shtwfgs.cn

case "$1" in
来源：http://gg.chemitech.net.cn

start) echo "启动" ;;
来源：http://lc.huanxung.cn

stop)  echo "停止" ;;
来源：http://yc.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://fp.yuexingan06.cn

esac
来源：http://kd.newstarts.cn

[R12] for 遍历文件
来源：http://xi.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://xd.colortex.cn

[R13] for 计数循环
来源：http://hr.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://hl.haigaiapp.cn

[R14] C 风格 for
来源：http://un.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vc.huixiangedu.cn

[R15] while 逐行读文件
来源：http://aa.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ta.huixinmuqiang.cn

[R16] until 等待条件
来源：http://co.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://by.newstarts.cn

[R17] 数组定义与取值
来源：http://bd.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sl.muxihuayi.cn

[R18] 遍历数组
来源：http://de.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://my.nicolike.cn

[R19] 数组长度
来源：http://hp.huixiangedu.cn

echo "${#arr[@]}"
来源：http://yo.shxzukj.cn

[R20] 关联数组（字典）
来源：http://sg.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://db.asd995.cn

[R21] 字符串长度
来源：http://gm.chemitech.net.cn

echo "${#s}"
来源：http://zy.9csxet.cn

[R22] 截取子串
来源：http://zp.szsharing.cn

echo "${s:0:5}"
来源：http://gq.shxzskj.cn

[R23] 字符串替换
来源：http://wq.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ri.huixiangedu.cn

[R24] 大小写转换
来源：http://hf.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zv.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://re.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sf.hahajie.cn

[R26] 命令替换
来源：http://ty.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://xk.szxytkj.cn

[R27] 算术展开
来源：http://ey.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://sj.huanxung.cn

[R28] 浮点运算
来源：http://ig.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://il.yuexingan06.cn

[R29] 定义函数
来源：http://um.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nx.bjjhwx.cn

[R30] 函数返回状态码
来源：http://zr.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://rj.nszjky.cn

[R31] 局部变量
来源：http://ta.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://fs.haigaiapp.cn

[R32] 参数个数校验
来源：http://sp.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ym.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://ed.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ye.9csxet.cn

[R34] 退出时清理
来源：http://wi.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pz.nicolike.cn

[R35] 后台执行并等待
来源：http://wy.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cp.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://fh.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yw.szsharing.cn

[R37] 把输出赋给变量
来源：http://oe.panjiajie.cn

files=$(ls -1)
来源：http://lg.shxzukj.cn

[R38] 管道串联
来源：http://nn.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://zi.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://ye.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://yn.muxihuayi.cn

[R40] 追加写日志
来源：http://pe.huanxung.cn

echo "log" >> out.log
来源：http://bm.huixiangedu.cn

[R41] 丢弃输出
来源：http://kz.asd995.cn

cmd >/dev/null 2>&1
来源：http://jg.wgjwhj.cn

[R42] 输入重定向
来源：http://nj.chemitech.net.cn

wc -l < a.txt
来源：http://gz.haigaiapp.cn

[R43] 按名字查找文件
来源：http://ab.bookmarksfly.cn


<!-- 参考信息 -->