代发 wailian999

CREATE TABLE users (
来源：http://gu.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oa.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://sg.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://cv.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mv.chemitech.net.cn

);
来源：http://jk.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://ve.wgjwhj.cn

CREATE TABLE orders (
来源：http://yc.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jg.szsharing.cn

user_id INT NOT NULL,
来源：http://hz.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://ry.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ws.521024.cn

);
来源：http://xn.nszjky.cn

[Q03] 增加列
来源：http://nb.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nr.hnjuh.cn

[Q04] 修改列类型
来源：http://ti.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vp.chemitech.net.cn

[Q05] 重命名列
来源：http://zw.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://le.yuexingan06.cn

[Q06] 删除列
来源：http://jr.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kr.muxihuayi.cn

[Q07] 删除表
来源：http://gg.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://dv.szsharing.cn

[Q08] 创建普通索引
来源：http://na.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bv.9csxet.cn

[Q09] 创建唯一索引
来源：http://hh.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fo.521024.cn

[Q10] 插入单行
来源：http://hv.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rp.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://ec.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sg.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://xt.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qf.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qn.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://en.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gw.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://ws.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sp.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lp.hnjuh.cn

[Q15] 查询全部
来源：http://ih.huixinmuqiang.cn

SELECT * FROM users;
来源：http://wy.shtwfgs.cn

[Q16] 查询指定列
来源：http://mo.panjiajie.cn

SELECT id, name FROM users;
来源：http://lz.shxzskj.cn

[Q17] 条件查询
来源：http://om.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fw.9csxet.cn

[Q18] 模糊匹配
来源：http://bp.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xo.9csxet.cn

[Q19] 范围查询
来源：http://qs.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ee.bjjhwx.cn

[Q20] IN 列表
来源：http://ai.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vw.szxytkj.cn

[Q21] 空值判断
来源：http://lo.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mf.gzmigu.cn

[Q22] 排序
来源：http://cc.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eh.hahajie.cn

[Q23] 分页
来源：http://fg.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ux.hahajie.cn

[Q24] 去重
来源：http://pa.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://zc.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://us.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fn.asd995.cn

[Q26] 计数
来源：http://vl.521024.cn

SELECT COUNT(*) FROM users;
来源：http://cv.shxzukj.cn

[Q27] 条件计数
来源：http://tp.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ub.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://kt.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pf.wgjwhj.cn

[Q29] 最大最小值
来源：http://as.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qp.bookmarksfly.cn

[Q30] 分组统计
来源：http://oh.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ys.newstarts.cn

[Q31] 分组后过滤
来源：http://wo.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vk.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://ki.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cc.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://em.chemitech.net.cn

[Q33] 多列分组
来源：http://ei.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sh.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://oi.lnxyls.cn

SELECT * FROM (
来源：http://xv.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ad.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://qi.colortex.cn

[Q35] 内连接
来源：http://ea.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://af.wgjwhj.cn

[Q36] 左连接
来源：http://og.asd995.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wz.hnjuh.cn

[Q37] 右连接
来源：http://gt.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ck.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dz.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yt.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://ti.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ys.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rr.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bd.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nn.yuexingan06.cn

[Q41] 多表连接
来源：http://sl.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rf.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://nh.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://ye.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://ei.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://aq.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dn.shxzukj.cn

[Q43] 标量子查询
来源：http://sz.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ao.chemitech.net.cn

[Q44] IN 子查询
来源：http://tp.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://am.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://dz.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yw.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xf.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dc.shxzskj.cn

[Q47] 与平均值比较
来源：http://im.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pn.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://wf.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ij.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://qt.colortex.cn

[Q49] 更新单行
来源：http://wn.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fc.bookmarksfly.cn

[Q50] 批量更新
来源：http://kv.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ui.szxytkj.cn

[Q51] 用子查询更新
来源：http://xh.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mi.shxzukj.cn

[Q52] 删除指定行
来源：http://sc.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://zp.szsharing.cn

[Q53] 按条件删除
来源：http://na.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ao.jctech888.com.cn

[Q54] 清空表
来源：http://qs.nszjky.cn

TRUNCATE TABLE logs;
来源：http://fo.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://js.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iy.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://pd.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dm.muxihuayi.cn

[Q57] 行号
来源：http://bj.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://au.521024.cn

[Q58] 累计求和
来源：http://na.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ly.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://fy.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ln.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://tr.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oi.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gc.hahajie.cn

[Q61] 移动平均
来源：http://rn.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fh.huixiangedu.cn

[Q62] 分组占比
来源：http://xe.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eg.hahajie.cn

[Q63] 开启事务
来源：http://hk.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rr.yuntaijiaju.cn

[Q64] 提交事务
来源：http://sw.jctech888.com.cn

COMMIT;
来源：http://tr.hnjuh.cn

[Q65] 回滚事务
来源：http://kr.asd995.cn

ROLLBACK;
来源：http://gk.szxytkj.cn

[Q66] 行锁查询
来源：http://cb.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lr.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://ng.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jq.9csxet.cn

[Q68] 保存点
来源：http://eh.shxzskj.cn

SAVEPOINT sp1;
来源：http://ap.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://qj.chemitech.net.cn

[Q69] 查看执行计划
来源：http://ea.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://if.chemitech.net.cn

[Q70] 更新统计信息
来源：http://fm.9csxet.cn

ANALYZE TABLE users;
来源：http://sr.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://rq.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gj.huixinmuqiang.cn

[Q72] 查看索引
来源：http://ai.9csxet.cn

SHOW INDEX FROM users;
来源：http://fd.panjiajie.cn

[Q73] 查看表状态
来源：http://ii.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wb.hnjuh.cn

[Q74] 强制使用索引
来源：http://tl.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qp.bookmarksfly.cn

[Q75] 日期格式化
来源：http://yt.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gu.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://su.bjjhwx.cn

[Q76] 按天统计
来源：http://qz.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xu.asd995.cn

[Q77] 时间加减
来源：http://im.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ub.wgjwhj.cn

[Q78] 当前时间
来源：http://tr.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eq.asd995.cn

[Q79] 字符串拼接
来源：http://yn.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tx.9csxet.cn

[Q80] 字符串截取
来源：http://th.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ng.gzmigu.cn

[Q81] 字符串替换
来源：http://rg.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ax.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://di.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bj.jctech888.com.cn

[Q83] 大小写转换
来源：http://mx.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://st.jctech888.com.cn

[Q84] 去除首尾空格
来源：http://yb.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://ps.asd995.cn

[Q85] 数值取整
来源：http://ak.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cp.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://ra.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mq.nicolike.cn

[Q87] JSON 字段做条件
来源：http://yr.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cv.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://jj.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aq.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fx.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://zv.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rx.yuexingan06.cn

[Q90] 生成序号列
来源：http://yl.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ex.521024.cn

================================================================================
来源：http://sy.jianghongdianzi.cn

R. Bash 专题
来源：http://yb.521024.cn

================================================================================
来源：http://bi.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://ti.panjiajie.cn

#!/usr/bin/env bash
来源：http://ao.nicolike.cn

set -euo pipefail
来源：http://se.szxytkj.cn

[R02] 变量赋值与使用
来源：http://ck.szxytkj.cn

name="Tom"; echo "$name"
来源：http://cj.colortex.cn

[R03] 只读变量
来源：http://mq.shxzukj.cn

readonly PI=3.14
来源：http://xp.colortex.cn

[R04] 位置参数
来源：http://jp.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://en.jctech888.com.cn

[R05] 参数默认值
来源：http://zh.lnxyls.cn

name="${1:-default}"
来源：http://qj.9csxet.cn

[R06] 判断命令是否存在
来源：http://nd.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jo.bjjhwx.cn

[R07] if 判断文件
来源：http://op.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pm.newstarts.cn

[R08] 数值比较
来源：http://kh.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ip.chemitech.net.cn

[R09] 字符串比较
来源：http://by.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ou.nszjky.cn

[R10] 正则匹配
来源：http://mu.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://he.muxihuayi.cn

[R11] case 多分支
来源：http://we.yuntaijiaju.cn

case "$1" in
来源：http://zj.newstarts.cn

start) echo "启动" ;;
来源：http://ld.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://az.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://xu.asd995.cn

