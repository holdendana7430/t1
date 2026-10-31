代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hg.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xa.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mn.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tf.chemitech.net.cn

================================================================================
来源：http://pg.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://le.szxytkj.cn

================================================================================
来源：http://mh.nicolike.cn

[Q01] 创建表
来源：http://te.szsharing.cn

CREATE TABLE users (
来源：http://oz.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://av.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://wh.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://vx.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lf.nicolike.cn

);
来源：http://jo.9csxet.cn

[Q02] 创建带外键的表
来源：http://ee.muxihuayi.cn

CREATE TABLE orders (
来源：http://kg.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bs.nicolike.cn

user_id INT NOT NULL,
来源：http://yf.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://np.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xa.gzmigu.cn

);
来源：http://bv.nszjky.cn

[Q03] 增加列
来源：http://bf.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wo.colortex.cn

[Q04] 修改列类型
来源：http://vy.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://si.yuexingan06.cn

[Q05] 重命名列
来源：http://aj.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wi.szsharing.cn

[Q06] 删除列
来源：http://ob.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qe.newstarts.cn

[Q07] 删除表
来源：http://wl.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://aj.gzmigu.cn

[Q08] 创建普通索引
来源：http://ff.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://td.huanxung.cn

[Q09] 创建唯一索引
来源：http://bv.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gh.asd995.cn

[Q10] 插入单行
来源：http://jw.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oz.9csxet.cn

[Q11] 一次插入多行
来源：http://ob.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vy.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://di.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ea.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://na.newstarts.cn

[Q13] 忽略重复插入
来源：http://ze.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ad.shtwfgs.cn

[Q14] 存在则更新（upsert）
来源：http://le.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ht.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lt.wgjwhj.cn

[Q15] 查询全部
来源：http://nv.bookmarksfly.cn

SELECT * FROM users;
来源：http://lj.lnxyls.cn

[Q16] 查询指定列
来源：http://gh.shxzskj.cn

SELECT id, name FROM users;
来源：http://ps.haigaiapp.cn

[Q17] 条件查询
来源：http://le.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qa.szxytkj.cn

[Q18] 模糊匹配
来源：http://dt.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sc.haigaiapp.cn

[Q19] 范围查询
来源：http://zz.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sn.gzmigu.cn

[Q20] IN 列表
来源：http://jf.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jg.hahajie.cn

[Q21] 空值判断
来源：http://ow.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wb.szsharing.cn

[Q22] 排序
来源：http://pa.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gk.haigaiapp.cn

[Q23] 分页
来源：http://sk.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ea.bookmarksfly.cn

[Q24] 去重
来源：http://pn.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://rf.gzmigu.cn

[Q25] 只取前 N 条
来源：http://wb.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tg.panjiajie.cn

[Q26] 计数
来源：http://qw.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://eq.521024.cn

[Q27] 条件计数
来源：http://fd.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wo.huixiangedu.cn

[Q28] 求和与平均
来源：http://uh.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qj.szsharing.cn

[Q29] 最大最小值
来源：http://zi.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dj.yuexingan06.cn

[Q30] 分组统计
来源：http://kr.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aj.huanxung.cn

[Q31] 分组后过滤
来源：http://sc.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://th.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://ij.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kn.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sb.nicolike.cn

[Q33] 多列分组
来源：http://wf.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xg.muxihuayi.cn

[Q34] 每组取第一条
来源：http://ea.nszjky.cn

SELECT * FROM (
来源：http://sa.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bv.yuexingan06.cn

) t WHERE rn = 1;
来源：http://pf.chemitech.net.cn

[Q35] 内连接
来源：http://wf.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gh.chemitech.net.cn

[Q36] 左连接
来源：http://sy.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kd.panjiajie.cn

[Q37] 右连接
来源：http://bu.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zn.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gi.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oj.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://ky.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xr.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ca.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nr.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kh.wgjwhj.cn

[Q41] 多表连接
来源：http://uw.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lh.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://ns.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://pe.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://dv.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://dw.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gf.wgjwhj.cn

[Q43] 标量子查询
来源：http://pk.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nv.haigaiapp.cn

[Q44] IN 子查询
来源：http://ch.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://le.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://sg.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hd.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fj.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ny.yuexingan06.cn

[Q47] 与平均值比较
来源：http://qf.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jx.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://cr.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tv.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://hj.nszjky.cn

[Q49] 更新单行
来源：http://pq.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mz.huixiangedu.cn

[Q50] 批量更新
来源：http://bp.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jx.bjjhwx.cn

[Q51] 用子查询更新
来源：http://sd.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vr.nszjky.cn

[Q52] 删除指定行
来源：http://cu.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://hi.huanxung.cn

[Q53] 按条件删除
来源：http://hr.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ko.9csxet.cn

[Q54] 清空表
来源：http://fy.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://qi.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://sq.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fm.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://bb.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cj.jctech888.com.cn

[Q57] 行号
来源：http://kd.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ee.chemitech.net.cn

[Q58] 累计求和
来源：http://ar.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://or.shxzskj.cn

[Q59] 分组内累计
来源：http://kp.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lo.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://mj.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oi.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ic.huixiangedu.cn

[Q61] 移动平均
来源：http://hl.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vs.jctech888.com.cn

[Q62] 分组占比
来源：http://pj.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mu.yuexingan06.cn

[Q63] 开启事务
来源：http://fe.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ag.nszjky.cn

[Q64] 提交事务
来源：http://yt.bjjhwx.cn

COMMIT;
来源：http://bf.szsharing.cn

[Q65] 回滚事务
来源：http://ie.chemitech.net.cn

ROLLBACK;
来源：http://mp.colortex.cn

[Q66] 行锁查询
来源：http://dv.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gw.gzmigu.cn

