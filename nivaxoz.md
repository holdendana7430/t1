代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wz.yuexingan06.cn

user_id INT NOT NULL,
来源：http://iv.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://oh.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ga.yuexingan06.cn

);
来源：http://fo.gzmigu.cn

[Q03] 增加列
来源：http://iv.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wa.nszjky.cn

[Q04] 修改列类型
来源：http://et.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pl.asd995.cn

[Q05] 重命名列
来源：http://rg.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hq.huixiangedu.cn

[Q06] 删除列
来源：http://wi.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://am.lnxyls.cn

[Q07] 删除表
来源：http://yu.jctech888.com.cn

DROP TABLE IF EXISTS orders;
来源：http://zs.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://yp.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bx.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://vv.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ov.hahajie.cn

[Q10] 插入单行
来源：http://vw.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fu.shxzukj.cn

[Q11] 一次插入多行
来源：http://jg.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bq.colortex.cn

[Q12] 插入后取自增 ID
来源：http://em.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bj.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jv.shxzukj.cn

[Q13] 忽略重复插入
来源：http://bs.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zi.521024.cn

[Q14] 存在则更新（upsert）
来源：http://sn.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bb.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pg.chemitech.net.cn

[Q15] 查询全部
来源：http://gw.bjjhwx.cn

SELECT * FROM users;
来源：http://zy.asd995.cn

[Q16] 查询指定列
来源：http://tv.shxzukj.cn

SELECT id, name FROM users;
来源：http://fj.gzmigu.cn

[Q17] 条件查询
来源：http://us.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://to.nicolike.cn

[Q18] 模糊匹配
来源：http://gs.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hh.haigaiapp.cn

[Q19] 范围查询
来源：http://gg.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lc.shxzukj.cn

[Q20] IN 列表
来源：http://qg.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://on.muxihuayi.cn

[Q21] 空值判断
来源：http://pn.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rj.hahajie.cn

[Q22] 排序
来源：http://hn.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fk.szxytkj.cn

[Q23] 分页
来源：http://qn.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xn.newstarts.cn

[Q24] 去重
来源：http://vy.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://ou.szxytkj.cn

[Q25] 只取前 N 条
来源：http://rg.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vj.lnxyls.cn

[Q26] 计数
来源：http://lb.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://gq.shxzskj.cn

[Q27] 条件计数
来源：http://oj.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tl.bookmarksfly.cn

[Q28] 求和与平均
来源：http://cd.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kc.shxzukj.cn

[Q29] 最大最小值
来源：http://ow.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://im.szsharing.cn

[Q30] 分组统计
来源：http://eh.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tr.muxihuayi.cn

[Q31] 分组后过滤
来源：http://ty.jctech888.com.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vq.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://ol.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ul.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pn.gzmigu.cn

[Q33] 多列分组
来源：http://pl.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jp.shtwfgs.cn

[Q34] 每组取第一条
来源：http://fn.muxihuayi.cn

