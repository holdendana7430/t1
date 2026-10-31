代发 wailian999

CREATE TABLE users (
来源：http://ev.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iv.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://di.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://lc.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ir.shtwfgs.cn

);
来源：http://wq.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://hg.huixiangedu.cn

CREATE TABLE orders (
来源：http://in.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vz.9csxet.cn

user_id INT NOT NULL,
来源：http://my.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://lp.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sr.szsharing.cn

);
来源：http://bv.chemitech.net.cn

[Q03] 增加列
来源：http://em.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yh.hahajie.cn

[Q04] 修改列类型
来源：http://ls.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nb.9csxet.cn

[Q05] 重命名列
来源：http://kv.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jf.szsharing.cn

[Q06] 删除列
来源：http://go.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fw.bookmarksfly.cn

[Q07] 删除表
来源：http://or.gzmigu.cn

DROP TABLE IF EXISTS orders;
来源：http://uk.szsharing.cn

[Q08] 创建普通索引
来源：http://pz.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://aw.panjiajie.cn

[Q09] 创建唯一索引
来源：http://fx.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cb.newstarts.cn

[Q10] 插入单行
来源：http://fo.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ga.asd995.cn

[Q11] 一次插入多行
来源：http://sf.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kr.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://xg.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://el.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aj.shxzskj.cn

[Q13] 忽略重复插入
来源：http://jq.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mk.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://cd.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gn.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://km.shxzskj.cn

[Q15] 查询全部
来源：http://sq.bookmarksfly.cn

SELECT * FROM users;
来源：http://qq.wgjwhj.cn

[Q16] 查询指定列
来源：http://uo.haigaiapp.cn

SELECT id, name FROM users;
来源：http://ok.colortex.cn

[Q17] 条件查询
来源：http://tc.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mg.shtwfgs.cn

[Q18] 模糊匹配
来源：http://nq.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cf.asd995.cn

[Q19] 范围查询
来源：http://ez.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cy.lnxyls.cn

[Q20] IN 列表
来源：http://wb.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://px.9csxet.cn

[Q21] 空值判断
来源：http://em.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qh.asd995.cn

[Q22] 排序
来源：http://sh.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uv.yuntaijiaju.cn

[Q23] 分页
来源：http://fy.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vv.nszjky.cn

[Q24] 去重
来源：http://me.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://qi.panjiajie.cn

[Q25] 只取前 N 条
来源：http://vo.yuexingan06.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fr.jianghongdianzi.cn

[Q26] 计数
来源：http://ra.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://rl.shxzukj.cn

[Q27] 条件计数
来源：http://tr.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tx.hahajie.cn

[Q28] 求和与平均
来源：http://yy.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ub.yuexingan06.cn

[Q29] 最大最小值
来源：http://pc.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nm.panjiajie.cn

[Q30] 分组统计
来源：http://rd.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vd.jctech888.com.cn

[Q31] 分组后过滤
来源：http://vs.haigaiapp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wp.szsharing.cn

[Q32] 分组拼接字符串
来源：http://tf.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ye.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ti.hnjuh.cn

[Q33] 多列分组
来源：http://kn.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mx.jctech888.com.cn

[Q34] 每组取第一条
来源：http://we.huanxung.cn

SELECT * FROM (
来源：http://ux.nicolike.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nu.lnxyls.cn

) t WHERE rn = 1;
来源：http://um.lnxyls.cn

[Q35] 内连接
来源：http://fe.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bq.colortex.cn

[Q36] 左连接
来源：http://mp.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bc.hahajie.cn

[Q37] 右连接
来源：http://fj.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vl.asd995.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cu.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ov.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://ng.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oq.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mm.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rm.shxzukj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ve.yuntaijiaju.cn

[Q41] 多表连接
来源：http://pn.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ve.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://bw.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://tw.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://td.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://ld.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://es.huixiangedu.cn

[Q43] 标量子查询
来源：http://tm.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jh.jctech888.com.cn

[Q44] IN 子查询
来源：http://dh.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ei.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://yi.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jp.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ep.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://en.hnjuh.cn