[Q67] 设置隔离级别
来源：http://la.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ea.chemitech.net.cn

[Q68] 保存点
来源：http://mb.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://bx.521024.cn

ROLLBACK TO sp1;
来源：http://se.shxzskj.cn

[Q69] 查看执行计划
来源：http://zb.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lu.9csxet.cn

[Q70] 更新统计信息
来源：http://pc.nicolike.cn

ANALYZE TABLE users;
来源：http://bn.gzmigu.cn

[Q71] 查看建表语句
来源：http://vi.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gt.szsharing.cn

[Q72] 查看索引
来源：http://of.huanxung.cn

SHOW INDEX FROM users;
来源：http://ew.wgjwhj.cn

[Q73] 查看表状态
来源：http://vx.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dr.bjjhwx.cn

[Q74] 强制使用索引
来源：http://ah.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gi.huixiangedu.cn

[Q75] 日期格式化
来源：http://bg.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iy.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vp.muxihuayi.cn

[Q76] 按天统计
来源：http://aj.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rb.huixiangedu.cn

[Q77] 时间加减
来源：http://rc.huanxung.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ys.chemitech.net.cn

[Q78] 当前时间
来源：http://il.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cu.nicolike.cn

[Q79] 字符串拼接
来源：http://hm.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ep.newstarts.cn

[Q80] 字符串截取
来源：http://ba.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ak.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://mw.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rm.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://xb.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ju.521024.cn

[Q83] 大小写转换
来源：http://jj.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zy.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://oh.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://nk.jctech888.com.cn

[Q85] 数值取整
来源：http://at.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lp.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://tf.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qa.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://lq.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ft.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://vb.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ta.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://si.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://qd.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fe.wgjwhj.cn

[Q90] 生成序号列
来源：http://di.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fs.9csxet.cn

================================================================================
来源：http://df.szxytkj.cn

R. Bash 专题
来源：http://mb.gzmigu.cn

================================================================================
来源：http://tk.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://jh.chemitech.net.cn

#!/usr/bin/env bash
来源：http://as.nszjky.cn

set -euo pipefail
来源：http://jj.colortex.cn

[R02] 变量赋值与使用
来源：http://kr.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://zr.9csxet.cn

[R03] 只读变量
来源：http://yo.chemitech.net.cn

readonly PI=3.14
来源：http://eb.shxzskj.cn

[R04] 位置参数
来源：http://wy.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gd.asd995.cn

[R05] 参数默认值
来源：http://ig.nszjky.cn

name="${1:-default}"
来源：http://nt.hahajie.cn

[R06] 判断命令是否存在
来源：http://dn.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mg.hnjuh.cn

[R07] if 判断文件
来源：http://rx.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tx.newstarts.cn

[R08] 数值比较
来源：http://oo.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ma.panjiajie.cn

[R09] 字符串比较
来源：http://uh.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pl.shtwfgs.cn

[R10] 正则匹配
来源：http://if.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kp.521024.cn

[R11] case 多分支
来源：http://xu.chemitech.net.cn

case "$1" in
来源：http://vi.shxzukj.cn

start) echo "启动" ;;
来源：http://wm.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://xc.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://qh.jianghongdianzi.cn

esac
来源：http://ip.hnjuh.cn

[R12] for 遍历文件
来源：http://yn.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://kh.9csxet.cn

[R13] for 计数循环
来源：http://ab.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://wu.lnxyls.cn

[R14] C 风格 for
来源：http://ln.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wo.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://by.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://io.haigaiapp.cn

[R16] until 等待条件
来源：http://rt.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ef.huixiangedu.cn

[R17] 数组定义与取值
来源：http://ut.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://as.hahajie.cn

[R18] 遍历数组
来源：http://ak.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nu.shxzukj.cn

[R19] 数组长度
来源：http://ms.huixiangedu.cn

echo "${#arr[@]}"
来源：http://zn.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://jm.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kw.yuexingan06.cn

[R21] 字符串长度
来源：http://ek.chemitech.net.cn

echo "${#s}"
来源：http://oh.nicolike.cn

[R22] 截取子串
来源：http://ip.shxzukj.cn

echo "${s:0:5}"
来源：http://mw.hnjuh.cn

[R23] 字符串替换
来源：http://jg.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uh.9csxet.cn

[R24] 大小写转换
来源：http://sy.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bv.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://wr.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nk.szxytkj.cn

[R26] 命令替换
来源：http://gr.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://ds.huixinmuqiang.cn

[R27] 算术展开
来源：http://me.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://zg.lnxyls.cn

[R28] 浮点运算
来源：http://vm.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://hh.chemitech.net.cn

[R29] 定义函数
来源：http://gs.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gc.szxytkj.cn

[R30] 函数返回状态码
来源：http://oq.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://xm.lnxyls.cn

[R31] 局部变量
来源：http://jo.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://rs.muxihuayi.cn

[R32] 参数个数校验
来源：http://bl.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nx.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://yj.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zy.szsharing.cn

[R34] 退出时清理
来源：http://yx.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gs.shxzukj.cn

[R35] 后台执行并等待
来源：http://ek.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://da.szxytkj.cn

[R36] 并发执行多个任务
来源：http://dn.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ab.shxzskj.cn

[R37] 把输出赋给变量
来源：http://eo.lnxyls.cn

files=$(ls -1)
来源：http://yh.muxihuayi.cn

[R38] 管道串联
来源：http://ca.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://in.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://zy.haigaiapp.cn

cmd > out.log 2>&1
来源：http://sk.yuntaijiaju.cn

[R40] 追加写日志
来源：http://zt.asd995.cn

echo "log" >> out.log
来源：http://wr.hnjuh.cn

[R41] 丢弃输出
来源：http://jx.nszjky.cn


<!-- 参考信息 -->