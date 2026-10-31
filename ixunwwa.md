代发 wailian999

CREATE TABLE users (
来源：http://sf.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ki.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://wj.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://sx.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fr.wgjwhj.cn

);
来源：http://fj.panjiajie.cn

[Q02] 创建带外键的表
来源：http://cx.bjjhwx.cn

CREATE TABLE orders (
来源：http://fs.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wa.shxzukj.cn

user_id INT NOT NULL,
来源：http://lm.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://yv.yuntaijiaju.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jw.wgjwhj.cn

);
来源：http://jn.521024.cn

[Q03] 增加列
来源：http://xp.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ok.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://os.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lu.szxytkj.cn

[Q05] 重命名列
来源：http://uz.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sa.nicolike.cn

[Q06] 删除列
来源：http://jl.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://es.jianghongdianzi.cn

[Q07] 删除表
来源：http://je.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://dp.newstarts.cn

[Q08] 创建普通索引
来源：http://yd.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://en.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://nn.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pd.jianghongdianzi.cn

[Q10] 插入单行
来源：http://xl.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mg.lnxyls.cn

[Q11] 一次插入多行
来源：http://ab.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bf.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://vg.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ch.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mg.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://zs.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ym.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://rn.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vi.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bm.bookmarksfly.cn

[Q15] 查询全部
来源：http://ph.szsharing.cn

SELECT * FROM users;
来源：http://wn.huixiangedu.cn

[Q16] 查询指定列
来源：http://sk.lnxyls.cn

SELECT id, name FROM users;
来源：http://kl.yuntaijiaju.cn

[Q17] 条件查询
来源：http://gh.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fw.yuexingan06.cn

[Q18] 模糊匹配
来源：http://pf.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ou.nszjky.cn

[Q19] 范围查询
来源：http://jx.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cg.nicolike.cn

[Q20] IN 列表
来源：http://is.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tl.shxzukj.cn

[Q21] 空值判断
来源：http://cs.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cc.yuexingan06.cn

[Q22] 排序
来源：http://lp.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vf.wgjwhj.cn

[Q23] 分页
来源：http://rl.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ga.newstarts.cn

[Q24] 去重
来源：http://hj.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://gr.9csxet.cn

[Q25] 只取前 N 条
来源：http://lo.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ic.shtwfgs.cn

[Q26] 计数
来源：http://ct.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://ql.colortex.cn

[Q27] 条件计数
来源：http://iy.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yq.hahajie.cn

[Q28] 求和与平均
来源：http://mq.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hs.521024.cn

[Q29] 最大最小值
来源：http://bu.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zt.shxzskj.cn

[Q30] 分组统计
来源：http://oc.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://az.haigaiapp.cn

[Q31] 分组后过滤
来源：http://qs.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ji.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://kt.haigaiapp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cc.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ww.yuexingan06.cn

[Q33] 多列分组
来源：http://ck.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zw.huanxung.cn

[Q34] 每组取第一条
来源：http://rg.yuntaijiaju.cn

SELECT * FROM (
来源：http://xp.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ey.shxzukj.cn

) t WHERE rn = 1;
来源：http://ly.bookmarksfly.cn

[Q35] 内连接
来源：http://sg.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qi.huixiangedu.cn

[Q36] 左连接
来源：http://fa.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hd.shtwfgs.cn

[Q37] 右连接
来源：http://hf.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qi.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ph.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lu.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://cv.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://es.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dt.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ib.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cq.szxytkj.cn

[Q41] 多表连接
来源：http://vr.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bg.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://ub.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://wm.521024.cn

[Q42] 连接条件附加过滤
来源：http://uf.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://pz.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kq.521024.cn

[Q43] 标量子查询
来源：http://pb.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vq.521024.cn

[Q44] IN 子查询
来源：http://du.lnxyls.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nt.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://nq.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hl.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ps.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://he.hahajie.cn

[Q47] 与平均值比较
来源：http://xb.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://li.asd995.cn

