代发 wailian999

CREATE TABLE users (
来源：http://uv.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ig.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://ft.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://in.521024.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://og.jctech888.com.cn

);
来源：http://zn.newstarts.cn

[Q02] 创建带外键的表
来源：http://ud.hnjuh.cn

CREATE TABLE orders (
来源：http://aa.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ho.szxytkj.cn

user_id INT NOT NULL,
来源：http://yq.colortex.cn

amount DECIMAL(10, 2),
来源：http://ll.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qc.shtwfgs.cn

);
来源：http://fk.shxzukj.cn

[Q03] 增加列
来源：http://vk.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jj.nicolike.cn

[Q04] 修改列类型
来源：http://rd.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nr.521024.cn

[Q05] 重命名列
来源：http://yx.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://do.wgjwhj.cn

[Q06] 删除列
来源：http://rd.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wy.szxytkj.cn

[Q07] 删除表
来源：http://cb.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://os.chemitech.net.cn

[Q08] 创建普通索引
来源：http://ue.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wo.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://xe.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ck.panjiajie.cn

[Q10] 插入单行
来源：http://ms.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ec.521024.cn

[Q11] 一次插入多行
来源：http://hc.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ov.wgjwhj.cn

[Q12] 插入后取自增 ID
来源：http://qq.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ez.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bk.shxzukj.cn

[Q13] 忽略重复插入
来源：http://hl.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qe.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://ua.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ea.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kh.huanxung.cn

[Q15] 查询全部
来源：http://jc.521024.cn

SELECT * FROM users;
来源：http://ki.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://nz.bjjhwx.cn

SELECT id, name FROM users;
来源：http://yl.wgjwhj.cn

[Q17] 条件查询
来源：http://jk.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bd.newstarts.cn

[Q18] 模糊匹配
来源：http://bc.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lb.wgjwhj.cn

[Q19] 范围查询
来源：http://us.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rf.haigaiapp.cn

[Q20] IN 列表
来源：http://ea.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cy.panjiajie.cn

[Q21] 空值判断
来源：http://dg.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ty.lnxyls.cn

[Q22] 排序
来源：http://nx.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fa.nicolike.cn

[Q23] 分页
来源：http://lb.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sn.huanxung.cn

[Q24] 去重
来源：http://iq.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://ia.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://wl.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ll.9csxet.cn

[Q26] 计数
来源：http://bf.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://nx.yuntaijiaju.cn

[Q27] 条件计数
来源：http://ad.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://te.gzmigu.cn

[Q28] 求和与平均
来源：http://fv.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ii.yuntaijiaju.cn

[Q29] 最大最小值
来源：http://yd.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wv.asd995.cn

[Q30] 分组统计
来源：http://tc.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lp.wgjwhj.cn

[Q31] 分组后过滤
来源：http://zr.jctech888.com.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sq.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://ab.colortex.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gz.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ih.muxihuayi.cn

[Q33] 多列分组
来源：http://rn.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lg.bjjhwx.cn

[Q34] 每组取第一条
来源：http://we.wgjwhj.cn

SELECT * FROM (
来源：http://wa.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lj.newstarts.cn

) t WHERE rn = 1;
来源：http://bn.colortex.cn

[Q35] 内连接
来源：http://ao.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tg.panjiajie.cn

[Q36] 左连接
来源：http://sd.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cl.panjiajie.cn

[Q37] 右连接
来源：http://js.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zl.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mc.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ro.gzmigu.cn

[Q39] 自连接（查上下级）
来源：http://bo.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wl.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lq.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ck.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mf.shxzukj.cn

[Q41] 多表连接
来源：http://jr.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yt.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://ga.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://ok.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://vz.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://yk.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yj.huixiangedu.cn

[Q43] 标量子查询
来源：http://vv.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yj.lnxyls.cn

[Q44] IN 子查询
来源：http://vj.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qp.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://pl.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xp.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kw.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qi.chemitech.net.cn

