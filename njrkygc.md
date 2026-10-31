代发 wailian999

CREATE TABLE users (
来源：http://bw.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xx.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://in.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://cs.jctech888.com.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pn.newstarts.cn

);
来源：http://qu.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://vy.huixiangedu.cn

CREATE TABLE orders (
来源：http://tt.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://td.shtwfgs.cn

user_id INT NOT NULL,
来源：http://gl.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://ou.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://al.haigaiapp.cn

);
来源：http://bk.hnjuh.cn

[Q03] 增加列
来源：http://yk.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mc.gzmigu.cn

[Q04] 修改列类型
来源：http://kz.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gt.lnxyls.cn

[Q05] 重命名列
来源：http://hz.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lk.wgjwhj.cn

[Q06] 删除列
来源：http://mb.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://db.shxzukj.cn

[Q07] 删除表
来源：http://dz.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://fl.chemitech.net.cn

[Q08] 创建普通索引
来源：http://qs.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nc.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://xz.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ob.hnjuh.cn

[Q10] 插入单行
来源：http://tm.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://na.shxzskj.cn

[Q11] 一次插入多行
来源：http://jh.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qf.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://bn.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sy.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uo.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://kc.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wk.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://na.panjiajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zg.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pv.panjiajie.cn

[Q15] 查询全部
来源：http://fa.nszjky.cn

SELECT * FROM users;
来源：http://hp.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://ll.haigaiapp.cn

SELECT id, name FROM users;
来源：http://sb.bookmarksfly.cn

[Q17] 条件查询
来源：http://ie.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ul.wgjwhj.cn

[Q18] 模糊匹配
来源：http://ei.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gf.9csxet.cn

[Q19] 范围查询
来源：http://vq.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lm.szsharing.cn

[Q20] IN 列表
来源：http://pg.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ck.asd995.cn

[Q21] 空值判断
来源：http://tk.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lp.szsharing.cn

[Q22] 排序
来源：http://jm.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fl.szsharing.cn

[Q23] 分页
来源：http://pq.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vv.muxihuayi.cn

[Q24] 去重
来源：http://lb.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://wy.asd995.cn

[Q25] 只取前 N 条
来源：http://qa.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pm.jctech888.com.cn

[Q26] 计数
来源：http://jq.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://co.521024.cn

[Q27] 条件计数
来源：http://rq.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fd.chemitech.net.cn

[Q28] 求和与平均
来源：http://il.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cu.nszjky.cn

[Q29] 最大最小值
来源：http://zs.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oi.szsharing.cn

[Q30] 分组统计
来源：http://bv.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ay.chemitech.net.cn

[Q31] 分组后过滤
来源：http://gc.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sc.hahajie.cn

[Q32] 分组拼接字符串
来源：http://fp.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ec.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mu.nszjky.cn

[Q33] 多列分组
来源：http://ty.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yn.newstarts.cn

[Q34] 每组取第一条
来源：http://vm.muxihuayi.cn

SELECT * FROM (
来源：http://ea.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gw.colortex.cn

) t WHERE rn = 1;
来源：http://rt.yuexingan06.cn

[Q35] 内连接
来源：http://yb.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jl.nszjky.cn

[Q36] 左连接
来源：http://sp.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rl.yuntaijiaju.cn

[Q37] 右连接
来源：http://zq.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gr.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vn.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iy.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://nm.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://il.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lc.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tp.huixinmuqiang.cn

[Q41] 多表连接
来源：http://vr.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cx.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://ya.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://hy.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://wu.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://sv.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://re.huanxung.cn

[Q43] 标量子查询
来源：http://dp.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ui.bjjhwx.cn

[Q44] IN 子查询
来源：http://ps.bjjhwx.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://of.colortex.cn

[Q45] EXISTS 判断存在
来源：http://fr.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ef.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cm.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://px.shxzukj.cn

[Q47] 与平均值比较
来源：http://bs.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xk.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://ax.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zv.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://xl.newstarts.cn

[Q49] 更新单行
来源：http://wj.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xk.bookmarksfly.cn

