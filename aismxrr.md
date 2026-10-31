代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xb.muxihuayi.cn

user_id INT NOT NULL,
来源：http://se.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://ii.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gx.bookmarksfly.cn

);
来源：http://bt.huixinmuqiang.cn

[Q03] 增加列
来源：http://ey.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jy.wgjwhj.cn

[Q04] 修改列类型
来源：http://dt.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rn.shxzskj.cn

[Q05] 重命名列
来源：http://na.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yt.nicolike.cn

[Q06] 删除列
来源：http://fu.wgjwhj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ho.hnjuh.cn

[Q07] 删除表
来源：http://jh.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://ya.shxzukj.cn

[Q08] 创建普通索引
来源：http://oh.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xg.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://tu.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xa.szsharing.cn

[Q10] 插入单行
来源：http://up.panjiajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xx.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://bc.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qa.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://xq.nszjky.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oc.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ta.gzmigu.cn

[Q13] 忽略重复插入
来源：http://cg.9csxet.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cs.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://bz.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://st.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ma.huixinmuqiang.cn

[Q15] 查询全部
来源：http://fv.huixiangedu.cn

SELECT * FROM users;
来源：http://oc.jctech888.com.cn

[Q16] 查询指定列
来源：http://sb.panjiajie.cn

SELECT id, name FROM users;
来源：http://bq.muxihuayi.cn

[Q17] 条件查询
来源：http://nr.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nc.muxihuayi.cn

[Q18] 模糊匹配
来源：http://hb.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uh.yuexingan06.cn

[Q19] 范围查询
来源：http://pt.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wx.521024.cn

[Q20] IN 列表
来源：http://vb.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ct.shxzskj.cn

[Q21] 空值判断
来源：http://uy.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rb.nicolike.cn

[Q22] 排序
来源：http://qj.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kv.bookmarksfly.cn

[Q23] 分页
来源：http://ke.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://la.nszjky.cn

[Q24] 去重
来源：http://mx.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://hw.lnxyls.cn

[Q25] 只取前 N 条
来源：http://lj.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wr.huixiangedu.cn

[Q26] 计数
来源：http://xn.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://xl.nszjky.cn

[Q27] 条件计数
来源：http://tq.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wc.9csxet.cn

[Q28] 求和与平均
来源：http://ab.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kt.gzmigu.cn

[Q29] 最大最小值
来源：http://ms.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://aq.chemitech.net.cn

[Q30] 分组统计
来源：http://oo.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zr.huixinmuqiang.cn

[Q31] 分组后过滤
来源：http://mi.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pc.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://ff.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sm.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wq.9csxet.cn

[Q33] 多列分组
来源：http://ml.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dk.asd995.cn

[Q34] 每组取第一条
来源：http://hp.haigaiapp.cn

SELECT * FROM (
来源：http://xs.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rh.asd995.cn

) t WHERE rn = 1;
来源：http://is.9csxet.cn

[Q35] 内连接
来源：http://kx.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://su.shxzskj.cn

[Q36] 左连接
来源：http://qr.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tb.gzmigu.cn

[Q37] 右连接
来源：http://wq.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tn.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://en.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tz.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://jx.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yi.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ac.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vt.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vs.nicolike.cn

[Q41] 多表连接
来源：http://li.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xe.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://yi.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://mo.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://yh.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://gr.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rn.wgjwhj.cn

[Q43] 标量子查询
来源：http://qr.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tp.nicolike.cn

[Q44] IN 子查询
来源：http://vw.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fy.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://pr.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xk.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sn.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lc.yuexingan06.cn

[Q47] 与平均值比较
来源：http://ho.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oh.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://cb.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cf.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://qj.haigaiapp.cn

[Q49] 更新单行
来源：http://jd.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pe.yuexingan06.cn

[Q50] 批量更新
来源：http://qu.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oo.shxzukj.cn

[Q51] 用子查询更新
来源：http://ye.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tq.panjiajie.cn

[Q52] 删除指定行
来源：http://tr.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://fe.lnxyls.cn

[Q53] 按条件删除
来源：http://uv.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gd.lnxyls.cn

[Q54] 清空表
来源：http://vb.nicolike.cn

TRUNCATE TABLE logs;
来源：http://we.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://rs.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xg.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://ob.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uy.asd995.cn

[Q57] 行号
来源：http://qe.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gj.jianghongdianzi.cn

[Q58] 累计求和
来源：http://ux.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ke.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://kq.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dm.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://jg.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hg.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gb.jianghongdianzi.cn

[Q61] 移动平均
来源：http://sm.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mz.szxytkj.cn

[Q62] 分组占比
来源：http://kn.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sh.shtwfgs.cn

[Q63] 开启事务
来源：http://tg.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ib.shtwfgs.cn

[Q64] 提交事务
来源：http://qs.colortex.cn

COMMIT;
来源：http://sd.asd995.cn

[Q65] 回滚事务
来源：http://hb.huanxung.cn

ROLLBACK;
来源：http://uu.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://nl.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mt.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://jw.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ln.bookmarksfly.cn

[Q68] 保存点
来源：http://rm.shtwfgs.cn

SAVEPOINT sp1;
来源：http://zu.szxytkj.cn

ROLLBACK TO sp1;
来源：http://do.szxytkj.cn

[Q69] 查看执行计划
来源：http://ys.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pg.9csxet.cn

[Q70] 更新统计信息
来源：http://fc.jctech888.com.cn

ANALYZE TABLE users;
来源：http://vt.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://uo.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uj.yuntaijiaju.cn

[Q72] 查看索引
来源：http://jw.szsharing.cn

SHOW INDEX FROM users;
来源：http://zd.wgjwhj.cn

