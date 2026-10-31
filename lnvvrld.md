代发 wailian999

================================================================================
来源：http://br.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://va.chemitech.net.cn

================================================================================
来源：http://uk.shxzskj.cn

[Q01] 创建表
来源：http://em.huixinmuqiang.cn

CREATE TABLE users (
来源：http://pc.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fg.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://gj.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://dv.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dw.muxihuayi.cn

);
来源：http://yl.asd995.cn

[Q02] 创建带外键的表
来源：http://bn.lnxyls.cn

CREATE TABLE orders (
来源：http://sx.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ib.szsharing.cn

user_id INT NOT NULL,
来源：http://en.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://bx.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xb.521024.cn

);
来源：http://ep.newstarts.cn

[Q03] 增加列
来源：http://km.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mm.shxzskj.cn

[Q04] 修改列类型
来源：http://fn.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sr.hnjuh.cn

[Q05] 重命名列
来源：http://ya.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rl.yuexingan06.cn

[Q06] 删除列
来源：http://jd.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vu.9csxet.cn

[Q07] 删除表
来源：http://ln.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://we.huixiangedu.cn

[Q08] 创建普通索引
来源：http://ds.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://td.hnjuh.cn

[Q09] 创建唯一索引
来源：http://pk.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pg.nszjky.cn

[Q10] 插入单行
来源：http://hg.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ph.lnxyls.cn

[Q11] 一次插入多行
来源：http://jf.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aq.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://xe.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ha.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zg.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://or.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dj.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://jj.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ry.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bp.521024.cn

[Q15] 查询全部
来源：http://pi.shxzukj.cn

SELECT * FROM users;
来源：http://sl.nicolike.cn

[Q16] 查询指定列
来源：http://rj.huanxung.cn

SELECT id, name FROM users;
来源：http://ej.nicolike.cn

[Q17] 条件查询
来源：http://gt.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lx.hnjuh.cn

[Q18] 模糊匹配
来源：http://kr.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sn.szsharing.cn

[Q19] 范围查询
来源：http://ny.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mc.yuntaijiaju.cn

[Q20] IN 列表
来源：http://wg.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wt.shtwfgs.cn

[Q21] 空值判断
来源：http://pk.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cf.huixiangedu.cn

[Q22] 排序
来源：http://hb.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://su.szsharing.cn

[Q23] 分页
来源：http://df.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mn.gzmigu.cn

[Q24] 去重
来源：http://qi.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://hf.lnxyls.cn

[Q25] 只取前 N 条
来源：http://ni.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fx.521024.cn

[Q26] 计数
来源：http://xw.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://ew.bookmarksfly.cn

[Q27] 条件计数
来源：http://nx.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hg.bookmarksfly.cn

[Q28] 求和与平均
来源：http://ic.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qr.gzmigu.cn

[Q29] 最大最小值
来源：http://xp.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kj.bjjhwx.cn

[Q30] 分组统计
来源：http://zz.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://br.gzmigu.cn

[Q31] 分组后过滤
来源：http://fr.bookmarksfly.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hq.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://jg.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ed.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bt.hnjuh.cn

[Q33] 多列分组
来源：http://mv.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pu.huanxung.cn

[Q34] 每组取第一条
来源：http://rf.huixinmuqiang.cn

