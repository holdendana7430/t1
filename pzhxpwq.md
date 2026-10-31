代发 wailian999

CREATE TABLE users (
来源：http://qe.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vt.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://fi.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://dy.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yo.nszjky.cn

);
来源：http://hm.szxytkj.cn

[Q02] 创建带外键的表
来源：http://kv.521024.cn

CREATE TABLE orders (
来源：http://wk.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ne.gzmigu.cn

user_id INT NOT NULL,
来源：http://yz.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://so.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fj.9csxet.cn

);
来源：http://ag.chemitech.net.cn

[Q03] 增加列
来源：http://sh.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yv.gzmigu.cn

[Q04] 修改列类型
来源：http://id.hahajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zu.hahajie.cn

[Q05] 重命名列
来源：http://ub.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://is.szxytkj.cn

[Q06] 删除列
来源：http://aq.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ew.szsharing.cn

[Q07] 删除表
来源：http://ot.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://ct.colortex.cn

[Q08] 创建普通索引
来源：http://ls.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ap.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://qq.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ah.nicolike.cn

[Q10] 插入单行
来源：http://gi.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://an.nicolike.cn

[Q11] 一次插入多行
来源：http://mq.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kb.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://tv.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fc.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mu.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://nk.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ka.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://kk.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xu.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wp.gzmigu.cn

[Q15] 查询全部
来源：http://kt.colortex.cn

SELECT * FROM users;
来源：http://nw.huixiangedu.cn

[Q16] 查询指定列
来源：http://pf.chemitech.net.cn

SELECT id, name FROM users;
来源：http://fq.szxytkj.cn

[Q17] 条件查询
来源：http://pj.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qq.huixiangedu.cn

[Q18] 模糊匹配
来源：http://rs.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kb.hnjuh.cn

[Q19] 范围查询
来源：http://sm.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eh.shtwfgs.cn

[Q20] IN 列表
来源：http://ln.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://em.hahajie.cn

[Q21] 空值判断
来源：http://pv.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://im.muxihuayi.cn

[Q22] 排序
来源：http://rm.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mk.szsharing.cn

[Q23] 分页
来源：http://ry.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jl.521024.cn

[Q24] 去重
来源：http://by.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://kq.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://vw.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nm.muxihuayi.cn

[Q26] 计数
来源：http://gb.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://mw.hahajie.cn

[Q27] 条件计数
来源：http://ts.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gc.nicolike.cn

[Q28] 求和与平均
来源：http://ia.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ph.521024.cn

[Q29] 最大最小值
来源：http://ml.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vb.panjiajie.cn

[Q30] 分组统计
来源：http://ro.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ty.colortex.cn

[Q31] 分组后过滤
来源：http://dh.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fg.szsharing.cn

[Q32] 分组拼接字符串
来源：http://yg.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iv.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://es.hahajie.cn

[Q33] 多列分组
来源：http://nn.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://te.jctech888.com.cn

[Q34] 每组取第一条
来源：http://ht.hahajie.cn

SELECT * FROM (
来源：http://ap.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mq.shtwfgs.cn

) t WHERE rn = 1;
来源：http://bx.huanxung.cn

[Q35] 内连接
来源：http://kt.szsharing.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xn.bjjhwx.cn

[Q36] 左连接
来源：http://yo.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xw.huixiangedu.cn

[Q37] 右连接
来源：http://kg.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zt.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hp.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://us.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://ma.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cv.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ve.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ad.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oj.shtwfgs.cn

[Q41] 多表连接
来源：http://tm.huanxung.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mz.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://tw.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://yk.asd995.cn

[Q42] 连接条件附加过滤
来源：http://le.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://uy.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ey.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://qd.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ec.muxihuayi.cn

[Q44] IN 子查询
来源：http://ve.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lh.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://lv.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jb.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://iu.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ns.shxzskj.cn

[Q47] 与平均值比较
来源：http://xk.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cx.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://uc.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://re.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://zk.yuntaijiaju.cn