[Q73] 查看表状态
来源：http://ac.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bb.shtwfgs.cn

[Q74] 强制使用索引
来源：http://qm.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gx.gzmigu.cn

[Q75] 日期格式化
来源：http://ua.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://np.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vt.521024.cn

[Q76] 按天统计
来源：http://xw.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eq.panjiajie.cn

[Q77] 时间加减
来源：http://jm.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ep.hnjuh.cn

[Q78] 当前时间
来源：http://zu.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://md.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://ai.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kj.newstarts.cn

[Q80] 字符串截取
来源：http://jo.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gg.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://yu.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cm.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://rx.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oy.bookmarksfly.cn

[Q83] 大小写转换
来源：http://lo.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dv.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://om.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://zd.huanxung.cn

[Q85] 数值取整
来源：http://dr.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gd.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://my.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sn.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://wl.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ig.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://ly.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uv.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qh.hnjuh.cn

[Q89] 判断表是否存在
来源：http://mc.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bs.nszjky.cn

[Q90] 生成序号列
来源：http://ot.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sr.hahajie.cn

================================================================================
来源：http://ue.shxzskj.cn

R. Bash 专题
来源：http://uz.9csxet.cn

================================================================================
来源：http://qv.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://nb.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://kf.huixinmuqiang.cn

set -euo pipefail
来源：http://ti.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://ce.shxzskj.cn

name="Tom"; echo "$name"
来源：http://ft.nicolike.cn

[R03] 只读变量
来源：http://kv.huixiangedu.cn

readonly PI=3.14
来源：http://cp.panjiajie.cn

[R04] 位置参数
来源：http://bh.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://md.huixinmuqiang.cn

[R05] 参数默认值
来源：http://mk.szxytkj.cn

name="${1:-default}"
来源：http://op.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://is.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yg.bjjhwx.cn

[R07] if 判断文件
来源：http://zn.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sy.huixinmuqiang.cn

[R08] 数值比较
来源：http://wu.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fl.haigaiapp.cn

[R09] 字符串比较
来源：http://kk.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kv.bjjhwx.cn

[R10] 正则匹配
来源：http://dt.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fj.szxytkj.cn

[R11] case 多分支
来源：http://gr.521024.cn

case "$1" in
来源：http://cr.hahajie.cn

start) echo "启动" ;;
来源：http://eg.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://vi.huixinmuqiang.cn

*)     echo "未知命令" ;;
来源：http://at.jctech888.com.cn

esac
来源：http://ry.nicolike.cn

[R12] for 遍历文件
来源：http://et.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://or.jctech888.com.cn

[R13] for 计数循环
来源：http://ge.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://dr.haigaiapp.cn

[R14] C 风格 for
来源：http://mn.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iw.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://df.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nc.yuexingan06.cn

[R16] until 等待条件
来源：http://si.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://di.shxzskj.cn

[R17] 数组定义与取值
来源：http://sm.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ou.szsharing.cn

[R18] 遍历数组
来源：http://bk.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xb.shtwfgs.cn

[R19] 数组长度
来源：http://jj.haigaiapp.cn

echo "${#arr[@]}"
来源：http://op.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://yg.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ld.huixiangedu.cn

[R21] 字符串长度
来源：http://ee.newstarts.cn

echo "${#s}"
来源：http://on.szsharing.cn

[R22] 截取子串
来源：http://uq.jctech888.com.cn

echo "${s:0:5}"
来源：http://vo.wgjwhj.cn

[R23] 字符串替换
来源：http://qd.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ys.wgjwhj.cn

[R24] 大小写转换
来源：http://rb.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://at.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://ws.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cr.huixiangedu.cn

[R26] 命令替换
来源：http://bp.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://yp.panjiajie.cn

[R27] 算术展开
来源：http://hi.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://ab.colortex.cn

[R28] 浮点运算
来源：http://mf.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://zy.bjjhwx.cn

[R29] 定义函数
来源：http://li.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ge.gzmigu.cn

[R30] 函数返回状态码
来源：http://ga.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://hw.gzmigu.cn

[R31] 局部变量
来源：http://mw.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://tm.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://fg.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dy.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://lx.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fb.nszjky.cn

[R34] 退出时清理
来源：http://tk.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ga.shtwfgs.cn

[R35] 后台执行并等待
来源：http://ji.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ox.panjiajie.cn

[R36] 并发执行多个任务
来源：http://in.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dz.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://fr.521024.cn

files=$(ls -1)
来源：http://db.hnjuh.cn

[R38] 管道串联
来源：http://kh.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://zm.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://sc.panjiajie.cn

cmd > out.log 2>&1
来源：http://bq.jianghongdianzi.cn

[R40] 追加写日志
来源：http://dd.szxytkj.cn

echo "log" >> out.log
来源：http://in.521024.cn

[R41] 丢弃输出
来源：http://mk.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://qo.hahajie.cn

[R42] 输入重定向
来源：http://lj.chemitech.net.cn

wc -l < a.txt
来源：http://fx.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://xc.bjjhwx.cn

find . -name "*.log" -type f
来源：http://hx.asd995.cn

[R44] 按修改时间查找
来源：http://as.521024.cn

find . -mtime -7 -type f
来源：http://xk.shxzskj.cn

[R45] 批量删除
来源：http://av.521024.cn

find . -name "*.tmp" -delete
来源：http://pr.shxzukj.cn

[R46] 递归替换文件内容
来源：http://ex.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sw.wgjwhj.cn

[R47] sed 单行替换
来源：http://sq.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yd.muxihuayi.cn

[R48] awk 取指定列
来源：http://vc.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://df.jctech888.com.cn

[R49] awk 带条件
来源：http://dw.yuntaijiaju.cn


<!-- 参考信息 -->