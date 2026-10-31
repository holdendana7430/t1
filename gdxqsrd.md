代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ed.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ff.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uv.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oa.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lt.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zq.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dk.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fx.jianghongdianzi.cn

================================================================================
来源：http://dy.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zy.panjiajie.cn

================================================================================
来源：http://qs.shtwfgs.cn

[Q01] 创建表
来源：http://sf.asd995.cn

CREATE TABLE users (
来源：http://nh.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cb.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://ox.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://al.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mg.colortex.cn

);
来源：http://sd.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://bg.shxzskj.cn

CREATE TABLE orders (
来源：http://de.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ow.huixiangedu.cn

user_id INT NOT NULL,
来源：http://qn.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://sn.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vr.9csxet.cn

);
来源：http://mm.jctech888.com.cn

[Q03] 增加列
来源：http://fp.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vo.szxytkj.cn

[Q04] 修改列类型
来源：http://id.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hs.nicolike.cn

[Q05] 重命名列
来源：http://dz.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oa.asd995.cn

[Q06] 删除列
来源：http://nf.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hl.yuntaijiaju.cn

[Q07] 删除表
来源：http://og.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://qe.wgjwhj.cn

[Q08] 创建普通索引
来源：http://qc.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fw.asd995.cn

[Q09] 创建唯一索引
来源：http://fj.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rv.jianghongdianzi.cn

[Q10] 插入单行
来源：http://xc.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bv.chemitech.net.cn

[Q11] 一次插入多行
来源：http://qi.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ev.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://yc.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://os.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ni.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://ig.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sd.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://wp.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dw.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bh.asd995.cn

[Q15] 查询全部
来源：http://gv.jctech888.com.cn

SELECT * FROM users;
来源：http://rt.wgjwhj.cn

[Q16] 查询指定列
来源：http://fb.jctech888.com.cn

SELECT id, name FROM users;
来源：http://ad.lnxyls.cn

[Q17] 条件查询
来源：http://bf.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qt.muxihuayi.cn

[Q18] 模糊匹配
来源：http://cm.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dd.hnjuh.cn

[Q19] 范围查询
来源：http://ii.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ly.shtwfgs.cn

[Q20] IN 列表
来源：http://zn.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oa.wgjwhj.cn

[Q21] 空值判断
来源：http://ie.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://io.bookmarksfly.cn

[Q22] 排序
来源：http://fe.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bv.yuntaijiaju.cn

[Q23] 分页
来源：http://xl.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dg.huixiangedu.cn

[Q24] 去重
来源：http://fi.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://dc.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://vn.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yz.asd995.cn

[Q26] 计数
来源：http://rk.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://xt.haigaiapp.cn

[Q27] 条件计数
来源：http://wy.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ia.panjiajie.cn

[Q28] 求和与平均
来源：http://ge.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kp.huanxung.cn

[Q29] 最大最小值
来源：http://nc.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hs.wgjwhj.cn

[Q30] 分组统计
来源：http://iq.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gm.newstarts.cn

[Q31] 分组后过滤
来源：http://ga.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gv.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://sb.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vo.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fs.huanxung.cn

[Q33] 多列分组
来源：http://pg.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jq.szxytkj.cn

[Q34] 每组取第一条
来源：http://si.huanxung.cn

