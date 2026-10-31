代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dp.huanxung.cn

);
来源：http://ny.gzmigu.cn

[Q02] 创建带外键的表
来源：http://ro.szsharing.cn

CREATE TABLE orders (
来源：http://bl.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ze.lnxyls.cn

user_id INT NOT NULL,
来源：http://mu.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://eo.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yt.huixinmuqiang.cn

);
来源：http://ca.wgjwhj.cn

[Q03] 增加列
来源：http://hm.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hh.yuexingan06.cn

[Q04] 修改列类型
来源：http://vq.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lj.wgjwhj.cn

[Q05] 重命名列
来源：http://lf.nicolike.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zj.muxihuayi.cn

[Q06] 删除列
来源：http://yj.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rl.hnjuh.cn

[Q07] 删除表
来源：http://lb.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://ru.bjjhwx.cn

[Q08] 创建普通索引
来源：http://zm.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cs.muxihuayi.cn

[Q09] 创建唯一索引
来源：http://vt.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nd.panjiajie.cn

[Q10] 插入单行
来源：http://jn.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cj.yuexingan06.cn

[Q11] 一次插入多行
来源：http://ts.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jv.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://nh.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uq.nicolike.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zm.9csxet.cn

[Q13] 忽略重复插入
来源：http://vw.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ly.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://zy.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uo.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qf.shxzskj.cn

[Q15] 查询全部
来源：http://tu.asd995.cn

SELECT * FROM users;
来源：http://qd.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://ip.hahajie.cn

SELECT id, name FROM users;
来源：http://dg.colortex.cn

[Q17] 条件查询
来源：http://kr.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sh.huanxung.cn

[Q18] 模糊匹配
来源：http://gr.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fk.muxihuayi.cn

[Q19] 范围查询
来源：http://pg.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pm.shxzskj.cn

[Q20] IN 列表
来源：http://ky.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yx.huanxung.cn

[Q21] 空值判断
来源：http://tr.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hi.jianghongdianzi.cn

[Q22] 排序
来源：http://qi.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dz.hnjuh.cn

[Q23] 分页
来源：http://tv.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hj.yuexingan06.cn

[Q24] 去重
来源：http://ip.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://ik.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://px.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ot.wgjwhj.cn

[Q26] 计数
来源：http://cr.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://ur.lnxyls.cn

[Q27] 条件计数
来源：http://ab.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mx.huixiangedu.cn

[Q28] 求和与平均
来源：http://dr.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ke.shtwfgs.cn

[Q29] 最大最小值
来源：http://un.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ko.hahajie.cn

[Q30] 分组统计
来源：http://dk.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gy.521024.cn

[Q31] 分组后过滤
来源：http://xp.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pi.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://gw.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bt.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eq.muxihuayi.cn

[Q33] 多列分组
来源：http://af.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rj.nicolike.cn

[Q34] 每组取第一条
来源：http://wz.521024.cn

SELECT * FROM (
来源：http://mj.colortex.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ia.nicolike.cn

) t WHERE rn = 1;
来源：http://wk.newstarts.cn

[Q35] 内连接
来源：http://fk.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rv.colortex.cn

[Q36] 左连接
来源：http://vm.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dj.gzmigu.cn

[Q37] 右连接
来源：http://qx.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ea.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dx.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kv.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://vw.muxihuayi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ga.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jb.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gn.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ed.yuexingan06.cn

[Q41] 多表连接
来源：http://qt.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bj.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://hn.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://fx.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://fl.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://hp.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dn.szsharing.cn

[Q43] 标量子查询
来源：http://zq.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mj.szxytkj.cn

[Q44] IN 子查询
来源：http://ac.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wy.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://si.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sh.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jl.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sq.szxytkj.cn

[Q47] 与平均值比较
来源：http://ka.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eo.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://nt.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://en.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://vy.huixiangedu.cn

[Q49] 更新单行
来源：http://ki.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vk.huixiangedu.cn

