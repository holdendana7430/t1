代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ok.gzmigu.cn

);
来源：http://ps.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://xp.bookmarksfly.cn

CREATE TABLE orders (
来源：http://gu.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vb.521024.cn

user_id INT NOT NULL,
来源：http://vs.nszjky.cn

amount DECIMAL(10, 2),
来源：http://kx.yuntaijiaju.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gk.szxytkj.cn

);
来源：http://la.huixinmuqiang.cn

[Q03] 增加列
来源：http://ax.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nm.9csxet.cn

[Q04] 修改列类型
来源：http://gm.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ye.shxzukj.cn

[Q05] 重命名列
来源：http://ca.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rv.shtwfgs.cn

[Q06] 删除列
来源：http://dk.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qm.jctech888.com.cn

[Q07] 删除表
来源：http://ox.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://sb.colortex.cn

[Q08] 创建普通索引
来源：http://ng.9csxet.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bx.shxzskj.cn

[Q09] 创建唯一索引
来源：http://dp.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ow.bjjhwx.cn

[Q10] 插入单行
来源：http://sp.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xx.huixiangedu.cn

[Q11] 一次插入多行
来源：http://jz.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ro.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://wu.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wa.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jw.521024.cn

[Q13] 忽略重复插入
来源：http://rh.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dy.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://de.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://td.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ac.haigaiapp.cn

[Q15] 查询全部
来源：http://uv.bookmarksfly.cn

SELECT * FROM users;
来源：http://xx.shxzukj.cn

[Q16] 查询指定列
来源：http://zt.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://rh.muxihuayi.cn

[Q17] 条件查询
来源：http://eu.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kt.asd995.cn

[Q18] 模糊匹配
来源：http://es.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qo.jctech888.com.cn

[Q19] 范围查询
来源：http://km.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vp.panjiajie.cn

[Q20] IN 列表
来源：http://pp.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ai.shxzskj.cn

[Q21] 空值判断
来源：http://ls.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yq.bjjhwx.cn

[Q22] 排序
来源：http://np.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gk.hahajie.cn

[Q23] 分页
来源：http://kk.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wx.nszjky.cn

[Q24] 去重
来源：http://aj.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://ch.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://xn.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ou.huixinmuqiang.cn

[Q26] 计数
来源：http://ok.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://if.szxytkj.cn

[Q27] 条件计数
来源：http://lc.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://am.newstarts.cn

[Q28] 求和与平均
来源：http://bn.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ie.huixinmuqiang.cn

[Q29] 最大最小值
来源：http://fy.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://we.lnxyls.cn

[Q30] 分组统计
来源：http://cm.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gp.nicolike.cn

[Q31] 分组后过滤
来源：http://dl.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wb.asd995.cn

[Q32] 分组拼接字符串
来源：http://zh.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lh.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ro.9csxet.cn

[Q33] 多列分组
来源：http://zm.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ke.lnxyls.cn

[Q34] 每组取第一条
来源：http://al.bookmarksfly.cn

SELECT * FROM (
来源：http://bs.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ri.colortex.cn

) t WHERE rn = 1;
来源：http://dw.jctech888.com.cn

[Q35] 内连接
来源：http://oz.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vu.yuntaijiaju.cn

[Q36] 左连接
来源：http://mn.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ah.huixiangedu.cn

[Q37] 右连接
来源：http://mc.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://au.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zb.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wn.gzmigu.cn

[Q39] 自连接（查上下级）
来源：http://kw.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nx.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fn.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ie.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aj.yuntaijiaju.cn

[Q41] 多表连接
来源：http://hw.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ix.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://hx.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://nl.521024.cn

[Q42] 连接条件附加过滤
来源：http://ab.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://vm.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://we.muxihuayi.cn

[Q43] 标量子查询
来源：http://ka.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yv.gzmigu.cn

[Q44] IN 子查询
来源：http://zp.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jt.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://pv.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://do.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tn.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eh.colortex.cn

[Q47] 与平均值比较
来源：http://ty.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tz.huixiangedu.cn

[Q48] CTE 公用表表达式
来源：http://sb.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sc.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://aa.szxytkj.cn