SELECT * FROM (
来源：http://yb.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ry.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://mv.shtwfgs.cn

[Q35] 内连接
来源：http://hg.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dq.shxzskj.cn

[Q36] 左连接
来源：http://bs.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://es.shxzukj.cn

[Q37] 右连接
来源：http://on.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eg.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ue.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sb.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://fa.muxihuayi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ly.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ct.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://we.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vc.jctech888.com.cn

[Q41] 多表连接
来源：http://yi.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dc.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://dn.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://ee.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://km.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://hf.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zi.huanxung.cn

[Q43] 标量子查询
来源：http://zt.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uf.521024.cn

[Q44] IN 子查询
来源：http://yo.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tt.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://gc.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cs.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cd.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hw.bjjhwx.cn

[Q47] 与平均值比较
来源：http://ji.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yr.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://nc.jianghongdianzi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gy.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://fy.asd995.cn

[Q49] 更新单行
来源：http://kb.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sh.newstarts.cn

[Q50] 批量更新
来源：http://mz.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ji.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://tt.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ou.shtwfgs.cn

[Q52] 删除指定行
来源：http://yi.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://hp.jctech888.com.cn

[Q53] 按条件删除
来源：http://yx.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rp.shxzukj.cn

[Q54] 清空表
来源：http://mt.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://re.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://oe.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tn.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://jl.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yo.szxytkj.cn

[Q57] 行号
来源：http://hv.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://im.colortex.cn

[Q58] 累计求和
来源：http://ua.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kg.wgjwhj.cn

[Q59] 分组内累计
来源：http://tg.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xj.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://ou.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://am.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://er.bookmarksfly.cn

[Q61] 移动平均
来源：http://nc.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nv.9csxet.cn

[Q62] 分组占比
来源：http://fg.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gf.szxytkj.cn

[Q63] 开启事务
来源：http://jn.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xd.szxytkj.cn

[Q64] 提交事务
来源：http://eg.nicolike.cn

COMMIT;
来源：http://kb.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://dc.shtwfgs.cn

ROLLBACK;
来源：http://sk.hnjuh.cn

[Q66] 行锁查询
来源：http://nd.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mt.gzmigu.cn

[Q67] 设置隔离级别
来源：http://pa.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rm.shxzukj.cn

[Q68] 保存点
来源：http://bc.huanxung.cn

SAVEPOINT sp1;
来源：http://qw.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://hi.haigaiapp.cn

[Q69] 查看执行计划
来源：http://ua.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fs.nicolike.cn

[Q70] 更新统计信息
来源：http://gk.nicolike.cn

ANALYZE TABLE users;
来源：http://sk.haigaiapp.cn

[Q71] 查看建表语句
来源：http://qu.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rp.huanxung.cn

[Q72] 查看索引
来源：http://ll.newstarts.cn

SHOW INDEX FROM users;
来源：http://px.521024.cn

[Q73] 查看表状态
来源：http://se.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pb.asd995.cn

[Q74] 强制使用索引
来源：http://fa.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oz.huixiangedu.cn

[Q75] 日期格式化
来源：http://mj.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nn.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uu.colortex.cn

[Q76] 按天统计
来源：http://ee.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dw.yuntaijiaju.cn

[Q77] 时间加减
来源：http://pb.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hn.yuntaijiaju.cn

[Q78] 当前时间
来源：http://ov.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ww.gzmigu.cn

[Q79] 字符串拼接
来源：http://ie.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yr.521024.cn

[Q80] 字符串截取
来源：http://up.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://te.huixiangedu.cn

[Q81] 字符串替换
来源：http://go.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fe.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://hn.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rx.chemitech.net.cn

[Q83] 大小写转换
来源：http://qh.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kl.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://kz.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://sb.huixinmuqiang.cn

[Q85] 数值取整
来源：http://bo.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cl.colortex.cn

[Q86] 读取 JSON 字段
来源：http://ll.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ae.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://oe.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nq.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://om.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lk.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vm.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://yo.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pc.jctech888.com.cn

[Q90] 生成序号列
来源：http://us.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fx.huixiangedu.cn

================================================================================
来源：http://lg.bjjhwx.cn

R. Bash 专题
来源：http://aa.shtwfgs.cn

================================================================================
来源：http://bv.huanxung.cn

[R01] shebang 与严格模式
来源：http://ae.bjjhwx.cn

#!/usr/bin/env bash
来源：http://xt.gzmigu.cn

set -euo pipefail
来源：http://jg.szxytkj.cn

[R02] 变量赋值与使用
来源：http://tt.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://hn.huanxung.cn

[R03] 只读变量
来源：http://yd.lnxyls.cn

readonly PI=3.14
来源：http://bp.jianghongdianzi.cn

[R04] 位置参数
来源：http://da.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bq.newstarts.cn

[R05] 参数默认值
来源：http://uo.yuntaijiaju.cn

name="${1:-default}"
来源：http://zt.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://gx.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://az.jianghongdianzi.cn

[R07] if 判断文件
来源：http://cn.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dt.panjiajie.cn

[R08] 数值比较
来源：http://ks.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pt.yuntaijiaju.cn

[R09] 字符串比较
来源：http://sl.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vp.jianghongdianzi.cn

[R10] 正则匹配
来源：http://hj.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wy.muxihuayi.cn

[R11] case 多分支
来源：http://ro.huixinmuqiang.cn

case "$1" in
来源：http://hz.asd995.cn

start) echo "启动" ;;
来源：http://fv.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://es.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://ho.jianghongdianzi.cn

esac
来源：http://mi.szxytkj.cn

[R12] for 遍历文件
来源：http://vc.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://yy.colortex.cn

[R13] for 计数循环
来源：http://tf.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://mn.szsharing.cn

[R14] C 风格 for
来源：http://om.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cm.huanxung.cn

[R15] while 逐行读文件
来源：http://my.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ke.bookmarksfly.cn

[R16] until 等待条件
来源：http://xu.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ry.hnjuh.cn

[R17] 数组定义与取值
来源：http://sk.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jy.nicolike.cn

[R18] 遍历数组
来源：http://jd.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uw.szsharing.cn

[R19] 数组长度
来源：http://io.wgjwhj.cn

echo "${#arr[@]}"
来源：http://bj.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://gd.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ph.huixinmuqiang.cn

[R21] 字符串长度
来源：http://cd.jctech888.com.cn

echo "${#s}"
来源：http://lm.nszjky.cn

[R22] 截取子串
来源：http://vq.haigaiapp.cn

echo "${s:0:5}"
来源：http://oq.gzmigu.cn

[R23] 字符串替换
来源：http://qj.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qu.asd995.cn

[R24] 大小写转换
来源：http://yq.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ug.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://md.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://di.asd995.cn

[R26] 命令替换
来源：http://an.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://oe.jianghongdianzi.cn

[R27] 算术展开
来源：http://xh.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://xl.lnxyls.cn

[R28] 浮点运算
来源：http://za.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://eo.asd995.cn

[R29] 定义函数
来源：http://dy.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://et.9csxet.cn

[R30] 函数返回状态码
来源：http://nk.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://qv.nszjky.cn

[R31] 局部变量
来源：http://qy.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://pt.chemitech.net.cn

[R32] 参数个数校验
来源：http://vo.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qo.521024.cn

[R33] 捕获错误并提示行号
来源：http://vq.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dq.hnjuh.cn

[R34] 退出时清理
来源：http://yh.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dq.wgjwhj.cn

[R35] 后台执行并等待
来源：http://rg.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pb.9csxet.cn

[R36] 并发执行多个任务
来源：http://za.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qo.521024.cn

[R37] 把输出赋给变量
来源：http://jt.nszjky.cn

files=$(ls -1)
来源：http://nl.haigaiapp.cn

[R38] 管道串联
来源：http://df.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://vu.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://ie.lnxyls.cn


<!-- 参考信息 -->