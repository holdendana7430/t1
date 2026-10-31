代发 wailian999

CREATE TABLE users (
来源：http://ms.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lw.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://pw.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://rh.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jv.szsharing.cn

);
来源：http://ch.hnjuh.cn

[Q02] 创建带外键的表
来源：http://li.asd995.cn

CREATE TABLE orders (
来源：http://lq.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ss.newstarts.cn

user_id INT NOT NULL,
来源：http://ni.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://py.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dt.huanxung.cn

);
来源：http://ex.lnxyls.cn

[Q03] 增加列
来源：http://mq.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hl.szsharing.cn

[Q04] 修改列类型
来源：http://ey.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tj.521024.cn

[Q05] 重命名列
来源：http://vv.nicolike.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yk.nicolike.cn

[Q06] 删除列
来源：http://kk.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://oq.hahajie.cn

[Q07] 删除表
来源：http://ls.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://fm.szsharing.cn

[Q08] 创建普通索引
来源：http://om.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tw.muxihuayi.cn

[Q09] 创建唯一索引
来源：http://vd.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://os.szsharing.cn

[Q10] 插入单行
来源：http://pc.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://za.haigaiapp.cn

[Q11] 一次插入多行
来源：http://xr.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bj.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://iu.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rd.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dh.hahajie.cn

[Q13] 忽略重复插入
来源：http://ge.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ax.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://gi.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zt.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xd.bjjhwx.cn

[Q15] 查询全部
来源：http://so.shxzskj.cn

SELECT * FROM users;
来源：http://xk.gzmigu.cn

[Q16] 查询指定列
来源：http://so.wgjwhj.cn

SELECT id, name FROM users;
来源：http://oy.nszjky.cn

[Q17] 条件查询
来源：http://dz.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wj.asd995.cn

[Q18] 模糊匹配
来源：http://oj.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pk.panjiajie.cn

[Q19] 范围查询
来源：http://ku.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tc.nszjky.cn

[Q20] IN 列表
来源：http://sw.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tf.panjiajie.cn

[Q21] 空值判断
来源：http://jn.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hs.bookmarksfly.cn

[Q22] 排序
来源：http://tr.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gu.newstarts.cn

[Q23] 分页
来源：http://kv.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ks.newstarts.cn

[Q24] 去重
来源：http://ee.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://bc.lnxyls.cn

[Q25] 只取前 N 条
来源：http://yb.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xz.shtwfgs.cn

[Q26] 计数
来源：http://sv.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://jx.szsharing.cn

[Q27] 条件计数
来源：http://ig.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jr.521024.cn

[Q28] 求和与平均
来源：http://ay.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gs.chemitech.net.cn

[Q29] 最大最小值
来源：http://rv.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://us.colortex.cn

[Q30] 分组统计
来源：http://dm.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fo.newstarts.cn

[Q31] 分组后过滤
来源：http://jc.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yf.9csxet.cn

[Q32] 分组拼接字符串
来源：http://ff.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ac.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nm.nicolike.cn

[Q33] 多列分组
来源：http://ui.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tc.szsharing.cn

[Q34] 每组取第一条
来源：http://mo.shxzskj.cn

SELECT * FROM (
来源：http://qz.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://le.bjjhwx.cn

) t WHERE rn = 1;
来源：http://qi.jctech888.com.cn

[Q35] 内连接
来源：http://yq.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://te.huixiangedu.cn

[Q36] 左连接
来源：http://yk.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eo.nszjky.cn

[Q37] 右连接
来源：http://eq.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pk.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cl.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aj.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://ij.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bq.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hc.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lx.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://se.yuntaijiaju.cn

[Q41] 多表连接
来源：http://qa.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fs.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://ve.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://by.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://ph.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://dz.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lk.9csxet.cn

[Q43] 标量子查询
来源：http://kv.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zt.shxzskj.cn

[Q44] IN 子查询
来源：http://tf.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ks.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://ut.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iz.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gs.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mz.jctech888.com.cn