SELECT * FROM (
来源：http://qz.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ki.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://ln.521024.cn

[Q35] 内连接
来源：http://uv.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cb.szsharing.cn

[Q36] 左连接
来源：http://ej.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bw.chemitech.net.cn

[Q37] 右连接
来源：http://bj.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oj.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://go.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kh.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://ht.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ft.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qy.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ke.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sk.szxytkj.cn

[Q41] 多表连接
来源：http://fm.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jo.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://kg.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://ea.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://be.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://gk.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zm.haigaiapp.cn

[Q43] 标量子查询
来源：http://ju.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://if.jctech888.com.cn

[Q44] IN 子查询
来源：http://hs.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rr.colortex.cn

[Q45] EXISTS 判断存在
来源：http://uc.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://om.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xh.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jb.huixiangedu.cn

[Q47] 与平均值比较
来源：http://jk.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rr.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://gx.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gl.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://wm.gzmigu.cn

[Q49] 更新单行
来源：http://kr.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jg.huanxung.cn

[Q50] 批量更新
来源：http://yf.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wn.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://gf.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bw.colortex.cn

[Q52] 删除指定行
来源：http://av.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://vk.szsharing.cn

[Q53] 按条件删除
来源：http://yy.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uq.haigaiapp.cn

[Q54] 清空表
来源：http://sw.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://ro.colortex.cn

[Q55] 排名（并列占位）
来源：http://xz.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ra.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://on.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ei.yuntaijiaju.cn

[Q57] 行号
来源：http://bu.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wi.521024.cn

[Q58] 累计求和
来源：http://uc.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ca.shxzukj.cn

[Q59] 分组内累计
来源：http://lz.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zt.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://fw.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://da.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kv.bookmarksfly.cn

[Q61] 移动平均
来源：http://jo.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vu.newstarts.cn

[Q62] 分组占比
来源：http://tw.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bv.colortex.cn

[Q63] 开启事务
来源：http://ti.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fz.jianghongdianzi.cn

[Q64] 提交事务
来源：http://do.haigaiapp.cn

COMMIT;
来源：http://pd.wgjwhj.cn

[Q65] 回滚事务
来源：http://sg.yuntaijiaju.cn

ROLLBACK;
来源：http://ps.bjjhwx.cn

[Q66] 行锁查询
来源：http://xf.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vp.nszjky.cn

[Q67] 设置隔离级别
来源：http://sc.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hp.newstarts.cn

[Q68] 保存点
来源：http://xi.bjjhwx.cn

SAVEPOINT sp1;
来源：http://pz.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://ki.newstarts.cn

[Q69] 查看执行计划
来源：http://mf.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ct.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://qn.9csxet.cn

ANALYZE TABLE users;
来源：http://hi.szxytkj.cn

[Q71] 查看建表语句
来源：http://ki.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wr.521024.cn

[Q72] 查看索引
来源：http://yi.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://co.shxzskj.cn

[Q73] 查看表状态
来源：http://qd.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ww.szxytkj.cn

[Q74] 强制使用索引
来源：http://rv.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ml.nszjky.cn

[Q75] 日期格式化
来源：http://pa.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yh.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qh.asd995.cn

[Q76] 按天统计
来源：http://mp.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kn.huixinmuqiang.cn

[Q77] 时间加减
来源：http://dn.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kr.nszjky.cn

[Q78] 当前时间
来源：http://do.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://za.shxzskj.cn

[Q79] 字符串拼接
来源：http://ab.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://py.nszjky.cn

[Q80] 字符串截取
来源：http://fp.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ik.521024.cn

[Q81] 字符串替换
来源：http://hb.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ar.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://yk.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pi.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://ty.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jf.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://aq.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://yv.haigaiapp.cn

[Q85] 数值取整
来源：http://mm.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wc.asd995.cn

[Q86] 读取 JSON 字段
来源：http://sc.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vw.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://cp.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wu.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://ph.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tz.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wr.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://ep.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lw.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://mb.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kc.colortex.cn

================================================================================
来源：http://fy.jianghongdianzi.cn

R. Bash 专题
来源：http://ni.muxihuayi.cn

================================================================================
来源：http://wh.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://yc.521024.cn

#!/usr/bin/env bash
来源：http://tq.nicolike.cn

set -euo pipefail
来源：http://vu.szsharing.cn

[R02] 变量赋值与使用
来源：http://xl.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://jd.muxihuayi.cn

[R03] 只读变量
来源：http://on.yuexingan06.cn

readonly PI=3.14
来源：http://rj.gzmigu.cn

[R04] 位置参数
来源：http://hy.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pb.haigaiapp.cn

[R05] 参数默认值
来源：http://es.521024.cn

name="${1:-default}"
来源：http://vq.hnjuh.cn

[R06] 判断命令是否存在
来源：http://nb.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://av.asd995.cn

[R07] if 判断文件
来源：http://za.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mo.colortex.cn

[R08] 数值比较
来源：http://dj.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wk.shxzukj.cn

[R09] 字符串比较
来源：http://gf.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pn.9csxet.cn

[R10] 正则匹配
来源：http://vq.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yv.shxzukj.cn

[R11] case 多分支
来源：http://cp.szsharing.cn

case "$1" in
来源：http://ja.haigaiapp.cn

start) echo "启动" ;;
来源：http://bx.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://fo.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://xv.chemitech.net.cn