[Q50] 批量更新
来源：http://gm.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tq.colortex.cn

[Q51] 用子查询更新
来源：http://yv.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xi.szxytkj.cn

[Q52] 删除指定行
来源：http://oh.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://pd.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://yp.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ku.newstarts.cn

[Q54] 清空表
来源：http://mt.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://lo.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://st.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cq.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://av.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qr.shxzskj.cn

[Q57] 行号
来源：http://ns.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://el.chemitech.net.cn

[Q58] 累计求和
来源：http://ze.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ya.shxzskj.cn

[Q59] 分组内累计
来源：http://he.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nt.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://cq.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uf.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pv.haigaiapp.cn

[Q61] 移动平均
来源：http://sy.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yy.huanxung.cn

[Q62] 分组占比
来源：http://rv.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://us.huanxung.cn

[Q63] 开启事务
来源：http://to.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nt.gzmigu.cn

[Q64] 提交事务
来源：http://qb.yuntaijiaju.cn

COMMIT;
来源：http://lc.bjjhwx.cn

[Q65] 回滚事务
来源：http://hd.hnjuh.cn

ROLLBACK;
来源：http://bd.hahajie.cn

[Q66] 行锁查询
来源：http://os.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xn.hahajie.cn

[Q67] 设置隔离级别
来源：http://sk.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://em.szsharing.cn

[Q68] 保存点
来源：http://cn.yuexingan06.cn

SAVEPOINT sp1;
来源：http://cu.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://qv.hnjuh.cn

[Q69] 查看执行计划
来源：http://hh.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kr.shtwfgs.cn

[Q70] 更新统计信息
来源：http://df.colortex.cn

ANALYZE TABLE users;
来源：http://va.jctech888.com.cn

[Q71] 查看建表语句
来源：http://wh.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jm.jctech888.com.cn

[Q72] 查看索引
来源：http://ln.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://el.lnxyls.cn

[Q73] 查看表状态
来源：http://qw.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pi.lnxyls.cn

[Q74] 强制使用索引
来源：http://vn.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ei.huixiangedu.cn

[Q75] 日期格式化
来源：http://sc.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wu.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sb.muxihuayi.cn

[Q76] 按天统计
来源：http://bs.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xs.yuexingan06.cn

[Q77] 时间加减
来源：http://iu.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bh.521024.cn

[Q78] 当前时间
来源：http://do.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vj.hahajie.cn

[Q79] 字符串拼接
来源：http://sl.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lx.wgjwhj.cn

[Q80] 字符串截取
来源：http://au.9csxet.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bf.haigaiapp.cn

[Q81] 字符串替换
来源：http://ob.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ht.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://xb.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fj.hahajie.cn

[Q83] 大小写转换
来源：http://vk.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nf.szxytkj.cn

[Q84] 去除首尾空格
来源：http://xi.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://iu.shxzskj.cn

[Q85] 数值取整
来源：http://ue.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wg.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://ir.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xv.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://ug.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bt.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://tc.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jq.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ds.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://xi.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xa.hnjuh.cn

[Q90] 生成序号列
来源：http://pj.jctech888.com.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dv.bjjhwx.cn

================================================================================
来源：http://hl.bjjhwx.cn

R. Bash 专题
来源：http://jd.szsharing.cn

================================================================================
来源：http://le.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://lw.jctech888.com.cn

#!/usr/bin/env bash
来源：http://rv.shtwfgs.cn

set -euo pipefail
来源：http://ze.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://pk.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://bm.newstarts.cn

[R03] 只读变量
来源：http://am.nszjky.cn

readonly PI=3.14
来源：http://vp.panjiajie.cn

[R04] 位置参数
来源：http://lh.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wa.newstarts.cn

[R05] 参数默认值
来源：http://co.shtwfgs.cn

name="${1:-default}"
来源：http://xs.lnxyls.cn