[Q49] 更新单行
来源：http://im.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mc.szsharing.cn

[Q50] 批量更新
来源：http://ae.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xz.muxihuayi.cn

[Q51] 用子查询更新
来源：http://uq.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mk.szsharing.cn

[Q52] 删除指定行
来源：http://zq.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://vm.jctech888.com.cn

[Q53] 按条件删除
来源：http://nt.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mx.9csxet.cn

[Q54] 清空表
来源：http://qu.9csxet.cn

TRUNCATE TABLE logs;
来源：http://uc.nszjky.cn

[Q55] 排名（并列占位）
来源：http://my.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xf.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://hb.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ff.muxihuayi.cn

[Q57] 行号
来源：http://dg.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dl.gzmigu.cn

[Q58] 累计求和
来源：http://fd.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yi.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://aw.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hu.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://fq.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jw.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fm.newstarts.cn

[Q61] 移动平均
来源：http://cd.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sm.gzmigu.cn

[Q62] 分组占比
来源：http://wi.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yx.wgjwhj.cn

[Q63] 开启事务
来源：http://ig.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xn.hnjuh.cn

[Q64] 提交事务
来源：http://jq.521024.cn

COMMIT;
来源：http://zc.shxzukj.cn

[Q65] 回滚事务
来源：http://ae.hahajie.cn

ROLLBACK;
来源：http://wr.hahajie.cn

[Q66] 行锁查询
来源：http://ao.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zx.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://el.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zg.huanxung.cn

[Q68] 保存点
来源：http://gm.szsharing.cn

SAVEPOINT sp1;
来源：http://xy.hahajie.cn

ROLLBACK TO sp1;
来源：http://gs.lnxyls.cn

[Q69] 查看执行计划
来源：http://bq.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gj.hahajie.cn

[Q70] 更新统计信息
来源：http://vc.szsharing.cn

ANALYZE TABLE users;
来源：http://qj.huanxung.cn

[Q71] 查看建表语句
来源：http://lp.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hs.bjjhwx.cn

[Q72] 查看索引
来源：http://uh.huanxung.cn

SHOW INDEX FROM users;
来源：http://lh.muxihuayi.cn

[Q73] 查看表状态
来源：http://up.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://aw.panjiajie.cn

[Q74] 强制使用索引
来源：http://cs.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://az.colortex.cn

[Q75] 日期格式化
来源：http://mu.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gy.huanxung.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kp.newstarts.cn

[Q76] 按天统计
来源：http://on.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://il.huanxung.cn

[Q77] 时间加减
来源：http://cx.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vx.haigaiapp.cn

[Q78] 当前时间
来源：http://wu.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hm.huixiangedu.cn

[Q79] 字符串拼接
来源：http://ws.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ef.colortex.cn

[Q80] 字符串截取
来源：http://dr.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qb.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://wo.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gs.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://zx.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oy.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://wz.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://et.szxytkj.cn

[Q84] 去除首尾空格
来源：http://fp.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://wx.lnxyls.cn

[Q85] 数值取整
来源：http://ms.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bo.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://ok.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uw.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://tc.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://up.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://vb.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xu.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zi.shxzskj.cn

[Q89] 判断表是否存在
来源：http://cf.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ou.nicolike.cn

[Q90] 生成序号列
来源：http://kf.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dt.bjjhwx.cn

================================================================================
来源：http://cz.huixinmuqiang.cn

R. Bash 专题
来源：http://jo.hnjuh.cn

================================================================================
来源：http://ul.panjiajie.cn

[R01] shebang 与严格模式
来源：http://ei.colortex.cn

#!/usr/bin/env bash
来源：http://yg.lnxyls.cn

set -euo pipefail
来源：http://ed.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://wh.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://jh.gzmigu.cn

[R03] 只读变量
来源：http://ic.haigaiapp.cn

readonly PI=3.14
来源：http://al.521024.cn

[R04] 位置参数
来源：http://xp.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sj.shtwfgs.cn

[R05] 参数默认值
来源：http://aj.huixinmuqiang.cn

