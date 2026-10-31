代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rq.asd995.cn

user_id INT NOT NULL,
来源：http://xd.9csxet.cn

amount DECIMAL(10, 2),
来源：http://ve.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rf.jianghongdianzi.cn

);
来源：http://gj.muxihuayi.cn

[Q03] 增加列
来源：http://mn.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hh.gzmigu.cn

[Q04] 修改列类型
来源：http://tk.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ch.bjjhwx.cn

[Q05] 重命名列
来源：http://xk.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wq.asd995.cn

[Q06] 删除列
来源：http://gl.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cq.bookmarksfly.cn

[Q07] 删除表
来源：http://yj.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://rj.9csxet.cn

[Q08] 创建普通索引
来源：http://ky.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sb.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://og.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lg.lnxyls.cn

[Q10] 插入单行
来源：http://ig.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yk.szsharing.cn

[Q11] 一次插入多行
来源：http://st.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jk.bookmarksfly.cn

[Q12] 插入后取自增 ID
来源：http://fn.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xo.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bb.panjiajie.cn

[Q13] 忽略重复插入
来源：http://mj.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pp.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://sy.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oc.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://en.shxzskj.cn

[Q15] 查询全部
来源：http://ep.chemitech.net.cn

SELECT * FROM users;
来源：http://nk.wgjwhj.cn

[Q16] 查询指定列
来源：http://xv.nicolike.cn

SELECT id, name FROM users;
来源：http://so.asd995.cn

[Q17] 条件查询
来源：http://os.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ve.szsharing.cn

[Q18] 模糊匹配
来源：http://ng.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://by.haigaiapp.cn

[Q19] 范围查询
来源：http://ku.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wk.gzmigu.cn

[Q20] IN 列表
来源：http://jq.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mp.hahajie.cn

[Q21] 空值判断
来源：http://oy.bookmarksfly.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://re.hnjuh.cn

[Q22] 排序
来源：http://qr.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eu.shxzskj.cn

[Q23] 分页
来源：http://xt.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wz.chemitech.net.cn

[Q24] 去重
来源：http://rz.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://er.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://fa.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ng.huixiangedu.cn

[Q26] 计数
来源：http://jp.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://rs.wgjwhj.cn

[Q27] 条件计数
来源：http://tz.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uk.nszjky.cn

[Q28] 求和与平均
来源：http://it.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ua.shxzskj.cn

[Q29] 最大最小值
来源：http://fz.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gn.bjjhwx.cn

[Q30] 分组统计
来源：http://bh.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eg.jctech888.com.cn

[Q31] 分组后过滤
来源：http://ii.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pi.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://og.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dq.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ki.huixiangedu.cn

[Q33] 多列分组
来源：http://zx.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mu.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://jp.shtwfgs.cn

SELECT * FROM (
来源：http://eb.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ub.huixiangedu.cn

) t WHERE rn = 1;
来源：http://pv.muxihuayi.cn

[Q35] 内连接
来源：http://hb.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zf.hnjuh.cn

[Q36] 左连接
来源：http://jo.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xs.panjiajie.cn

[Q37] 右连接
来源：http://hu.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dm.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yx.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://br.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://bo.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ph.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pe.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tz.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://au.nszjky.cn

[Q41] 多表连接
来源：http://fg.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zd.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://bc.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://hm.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://fj.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://ac.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yc.nszjky.cn

[Q43] 标量子查询
来源：http://ii.lnxyls.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kz.shxzskj.cn

[Q44] IN 子查询
来源：http://sd.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ts.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://fy.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oq.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sd.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ju.huanxung.cn

[Q47] 与平均值比较
来源：http://rl.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://so.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://og.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vu.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://ad.lnxyls.cn

[Q49] 更新单行
来源：http://qk.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aw.jctech888.com.cn

[Q50] 批量更新
来源：http://yd.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://og.shxzukj.cn