[Q49] 更新单行
来源：http://wt.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fb.asd995.cn

[Q50] 批量更新
来源：http://ke.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lk.szsharing.cn

[Q51] 用子查询更新
来源：http://dy.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ix.lnxyls.cn

[Q52] 删除指定行
来源：http://zk.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://vl.wgjwhj.cn

[Q53] 按条件删除
来源：http://uu.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rc.wgjwhj.cn

[Q54] 清空表
来源：http://tc.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://ok.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://pw.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fj.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://gq.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fn.panjiajie.cn

[Q57] 行号
来源：http://yv.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qd.asd995.cn

[Q58] 累计求和
来源：http://fb.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vu.9csxet.cn

[Q59] 分组内累计
来源：http://zj.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fn.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://ns.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bm.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oe.jctech888.com.cn

[Q61] 移动平均
来源：http://tg.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yd.huanxung.cn

[Q62] 分组占比
来源：http://xv.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uf.panjiajie.cn

[Q63] 开启事务
来源：http://ek.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lt.chemitech.net.cn

[Q64] 提交事务
来源：http://mb.gzmigu.cn

COMMIT;
来源：http://kf.nszjky.cn

[Q65] 回滚事务
来源：http://gt.yuntaijiaju.cn

ROLLBACK;
来源：http://uf.jctech888.com.cn

[Q66] 行锁查询
来源：http://wy.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yh.newstarts.cn

[Q67] 设置隔离级别
来源：http://vj.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wf.huanxung.cn

[Q68] 保存点
来源：http://yv.szsharing.cn

SAVEPOINT sp1;
来源：http://rf.gzmigu.cn

ROLLBACK TO sp1;
来源：http://em.muxihuayi.cn

[Q69] 查看执行计划
来源：http://py.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://le.shxzskj.cn

[Q70] 更新统计信息
来源：http://fl.szsharing.cn

ANALYZE TABLE users;
来源：http://yb.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://xc.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fu.9csxet.cn

[Q72] 查看索引
来源：http://rl.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://at.huanxung.cn

[Q73] 查看表状态
来源：http://xd.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uk.chemitech.net.cn

[Q74] 强制使用索引
来源：http://uj.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tg.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://hv.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mg.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kc.huixinmuqiang.cn

[Q76] 按天统计
来源：http://ju.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dp.colortex.cn

[Q77] 时间加减
来源：http://tj.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gn.hahajie.cn

[Q78] 当前时间
来源：http://jb.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mj.nszjky.cn

[Q79] 字符串拼接
来源：http://zx.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mg.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://lh.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qg.szxytkj.cn

[Q81] 字符串替换
来源：http://xc.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cq.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://eo.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ls.shtwfgs.cn

[Q83] 大小写转换
来源：http://tp.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fg.colortex.cn

[Q84] 去除首尾空格
来源：http://cc.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://zu.lnxyls.cn

[Q85] 数值取整
来源：http://uc.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nz.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://qv.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lx.9csxet.cn

[Q87] JSON 字段做条件
来源：http://ux.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zn.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://rf.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fw.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jy.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://sj.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vb.newstarts.cn

[Q90] 生成序号列
来源：http://sw.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eg.newstarts.cn

================================================================================
来源：http://ug.nicolike.cn

R. Bash 专题
来源：http://cv.szsharing.cn

================================================================================
来源：http://fa.nszjky.cn

[R01] shebang 与严格模式
来源：http://wd.yuexingan06.cn

#!/usr/bin/env bash
来源：http://oe.panjiajie.cn

set -euo pipefail
来源：http://cv.szsharing.cn

[R02] 变量赋值与使用
来源：http://hr.shxzskj.cn

name="Tom"; echo "$name"
来源：http://ok.szsharing.cn

[R03] 只读变量
来源：http://pr.9csxet.cn

readonly PI=3.14
来源：http://ix.9csxet.cn

[R04] 位置参数
来源：http://so.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zc.huanxung.cn