[Q47] 与平均值比较
来源：http://br.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vt.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://al.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ui.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://eg.huixinmuqiang.cn

[Q49] 更新单行
来源：http://yi.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uc.hahajie.cn

[Q50] 批量更新
来源：http://hg.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vp.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://gx.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oi.newstarts.cn

[Q52] 删除指定行
来源：http://nv.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://qd.szsharing.cn

[Q53] 按条件删除
来源：http://ki.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yj.shxzukj.cn

[Q54] 清空表
来源：http://za.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://gr.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://ch.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uk.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://jh.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wy.shxzskj.cn

[Q57] 行号
来源：http://au.9csxet.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kd.haigaiapp.cn

[Q58] 累计求和
来源：http://xz.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wk.bookmarksfly.cn

[Q59] 分组内累计
来源：http://ri.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bt.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://un.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zh.huixinmuqiang.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oo.shxzskj.cn

[Q61] 移动平均
来源：http://eh.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vq.asd995.cn

[Q62] 分组占比
来源：http://kl.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vw.shxzukj.cn

[Q63] 开启事务
来源：http://ns.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zy.asd995.cn

[Q64] 提交事务
来源：http://rc.asd995.cn

COMMIT;
来源：http://kl.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://vm.jctech888.com.cn

ROLLBACK;
来源：http://hh.panjiajie.cn

[Q66] 行锁查询
来源：http://vg.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zu.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://pm.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ro.haigaiapp.cn

[Q68] 保存点
来源：http://os.yuexingan06.cn

SAVEPOINT sp1;
来源：http://ra.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://wg.gzmigu.cn

[Q69] 查看执行计划
来源：http://nt.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ax.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://ij.jctech888.com.cn

ANALYZE TABLE users;
来源：http://xa.9csxet.cn

[Q71] 查看建表语句
来源：http://hg.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://th.asd995.cn

[Q72] 查看索引
来源：http://ur.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://xi.chemitech.net.cn

[Q73] 查看表状态
来源：http://sa.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ti.gzmigu.cn

[Q74] 强制使用索引
来源：http://zo.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ez.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://rd.szsharing.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gg.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aq.haigaiapp.cn

[Q76] 按天统计
来源：http://df.shtwfgs.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vb.huixiangedu.cn

[Q77] 时间加减
来源：http://mq.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fw.panjiajie.cn

[Q78] 当前时间
来源：http://vl.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ou.szxytkj.cn

[Q79] 字符串拼接
来源：http://nd.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kl.jctech888.com.cn

[Q80] 字符串截取
来源：http://pf.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rh.huixiangedu.cn

[Q81] 字符串替换
来源：http://bs.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yb.521024.cn

[Q82] 字符长度与字节长度
来源：http://hs.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sl.bookmarksfly.cn

[Q83] 大小写转换
来源：http://zc.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aw.szsharing.cn

[Q84] 去除首尾空格
来源：http://aq.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://kk.hahajie.cn

[Q85] 数值取整
来源：http://hu.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://th.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://yp.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nq.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://jd.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pv.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://vi.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rb.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qc.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://od.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://if.wgjwhj.cn

[Q90] 生成序号列
来源：http://su.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vd.chemitech.net.cn

================================================================================
来源：http://vl.shxzukj.cn

R. Bash 专题
来源：http://gp.haigaiapp.cn

================================================================================
来源：http://nj.9csxet.cn

[R01] shebang 与严格模式
来源：http://ri.shtwfgs.cn

#!/usr/bin/env bash
来源：http://wm.muxihuayi.cn

set -euo pipefail
来源：http://xb.9csxet.cn

[R02] 变量赋值与使用
来源：http://kh.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://ni.muxihuayi.cn

[R03] 只读变量
来源：http://lt.hahajie.cn

readonly PI=3.14
来源：http://jq.gzmigu.cn

[R04] 位置参数
来源：http://ia.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ji.yuexingan06.cn

[R05] 参数默认值
来源：http://ml.shxzskj.cn