[Q50] 批量更新
来源：http://nw.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lt.bjjhwx.cn

[Q51] 用子查询更新
来源：http://gz.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rc.hnjuh.cn

[Q52] 删除指定行
来源：http://jm.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://gc.521024.cn

[Q53] 按条件删除
来源：http://ut.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pq.yuexingan06.cn

[Q54] 清空表
来源：http://al.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://no.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://is.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wx.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://bl.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://li.panjiajie.cn

[Q57] 行号
来源：http://iz.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://np.521024.cn

[Q58] 累计求和
来源：http://cf.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xn.shtwfgs.cn

[Q59] 分组内累计
来源：http://ja.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pr.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://ox.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://og.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fg.nszjky.cn

[Q61] 移动平均
来源：http://ls.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pm.shxzukj.cn

[Q62] 分组占比
来源：http://so.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zq.szsharing.cn

[Q63] 开启事务
来源：http://mr.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cy.wgjwhj.cn

[Q64] 提交事务
来源：http://hh.yuexingan06.cn

COMMIT;
来源：http://ee.muxihuayi.cn

[Q65] 回滚事务
来源：http://sd.jctech888.com.cn

ROLLBACK;
来源：http://bw.huanxung.cn

[Q66] 行锁查询
来源：http://up.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yr.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://vu.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://id.haigaiapp.cn

[Q68] 保存点
来源：http://kn.asd995.cn

SAVEPOINT sp1;
来源：http://lr.9csxet.cn

ROLLBACK TO sp1;
来源：http://by.yuexingan06.cn

[Q69] 查看执行计划
来源：http://li.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://te.lnxyls.cn

[Q70] 更新统计信息
来源：http://cq.muxihuayi.cn

ANALYZE TABLE users;
来源：http://qa.shxzukj.cn

[Q71] 查看建表语句
来源：http://pw.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uq.gzmigu.cn

[Q72] 查看索引
来源：http://rf.nicolike.cn

SHOW INDEX FROM users;
来源：http://hx.yuexingan06.cn

[Q73] 查看表状态
来源：http://yx.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wa.haigaiapp.cn

[Q74] 强制使用索引
来源：http://su.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ou.bjjhwx.cn

[Q75] 日期格式化
来源：http://ud.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jc.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gp.jianghongdianzi.cn

[Q76] 按天统计
来源：http://ew.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bl.jctech888.com.cn

[Q77] 时间加减
来源：http://yt.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ra.shxzukj.cn

[Q78] 当前时间
来源：http://go.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eq.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://rp.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wt.huanxung.cn

[Q80] 字符串截取
来源：http://ie.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rr.haigaiapp.cn

[Q81] 字符串替换
来源：http://io.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ny.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://hd.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ia.wgjwhj.cn

[Q83] 大小写转换
来源：http://gt.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bk.szxytkj.cn

[Q84] 去除首尾空格
来源：http://gh.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://pd.jianghongdianzi.cn

[Q85] 数值取整
来源：http://os.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mm.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://pw.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jj.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://yw.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gd.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://mi.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yu.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ry.szxytkj.cn

[Q89] 判断表是否存在
来源：http://kk.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hj.hnjuh.cn

[Q90] 生成序号列
来源：http://nl.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://or.szsharing.cn

================================================================================
来源：http://rf.yuntaijiaju.cn

R. Bash 专题
来源：http://ii.huanxung.cn

================================================================================
来源：http://ma.szxytkj.cn

[R01] shebang 与严格模式
来源：http://wg.gzmigu.cn

#!/usr/bin/env bash
来源：http://lp.yuexingan06.cn

set -euo pipefail
来源：http://zj.szsharing.cn

[R02] 变量赋值与使用
来源：http://fe.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://pb.jianghongdianzi.cn

[R03] 只读变量
来源：http://ia.newstarts.cn

readonly PI=3.14
来源：http://zp.lnxyls.cn

[R04] 位置参数
来源：http://ra.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iq.9csxet.cn

[R05] 参数默认值
来源：http://jf.shtwfgs.cn

