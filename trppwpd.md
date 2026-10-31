代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yy.521024.cn

);
来源：http://fe.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://sl.nicolike.cn

CREATE TABLE orders (
来源：http://js.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bm.muxihuayi.cn

user_id INT NOT NULL,
来源：http://cj.szsharing.cn

amount DECIMAL(10, 2),
来源：http://qe.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lm.jctech888.com.cn

);
来源：http://hx.huixiangedu.cn

[Q03] 增加列
来源：http://hc.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wo.hnjuh.cn

[Q04] 修改列类型
来源：http://ln.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kz.muxihuayi.cn

[Q05] 重命名列
来源：http://ss.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bv.bjjhwx.cn

[Q06] 删除列
来源：http://vm.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rn.huanxung.cn

[Q07] 删除表
来源：http://if.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://pp.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://em.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bo.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://qj.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qt.jianghongdianzi.cn

[Q10] 插入单行
来源：http://ep.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wg.gzmigu.cn

[Q11] 一次插入多行
来源：http://ql.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xd.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://fj.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yg.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://an.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://wt.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sb.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://wu.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://du.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nj.yuntaijiaju.cn

[Q15] 查询全部
来源：http://mt.yuexingan06.cn

SELECT * FROM users;
来源：http://ts.bjjhwx.cn

[Q16] 查询指定列
来源：http://kt.panjiajie.cn

SELECT id, name FROM users;
来源：http://es.yuntaijiaju.cn

[Q17] 条件查询
来源：http://ll.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ys.shxzukj.cn

[Q18] 模糊匹配
来源：http://qa.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sb.yuexingan06.cn

[Q19] 范围查询
来源：http://ai.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nv.jctech888.com.cn

[Q20] IN 列表
来源：http://hq.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fv.shtwfgs.cn

[Q21] 空值判断
来源：http://du.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rf.hahajie.cn

[Q22] 排序
来源：http://bt.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mb.nicolike.cn

[Q23] 分页
来源：http://yu.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dy.nszjky.cn

[Q24] 去重
来源：http://wz.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://iv.gzmigu.cn

[Q25] 只取前 N 条
来源：http://kk.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rz.shxzukj.cn

[Q26] 计数
来源：http://nh.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://nk.yuexingan06.cn

[Q27] 条件计数
来源：http://si.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ov.wgjwhj.cn

[Q28] 求和与平均
来源：http://pz.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wc.bookmarksfly.cn

[Q29] 最大最小值
来源：http://uz.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://au.newstarts.cn

[Q30] 分组统计
来源：http://vh.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bj.szxytkj.cn

[Q31] 分组后过滤
来源：http://qf.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zj.asd995.cn

[Q32] 分组拼接字符串
来源：http://jv.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://td.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ta.newstarts.cn

[Q33] 多列分组
来源：http://ta.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hx.nszjky.cn

[Q34] 每组取第一条
来源：http://dz.lnxyls.cn

SELECT * FROM (
来源：http://qi.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ll.521024.cn

) t WHERE rn = 1;
来源：http://kd.521024.cn

[Q35] 内连接
来源：http://gv.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fv.szxytkj.cn

[Q36] 左连接
来源：http://ny.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ik.colortex.cn

[Q37] 右连接
来源：http://un.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://as.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xp.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rr.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://qt.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rf.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qq.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wq.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rr.hnjuh.cn

[Q41] 多表连接
来源：http://yu.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hk.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://da.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://dp.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://jh.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://cx.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qt.colortex.cn

[Q43] 标量子查询
来源：http://pq.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qd.lnxyls.cn

[Q44] IN 子查询
来源：http://wd.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vb.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://wl.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vz.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://he.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ei.gzmigu.cn

[Q47] 与平均值比较
来源：http://dh.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xv.bjjhwx.cn

[Q48] CTE 公用表表达式
来源：http://nd.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ys.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://nd.nicolike.cn

[Q49] 更新单行
来源：http://vw.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cu.9csxet.cn

[Q50] 批量更新
来源：http://ka.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lz.haigaiapp.cn

