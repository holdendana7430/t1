代发 wailian999

PHP:  // 手写时间戳比较
来源：http://lm.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wh.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qa.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://px.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pd.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qx.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qg.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://vv.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ik.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ri.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fh.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bi.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://em.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hm.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bf.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yp.shxzskj.cn

================================================================================
来源：http://zg.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://te.bookmarksfly.cn

================================================================================
来源：http://po.panjiajie.cn

[Q01] 创建表
来源：http://gi.newstarts.cn

CREATE TABLE users (
来源：http://cx.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dy.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://rt.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://qw.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fm.shtwfgs.cn

);
来源：http://me.hahajie.cn

[Q02] 创建带外键的表
来源：http://as.newstarts.cn

CREATE TABLE orders (
来源：http://cj.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://st.muxihuayi.cn

user_id INT NOT NULL,
来源：http://eu.nszjky.cn

amount DECIMAL(10, 2),
来源：http://ye.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xo.haigaiapp.cn

);
来源：http://gt.chemitech.net.cn

[Q03] 增加列
来源：http://ln.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hr.szxytkj.cn

[Q04] 修改列类型
来源：http://um.hahajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ky.szxytkj.cn

[Q05] 重命名列
来源：http://zv.nszjky.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sj.panjiajie.cn

[Q06] 删除列
来源：http://vj.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bg.9csxet.cn

[Q07] 删除表
来源：http://sk.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://ds.521024.cn

[Q08] 创建普通索引
来源：http://ct.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lo.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://mk.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sx.hahajie.cn

[Q10] 插入单行
来源：http://sy.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://az.szxytkj.cn

[Q11] 一次插入多行
来源：http://qp.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gn.asd995.cn

[Q12] 插入后取自增 ID
来源：http://is.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hc.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ry.shxzukj.cn

[Q13] 忽略重复插入
来源：http://da.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jt.521024.cn

[Q14] 存在则更新（upsert）
来源：http://gf.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yc.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bc.nicolike.cn

[Q15] 查询全部
来源：http://wx.yuexingan06.cn

SELECT * FROM users;
来源：http://be.yuexingan06.cn

[Q16] 查询指定列
来源：http://ie.chemitech.net.cn

SELECT id, name FROM users;
来源：http://zl.huixinmuqiang.cn

[Q17] 条件查询
来源：http://vb.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hi.yuexingan06.cn

[Q18] 模糊匹配
来源：http://dj.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dz.wgjwhj.cn

[Q19] 范围查询
来源：http://wi.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nb.hnjuh.cn

[Q20] IN 列表
来源：http://za.shtwfgs.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ir.jianghongdianzi.cn

[Q21] 空值判断
来源：http://ea.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qg.chemitech.net.cn

[Q22] 排序
来源：http://nv.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xu.bookmarksfly.cn

[Q23] 分页
来源：http://ja.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://on.asd995.cn

[Q24] 去重
来源：http://mv.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://mb.szsharing.cn

[Q25] 只取前 N 条
来源：http://tv.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eo.shxzskj.cn

[Q26] 计数
来源：http://wl.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://at.bjjhwx.cn

[Q27] 条件计数
来源：http://fe.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://so.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://yq.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gn.9csxet.cn

[Q29] 最大最小值
来源：http://ah.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zx.yuntaijiaju.cn

[Q30] 分组统计
来源：http://km.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://im.shxzukj.cn

[Q31] 分组后过滤
来源：http://xd.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wd.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://aw.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lm.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hf.panjiajie.cn

[Q33] 多列分组
来源：http://bc.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jp.hahajie.cn

[Q34] 每组取第一条
来源：http://yk.szsharing.cn

SELECT * FROM (
来源：http://lt.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bj.colortex.cn

) t WHERE rn = 1;
来源：http://us.yuntaijiaju.cn

[Q35] 内连接
来源：http://xh.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jw.gzmigu.cn

[Q36] 左连接
来源：http://ie.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nj.nszjky.cn

[Q37] 右连接
来源：http://ec.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wl.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xv.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fa.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://gt.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xy.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ko.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rt.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xa.chemitech.net.cn

[Q41] 多表连接
来源：http://tt.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gw.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://gx.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://us.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://aw.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://of.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vf.asd995.cn

[Q43] 标量子查询
来源：http://jq.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wr.wgjwhj.cn

[Q44] IN 子查询
来源：http://ge.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cn.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://sa.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hl.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pi.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fe.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://zs.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ya.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://kq.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nm.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://hn.muxihuayi.cn

[Q49] 更新单行
来源：http://pn.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pa.szxytkj.cn

[Q50] 批量更新
来源：http://qd.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bh.newstarts.cn

[Q51] 用子查询更新
来源：http://gt.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pw.chemitech.net.cn

[Q52] 删除指定行
来源：http://cm.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://qa.jctech888.com.cn

[Q53] 按条件删除
来源：http://or.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fq.asd995.cn

[Q54] 清空表
来源：http://ws.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://pg.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://pn.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jr.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://gq.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://py.panjiajie.cn

[Q57] 行号
来源：http://mc.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xy.chemitech.net.cn

[Q58] 累计求和
来源：http://yt.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ez.colortex.cn

[Q59] 分组内累计
来源：http://pt.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ai.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://qr.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wg.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dv.nicolike.cn

[Q61] 移动平均
来源：http://nm.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qq.asd995.cn

[Q62] 分组占比
来源：http://sj.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tf.shxzukj.cn

[Q63] 开启事务
来源：http://dc.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vq.nicolike.cn

[Q64] 提交事务
来源：http://ee.yuntaijiaju.cn

COMMIT;
来源：http://eq.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://jq.yuexingan06.cn

