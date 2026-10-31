代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wv.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cv.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://og.hahajie.cn

[P08] 处理浮点精度问题
来源：http://vy.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rk.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://da.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cl.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://po.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kj.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kh.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uk.hahajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dk.newstarts.cn

================================================================================
来源：http://cz.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ur.asd995.cn

================================================================================
来源：http://gu.hahajie.cn

[Q01] 创建表
来源：http://sn.bookmarksfly.cn

CREATE TABLE users (
来源：http://rb.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://me.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://ex.bjjhwx.cn

email VARCHAR(100) UNIQUE,
来源：http://yq.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wa.wgjwhj.cn

);
来源：http://np.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://zd.muxihuayi.cn

CREATE TABLE orders (
来源：http://cf.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://am.shxzskj.cn

user_id INT NOT NULL,
来源：http://zc.szsharing.cn

amount DECIMAL(10, 2),
来源：http://mt.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bd.jctech888.com.cn

);
来源：http://qf.huixiangedu.cn

[Q03] 增加列
来源：http://ps.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mz.colortex.cn

[Q04] 修改列类型
来源：http://nr.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ky.nszjky.cn

[Q05] 重命名列
来源：http://fs.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://du.newstarts.cn

[Q06] 删除列
来源：http://mf.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ds.panjiajie.cn

[Q07] 删除表
来源：http://om.jctech888.com.cn

DROP TABLE IF EXISTS orders;
来源：http://hs.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://nu.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bd.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://vo.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yo.muxihuayi.cn

[Q10] 插入单行
来源：http://dj.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://os.gzmigu.cn

[Q11] 一次插入多行
来源：http://yj.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lr.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://hc.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hk.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ah.colortex.cn

[Q13] 忽略重复插入
来源：http://mw.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lm.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://ck.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qm.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ko.szxytkj.cn

[Q15] 查询全部
来源：http://ot.colortex.cn

SELECT * FROM users;
来源：http://ge.nicolike.cn

[Q16] 查询指定列
来源：http://id.chemitech.net.cn

SELECT id, name FROM users;
来源：http://rl.haigaiapp.cn

[Q17] 条件查询
来源：http://na.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cj.jctech888.com.cn

[Q18] 模糊匹配
来源：http://iw.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ae.bjjhwx.cn

[Q19] 范围查询
来源：http://ay.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kz.shxzukj.cn

[Q20] IN 列表
来源：http://wd.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ai.chemitech.net.cn

[Q21] 空值判断
来源：http://xh.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xr.9csxet.cn

[Q22] 排序
来源：http://jk.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gr.wgjwhj.cn

[Q23] 分页
来源：http://ic.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ov.9csxet.cn

[Q24] 去重
来源：http://cn.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://cg.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://ms.asd995.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ot.haigaiapp.cn

[Q26] 计数
来源：http://ie.yuntaijiaju.cn

SELECT COUNT(*) FROM users;
来源：http://wu.shtwfgs.cn

[Q27] 条件计数
来源：http://gm.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rt.newstarts.cn

[Q28] 求和与平均
来源：http://xq.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xw.shxzskj.cn

[Q29] 最大最小值
来源：http://dg.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tb.newstarts.cn

[Q30] 分组统计
来源：http://wa.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ui.nszjky.cn

[Q31] 分组后过滤
来源：http://ei.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wx.nicolike.cn

[Q32] 分组拼接字符串
来源：http://ci.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ps.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xw.szxytkj.cn

[Q33] 多列分组
来源：http://yh.huixiangedu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yp.nicolike.cn

[Q34] 每组取第一条
来源：http://au.chemitech.net.cn

SELECT * FROM (
来源：http://it.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qt.shxzskj.cn

) t WHERE rn = 1;
来源：http://tb.bjjhwx.cn

[Q35] 内连接
来源：http://as.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hw.jianghongdianzi.cn

[Q36] 左连接
来源：http://tt.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pt.haigaiapp.cn