esac
来源：http://uv.yuexingan06.cn

[R12] for 遍历文件
来源：http://ew.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://cb.haigaiapp.cn

[R13] for 计数循环
来源：http://fp.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://kw.szsharing.cn

[R14] C 风格 for
来源：http://zy.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qf.shtwfgs.cn

[R15] while 逐行读文件
来源：http://vt.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oi.lnxyls.cn

[R16] until 等待条件
来源：http://ps.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://op.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://cn.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zs.newstarts.cn

[R18] 遍历数组
来源：http://lo.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kc.colortex.cn

[R19] 数组长度
来源：http://zt.szsharing.cn

echo "${#arr[@]}"
来源：http://of.szsharing.cn

[R20] 关联数组（字典）
来源：http://wo.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ry.szsharing.cn

[R21] 字符串长度
来源：http://wx.yuexingan06.cn

echo "${#s}"
来源：http://jn.nszjky.cn

[R22] 截取子串
来源：http://dg.jctech888.com.cn

echo "${s:0:5}"
来源：http://zo.shtwfgs.cn

[R23] 字符串替换
来源：http://gq.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mn.huanxung.cn

[R24] 大小写转换
来源：http://fh.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bu.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://xa.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://je.muxihuayi.cn

[R26] 命令替换
来源：http://zt.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://zq.shxzukj.cn

[R27] 算术展开
来源：http://xe.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://ls.muxihuayi.cn

[R28] 浮点运算
来源：http://ts.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://dg.hahajie.cn

[R29] 定义函数
来源：http://qh.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yb.lnxyls.cn

[R30] 函数返回状态码
来源：http://xo.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://gi.gzmigu.cn

[R31] 局部变量
来源：http://xs.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://au.chemitech.net.cn

[R32] 参数个数校验
来源：http://wq.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xh.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://iw.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wo.9csxet.cn

[R34] 退出时清理
来源：http://lq.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qo.lnxyls.cn

[R35] 后台执行并等待
来源：http://fe.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cv.colortex.cn

[R36] 并发执行多个任务
来源：http://yl.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nv.panjiajie.cn

[R37] 把输出赋给变量
来源：http://xf.panjiajie.cn

files=$(ls -1)
来源：http://xw.lnxyls.cn

[R38] 管道串联
来源：http://ux.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://aj.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://ez.huixiangedu.cn

cmd > out.log 2>&1
来源：http://tm.huixinmuqiang.cn

[R40] 追加写日志
来源：http://qd.shtwfgs.cn

echo "log" >> out.log
来源：http://dz.hnjuh.cn

[R41] 丢弃输出
来源：http://we.nicolike.cn

cmd >/dev/null 2>&1
来源：http://hq.shxzukj.cn

[R42] 输入重定向
来源：http://kt.hnjuh.cn

wc -l < a.txt
来源：http://ic.shxzukj.cn

[R43] 按名字查找文件
来源：http://xd.yuntaijiaju.cn


<!-- 参考信息 -->