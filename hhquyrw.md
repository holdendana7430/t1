代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qm.lnxyls.cn

user_id INT NOT NULL,
来源：http://yb.9csxet.cn

amount DECIMAL(10, 2),
来源：http://jn.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://km.yuexingan06.cn

);
来源：http://fj.shxzskj.cn

[Q03] 增加列
来源：http://ec.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bf.colortex.cn

[Q04] 修改列类型
来源：http://fx.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yw.nszjky.cn

[Q05] 重命名列
来源：http://jf.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ji.lnxyls.cn

[Q06] 删除列
来源：http://qx.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xp.szxytkj.cn

[Q07] 删除表
来源：http://ol.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://dm.shxzskj.cn

[Q08] 创建普通索引
来源：http://eh.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://he.asd995.cn

[Q09] 创建唯一索引
来源：http://hr.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://id.wgjwhj.cn

[Q10] 插入单行
来源：http://vo.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oa.9csxet.cn

[Q11] 一次插入多行
来源：http://mg.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ix.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://pt.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qj.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sg.szxytkj.cn

[Q13] 忽略重复插入
来源：http://qj.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bl.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://ku.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ug.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mc.yuexingan06.cn

[Q15] 查询全部
来源：http://un.521024.cn

SELECT * FROM users;
来源：http://xz.bookmarksfly.cn

[Q16] 查询指定列
来源：http://bm.bjjhwx.cn

SELECT id, name FROM users;
来源：http://nr.huixinmuqiang.cn

[Q17] 条件查询
来源：http://wx.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bp.shxzukj.cn

[Q18] 模糊匹配
来源：http://bf.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wg.szsharing.cn

[Q19] 范围查询
来源：http://bj.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lr.yuexingan06.cn

[Q20] IN 列表
来源：http://ww.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mo.panjiajie.cn

[Q21] 空值判断
来源：http://id.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cm.hnjuh.cn

[Q22] 排序
来源：http://zo.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ib.huixiangedu.cn

[Q23] 分页
来源：http://rk.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bp.szsharing.cn

[Q24] 去重
来源：http://la.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://sg.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://yp.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rl.huixinmuqiang.cn

[Q26] 计数
来源：http://zk.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://ut.nicolike.cn

[Q27] 条件计数
来源：http://ro.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://le.gzmigu.cn

[Q28] 求和与平均
来源：http://zm.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mk.panjiajie.cn

[Q29] 最大最小值
来源：http://dt.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fu.asd995.cn

[Q30] 分组统计
来源：http://yp.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pz.huanxung.cn

[Q31] 分组后过滤
来源：http://mz.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fb.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://dj.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ee.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qn.huixinmuqiang.cn

[Q33] 多列分组
来源：http://qb.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mh.bjjhwx.cn

[Q34] 每组取第一条
来源：http://ir.newstarts.cn

SELECT * FROM (
来源：http://gz.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kf.asd995.cn

) t WHERE rn = 1;
来源：http://wv.huixinmuqiang.cn

[Q35] 内连接
来源：http://oc.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cx.nszjky.cn

[Q36] 左连接
来源：http://rx.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ui.lnxyls.cn

[Q37] 右连接
来源：http://km.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aj.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rx.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://za.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://bi.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yc.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xo.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ub.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ta.panjiajie.cn

[Q41] 多表连接
来源：http://ac.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hm.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://py.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://gz.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://nu.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://uu.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wp.nicolike.cn

[Q43] 标量子查询
来源：http://lz.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bg.newstarts.cn

[Q44] IN 子查询
来源：http://jr.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gg.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://kg.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bz.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ge.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ar.lnxyls.cn

[Q47] 与平均值比较
来源：http://pq.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rx.colortex.cn

[Q48] CTE 公用表表达式
来源：http://fj.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jh.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://ct.521024.cn

[Q49] 更新单行
来源：http://sh.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sl.yuexingan06.cn

[Q50] 批量更新
来源：http://sp.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xh.bjjhwx.cn