[Q37] 右连接
来源：http://rq.newstarts.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zd.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xs.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fu.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://if.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xs.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cg.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lh.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://te.szsharing.cn

[Q41] 多表连接
来源：http://xi.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dt.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://ne.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://bp.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://nq.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://qh.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pj.huixiangedu.cn

[Q43] 标量子查询
来源：http://pd.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fe.szxytkj.cn

[Q44] IN 子查询
来源：http://jp.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jf.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://xu.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sr.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wt.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ta.gzmigu.cn

[Q47] 与平均值比较
来源：http://vu.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dz.521024.cn

[Q48] CTE 公用表表达式
来源：http://xv.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gb.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://tf.yuntaijiaju.cn

[Q49] 更新单行
来源：http://ue.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wj.huanxung.cn

[Q50] 批量更新
来源：http://ld.newstarts.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://im.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://lw.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iq.muxihuayi.cn

[Q52] 删除指定行
来源：http://wi.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://ms.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://fm.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ml.yuexingan06.cn

[Q54] 清空表
来源：http://vy.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://sl.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://hw.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://np.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://cz.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qf.shtwfgs.cn

[Q57] 行号
来源：http://oj.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://th.huixiangedu.cn

[Q58] 累计求和
来源：http://nb.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bn.shtwfgs.cn

[Q59] 分组内累计
来源：http://fr.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qs.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://nn.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ac.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zg.lnxyls.cn

[Q61] 移动平均
来源：http://fc.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qa.bjjhwx.cn

[Q62] 分组占比
来源：http://ak.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mr.szxytkj.cn

[Q63] 开启事务
来源：http://bz.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fh.szxytkj.cn

[Q64] 提交事务
来源：http://wh.wgjwhj.cn

COMMIT;
来源：http://uo.shxzskj.cn

[Q65] 回滚事务
来源：http://ew.panjiajie.cn

ROLLBACK;
来源：http://vu.haigaiapp.cn

[Q66] 行锁查询
来源：http://ke.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://va.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://cb.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vt.chemitech.net.cn

[Q68] 保存点
来源：http://gt.521024.cn

SAVEPOINT sp1;
来源：http://uu.shxzskj.cn

ROLLBACK TO sp1;
来源：http://pe.asd995.cn

[Q69] 查看执行计划
来源：http://mx.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mo.shxzukj.cn

[Q70] 更新统计信息
来源：http://dr.bjjhwx.cn

ANALYZE TABLE users;
来源：http://kp.asd995.cn

[Q71] 查看建表语句
来源：http://yj.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://op.huixinmuqiang.cn

[Q72] 查看索引
来源：http://ib.szxytkj.cn

SHOW INDEX FROM users;
来源：http://lt.haigaiapp.cn

[Q73] 查看表状态
来源：http://hk.haigaiapp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xj.szxytkj.cn

[Q74] 强制使用索引
来源：http://wx.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ia.haigaiapp.cn

[Q75] 日期格式化
来源：http://op.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yz.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fb.jianghongdianzi.cn

[Q76] 按天统计
来源：http://hk.shtwfgs.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wy.huixinmuqiang.cn

[Q77] 时间加减
来源：http://bu.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tf.huixiangedu.cn

[Q78] 当前时间
来源：http://rp.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xc.haigaiapp.cn

[Q79] 字符串拼接
来源：http://el.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ea.huixiangedu.cn

[Q80] 字符串截取
来源：http://vw.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lz.newstarts.cn

[Q81] 字符串替换
来源：http://zi.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wk.521024.cn

[Q82] 字符长度与字节长度
来源：http://wr.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bd.jctech888.com.cn

[Q83] 大小写转换
来源：http://te.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sd.521024.cn

[Q84] 去除首尾空格
来源：http://sr.521024.cn

SELECT TRIM(name) FROM users;
来源：http://jb.shxzskj.cn

[Q85] 数值取整
来源：http://pb.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hd.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://dq.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://og.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://dr.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nd.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://oh.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ln.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ml.9csxet.cn