[R06] 判断命令是否存在
来源：http://eo.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://he.jctech888.com.cn

[R07] if 判断文件
来源：http://jz.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bo.nszjky.cn

[R08] 数值比较
来源：http://bh.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pg.hahajie.cn

[R09] 字符串比较
来源：http://ef.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hc.haigaiapp.cn

[R10] 正则匹配
来源：http://vf.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mr.hahajie.cn

[R11] case 多分支
来源：http://tc.szxytkj.cn

case "$1" in
来源：http://wh.wgjwhj.cn

start) echo "启动" ;;
来源：http://de.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://gm.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://qe.huanxung.cn

esac
来源：http://le.wgjwhj.cn

[R12] for 遍历文件
来源：http://ym.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://gv.yuntaijiaju.cn

[R13] for 计数循环
来源：http://xr.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://gu.yuexingan06.cn

[R14] C 风格 for
来源：http://ng.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pr.wgjwhj.cn

[R15] while 逐行读文件
来源：http://cj.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fe.yuexingan06.cn

[R16] until 等待条件
来源：http://qk.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ww.szxytkj.cn

[R17] 数组定义与取值
来源：http://fg.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wb.muxihuayi.cn

[R18] 遍历数组
来源：http://ng.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ek.jctech888.com.cn

[R19] 数组长度
来源：http://pc.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://sp.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://lw.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ck.hnjuh.cn

[R21] 字符串长度
来源：http://pb.yuexingan06.cn

echo "${#s}"
来源：http://qo.lnxyls.cn

[R22] 截取子串
来源：http://by.huanxung.cn

echo "${s:0:5}"
来源：http://kk.szxytkj.cn

[R23] 字符串替换
来源：http://ak.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pa.szsharing.cn

[R24] 大小写转换
来源：http://xr.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kl.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://vb.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qp.lnxyls.cn

[R26] 命令替换
来源：http://ml.521024.cn

now=$(date +%F); echo "$now"
来源：http://pq.jianghongdianzi.cn

[R27] 算术展开
来源：http://tk.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://vw.shxzukj.cn

[R28] 浮点运算
来源：http://uc.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://zk.hnjuh.cn

[R29] 定义函数
来源：http://rp.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ql.wgjwhj.cn

[R30] 函数返回状态码
来源：http://vz.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ns.chemitech.net.cn

[R31] 局部变量
来源：http://fj.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://hj.colortex.cn

[R32] 参数个数校验
来源：http://gj.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jx.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://yv.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fx.szsharing.cn

[R34] 退出时清理
来源：http://fq.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hp.shxzskj.cn

[R35] 后台执行并等待
来源：http://tc.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gj.panjiajie.cn

[R36] 并发执行多个任务
来源：http://if.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yo.huanxung.cn

[R37] 把输出赋给变量
来源：http://rk.521024.cn

files=$(ls -1)
来源：http://nm.lnxyls.cn

[R38] 管道串联
来源：http://qf.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://li.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://hv.wgjwhj.cn

cmd > out.log 2>&1
来源：http://ub.hnjuh.cn

[R40] 追加写日志
来源：http://ek.asd995.cn

echo "log" >> out.log
来源：http://rb.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://nl.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://sx.9csxet.cn

[R42] 输入重定向
来源：http://rs.huanxung.cn

wc -l < a.txt
来源：http://kw.wgjwhj.cn

[R43] 按名字查找文件
来源：http://sk.gzmigu.cn

find . -name "*.log" -type f
来源：http://zc.9csxet.cn

[R44] 按修改时间查找
来源：http://cv.9csxet.cn

find . -mtime -7 -type f
来源：http://pv.hnjuh.cn

[R45] 批量删除
来源：http://gb.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://ro.nszjky.cn

[R46] 递归替换文件内容
来源：http://ie.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tn.shxzukj.cn

[R47] sed 单行替换
来源：http://ng.hahajie.cn


<!-- 参考信息 -->