name="${1:-default}"
来源：http://la.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://oa.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://po.huanxung.cn

[R07] if 判断文件
来源：http://pc.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pv.wgjwhj.cn

[R08] 数值比较
来源：http://ke.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ae.wgjwhj.cn

[R09] 字符串比较
来源：http://yr.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mm.yuntaijiaju.cn

[R10] 正则匹配
来源：http://zt.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mf.shxzskj.cn

[R11] case 多分支
来源：http://gg.jctech888.com.cn

case "$1" in
来源：http://xx.hnjuh.cn

start) echo "启动" ;;
来源：http://ho.huanxung.cn

stop)  echo "停止" ;;
来源：http://ma.gzmigu.cn

*)     echo "未知命令" ;;
来源：http://lp.asd995.cn

esac
来源：http://wx.szsharing.cn

[R12] for 遍历文件
来源：http://yn.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://wu.yuntaijiaju.cn

[R13] for 计数循环
来源：http://cv.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://cx.bookmarksfly.cn

[R14] C 风格 for
来源：http://pn.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pn.shxzukj.cn

[R15] while 逐行读文件
来源：http://uk.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xf.muxihuayi.cn

[R16] until 等待条件
来源：http://bi.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jn.colortex.cn

[R17] 数组定义与取值
来源：http://fc.huanxung.cn

arr=(a b c); echo "${arr[0]}"
来源：http://km.chemitech.net.cn

[R18] 遍历数组
来源：http://or.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uk.bjjhwx.cn

[R19] 数组长度
来源：http://ej.hnjuh.cn

echo "${#arr[@]}"
来源：http://aw.nszjky.cn

[R20] 关联数组（字典）
来源：http://yu.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zw.huixiangedu.cn

[R21] 字符串长度
来源：http://er.hnjuh.cn

echo "${#s}"
来源：http://ms.hahajie.cn

[R22] 截取子串
来源：http://qq.haigaiapp.cn

echo "${s:0:5}"
来源：http://dy.9csxet.cn

[R23] 字符串替换
来源：http://ck.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ay.shxzskj.cn

[R24] 大小写转换
来源：http://aj.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kz.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://sq.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xc.asd995.cn

[R26] 命令替换
来源：http://kv.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://zv.jianghongdianzi.cn

[R27] 算术展开
来源：http://ky.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://ln.wgjwhj.cn

[R28] 浮点运算
来源：http://cq.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://eo.colortex.cn

[R29] 定义函数
来源：http://uj.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ki.9csxet.cn

[R30] 函数返回状态码
来源：http://eo.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://cy.panjiajie.cn

[R31] 局部变量
来源：http://uo.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://rm.newstarts.cn

[R32] 参数个数校验
来源：http://rm.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vg.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://ti.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jj.newstarts.cn

[R34] 退出时清理
来源：http://xe.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xf.gzmigu.cn

[R35] 后台执行并等待
来源：http://ix.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ky.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://fl.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pf.panjiajie.cn

[R37] 把输出赋给变量
来源：http://hk.bjjhwx.cn

files=$(ls -1)
来源：http://vt.huanxung.cn

[R38] 管道串联
来源：http://um.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://ic.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://ee.lnxyls.cn

cmd > out.log 2>&1
来源：http://av.jianghongdianzi.cn

[R40] 追加写日志
来源：http://mb.nicolike.cn

echo "log" >> out.log
来源：http://qq.nszjky.cn

[R41] 丢弃输出
来源：http://xk.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://fa.huixiangedu.cn

[R42] 输入重定向
来源：http://xe.muxihuayi.cn

wc -l < a.txt
来源：http://ah.shxzskj.cn

[R43] 按名字查找文件
来源：http://rm.shxzskj.cn

find . -name "*.log" -type f
来源：http://aq.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://wo.lnxyls.cn

find . -mtime -7 -type f
来源：http://br.yuexingan06.cn

[R45] 批量删除
来源：http://hi.hahajie.cn


<!-- 参考信息 -->