SELECT * FROM (
来源：http://wq.nicolike.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tw.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://sz.hnjuh.cn

[Q35] 内连接
来源：http://hu.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hw.bookmarksfly.cn

[Q36] 左连接
来源：http://if.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://az.lnxyls.cn

[Q37] 右连接
来源：http://dr.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rg.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bw.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ht.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://sv.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ah.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vq.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pm.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vh.huixinmuqiang.cn

[Q41] 多表连接
来源：http://fu.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ne.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://sa.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://pm.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://el.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://bh.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sp.haigaiapp.cn

[Q43] 标量子查询
来源：http://ko.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://on.521024.cn

[Q44] IN 子查询
来源：http://wy.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hl.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://mi.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dk.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ap.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lz.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://vg.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lh.colortex.cn

[Q48] CTE 公用表表达式
来源：http://mr.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ep.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://wd.huanxung.cn

[Q49] 更新单行
来源：http://ke.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ea.chemitech.net.cn

[Q50] 批量更新
来源：http://ve.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hr.hahajie.cn

[Q51] 用子查询更新
来源：http://ii.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ch.newstarts.cn

[Q52] 删除指定行
来源：http://bk.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://cy.hnjuh.cn

[Q53] 按条件删除
来源：http://li.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jf.wgjwhj.cn

[Q54] 清空表
来源：http://af.szsharing.cn

TRUNCATE TABLE logs;
来源：http://en.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://ni.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://el.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://km.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uu.haigaiapp.cn

[Q57] 行号
来源：http://ac.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://av.521024.cn

[Q58] 累计求和
来源：http://hi.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ln.haigaiapp.cn

[Q59] 分组内累计
来源：http://bf.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://os.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://df.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gy.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ca.huixinmuqiang.cn

[Q61] 移动平均
来源：http://zh.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fq.hahajie.cn

[Q62] 分组占比
来源：http://zl.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mk.521024.cn

[Q63] 开启事务
来源：http://ff.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://on.nszjky.cn

[Q64] 提交事务
来源：http://sm.yuntaijiaju.cn

COMMIT;
来源：http://ib.shxzukj.cn

[Q65] 回滚事务
来源：http://cn.asd995.cn

ROLLBACK;
来源：http://mw.colortex.cn

[Q66] 行锁查询
来源：http://fv.colortex.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yy.colortex.cn

[Q67] 设置隔离级别
来源：http://vz.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://le.lnxyls.cn

[Q68] 保存点
来源：http://wn.jianghongdianzi.cn

SAVEPOINT sp1;
来源：http://rg.szxytkj.cn

ROLLBACK TO sp1;
来源：http://kv.panjiajie.cn

[Q69] 查看执行计划
来源：http://rq.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lz.jctech888.com.cn

[Q70] 更新统计信息
来源：http://dj.newstarts.cn

ANALYZE TABLE users;
来源：http://zy.wgjwhj.cn

[Q71] 查看建表语句
来源：http://la.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rt.hahajie.cn

[Q72] 查看索引
来源：http://md.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://mz.gzmigu.cn

[Q73] 查看表状态
来源：http://nq.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://eo.gzmigu.cn

[Q74] 强制使用索引
来源：http://lk.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gc.yuexingan06.cn

[Q75] 日期格式化
来源：http://mn.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yb.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yh.shxzukj.cn

[Q76] 按天统计
来源：http://ul.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ox.521024.cn

[Q77] 时间加减
来源：http://jr.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yt.shxzukj.cn

[Q78] 当前时间
来源：http://sf.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ni.hahajie.cn

[Q79] 字符串拼接
来源：http://hw.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://be.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://ii.panjiajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://as.bookmarksfly.cn

[Q81] 字符串替换
来源：http://jb.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pj.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://hg.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bp.bookmarksfly.cn

[Q83] 大小写转换
来源：http://sg.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nu.521024.cn

[Q84] 去除首尾空格
来源：http://xw.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://im.colortex.cn

[Q85] 数值取整
来源：http://ti.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wq.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://aa.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://us.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://jp.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sy.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://pa.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ru.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://os.9csxet.cn

[Q89] 判断表是否存在
来源：http://tm.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fn.colortex.cn

[Q90] 生成序号列
来源：http://ca.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wy.jianghongdianzi.cn

================================================================================
来源：http://bq.lnxyls.cn

R. Bash 专题
来源：http://sr.bookmarksfly.cn

================================================================================
来源：http://gg.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://bu.nicolike.cn

#!/usr/bin/env bash
来源：http://rl.newstarts.cn

set -euo pipefail
来源：http://be.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://wq.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://vf.hnjuh.cn

[R03] 只读变量
来源：http://uc.9csxet.cn

readonly PI=3.14
来源：http://tf.szxytkj.cn

[R04] 位置参数
来源：http://mi.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kf.huanxung.cn

[R05] 参数默认值
来源：http://qa.szxytkj.cn

name="${1:-default}"
来源：http://cp.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://iw.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zl.szxytkj.cn

[R07] if 判断文件
来源：http://jq.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cq.gzmigu.cn

[R08] 数值比较
来源：http://zj.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lj.shxzskj.cn

[R09] 字符串比较
来源：http://lb.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xh.colortex.cn

[R10] 正则匹配
来源：http://oy.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xp.nicolike.cn

[R11] case 多分支
来源：http://ao.asd995.cn

case "$1" in
来源：http://dy.huixiangedu.cn

start) echo "启动" ;;
来源：http://gd.nicolike.cn