[Q51] 用子查询更新
来源：http://bu.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wr.shxzukj.cn

[Q52] 删除指定行
来源：http://kk.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://qw.9csxet.cn

[Q53] 按条件删除
来源：http://wy.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yv.wgjwhj.cn

[Q54] 清空表
来源：http://ax.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://td.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://et.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jz.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://fu.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ap.szsharing.cn

[Q57] 行号
来源：http://xw.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hp.shxzskj.cn

[Q58] 累计求和
来源：http://le.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sj.huixiangedu.cn

[Q59] 分组内累计
来源：http://ci.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hg.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://dq.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ov.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ax.yuexingan06.cn

[Q61] 移动平均
来源：http://zc.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ga.bookmarksfly.cn

[Q62] 分组占比
来源：http://as.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lk.muxihuayi.cn

[Q63] 开启事务
来源：http://em.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xa.9csxet.cn

[Q64] 提交事务
来源：http://ta.nszjky.cn

COMMIT;
来源：http://rd.521024.cn

[Q65] 回滚事务
来源：http://eg.yuexingan06.cn

ROLLBACK;
来源：http://kn.hahajie.cn

[Q66] 行锁查询
来源：http://ly.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nm.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://bg.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fm.colortex.cn

[Q68] 保存点
来源：http://lx.haigaiapp.cn

SAVEPOINT sp1;
来源：http://ub.hnjuh.cn

ROLLBACK TO sp1;
来源：http://zi.huanxung.cn

[Q69] 查看执行计划
来源：http://ns.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rf.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://cx.shtwfgs.cn

ANALYZE TABLE users;
来源：http://hm.hahajie.cn

[Q71] 查看建表语句
来源：http://sz.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bu.bjjhwx.cn

[Q72] 查看索引
来源：http://jf.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://sj.shxzukj.cn

[Q73] 查看表状态
来源：http://sb.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yh.chemitech.net.cn

[Q74] 强制使用索引
来源：http://aw.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bv.haigaiapp.cn

[Q75] 日期格式化
来源：http://sx.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dt.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pm.panjiajie.cn

[Q76] 按天统计
来源：http://ax.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://us.szsharing.cn

[Q77] 时间加减
来源：http://bi.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lv.nicolike.cn

[Q78] 当前时间
来源：http://tw.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xj.wgjwhj.cn

[Q79] 字符串拼接
来源：http://bk.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lr.nicolike.cn

[Q80] 字符串截取
来源：http://jk.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vw.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://wi.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ox.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://fe.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gs.muxihuayi.cn

[Q83] 大小写转换
来源：http://gk.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uz.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://pu.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://qb.nszjky.cn

[Q85] 数值取整
来源：http://xs.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bx.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://ak.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cm.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://py.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ua.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://tr.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xe.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cg.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://mz.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yt.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://ke.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ya.huanxung.cn

================================================================================
来源：http://lc.9csxet.cn

R. Bash 专题
来源：http://vv.bjjhwx.cn

================================================================================
来源：http://eo.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://rr.huixiangedu.cn

#!/usr/bin/env bash
来源：http://zf.huixinmuqiang.cn

set -euo pipefail
来源：http://lx.gzmigu.cn

[R02] 变量赋值与使用
来源：http://hw.szsharing.cn

name="Tom"; echo "$name"
来源：http://cl.szsharing.cn

[R03] 只读变量
来源：http://zv.shxzukj.cn

readonly PI=3.14
来源：http://ip.asd995.cn

[R04] 位置参数
来源：http://zc.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mz.hnjuh.cn

[R05] 参数默认值
来源：http://fp.chemitech.net.cn

name="${1:-default}"
来源：http://vc.szxytkj.cn

[R06] 判断命令是否存在
来源：http://ha.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yf.shxzskj.cn

[R07] if 判断文件
来源：http://fa.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ts.jianghongdianzi.cn

[R08] 数值比较
来源：http://gf.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nc.bjjhwx.cn

