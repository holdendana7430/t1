代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rr.chemitech.net.cn

TS:   if (x == null) {}
来源：http://ki.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vr.hahajie.cn

Go:   if x == nil {}
来源：http://rf.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sf.asd995.cn

C#:   if (x is null) {}
来源：http://tc.jctech888.com.cn

[P07] 防抖与节流
来源：http://rj.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pi.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://ij.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dm.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://do.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ag.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nh.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dj.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ki.hahajie.cn

[P08] 处理浮点精度问题
来源：http://fp.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mr.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qn.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qp.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sw.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kx.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nl.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gx.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bc.nicolike.cn

================================================================================
来源：http://xy.9csxet.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yk.colortex.cn

================================================================================
来源：http://gp.gzmigu.cn

[Q01] 创建表
来源：http://yc.jctech888.com.cn

CREATE TABLE users (
来源：http://wm.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pe.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://yf.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://ya.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://op.wgjwhj.cn

);
来源：http://or.gzmigu.cn

[Q02] 创建带外键的表
来源：http://xq.panjiajie.cn

CREATE TABLE orders (
来源：http://kj.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bi.hahajie.cn

user_id INT NOT NULL,
来源：http://ik.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://ze.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vg.yuntaijiaju.cn

);
来源：http://fn.haigaiapp.cn

[Q03] 增加列
来源：http://nz.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gd.panjiajie.cn

[Q04] 修改列类型
来源：http://mp.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vq.panjiajie.cn

[Q05] 重命名列
来源：http://dv.nszjky.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ff.asd995.cn

[Q06] 删除列
来源：http://iy.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sj.nszjky.cn

[Q07] 删除表
来源：http://id.jctech888.com.cn

DROP TABLE IF EXISTS orders;
来源：http://be.newstarts.cn

[Q08] 创建普通索引
来源：http://dc.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ox.panjiajie.cn

[Q09] 创建唯一索引
来源：http://tn.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vb.nicolike.cn

[Q10] 插入单行
来源：http://cr.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xx.lnxyls.cn

[Q11] 一次插入多行
来源：http://tg.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mh.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://rg.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ik.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ms.hahajie.cn

[Q13] 忽略重复插入
来源：http://iy.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qg.panjiajie.cn

[Q14] 存在则更新（upsert）
来源：http://qe.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qj.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lc.nszjky.cn

[Q15] 查询全部
来源：http://ol.lnxyls.cn

SELECT * FROM users;
来源：http://xg.muxihuayi.cn

[Q16] 查询指定列
来源：http://ox.chemitech.net.cn

SELECT id, name FROM users;
来源：http://lm.colortex.cn

[Q17] 条件查询
来源：http://pe.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ud.haigaiapp.cn

[Q18] 模糊匹配
来源：http://hv.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ok.bookmarksfly.cn

[Q19] 范围查询
来源：http://pv.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mf.shtwfgs.cn

[Q20] IN 列表
来源：http://lo.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wv.jianghongdianzi.cn

[Q21] 空值判断
来源：http://sc.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hl.colortex.cn

[Q22] 排序
来源：http://ef.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mf.newstarts.cn

[Q23] 分页
来源：http://io.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ml.bjjhwx.cn

[Q24] 去重
来源：http://dx.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://zm.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://fv.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wl.szxytkj.cn

[Q26] 计数
来源：http://au.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://lh.9csxet.cn

[Q27] 条件计数
来源：http://hj.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gk.szsharing.cn

[Q28] 求和与平均
来源：http://ez.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sb.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://sz.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jv.yuntaijiaju.cn

[Q30] 分组统计
来源：http://yh.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xo.hahajie.cn

[Q31] 分组后过滤
来源：http://lw.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ba.huanxung.cn

[Q32] 分组拼接字符串
来源：http://li.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ys.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ln.9csxet.cn

[Q33] 多列分组
来源：http://kc.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gu.hnjuh.cn

[Q34] 每组取第一条
来源：http://df.panjiajie.cn

SELECT * FROM (
来源：http://hl.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bz.wgjwhj.cn

) t WHERE rn = 1;
来源：http://ou.nicolike.cn

[Q35] 内连接
来源：http://mt.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ct.newstarts.cn

[Q36] 左连接
来源：http://bw.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pd.jianghongdianzi.cn

[Q37] 右连接
来源：http://io.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qa.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ma.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://jf.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gq.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gi.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fv.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ir.nszjky.cn

[Q41] 多表连接
来源：http://nh.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gt.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://zh.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://ev.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://hc.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://ei.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sx.nicolike.cn

[Q43] 标量子查询
来源：http://sp.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bt.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://rl.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ow.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://tt.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yx.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ne.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://md.colortex.cn

[Q47] 与平均值比较
来源：http://be.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://en.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://hq.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yz.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://li.asd995.cn

[Q49] 更新单行
来源：http://pl.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xb.newstarts.cn

[Q50] 批量更新
来源：http://ai.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pb.szxytkj.cn

[Q51] 用子查询更新
来源：http://sx.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fu.huixiangedu.cn

[Q52] 删除指定行
来源：http://ym.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://uu.huanxung.cn

[Q53] 按条件删除
来源：http://zi.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vs.521024.cn

[Q54] 清空表
来源：http://cj.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://aw.szsharing.cn

[Q55] 排名（并列占位）
来源：http://lu.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zt.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://gz.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ui.newstarts.cn

[Q57] 行号
来源：http://vz.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://au.asd995.cn

[Q58] 累计求和
来源：http://ez.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ki.huanxung.cn

[Q59] 分组内累计
来源：http://du.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ns.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://yx.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hp.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://au.asd995.cn

[Q61] 移动平均
来源：http://gi.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gl.shxzskj.cn