[Q47] 与平均值比较
来源：http://gl.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wp.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://dx.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yb.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://bp.asd995.cn

[Q49] 更新单行
来源：http://lj.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hi.szsharing.cn

[Q50] 批量更新
来源：http://ja.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rr.szsharing.cn

[Q51] 用子查询更新
来源：http://vn.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rb.szsharing.cn

[Q52] 删除指定行
来源：http://rs.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://yi.jctech888.com.cn

[Q53] 按条件删除
来源：http://bt.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rq.asd995.cn

[Q54] 清空表
来源：http://zg.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://xy.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://na.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eb.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://la.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xk.wgjwhj.cn

[Q57] 行号
来源：http://vi.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yq.chemitech.net.cn

[Q58] 累计求和
来源：http://iv.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gv.521024.cn

[Q59] 分组内累计
来源：http://tf.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ob.521024.cn

[Q60] 取上一行 / 下一行
来源：http://zu.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ri.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pj.yuexingan06.cn

[Q61] 移动平均
来源：http://uq.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ic.shxzskj.cn

[Q62] 分组占比
来源：http://eu.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lg.shxzukj.cn

[Q63] 开启事务
来源：http://wj.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dh.shxzskj.cn

[Q64] 提交事务
来源：http://qi.jianghongdianzi.cn

COMMIT;
来源：http://ld.haigaiapp.cn

[Q65] 回滚事务
来源：http://ru.jctech888.com.cn

ROLLBACK;
来源：http://kr.haigaiapp.cn

[Q66] 行锁查询
来源：http://pt.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sv.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://wp.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cs.lnxyls.cn

[Q68] 保存点
来源：http://kd.bjjhwx.cn

SAVEPOINT sp1;
来源：http://gs.szxytkj.cn

ROLLBACK TO sp1;
来源：http://sx.haigaiapp.cn

[Q69] 查看执行计划
来源：http://rc.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wa.muxihuayi.cn

[Q70] 更新统计信息
来源：http://fs.wgjwhj.cn

ANALYZE TABLE users;
来源：http://iw.lnxyls.cn

[Q71] 查看建表语句
来源：http://um.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ur.521024.cn

[Q72] 查看索引
来源：http://yu.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://ti.shtwfgs.cn

[Q73] 查看表状态
来源：http://xe.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gx.muxihuayi.cn

[Q74] 强制使用索引
来源：http://ky.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ad.wgjwhj.cn

[Q75] 日期格式化
来源：http://ds.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dg.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zv.bjjhwx.cn

[Q76] 按天统计
来源：http://sl.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ls.521024.cn

[Q77] 时间加减
来源：http://jk.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nu.jctech888.com.cn

[Q78] 当前时间
来源：http://aq.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://in.9csxet.cn

[Q79] 字符串拼接
来源：http://pw.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aa.shtwfgs.cn

[Q80] 字符串截取
来源：http://hc.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ui.colortex.cn

[Q81] 字符串替换
来源：http://ak.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wc.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://yi.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zn.yuexingan06.cn

[Q83] 大小写转换
来源：http://em.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cd.panjiajie.cn

[Q84] 去除首尾空格
来源：http://fs.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://pa.bjjhwx.cn

[Q85] 数值取整
来源：http://un.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aw.asd995.cn

[Q86] 读取 JSON 字段
来源：http://jh.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://er.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://rc.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pl.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://nz.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wa.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://na.huanxung.cn

[Q89] 判断表是否存在
来源：http://iy.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xq.muxihuayi.cn

[Q90] 生成序号列
来源：http://nv.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vp.jctech888.com.cn

================================================================================
来源：http://gd.521024.cn

R. Bash 专题
来源：http://ma.wgjwhj.cn

================================================================================
来源：http://du.newstarts.cn

[R01] shebang 与严格模式
来源：http://og.9csxet.cn

#!/usr/bin/env bash
来源：http://ee.huanxung.cn

set -euo pipefail
来源：http://qx.szsharing.cn

[R02] 变量赋值与使用
来源：http://hy.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://yt.huixinmuqiang.cn

[R03] 只读变量
来源：http://fg.bjjhwx.cn