[R09] 字符串比较
来源：http://ah.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ao.huixinmuqiang.cn

[R10] 正则匹配
来源：http://xf.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kl.nicolike.cn

[R11] case 多分支
来源：http://bz.huixiangedu.cn

case "$1" in
来源：http://vr.nicolike.cn

start) echo "启动" ;;
来源：http://fa.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://my.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://oj.huixinmuqiang.cn

esac
来源：http://oe.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://wl.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://vm.nszjky.cn

[R13] for 计数循环
来源：http://cq.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://le.bjjhwx.cn

[R14] C 风格 for
来源：http://wz.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pr.szxytkj.cn

[R15] while 逐行读文件
来源：http://wh.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://be.jianghongdianzi.cn

[R16] until 等待条件
来源：http://lt.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wp.521024.cn

[R17] 数组定义与取值
来源：http://ml.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tp.9csxet.cn

[R18] 遍历数组
来源：http://bd.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://di.bjjhwx.cn

[R19] 数组长度
来源：http://sn.panjiajie.cn

echo "${#arr[@]}"
来源：http://jr.gzmigu.cn

[R20] 关联数组（字典）
来源：http://zz.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iq.newstarts.cn

[R21] 字符串长度
来源：http://ht.huanxung.cn

echo "${#s}"
来源：http://pv.bjjhwx.cn

[R22] 截取子串
来源：http://qz.szxytkj.cn

echo "${s:0:5}"
来源：http://xa.yuntaijiaju.cn

[R23] 字符串替换
来源：http://md.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nu.huixiangedu.cn

[R24] 大小写转换
来源：http://bz.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vx.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://sc.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dn.9csxet.cn

[R26] 命令替换
来源：http://ok.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://cw.jianghongdianzi.cn

[R27] 算术展开
来源：http://mq.9csxet.cn

echo $((1 + 2 * 3))
来源：http://dp.huixiangedu.cn

[R28] 浮点运算
来源：http://zk.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://so.yuexingan06.cn

[R29] 定义函数
来源：http://yo.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://om.huixiangedu.cn

[R30] 函数返回状态码
来源：http://mk.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://hz.hahajie.cn

[R31] 局部变量
来源：http://tp.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://ye.yuexingan06.cn

[R32] 参数个数校验
来源：http://sb.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qz.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://ze.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sq.newstarts.cn

[R34] 退出时清理
来源：http://ra.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://as.huixiangedu.cn

[R35] 后台执行并等待
来源：http://qj.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jd.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://co.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fd.gzmigu.cn

[R37] 把输出赋给变量
来源：http://io.huixinmuqiang.cn

files=$(ls -1)
来源：http://zb.bjjhwx.cn

[R38] 管道串联
来源：http://ts.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://ss.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://dp.asd995.cn

cmd > out.log 2>&1
来源：http://sd.jianghongdianzi.cn

[R40] 追加写日志
来源：http://xw.newstarts.cn

echo "log" >> out.log
来源：http://oy.wgjwhj.cn

[R41] 丢弃输出
来源：http://eq.newstarts.cn

cmd >/dev/null 2>&1
来源：http://vo.muxihuayi.cn

[R42] 输入重定向
来源：http://jf.hahajie.cn

wc -l < a.txt
来源：http://qa.asd995.cn

[R43] 按名字查找文件
来源：http://rl.wgjwhj.cn

find . -name "*.log" -type f
来源：http://nf.chemitech.net.cn

[R44] 按修改时间查找
来源：http://gy.521024.cn

find . -mtime -7 -type f
来源：http://al.huixinmuqiang.cn

[R45] 批量删除
来源：http://et.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://ol.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://kz.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ok.hnjuh.cn

[R47] sed 单行替换
来源：http://sy.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rd.huanxung.cn

[R48] awk 取指定列
来源：http://pu.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://xu.haigaiapp.cn

[R49] awk 带条件
来源：http://mv.haigaiapp.cn


<!-- 参考信息 -->