ROLLBACK;
来源：http://zx.colortex.cn

[Q66] 行锁查询
来源：http://na.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pl.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://kq.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://il.huixiangedu.cn

[Q68] 保存点
来源：http://yy.chemitech.net.cn

SAVEPOINT sp1;
来源：http://gm.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://of.jctech888.com.cn

[Q69] 查看执行计划
来源：http://hp.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://co.haigaiapp.cn

[Q70] 更新统计信息
来源：http://al.panjiajie.cn

ANALYZE TABLE users;
来源：http://ph.shxzukj.cn

[Q71] 查看建表语句
来源：http://ju.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zy.szxytkj.cn

[Q72] 查看索引
来源：http://fq.nszjky.cn

SHOW INDEX FROM users;
来源：http://zx.asd995.cn

[Q73] 查看表状态
来源：http://ew.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lq.colortex.cn

[Q74] 强制使用索引
来源：http://pr.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kh.gzmigu.cn

[Q75] 日期格式化
来源：http://xq.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xb.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fv.yuntaijiaju.cn

[Q76] 按天统计
来源：http://yf.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uo.jianghongdianzi.cn

[Q77] 时间加减
来源：http://og.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kp.colortex.cn

[Q78] 当前时间
来源：http://kk.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pi.huanxung.cn

[Q79] 字符串拼接
来源：http://rd.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pl.bookmarksfly.cn

[Q80] 字符串截取
来源：http://lo.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ll.haigaiapp.cn

[Q81] 字符串替换
来源：http://xr.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zq.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://vi.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gx.9csxet.cn

[Q83] 大小写转换
来源：http://ob.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gk.shxzskj.cn

[Q84] 去除首尾空格
来源：http://hw.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://ab.lnxyls.cn

[Q85] 数值取整
来源：http://tj.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mu.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://kf.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dv.szsharing.cn

[Q87] JSON 字段做条件
来源：http://yr.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dz.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://ke.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lx.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vp.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://yh.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jc.shtwfgs.cn

[Q90] 生成序号列
来源：http://kc.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ws.521024.cn

================================================================================
来源：http://eg.huixiangedu.cn

R. Bash 专题
来源：http://yq.wgjwhj.cn

================================================================================
来源：http://ap.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://mm.colortex.cn

#!/usr/bin/env bash
来源：http://fr.lnxyls.cn

set -euo pipefail
来源：http://yi.shxzskj.cn

[R02] 变量赋值与使用
来源：http://sh.shxzukj.cn

name="Tom"; echo "$name"
来源：http://qc.hahajie.cn

[R03] 只读变量
来源：http://na.lnxyls.cn

readonly PI=3.14
来源：http://al.shtwfgs.cn

[R04] 位置参数
来源：http://rm.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dy.wgjwhj.cn

[R05] 参数默认值
来源：http://ro.lnxyls.cn

name="${1:-default}"
来源：http://vl.521024.cn

[R06] 判断命令是否存在
来源：http://xq.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ng.bjjhwx.cn

[R07] if 判断文件
来源：http://na.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ri.yuntaijiaju.cn

[R08] 数值比较
来源：http://me.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mj.jctech888.com.cn

[R09] 字符串比较
来源：http://zh.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hh.haigaiapp.cn

[R10] 正则匹配
来源：http://kh.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zk.newstarts.cn

[R11] case 多分支
来源：http://qj.hnjuh.cn

case "$1" in
来源：http://cc.colortex.cn

start) echo "启动" ;;
来源：http://pl.szxytkj.cn

stop)  echo "停止" ;;
来源：http://wx.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://aa.shxzskj.cn

esac
来源：http://co.newstarts.cn

[R12] for 遍历文件
来源：http://fh.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://bc.yuexingan06.cn

[R13] for 计数循环
来源：http://wj.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://jt.yuexingan06.cn

[R14] C 风格 for
来源：http://zc.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gz.newstarts.cn

[R15] while 逐行读文件
来源：http://gb.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zi.shxzukj.cn

[R16] until 等待条件
来源：http://gb.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ck.521024.cn

[R17] 数组定义与取值
来源：http://kc.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fj.bjjhwx.cn

[R18] 遍历数组
来源：http://tf.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gd.muxihuayi.cn

[R19] 数组长度
来源：http://bf.wgjwhj.cn

echo "${#arr[@]}"
来源：http://pw.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://zc.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://et.haigaiapp.cn

[R21] 字符串长度
来源：http://ai.colortex.cn

echo "${#s}"
来源：http://vc.chemitech.net.cn

[R22] 截取子串
来源：http://md.nicolike.cn

echo "${s:0:5}"
来源：http://hh.chemitech.net.cn

[R23] 字符串替换
来源：http://py.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cz.bookmarksfly.cn

[R24] 大小写转换
来源：http://py.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kc.521024.cn

[R25] 去后缀 / 去前缀
来源：http://wn.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zd.shxzukj.cn

[R26] 命令替换
来源：http://rp.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://gs.chemitech.net.cn

[R27] 算术展开
来源：http://jh.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://mh.nszjky.cn

[R28] 浮点运算
来源：http://qi.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://db.huixinmuqiang.cn

[R29] 定义函数
来源：http://sd.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ft.nszjky.cn

[R30] 函数返回状态码
来源：http://wt.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://jz.haigaiapp.cn

[R31] 局部变量
来源：http://cv.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://ui.chemitech.net.cn

[R32] 参数个数校验
来源：http://yn.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lr.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://fq.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gj.asd995.cn

[R34] 退出时清理
来源：http://gb.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pf.muxihuayi.cn

[R35] 后台执行并等待
来源：http://hh.colortex.cn


<!-- 参考信息 -->