[Q48] CTE 公用表表达式
来源：http://kg.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mj.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://cl.huixinmuqiang.cn

[Q49] 更新单行
来源：http://yn.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://es.chemitech.net.cn

[Q50] 批量更新
来源：http://yt.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qt.gzmigu.cn

[Q51] 用子查询更新
来源：http://bo.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://om.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://vy.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://an.lnxyls.cn

[Q53] 按条件删除
来源：http://rw.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://li.panjiajie.cn

[Q54] 清空表
来源：http://dg.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://up.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://hu.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xq.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://ex.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fb.chemitech.net.cn

[Q57] 行号
来源：http://qr.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kq.521024.cn

[Q58] 累计求和
来源：http://br.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yn.szsharing.cn

[Q59] 分组内累计
来源：http://hq.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dw.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://qc.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kt.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qw.lnxyls.cn

[Q61] 移动平均
来源：http://nb.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bo.muxihuayi.cn

[Q62] 分组占比
来源：http://op.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kh.hahajie.cn

[Q63] 开启事务
来源：http://ip.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://os.huixiangedu.cn

[Q64] 提交事务
来源：http://rr.521024.cn

COMMIT;
来源：http://tc.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://cn.shxzukj.cn

ROLLBACK;
来源：http://ke.gzmigu.cn

[Q66] 行锁查询
来源：http://lg.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mp.lnxyls.cn

[Q67] 设置隔离级别
来源：http://pv.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vl.nszjky.cn

[Q68] 保存点
来源：http://vx.jctech888.com.cn

SAVEPOINT sp1;
来源：http://rd.colortex.cn

ROLLBACK TO sp1;
来源：http://dq.521024.cn

[Q69] 查看执行计划
来源：http://bm.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yv.shxzskj.cn

[Q70] 更新统计信息
来源：http://wj.yuexingan06.cn

ANALYZE TABLE users;
来源：http://ed.newstarts.cn

[Q71] 查看建表语句
来源：http://zh.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nu.shxzskj.cn

[Q72] 查看索引
来源：http://jr.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://gy.panjiajie.cn

[Q73] 查看表状态
来源：http://kp.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xu.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://am.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cp.szxytkj.cn

[Q75] 日期格式化
来源：http://ii.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xk.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nc.nszjky.cn

[Q76] 按天统计
来源：http://ns.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sa.shtwfgs.cn

[Q77] 时间加减
来源：http://ko.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jp.521024.cn

[Q78] 当前时间
来源：http://ia.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kj.chemitech.net.cn

[Q79] 字符串拼接
来源：http://tp.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qe.gzmigu.cn

[Q80] 字符串截取
来源：http://kw.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pe.wgjwhj.cn

[Q81] 字符串替换
来源：http://dn.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mc.521024.cn

[Q82] 字符长度与字节长度
来源：http://nt.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://px.nicolike.cn

[Q83] 大小写转换
来源：http://db.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qv.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://je.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://ld.wgjwhj.cn

[Q85] 数值取整
来源：http://hl.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pn.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://ga.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://co.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://bl.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wc.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://te.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bq.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hu.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://tp.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xv.gzmigu.cn

[Q90] 生成序号列
来源：http://uu.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vs.hnjuh.cn

================================================================================
来源：http://oj.newstarts.cn

R. Bash 专题
来源：http://wz.muxihuayi.cn

================================================================================
来源：http://fh.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://mx.nicolike.cn

#!/usr/bin/env bash
来源：http://ww.nicolike.cn

set -euo pipefail
来源：http://av.szxytkj.cn

[R02] 变量赋值与使用
来源：http://lk.shxzskj.cn

name="Tom"; echo "$name"
来源：http://gi.huixiangedu.cn

[R03] 只读变量
来源：http://qk.9csxet.cn

readonly PI=3.14
来源：http://bo.huixiangedu.cn

[R04] 位置参数
来源：http://ag.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bf.huixinmuqiang.cn