[Q62] 分组占比
来源：http://ko.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wp.bjjhwx.cn

[Q63] 开启事务
来源：http://ow.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ly.bjjhwx.cn

[Q64] 提交事务
来源：http://nz.muxihuayi.cn

COMMIT;
来源：http://cq.szsharing.cn

[Q65] 回滚事务
来源：http://gp.shtwfgs.cn

ROLLBACK;
来源：http://no.9csxet.cn

[Q66] 行锁查询
来源：http://tr.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ss.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://ql.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ya.muxihuayi.cn

[Q68] 保存点
来源：http://jr.szxytkj.cn

SAVEPOINT sp1;
来源：http://sa.huanxung.cn

ROLLBACK TO sp1;
来源：http://hd.jctech888.com.cn

[Q69] 查看执行计划
来源：http://kq.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ba.9csxet.cn

[Q70] 更新统计信息
来源：http://wa.shtwfgs.cn

ANALYZE TABLE users;
来源：http://jr.9csxet.cn

[Q71] 查看建表语句
来源：http://cu.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vc.9csxet.cn

[Q72] 查看索引
来源：http://wy.hnjuh.cn

SHOW INDEX FROM users;
来源：http://qz.9csxet.cn

[Q73] 查看表状态
来源：http://jy.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ao.yuexingan06.cn

[Q74] 强制使用索引
来源：http://vn.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fj.haigaiapp.cn

[Q75] 日期格式化
来源：http://mx.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dl.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fi.nszjky.cn

[Q76] 按天统计
来源：http://sd.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ct.haigaiapp.cn

[Q77] 时间加减
来源：http://ml.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kv.yuexingan06.cn

[Q78] 当前时间
来源：http://ak.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xk.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://ez.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sn.shxzukj.cn

[Q80] 字符串截取
来源：http://wo.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wb.jctech888.com.cn

[Q81] 字符串替换
来源：http://ft.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tc.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://dw.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vi.colortex.cn

[Q83] 大小写转换
来源：http://lo.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ij.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://vx.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://mb.yuexingan06.cn

[Q85] 数值取整
来源：http://lx.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cp.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://ul.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tr.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://ql.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uh.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://bc.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://un.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oq.hahajie.cn

[Q89] 判断表是否存在
来源：http://uz.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fn.szsharing.cn

[Q90] 生成序号列
来源：http://rp.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bh.lnxyls.cn

================================================================================
来源：http://tz.9csxet.cn

R. Bash 专题
来源：http://zy.asd995.cn

================================================================================
来源：http://jr.gzmigu.cn

[R01] shebang 与严格模式
来源：http://xq.colortex.cn

#!/usr/bin/env bash
来源：http://zu.521024.cn

set -euo pipefail
来源：http://el.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://sd.huanxung.cn

name="Tom"; echo "$name"
来源：http://ny.szsharing.cn

[R03] 只读变量
来源：http://qb.huixiangedu.cn

readonly PI=3.14
来源：http://zh.yuntaijiaju.cn

[R04] 位置参数
来源：http://pm.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ef.nicolike.cn

[R05] 参数默认值
来源：http://xz.bookmarksfly.cn

name="${1:-default}"
来源：http://vc.9csxet.cn

[R06] 判断命令是否存在
来源：http://in.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zb.shtwfgs.cn

[R07] if 判断文件
来源：http://vo.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jf.nszjky.cn

[R08] 数值比较
来源：http://ww.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://or.muxihuayi.cn

[R09] 字符串比较
来源：http://kk.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mz.shxzskj.cn

[R10] 正则匹配
来源：http://zw.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tp.nszjky.cn

[R11] case 多分支
来源：http://ye.shtwfgs.cn

case "$1" in
来源：http://mz.9csxet.cn

start) echo "启动" ;;
来源：http://kn.lnxyls.cn

stop)  echo "停止" ;;
来源：http://wh.521024.cn

*)     echo "未知命令" ;;
来源：http://wm.shtwfgs.cn

esac
来源：http://dz.bookmarksfly.cn

[R12] for 遍历文件
来源：http://ie.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://kx.huixiangedu.cn

[R13] for 计数循环
来源：http://og.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://am.lnxyls.cn

[R14] C 风格 for
来源：http://rw.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gq.huanxung.cn

[R15] while 逐行读文件
来源：http://lv.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xb.haigaiapp.cn

[R16] until 等待条件
来源：http://xy.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zv.hnjuh.cn

[R17] 数组定义与取值
来源：http://qm.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bw.muxihuayi.cn

[R18] 遍历数组
来源：http://gv.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jy.szxytkj.cn

[R19] 数组长度
来源：http://qt.panjiajie.cn

echo "${#arr[@]}"
来源：http://tz.gzmigu.cn

[R20] 关联数组（字典）
来源：http://kr.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ad.haigaiapp.cn

[R21] 字符串长度
来源：http://pg.wgjwhj.cn

echo "${#s}"
来源：http://om.bjjhwx.cn

[R22] 截取子串
来源：http://ja.chemitech.net.cn

echo "${s:0:5}"
来源：http://gy.asd995.cn

[R23] 字符串替换
来源：http://tr.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xy.yuexingan06.cn

[R24] 大小写转换
来源：http://ca.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vq.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://wa.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ga.wgjwhj.cn

[R26] 命令替换
来源：http://vm.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://fk.haigaiapp.cn

[R27] 算术展开
来源：http://sl.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://pg.yuexingan06.cn

[R28] 浮点运算
来源：http://bg.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://fe.bjjhwx.cn

[R29] 定义函数
来源：http://tr.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mx.panjiajie.cn

[R30] 函数返回状态码
来源：http://pb.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://hb.muxihuayi.cn

[R31] 局部变量
来源：http://ji.lnxyls.cn


<!-- 参考信息 -->