name="${1:-default}"
来源：http://hp.lnxyls.cn

[R06] 判断命令是否存在
来源：http://ec.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lb.bookmarksfly.cn

[R07] if 判断文件
来源：http://zg.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lk.jctech888.com.cn

[R08] 数值比较
来源：http://lo.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qq.lnxyls.cn

[R09] 字符串比较
来源：http://qh.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jt.wgjwhj.cn

[R10] 正则匹配
来源：http://lt.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fr.9csxet.cn

[R11] case 多分支
来源：http://tw.shxzskj.cn

case "$1" in
来源：http://wm.gzmigu.cn

start) echo "启动" ;;
来源：http://fr.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://qw.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://qh.huanxung.cn

esac
来源：http://ky.yuexingan06.cn

[R12] for 遍历文件
来源：http://vu.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://nv.bjjhwx.cn

[R13] for 计数循环
来源：http://to.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://qg.bjjhwx.cn

[R14] C 风格 for
来源：http://cb.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vf.haigaiapp.cn

[R15] while 逐行读文件
来源：http://bi.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vi.muxihuayi.cn

[R16] until 等待条件
来源：http://kv.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://je.521024.cn

[R17] 数组定义与取值
来源：http://pf.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fl.shtwfgs.cn

[R18] 遍历数组
来源：http://le.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pa.chemitech.net.cn

[R19] 数组长度
来源：http://xo.gzmigu.cn

echo "${#arr[@]}"
来源：http://ee.asd995.cn

[R20] 关联数组（字典）
来源：http://ok.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tj.gzmigu.cn

[R21] 字符串长度
来源：http://zt.asd995.cn

echo "${#s}"
来源：http://vy.521024.cn

[R22] 截取子串
来源：http://fm.szsharing.cn

echo "${s:0:5}"
来源：http://fk.yuexingan06.cn

[R23] 字符串替换
来源：http://mt.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tx.haigaiapp.cn

[R24] 大小写转换
来源：http://vf.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ku.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://ih.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cl.yuntaijiaju.cn

[R26] 命令替换
来源：http://ov.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://hg.bookmarksfly.cn

[R27] 算术展开
来源：http://jc.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://cm.shxzskj.cn

[R28] 浮点运算
来源：http://fz.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://lp.huixiangedu.cn

[R29] 定义函数
来源：http://um.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ep.shtwfgs.cn

[R30] 函数返回状态码
来源：http://qd.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://tp.yuexingan06.cn

[R31] 局部变量
来源：http://cd.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://wq.shxzukj.cn

[R32] 参数个数校验
来源：http://lb.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fv.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://ku.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fc.asd995.cn

[R34] 退出时清理
来源：http://bv.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ae.lnxyls.cn

[R35] 后台执行并等待
来源：http://lg.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lh.hahajie.cn

[R36] 并发执行多个任务
来源：http://ku.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nz.hnjuh.cn

[R37] 把输出赋给变量
来源：http://ij.yuntaijiaju.cn

files=$(ls -1)
来源：http://ut.jctech888.com.cn

[R38] 管道串联
来源：http://pp.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://el.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://id.nicolike.cn

cmd > out.log 2>&1
来源：http://ji.gzmigu.cn

[R40] 追加写日志
来源：http://oe.521024.cn

echo "log" >> out.log
来源：http://ex.shxzukj.cn

[R41] 丢弃输出
来源：http://fe.nszjky.cn

cmd >/dev/null 2>&1
来源：http://hi.huanxung.cn

[R42] 输入重定向
来源：http://we.nszjky.cn

wc -l < a.txt
来源：http://oj.nszjky.cn

[R43] 按名字查找文件
来源：http://or.521024.cn

find . -name "*.log" -type f
来源：http://nu.nszjky.cn

[R44] 按修改时间查找
来源：http://au.panjiajie.cn

find . -mtime -7 -type f
来源：http://my.panjiajie.cn

[R45] 批量删除
来源：http://jb.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://sw.hnjuh.cn

[R46] 递归替换文件内容
来源：http://qq.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qh.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://md.bookmarksfly.cn


<!-- 参考信息 -->