[Q89] 判断表是否存在
来源：http://xq.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wl.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://pt.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://is.colortex.cn

================================================================================
来源：http://qs.huanxung.cn

R. Bash 专题
来源：http://np.haigaiapp.cn

================================================================================
来源：http://wl.shxzukj.cn

[R01] shebang 与严格模式
来源：http://pl.wgjwhj.cn

#!/usr/bin/env bash
来源：http://uv.hahajie.cn

set -euo pipefail
来源：http://gt.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://aw.szsharing.cn

name="Tom"; echo "$name"
来源：http://cm.shxzukj.cn

[R03] 只读变量
来源：http://ku.shtwfgs.cn

readonly PI=3.14
来源：http://qu.huanxung.cn

[R04] 位置参数
来源：http://xf.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lv.jianghongdianzi.cn

[R05] 参数默认值
来源：http://we.jianghongdianzi.cn

name="${1:-default}"
来源：http://dd.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://ff.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lx.asd995.cn

[R07] if 判断文件
来源：http://fz.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://us.shtwfgs.cn

[R08] 数值比较
来源：http://ww.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qw.huixiangedu.cn

[R09] 字符串比较
来源：http://sb.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ao.shtwfgs.cn

[R10] 正则匹配
来源：http://de.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kp.szxytkj.cn

[R11] case 多分支
来源：http://fa.hnjuh.cn

case "$1" in
来源：http://uy.panjiajie.cn

start) echo "启动" ;;
来源：http://nl.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://ma.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://sk.hahajie.cn

esac
来源：http://cc.hahajie.cn

[R12] for 遍历文件
来源：http://th.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://rh.huanxung.cn

[R13] for 计数循环
来源：http://gc.asd995.cn

for i in {1..10}; do echo "$i"; done
来源：http://ft.asd995.cn

[R14] C 风格 for
来源：http://gv.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nq.szsharing.cn

[R15] while 逐行读文件
来源：http://od.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ee.hahajie.cn

[R16] until 等待条件
来源：http://ko.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nv.jctech888.com.cn

[R17] 数组定义与取值
来源：http://gn.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vv.newstarts.cn

[R18] 遍历数组
来源：http://or.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zr.hnjuh.cn

[R19] 数组长度
来源：http://vf.szsharing.cn

echo "${#arr[@]}"
来源：http://xw.lnxyls.cn

[R20] 关联数组（字典）
来源：http://ml.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zh.9csxet.cn

[R21] 字符串长度
来源：http://bp.huixinmuqiang.cn

echo "${#s}"
来源：http://ti.haigaiapp.cn

[R22] 截取子串
来源：http://jf.colortex.cn

echo "${s:0:5}"
来源：http://bc.chemitech.net.cn

[R23] 字符串替换
来源：http://ke.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yd.nszjky.cn

[R24] 大小写转换
来源：http://pw.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ei.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://aa.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ab.9csxet.cn

[R26] 命令替换
来源：http://kf.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://vf.yuntaijiaju.cn

[R27] 算术展开
来源：http://as.asd995.cn

echo $((1 + 2 * 3))
来源：http://pc.9csxet.cn

[R28] 浮点运算
来源：http://sc.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://dg.haigaiapp.cn

[R29] 定义函数
来源：http://kp.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://py.shxzukj.cn

[R30] 函数返回状态码
来源：http://tg.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://bt.wgjwhj.cn

[R31] 局部变量
来源：http://ho.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://zp.newstarts.cn

[R32] 参数个数校验
来源：http://zm.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ws.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://jd.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cu.shxzukj.cn

[R34] 退出时清理
来源：http://th.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ff.yuexingan06.cn

[R35] 后台执行并等待
来源：http://de.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uy.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://vt.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sr.huanxung.cn

[R37] 把输出赋给变量
来源：http://xy.haigaiapp.cn


<!-- 参考信息 -->