stop)  echo "停止" ;;
来源：http://rn.colortex.cn

*)     echo "未知命令" ;;
来源：http://yy.szsharing.cn

esac
来源：http://gi.panjiajie.cn

[R12] for 遍历文件
来源：http://mr.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://ce.9csxet.cn

[R13] for 计数循环
来源：http://lv.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://dy.szsharing.cn

[R14] C 风格 for
来源：http://gy.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ao.nicolike.cn

[R15] while 逐行读文件
来源：http://nz.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wb.521024.cn

[R16] until 等待条件
来源：http://bo.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oy.asd995.cn

[R17] 数组定义与取值
来源：http://et.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fw.shxzskj.cn

[R18] 遍历数组
来源：http://jj.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vu.bookmarksfly.cn

[R19] 数组长度
来源：http://zh.lnxyls.cn

echo "${#arr[@]}"
来源：http://ya.gzmigu.cn

[R20] 关联数组（字典）
来源：http://ja.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fa.9csxet.cn

[R21] 字符串长度
来源：http://ty.jctech888.com.cn

echo "${#s}"
来源：http://iv.shxzskj.cn

[R22] 截取子串
来源：http://mp.hnjuh.cn

echo "${s:0:5}"
来源：http://pl.yuexingan06.cn

[R23] 字符串替换
来源：http://kp.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://my.wgjwhj.cn

[R24] 大小写转换
来源：http://lx.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xf.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://sc.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lc.haigaiapp.cn

[R26] 命令替换
来源：http://dw.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://bz.huixiangedu.cn

[R27] 算术展开
来源：http://ga.9csxet.cn

echo $((1 + 2 * 3))
来源：http://zl.521024.cn

[R28] 浮点运算
来源：http://dm.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://sk.bjjhwx.cn

[R29] 定义函数
来源：http://oi.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ql.shtwfgs.cn

[R30] 函数返回状态码
来源：http://ur.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://zs.9csxet.cn

[R31] 局部变量
来源：http://tw.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://kf.shxzukj.cn

[R32] 参数个数校验
来源：http://vn.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ot.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://ux.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tm.yuntaijiaju.cn

[R34] 退出时清理
来源：http://mh.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ig.shtwfgs.cn

[R35] 后台执行并等待
来源：http://fo.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ht.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://sj.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kc.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://js.muxihuayi.cn

files=$(ls -1)
来源：http://ma.panjiajie.cn

[R38] 管道串联
来源：http://rf.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://ny.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://ii.huanxung.cn

cmd > out.log 2>&1
来源：http://bx.lnxyls.cn

[R40] 追加写日志
来源：http://lo.lnxyls.cn

echo "log" >> out.log
来源：http://lb.bjjhwx.cn

[R41] 丢弃输出
来源：http://el.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://ad.szxytkj.cn

[R42] 输入重定向
来源：http://yk.colortex.cn

wc -l < a.txt
来源：http://ld.shxzukj.cn

[R43] 按名字查找文件
来源：http://wd.newstarts.cn

find . -name "*.log" -type f
来源：http://co.muxihuayi.cn

[R44] 按修改时间查找
来源：http://jt.shtwfgs.cn

find . -mtime -7 -type f
来源：http://sm.yuntaijiaju.cn

[R45] 批量删除
来源：http://km.nicolike.cn

find . -name "*.tmp" -delete
来源：http://sp.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://aq.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vc.521024.cn

[R47] sed 单行替换
来源：http://hz.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vr.shxzskj.cn

[R48] awk 取指定列
来源：http://fm.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://yv.shxzukj.cn

[R49] awk 带条件
来源：http://zx.yuexingan06.cn


<!-- 参考信息 -->