[Q51] 用子查询更新
来源：http://jt.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ea.huixiangedu.cn

[Q52] 删除指定行
来源：http://qz.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://zu.panjiajie.cn

[Q53] 按条件删除
来源：http://wn.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lo.muxihuayi.cn

[Q54] 清空表
来源：http://mv.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://jz.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://bh.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kz.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://hh.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yf.huixinmuqiang.cn

[Q57] 行号
来源：http://hy.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ps.9csxet.cn

[Q58] 累计求和
来源：http://ob.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ej.szxytkj.cn

[Q59] 分组内累计
来源：http://oo.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xy.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://wv.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ux.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wm.asd995.cn

[Q61] 移动平均
来源：http://fv.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kf.colortex.cn

[Q62] 分组占比
来源：http://xd.shxzukj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hw.huixinmuqiang.cn

[Q63] 开启事务
来源：http://sv.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qs.newstarts.cn

[Q64] 提交事务
来源：http://em.hnjuh.cn

COMMIT;
来源：http://sl.shxzukj.cn

[Q65] 回滚事务
来源：http://iv.chemitech.net.cn

ROLLBACK;
来源：http://xb.bjjhwx.cn

[Q66] 行锁查询
来源：http://ik.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ng.gzmigu.cn

[Q67] 设置隔离级别
来源：http://fd.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qu.asd995.cn

[Q68] 保存点
来源：http://ot.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://de.panjiajie.cn

ROLLBACK TO sp1;
来源：http://qc.hahajie.cn

[Q69] 查看执行计划
来源：http://au.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uz.szxytkj.cn

[Q70] 更新统计信息
来源：http://be.newstarts.cn

ANALYZE TABLE users;
来源：http://jz.gzmigu.cn

[Q71] 查看建表语句
来源：http://kh.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ab.bookmarksfly.cn

[Q72] 查看索引
来源：http://mm.hnjuh.cn

SHOW INDEX FROM users;
来源：http://yt.hnjuh.cn

[Q73] 查看表状态
来源：http://db.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://it.newstarts.cn

[Q74] 强制使用索引
来源：http://ru.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iw.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://wk.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ft.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ca.9csxet.cn

[Q76] 按天统计
来源：http://mo.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gz.huixinmuqiang.cn

[Q77] 时间加减
来源：http://sd.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wl.shxzukj.cn

[Q78] 当前时间
来源：http://co.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wz.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://ux.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gx.shxzukj.cn

[Q80] 字符串截取
来源：http://mm.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vw.muxihuayi.cn

[Q81] 字符串替换
来源：http://tv.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pf.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://gr.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kn.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://zz.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ej.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://tt.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://kc.huixinmuqiang.cn

[Q85] 数值取整
来源：http://vc.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://py.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://mi.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ee.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://yk.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xn.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://vl.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iw.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ho.nicolike.cn

[Q89] 判断表是否存在
来源：http://oo.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sy.hnjuh.cn

[Q90] 生成序号列
来源：http://jh.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ol.shxzukj.cn

================================================================================
来源：http://ln.panjiajie.cn

R. Bash 专题
来源：http://rg.shtwfgs.cn

================================================================================
来源：http://we.gzmigu.cn

[R01] shebang 与严格模式
来源：http://fj.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://nm.haigaiapp.cn

set -euo pipefail
来源：http://ze.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://uz.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://wt.muxihuayi.cn

[R03] 只读变量
来源：http://vc.huanxung.cn

readonly PI=3.14
来源：http://pb.chemitech.net.cn

[R04] 位置参数
来源：http://ia.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ys.newstarts.cn

[R05] 参数默认值
来源：http://vm.bookmarksfly.cn

name="${1:-default}"
来源：http://py.nszjky.cn

[R06] 判断命令是否存在
来源：http://zs.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gz.huixinmuqiang.cn

[R07] if 判断文件
来源：http://pj.nszjky.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rb.newstarts.cn