esac
来源：http://je.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://xd.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://mr.9csxet.cn

[R13] for 计数循环
来源：http://at.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://xz.huanxung.cn

[R14] C 风格 for
来源：http://yk.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ot.521024.cn

[R15] while 逐行读文件
来源：http://vd.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pf.szxytkj.cn

[R16] until 等待条件
来源：http://fb.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://id.szxytkj.cn

[R17] 数组定义与取值
来源：http://pl.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pi.shxzukj.cn

[R18] 遍历数组
来源：http://fu.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nt.jctech888.com.cn

[R19] 数组长度
来源：http://he.chemitech.net.cn

echo "${#arr[@]}"
来源：http://gm.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://bm.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nz.wgjwhj.cn

[R21] 字符串长度
来源：http://rv.jctech888.com.cn

echo "${#s}"
来源：http://wv.wgjwhj.cn

[R22] 截取子串
来源：http://qp.shtwfgs.cn

echo "${s:0:5}"
来源：http://gu.nszjky.cn

[R23] 字符串替换
来源：http://bx.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xk.wgjwhj.cn

[R24] 大小写转换
来源：http://ew.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ls.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://zj.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vt.panjiajie.cn

[R26] 命令替换
来源：http://er.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://qr.9csxet.cn

[R27] 算术展开
来源：http://nw.asd995.cn

echo $((1 + 2 * 3))
来源：http://kt.bookmarksfly.cn

[R28] 浮点运算
来源：http://bn.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://ot.nszjky.cn

[R29] 定义函数
来源：http://sr.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mv.jctech888.com.cn

[R30] 函数返回状态码
来源：http://wi.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://oj.9csxet.cn

[R31] 局部变量
来源：http://ok.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://zx.gzmigu.cn

[R32] 参数个数校验
来源：http://nb.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ya.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://mi.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dt.hnjuh.cn

[R34] 退出时清理
来源：http://qk.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kh.bjjhwx.cn

[R35] 后台执行并等待
来源：http://vh.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ot.hnjuh.cn

[R36] 并发执行多个任务
来源：http://fr.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lz.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://sz.9csxet.cn

files=$(ls -1)
来源：http://st.huixinmuqiang.cn

[R38] 管道串联
来源：http://jw.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://bw.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://xc.chemitech.net.cn

cmd > out.log 2>&1
来源：http://nz.chemitech.net.cn

[R40] 追加写日志
来源：http://tr.huixinmuqiang.cn

echo "log" >> out.log
来源：http://qd.nicolike.cn

[R41] 丢弃输出
来源：http://rl.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://sj.9csxet.cn

[R42] 输入重定向
来源：http://ff.wgjwhj.cn

wc -l < a.txt
来源：http://cq.panjiajie.cn

[R43] 按名字查找文件
来源：http://wc.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://mw.panjiajie.cn

[R44] 按修改时间查找
来源：http://iz.shxzskj.cn

find . -mtime -7 -type f
来源：http://xj.hnjuh.cn

[R45] 批量删除
来源：http://cj.yuntaijiaju.cn


<!-- 参考信息 -->