readonly PI=3.14
来源：http://xe.huixiangedu.cn

[R04] 位置参数
来源：http://km.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yt.szsharing.cn

[R05] 参数默认值
来源：http://pa.wgjwhj.cn

name="${1:-default}"
来源：http://vb.shxzukj.cn

[R06] 判断命令是否存在
来源：http://ix.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xd.asd995.cn

[R07] if 判断文件
来源：http://ob.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zc.gzmigu.cn

[R08] 数值比较
来源：http://pi.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qm.colortex.cn

[R09] 字符串比较
来源：http://uz.nszjky.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jb.nszjky.cn

[R10] 正则匹配
来源：http://pf.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ed.jianghongdianzi.cn

[R11] case 多分支
来源：http://yg.gzmigu.cn

case "$1" in
来源：http://li.szsharing.cn

start) echo "启动" ;;
来源：http://pk.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://nn.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://pb.wgjwhj.cn

esac
来源：http://ru.muxihuayi.cn

[R12] for 遍历文件
来源：http://en.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://zs.huixiangedu.cn

[R13] for 计数循环
来源：http://lz.asd995.cn

for i in {1..10}; do echo "$i"; done
来源：http://tc.chemitech.net.cn

[R14] C 风格 for
来源：http://ip.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bh.bjjhwx.cn

[R15] while 逐行读文件
来源：http://yh.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://de.asd995.cn

[R16] until 等待条件
来源：http://fk.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://il.hnjuh.cn

[R17] 数组定义与取值
来源：http://ro.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yj.yuntaijiaju.cn

[R18] 遍历数组
来源：http://pt.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://it.muxihuayi.cn

[R19] 数组长度
来源：http://jz.nszjky.cn

echo "${#arr[@]}"
来源：http://es.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://bl.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qw.nszjky.cn

[R21] 字符串长度
来源：http://fn.gzmigu.cn

echo "${#s}"
来源：http://qi.huanxung.cn

[R22] 截取子串
来源：http://rx.lnxyls.cn

echo "${s:0:5}"
来源：http://tu.nicolike.cn

[R23] 字符串替换
来源：http://jj.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iu.shtwfgs.cn

[R24] 大小写转换
来源：http://wk.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yq.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://gb.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eg.huixinmuqiang.cn

[R26] 命令替换
来源：http://ym.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://mu.9csxet.cn

[R27] 算术展开
来源：http://wp.nicolike.cn

echo $((1 + 2 * 3))
来源：http://da.nicolike.cn

[R28] 浮点运算
来源：http://pp.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://ou.colortex.cn

[R29] 定义函数
来源：http://da.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ra.gzmigu.cn

[R30] 函数返回状态码
来源：http://qp.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://kj.huixinmuqiang.cn

[R31] 局部变量
来源：http://mp.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://pa.shxzskj.cn

[R32] 参数个数校验
来源：http://wk.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zn.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://mp.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rx.muxihuayi.cn

[R34] 退出时清理
来源：http://nw.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sl.521024.cn

[R35] 后台执行并等待
来源：http://yv.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yf.hahajie.cn

[R36] 并发执行多个任务
来源：http://ou.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://of.nicolike.cn

[R37] 把输出赋给变量
来源：http://xv.colortex.cn

files=$(ls -1)
来源：http://ql.colortex.cn

[R38] 管道串联
来源：http://nh.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://hc.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://px.yuexingan06.cn

cmd > out.log 2>&1
来源：http://dw.bookmarksfly.cn

[R40] 追加写日志
来源：http://si.chemitech.net.cn

echo "log" >> out.log
来源：http://pt.chemitech.net.cn

[R41] 丢弃输出
来源：http://rl.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://mx.wgjwhj.cn

[R42] 输入重定向
来源：http://wx.szxytkj.cn

wc -l < a.txt
来源：http://vf.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://qi.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://ra.huanxung.cn

[R44] 按修改时间查找
来源：http://my.szsharing.cn

find . -mtime -7 -type f
来源：http://ub.shxzskj.cn

[R45] 批量删除
来源：http://ue.gzmigu.cn


<!-- 参考信息 -->