[R05] 参数默认值
来源：http://rv.shtwfgs.cn

name="${1:-default}"
来源：http://kp.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://pn.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pr.wgjwhj.cn

[R07] if 判断文件
来源：http://dz.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vi.shxzukj.cn

[R08] 数值比较
来源：http://tj.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ir.huanxung.cn

[R09] 字符串比较
来源：http://oi.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dx.lnxyls.cn

[R10] 正则匹配
来源：http://hg.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cd.newstarts.cn

[R11] case 多分支
来源：http://cp.shtwfgs.cn

case "$1" in
来源：http://rn.hnjuh.cn

start) echo "启动" ;;
来源：http://iv.hnjuh.cn

stop)  echo "停止" ;;
来源：http://wi.huanxung.cn

*)     echo "未知命令" ;;
来源：http://lj.nszjky.cn

esac
来源：http://tr.wgjwhj.cn

[R12] for 遍历文件
来源：http://dv.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://ue.nszjky.cn

[R13] for 计数循环
来源：http://fb.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://bu.yuexingan06.cn

[R14] C 风格 for
来源：http://st.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://db.asd995.cn

[R15] while 逐行读文件
来源：http://gd.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dk.shxzukj.cn

[R16] until 等待条件
来源：http://jy.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vn.nicolike.cn

[R17] 数组定义与取值
来源：http://rm.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wa.huixinmuqiang.cn

[R18] 遍历数组
来源：http://ts.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fl.asd995.cn

[R19] 数组长度
来源：http://fm.shxzskj.cn

echo "${#arr[@]}"
来源：http://xx.shxzskj.cn

[R20] 关联数组（字典）
来源：http://zg.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uc.huanxung.cn

[R21] 字符串长度
来源：http://sk.szsharing.cn

echo "${#s}"
来源：http://oz.newstarts.cn

[R22] 截取子串
来源：http://io.haigaiapp.cn

echo "${s:0:5}"
来源：http://dr.huixinmuqiang.cn

[R23] 字符串替换
来源：http://lb.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jz.panjiajie.cn

[R24] 大小写转换
来源：http://gw.nszjky.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pv.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://fq.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cp.9csxet.cn

[R26] 命令替换
来源：http://tc.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://aa.muxihuayi.cn

[R27] 算术展开
来源：http://yc.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://id.szxytkj.cn

[R28] 浮点运算
来源：http://kv.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://iv.shxzskj.cn

[R29] 定义函数
来源：http://md.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qd.hahajie.cn

[R30] 函数返回状态码
来源：http://yc.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://cd.yuexingan06.cn

[R31] 局部变量
来源：http://at.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://mr.shtwfgs.cn

[R32] 参数个数校验
来源：http://ja.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mn.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://ar.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lb.szxytkj.cn

[R34] 退出时清理
来源：http://ro.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fk.shxzukj.cn

[R35] 后台执行并等待
来源：http://wh.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hx.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://qp.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lz.asd995.cn

[R37] 把输出赋给变量
来源：http://ki.muxihuayi.cn

files=$(ls -1)
来源：http://zc.huixiangedu.cn

[R38] 管道串联
来源：http://oo.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://sy.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://rl.yuexingan06.cn

cmd > out.log 2>&1
来源：http://rk.hahajie.cn

[R40] 追加写日志
来源：http://sl.chemitech.net.cn

echo "log" >> out.log
来源：http://zo.jctech888.com.cn

[R41] 丢弃输出
来源：http://ua.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://ag.bookmarksfly.cn

[R42] 输入重定向
来源：http://nq.szxytkj.cn

wc -l < a.txt
来源：http://js.wgjwhj.cn

[R43] 按名字查找文件
来源：http://tf.asd995.cn

find . -name "*.log" -type f
来源：http://rr.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://uc.shtwfgs.cn

find . -mtime -7 -type f
来源：http://kh.huanxung.cn

[R45] 批量删除
来源：http://oy.nicolike.cn


<!-- 参考信息 -->