[R05] 参数默认值
来源：http://ge.haigaiapp.cn

name="${1:-default}"
来源：http://kg.panjiajie.cn

[R06] 判断命令是否存在
来源：http://dt.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qh.szxytkj.cn

[R07] if 判断文件
来源：http://ol.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tn.bjjhwx.cn

[R08] 数值比较
来源：http://sz.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qp.haigaiapp.cn

[R09] 字符串比较
来源：http://gg.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wv.nszjky.cn

[R10] 正则匹配
来源：http://bm.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bs.shxzskj.cn

[R11] case 多分支
来源：http://lk.panjiajie.cn

case "$1" in
来源：http://en.lnxyls.cn

start) echo "启动" ;;
来源：http://qw.hahajie.cn

stop)  echo "停止" ;;
来源：http://ou.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://tx.chemitech.net.cn

esac
来源：http://wj.jctech888.com.cn

[R12] for 遍历文件
来源：http://zn.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://lx.bookmarksfly.cn

[R13] for 计数循环
来源：http://he.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://rr.yuntaijiaju.cn

[R14] C 风格 for
来源：http://hm.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cj.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://kl.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eb.szxytkj.cn

[R16] until 等待条件
来源：http://ox.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fc.gzmigu.cn

[R17] 数组定义与取值
来源：http://bk.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://iu.huixiangedu.cn

[R18] 遍历数组
来源：http://xm.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xm.szsharing.cn

[R19] 数组长度
来源：http://oz.shxzukj.cn

echo "${#arr[@]}"
来源：http://we.szsharing.cn

[R20] 关联数组（字典）
来源：http://tw.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://we.shxzukj.cn

[R21] 字符串长度
来源：http://cf.wgjwhj.cn

echo "${#s}"
来源：http://zm.szsharing.cn

[R22] 截取子串
来源：http://qs.hahajie.cn

echo "${s:0:5}"
来源：http://zu.hnjuh.cn

[R23] 字符串替换
来源：http://lr.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ji.yuntaijiaju.cn

[R24] 大小写转换
来源：http://zt.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ou.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://mx.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bo.szxytkj.cn

[R26] 命令替换
来源：http://ob.asd995.cn

now=$(date +%F); echo "$now"
来源：http://gd.asd995.cn

[R27] 算术展开
来源：http://sq.huanxung.cn

echo $((1 + 2 * 3))
来源：http://ja.wgjwhj.cn

[R28] 浮点运算
来源：http://zu.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://vf.huixinmuqiang.cn

[R29] 定义函数
来源：http://ue.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dw.nicolike.cn

[R30] 函数返回状态码
来源：http://dw.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://lu.muxihuayi.cn

[R31] 局部变量
来源：http://mk.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://oc.colortex.cn

[R32] 参数个数校验
来源：http://wb.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rf.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://al.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qo.panjiajie.cn

[R34] 退出时清理
来源：http://al.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pl.nszjky.cn

[R35] 后台执行并等待
来源：http://dk.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gd.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://gq.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gd.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://wz.huixiangedu.cn

files=$(ls -1)
来源：http://jj.gzmigu.cn

[R38] 管道串联
来源：http://hp.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://qs.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://yw.newstarts.cn

cmd > out.log 2>&1
来源：http://hu.521024.cn

[R40] 追加写日志
来源：http://mx.shxzukj.cn

echo "log" >> out.log
来源：http://bb.haigaiapp.cn

[R41] 丢弃输出
来源：http://gn.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://ht.shtwfgs.cn

[R42] 输入重定向
来源：http://gn.hnjuh.cn

wc -l < a.txt
来源：http://rl.szxytkj.cn

[R43] 按名字查找文件
来源：http://ya.gzmigu.cn

find . -name "*.log" -type f
来源：http://xo.nicolike.cn

[R44] 按修改时间查找
来源：http://ic.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://fl.yuexingan06.cn

[R45] 批量删除
来源：http://zh.panjiajie.cn


<!-- 参考信息 -->