[Q51] 用子查询更新
来源：http://pv.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sy.huanxung.cn

[Q52] 删除指定行
来源：http://rr.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://ja.muxihuayi.cn

[Q53] 按条件删除
来源：http://cv.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rk.chemitech.net.cn

[Q54] 清空表
来源：http://vb.nicolike.cn

TRUNCATE TABLE logs;
来源：http://ce.hahajie.cn

[Q55] 排名（并列占位）
来源：http://jx.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://le.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://le.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dk.huixiangedu.cn

[Q57] 行号
来源：http://fh.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gy.jctech888.com.cn

[Q58] 累计求和
来源：http://lu.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://af.521024.cn

[Q59] 分组内累计
来源：http://uq.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jc.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://bn.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kd.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.haigaiapp.cn

[Q61] 移动平均
来源：http://yf.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ub.nszjky.cn

[Q62] 分组占比
来源：http://uq.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ln.hnjuh.cn

[Q63] 开启事务
来源：http://te.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ql.bjjhwx.cn

[Q64] 提交事务
来源：http://xv.jctech888.com.cn

COMMIT;
来源：http://pz.newstarts.cn

[Q65] 回滚事务
来源：http://tg.nicolike.cn

ROLLBACK;
来源：http://xo.shxzukj.cn

[Q66] 行锁查询
来源：http://gb.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bx.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://jg.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sp.huanxung.cn

[Q68] 保存点
来源：http://gi.521024.cn

SAVEPOINT sp1;
来源：http://ij.colortex.cn

ROLLBACK TO sp1;
来源：http://rm.nszjky.cn

[Q69] 查看执行计划
来源：http://tg.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://aw.muxihuayi.cn

[Q70] 更新统计信息
来源：http://rr.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://zb.huixiangedu.cn

[Q71] 查看建表语句
来源：http://sv.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ns.hnjuh.cn

[Q72] 查看索引
来源：http://xi.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://ct.huanxung.cn

[Q73] 查看表状态
来源：http://jm.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oe.nicolike.cn

[Q74] 强制使用索引
来源：http://bu.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://db.shxzukj.cn

[Q75] 日期格式化
来源：http://qw.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ge.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pn.hahajie.cn

[Q76] 按天统计
来源：http://dy.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zh.jianghongdianzi.cn

[Q77] 时间加减
来源：http://yf.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sh.panjiajie.cn

[Q78] 当前时间
来源：http://gk.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://px.hnjuh.cn

[Q79] 字符串拼接
来源：http://xz.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nq.9csxet.cn

[Q80] 字符串截取
来源：http://ll.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sj.gzmigu.cn

[Q81] 字符串替换
来源：http://jm.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zr.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://pj.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mo.shxzukj.cn

[Q83] 大小写转换
来源：http://ph.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vl.hahajie.cn

[Q84] 去除首尾空格
来源：http://aa.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://sw.asd995.cn

[Q85] 数值取整
来源：http://mo.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ym.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://qm.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://os.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://vx.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fn.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://wd.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ir.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mc.lnxyls.cn

[Q89] 判断表是否存在
来源：http://ts.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ir.nicolike.cn

[Q90] 生成序号列
来源：http://ep.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ly.jctech888.com.cn

================================================================================
来源：http://oc.gzmigu.cn

R. Bash 专题
来源：http://sq.hahajie.cn

================================================================================
来源：http://jp.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://is.szsharing.cn

#!/usr/bin/env bash
来源：http://yg.nszjky.cn

set -euo pipefail
来源：http://ba.hnjuh.cn

[R02] 变量赋值与使用
来源：http://mv.nszjky.cn

name="Tom"; echo "$name"
来源：http://np.huanxung.cn

[R03] 只读变量
来源：http://du.huixinmuqiang.cn

readonly PI=3.14
来源：http://lp.szsharing.cn

[R04] 位置参数
来源：http://uw.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wt.bjjhwx.cn

[R05] 参数默认值
来源：http://fw.lnxyls.cn

name="${1:-default}"
来源：http://kb.521024.cn