[R08] 数值比较
来源：http://vr.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://st.huixinmuqiang.cn

[R09] 字符串比较
来源：http://vd.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mk.9csxet.cn

[R10] 正则匹配
来源：http://fc.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bz.jctech888.com.cn

[R11] case 多分支
来源：http://el.hahajie.cn

case "$1" in
来源：http://uy.lnxyls.cn

start) echo "启动" ;;
来源：http://xg.asd995.cn

stop)  echo "停止" ;;
来源：http://du.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://vt.haigaiapp.cn

esac
来源：http://ax.hahajie.cn

[R12] for 遍历文件
来源：http://cp.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://gf.shxzukj.cn

[R13] for 计数循环
来源：http://sx.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://ui.huixinmuqiang.cn

[R14] C 风格 for
来源：http://ae.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xo.huanxung.cn

[R15] while 逐行读文件
来源：http://zd.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ka.521024.cn

[R16] until 等待条件
来源：http://ik.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ms.huanxung.cn

[R17] 数组定义与取值
来源：http://cs.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qm.jctech888.com.cn

[R18] 遍历数组
来源：http://ip.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tb.haigaiapp.cn

[R19] 数组长度
来源：http://de.asd995.cn

echo "${#arr[@]}"
来源：http://sr.hahajie.cn

[R20] 关联数组（字典）
来源：http://ir.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kt.huanxung.cn

[R21] 字符串长度
来源：http://qo.shxzukj.cn

echo "${#s}"
来源：http://zp.shxzukj.cn

[R22] 截取子串
来源：http://te.wgjwhj.cn

echo "${s:0:5}"
来源：http://na.9csxet.cn

[R23] 字符串替换
来源：http://iw.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wa.gzmigu.cn

[R24] 大小写转换
来源：http://fq.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xl.521024.cn

[R25] 去后缀 / 去前缀
来源：http://rx.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jt.shxzskj.cn

[R26] 命令替换
来源：http://oh.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://sw.yuexingan06.cn

[R27] 算术展开
来源：http://tc.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://us.colortex.cn

[R28] 浮点运算
来源：http://wm.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://ab.haigaiapp.cn

[R29] 定义函数
来源：http://jh.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wy.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://cm.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://qa.huixinmuqiang.cn

[R31] 局部变量
来源：http://pr.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://fh.hahajie.cn

[R32] 参数个数校验
来源：http://hc.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xw.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://vf.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eu.shtwfgs.cn

[R34] 退出时清理
来源：http://qv.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://am.huixiangedu.cn

[R35] 后台执行并等待
来源：http://qu.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qc.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://lb.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ey.521024.cn

[R37] 把输出赋给变量
来源：http://gr.521024.cn

files=$(ls -1)
来源：http://tn.nszjky.cn

[R38] 管道串联
来源：http://kv.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://br.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://ua.521024.cn

cmd > out.log 2>&1
来源：http://zd.colortex.cn

[R40] 追加写日志
来源：http://px.bjjhwx.cn

echo "log" >> out.log
来源：http://jo.panjiajie.cn

[R41] 丢弃输出
来源：http://dj.521024.cn

cmd >/dev/null 2>&1
来源：http://kq.yuntaijiaju.cn

[R42] 输入重定向
来源：http://el.szxytkj.cn

wc -l < a.txt
来源：http://ud.jctech888.com.cn

[R43] 按名字查找文件
来源：http://tw.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://hu.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://xf.huanxung.cn

find . -mtime -7 -type f
来源：http://up.szsharing.cn

[R45] 批量删除
来源：http://xh.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://wv.szxytkj.cn

[R46] 递归替换文件内容
来源：http://cx.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oa.bookmarksfly.cn

[R47] sed 单行替换
来源：http://tl.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ab.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://xv.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://kn.bjjhwx.cn

[R49] awk 带条件
来源：http://bv.521024.cn


<!-- 参考信息 -->