name="${1:-default}"
来源：http://eg.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://ra.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pa.nszjky.cn

[R07] if 判断文件
来源：http://dx.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bv.huanxung.cn

[R08] 数值比较
来源：http://cr.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://op.wgjwhj.cn

[R09] 字符串比较
来源：http://xa.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bc.huanxung.cn

[R10] 正则匹配
来源：http://wm.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bh.huixinmuqiang.cn

[R11] case 多分支
来源：http://ar.jianghongdianzi.cn

case "$1" in
来源：http://ag.chemitech.net.cn

start) echo "启动" ;;
来源：http://up.gzmigu.cn

stop)  echo "停止" ;;
来源：http://vh.szsharing.cn

*)     echo "未知命令" ;;
来源：http://ew.521024.cn

esac
来源：http://nr.lnxyls.cn

[R12] for 遍历文件
来源：http://jq.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://gm.nicolike.cn

[R13] for 计数循环
来源：http://bm.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://gb.nicolike.cn

[R14] C 风格 for
来源：http://an.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ap.panjiajie.cn

[R15] while 逐行读文件
来源：http://jq.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gm.jctech888.com.cn

[R16] until 等待条件
来源：http://dc.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pb.panjiajie.cn

[R17] 数组定义与取值
来源：http://pd.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uc.bjjhwx.cn

[R18] 遍历数组
来源：http://ow.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wg.szsharing.cn

[R19] 数组长度
来源：http://ps.lnxyls.cn

echo "${#arr[@]}"
来源：http://uv.nicolike.cn

[R20] 关联数组（字典）
来源：http://tw.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kh.yuntaijiaju.cn

[R21] 字符串长度
来源：http://ii.shxzukj.cn

echo "${#s}"
来源：http://kq.hahajie.cn

[R22] 截取子串
来源：http://mp.muxihuayi.cn

echo "${s:0:5}"
来源：http://ap.jianghongdianzi.cn

[R23] 字符串替换
来源：http://uj.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rp.hnjuh.cn

[R24] 大小写转换
来源：http://kh.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pk.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://vd.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mp.huixiangedu.cn

[R26] 命令替换
来源：http://ls.521024.cn

now=$(date +%F); echo "$now"
来源：http://tr.shxzukj.cn

[R27] 算术展开
来源：http://ak.9csxet.cn

echo $((1 + 2 * 3))
来源：http://jx.bookmarksfly.cn

[R28] 浮点运算
来源：http://ec.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://vj.bookmarksfly.cn

[R29] 定义函数
来源：http://lu.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sf.gzmigu.cn

[R30] 函数返回状态码
来源：http://br.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://cb.szxytkj.cn

[R31] 局部变量
来源：http://ab.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://kx.colortex.cn

[R32] 参数个数校验
来源：http://zf.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xa.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://yf.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zq.huixiangedu.cn

[R34] 退出时清理
来源：http://uw.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xv.521024.cn

[R35] 后台执行并等待
来源：http://vi.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iv.nszjky.cn

[R36] 并发执行多个任务
来源：http://lu.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gj.shxzukj.cn

[R37] 把输出赋给变量
来源：http://gl.szsharing.cn

files=$(ls -1)
来源：http://wf.jctech888.com.cn

[R38] 管道串联
来源：http://hh.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://kq.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://gv.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://ek.colortex.cn

[R40] 追加写日志
来源：http://jq.asd995.cn

echo "log" >> out.log
来源：http://vt.szsharing.cn

[R41] 丢弃输出
来源：http://db.szsharing.cn

cmd >/dev/null 2>&1
来源：http://bj.muxihuayi.cn

[R42] 输入重定向
来源：http://qq.bjjhwx.cn

wc -l < a.txt
来源：http://mj.szsharing.cn

[R43] 按名字查找文件
来源：http://ec.szxytkj.cn

find . -name "*.log" -type f
来源：http://ea.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://ck.chemitech.net.cn

find . -mtime -7 -type f
来源：http://md.colortex.cn

[R45] 批量删除
来源：http://ih.huixinmuqiang.cn


<!-- 参考信息 -->