[Q47] 与平均值比较
来源：http://eq.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ob.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://db.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zq.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://ny.huixiangedu.cn

[Q49] 更新单行
来源：http://fg.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rv.bjjhwx.cn

[Q50] 批量更新
来源：http://yn.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sq.shxzukj.cn

[Q51] 用子查询更新
来源：http://gk.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ym.muxihuayi.cn

[Q52] 删除指定行
来源：http://yc.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://mg.panjiajie.cn

[Q53] 按条件删除
来源：http://xw.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bs.haigaiapp.cn

[Q54] 清空表
来源：http://oc.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://gk.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://pj.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lj.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://dq.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vv.bookmarksfly.cn

[Q57] 行号
来源：http://gy.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gv.bookmarksfly.cn

[Q58] 累计求和
来源：http://ja.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ix.nszjky.cn

[Q59] 分组内累计
来源：http://va.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://du.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://iy.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ir.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ob.chemitech.net.cn

[Q61] 移动平均
来源：http://dj.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dt.chemitech.net.cn

[Q62] 分组占比
来源：http://ti.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wt.szxytkj.cn

[Q63] 开启事务
来源：http://qh.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pp.szxytkj.cn

[Q64] 提交事务
来源：http://yh.shtwfgs.cn

COMMIT;
来源：http://no.yuexingan06.cn

[Q65] 回滚事务
来源：http://kw.shxzskj.cn

ROLLBACK;
来源：http://yf.szsharing.cn

[Q66] 行锁查询
来源：http://qk.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vt.szxytkj.cn

[Q67] 设置隔离级别
来源：http://av.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bl.jctech888.com.cn

[Q68] 保存点
来源：http://xq.muxihuayi.cn

SAVEPOINT sp1;
来源：http://aa.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://pf.521024.cn

[Q69] 查看执行计划
来源：http://fz.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jd.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://wc.shtwfgs.cn

ANALYZE TABLE users;
来源：http://iz.colortex.cn

[Q71] 查看建表语句
来源：http://hx.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ni.bjjhwx.cn

[Q72] 查看索引
来源：http://od.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://fb.haigaiapp.cn

[Q73] 查看表状态
来源：http://la.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pd.haigaiapp.cn

[Q74] 强制使用索引
来源：http://fg.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wy.shxzukj.cn

[Q75] 日期格式化
来源：http://tf.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wj.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nb.huixiangedu.cn

[Q76] 按天统计
来源：http://ol.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xf.521024.cn

[Q77] 时间加减
来源：http://ko.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://id.nicolike.cn

[Q78] 当前时间
来源：http://qm.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://us.shxzukj.cn

[Q79] 字符串拼接
来源：http://ww.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tz.chemitech.net.cn

[Q80] 字符串截取
来源：http://ks.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xj.shtwfgs.cn

[Q81] 字符串替换
来源：http://kv.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yo.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://cf.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pd.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://rp.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bp.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://jz.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://vt.nszjky.cn

[Q85] 数值取整
来源：http://vy.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mr.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://be.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jv.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://ty.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xr.huanxung.cn

[Q88] 行转列（条件聚合）
来源：http://ou.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dd.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bp.colortex.cn

[Q89] 判断表是否存在
来源：http://gt.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gq.bookmarksfly.cn

[Q90] 生成序号列
来源：http://hk.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://of.lnxyls.cn

================================================================================
来源：http://wa.shxzskj.cn

R. Bash 专题
来源：http://cz.muxihuayi.cn

================================================================================
来源：http://xf.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://hn.colortex.cn

#!/usr/bin/env bash
来源：http://cy.hnjuh.cn

set -euo pipefail
来源：http://ub.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://ry.newstarts.cn

name="Tom"; echo "$name"
来源：http://mp.asd995.cn

[R03] 只读变量
来源：http://cx.nszjky.cn

readonly PI=3.14
来源：http://sp.muxihuayi.cn

[R04] 位置参数
来源：http://rs.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ww.panjiajie.cn