[R06] 判断命令是否存在
来源：http://rp.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cc.wgjwhj.cn

[R07] if 判断文件
来源：http://yx.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fw.bookmarksfly.cn

[R08] 数值比较
来源：http://xb.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pe.shxzskj.cn

[R09] 字符串比较
来源：http://ty.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uf.szsharing.cn

[R10] 正则匹配
来源：http://zk.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fi.szsharing.cn

[R11] case 多分支
来源：http://gf.colortex.cn

case "$1" in
来源：http://kf.huixiangedu.cn

start) echo "启动" ;;
来源：http://bd.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://bt.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://ah.chemitech.net.cn

esac
来源：http://wx.gzmigu.cn

[R12] for 遍历文件
来源：http://cy.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://li.nszjky.cn

[R13] for 计数循环
来源：http://lb.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://rt.szsharing.cn

[R14] C 风格 for
来源：http://ao.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rf.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://zh.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mm.szxytkj.cn

[R16] until 等待条件
来源：http://uu.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ke.lnxyls.cn

[R17] 数组定义与取值
来源：http://vc.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vz.nszjky.cn

[R18] 遍历数组
来源：http://ia.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ni.muxihuayi.cn

[R19] 数组长度
来源：http://dn.9csxet.cn

echo "${#arr[@]}"
来源：http://yz.szsharing.cn

[R20] 关联数组（字典）
来源：http://lg.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://op.szxytkj.cn

[R21] 字符串长度
来源：http://wg.9csxet.cn

echo "${#s}"
来源：http://we.yuexingan06.cn

[R22] 截取子串
来源：http://mq.chemitech.net.cn

echo "${s:0:5}"
来源：http://cr.bjjhwx.cn

[R23] 字符串替换
来源：http://or.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hs.hnjuh.cn

[R24] 大小写转换
来源：http://cl.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bc.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://cf.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://do.huixiangedu.cn

[R26] 命令替换
来源：http://gm.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://tp.hahajie.cn

[R27] 算术展开
来源：http://rb.colortex.cn

echo $((1 + 2 * 3))
来源：http://av.huixiangedu.cn

[R28] 浮点运算
来源：http://ur.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://mn.hnjuh.cn

[R29] 定义函数
来源：http://ek.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xb.haigaiapp.cn

[R30] 函数返回状态码
来源：http://iw.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://si.jctech888.com.cn

[R31] 局部变量
来源：http://od.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://jr.nszjky.cn

[R32] 参数个数校验
来源：http://ru.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zt.521024.cn

[R33] 捕获错误并提示行号
来源：http://gf.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ar.asd995.cn

[R34] 退出时清理
来源：http://vk.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nd.nszjky.cn

[R35] 后台执行并等待
来源：http://eg.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ov.szsharing.cn

[R36] 并发执行多个任务
来源：http://jz.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lm.shxzskj.cn

[R37] 把输出赋给变量
来源：http://xa.shxzukj.cn

files=$(ls -1)
来源：http://us.wgjwhj.cn

[R38] 管道串联
来源：http://gm.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://oe.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://vc.yuexingan06.cn

cmd > out.log 2>&1
来源：http://fz.huanxung.cn

[R40] 追加写日志
来源：http://tr.huixinmuqiang.cn

echo "log" >> out.log
来源：http://aq.colortex.cn

[R41] 丢弃输出
来源：http://qc.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://cn.haigaiapp.cn

[R42] 输入重定向
来源：http://gn.panjiajie.cn

wc -l < a.txt
来源：http://ib.panjiajie.cn

[R43] 按名字查找文件
来源：http://to.shtwfgs.cn

find . -name "*.log" -type f
来源：http://fm.szxytkj.cn

[R44] 按修改时间查找
来源：http://pq.hnjuh.cn

find . -mtime -7 -type f
来源：http://gz.huixiangedu.cn

[R45] 批量删除
来源：http://mz.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://iz.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://lt.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pw.lnxyls.cn

[R47] sed 单行替换
来源：http://mg.yuexingan06.cn


<!-- 参考信息 -->