[R05] 参数默认值
来源：http://ze.huanxung.cn

name="${1:-default}"
来源：http://ud.newstarts.cn

[R06] 判断命令是否存在
来源：http://kq.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nz.muxihuayi.cn

[R07] if 判断文件
来源：http://ru.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://za.bookmarksfly.cn

[R08] 数值比较
来源：http://cb.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yd.gzmigu.cn

[R09] 字符串比较
来源：http://pq.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ht.wgjwhj.cn

[R10] 正则匹配
来源：http://ch.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://am.szsharing.cn

[R11] case 多分支
来源：http://zz.yuexingan06.cn

case "$1" in
来源：http://kk.szxytkj.cn

start) echo "启动" ;;
来源：http://pw.shxzskj.cn

stop)  echo "停止" ;;
来源：http://vo.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://bj.newstarts.cn

esac
来源：http://yt.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://kt.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://xt.newstarts.cn

[R13] for 计数循环
来源：http://ds.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://fq.chemitech.net.cn

[R14] C 风格 for
来源：http://dx.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qg.huixiangedu.cn

[R15] while 逐行读文件
来源：http://lt.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://to.huixiangedu.cn

[R16] until 等待条件
来源：http://iw.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ri.muxihuayi.cn

[R17] 数组定义与取值
来源：http://lk.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gr.newstarts.cn

[R18] 遍历数组
来源：http://zl.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gf.muxihuayi.cn

[R19] 数组长度
来源：http://mj.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://jc.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://za.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hk.shxzskj.cn

[R21] 字符串长度
来源：http://wt.shxzukj.cn

echo "${#s}"
来源：http://cs.panjiajie.cn

[R22] 截取子串
来源：http://er.hnjuh.cn

echo "${s:0:5}"
来源：http://sp.nicolike.cn

[R23] 字符串替换
来源：http://zq.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jb.jianghongdianzi.cn

[R24] 大小写转换
来源：http://hz.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://oj.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://uv.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://iy.yuexingan06.cn

[R26] 命令替换
来源：http://gq.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://wr.chemitech.net.cn

[R27] 算术展开
来源：http://km.9csxet.cn

echo $((1 + 2 * 3))
来源：http://af.asd995.cn

[R28] 浮点运算
来源：http://bg.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://yt.9csxet.cn

[R29] 定义函数
来源：http://kd.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://az.hnjuh.cn

[R30] 函数返回状态码
来源：http://ru.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://lf.gzmigu.cn

[R31] 局部变量
来源：http://ks.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://sd.asd995.cn

[R32] 参数个数校验
来源：http://gi.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gb.521024.cn

[R33] 捕获错误并提示行号
来源：http://ji.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zk.gzmigu.cn

[R34] 退出时清理
来源：http://ek.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uw.nszjky.cn

[R35] 后台执行并等待
来源：http://ff.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uc.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://aq.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ot.hnjuh.cn

[R37] 把输出赋给变量
来源：http://fi.yuexingan06.cn

files=$(ls -1)
来源：http://sd.nszjky.cn

[R38] 管道串联
来源：http://eo.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://xg.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://zf.gzmigu.cn

cmd > out.log 2>&1
来源：http://iq.jianghongdianzi.cn

[R40] 追加写日志
来源：http://xx.hahajie.cn

echo "log" >> out.log
来源：http://re.bjjhwx.cn

[R41] 丢弃输出
来源：http://dy.asd995.cn

cmd >/dev/null 2>&1
来源：http://yc.521024.cn

[R42] 输入重定向
来源：http://tq.yuntaijiaju.cn

wc -l < a.txt
来源：http://mv.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://qh.hnjuh.cn

find . -name "*.log" -type f
来源：http://fr.lnxyls.cn

[R44] 按修改时间查找
来源：http://hg.521024.cn

find . -mtime -7 -type f
来源：http://km.muxihuayi.cn

[R45] 批量删除
来源：http://dg.nicolike.cn


<!-- 参考信息 -->