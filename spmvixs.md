代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xy.hahajie.cn

user_id INT NOT NULL,
来源：http://nf.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://fn.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vm.huixinmuqiang.cn

);
来源：http://mn.szxytkj.cn

[Q03] 增加列
来源：http://gy.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xx.panjiajie.cn

[Q04] 修改列类型
来源：http://jr.shxzukj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mz.shxzukj.cn

[Q05] 重命名列
来源：http://pz.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ag.bjjhwx.cn

[Q06] 删除列
来源：http://cf.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ez.nicolike.cn

[Q07] 删除表
来源：http://zz.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://bf.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://js.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kn.hnjuh.cn

[Q09] 创建唯一索引
来源：http://bk.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gj.hahajie.cn

[Q10] 插入单行
来源：http://vu.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ii.9csxet.cn

[Q11] 一次插入多行
来源：http://ki.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://if.521024.cn

[Q12] 插入后取自增 ID
来源：http://cx.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qg.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mf.newstarts.cn

[Q13] 忽略重复插入
来源：http://wk.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xv.521024.cn

[Q14] 存在则更新（upsert）
来源：http://ro.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fw.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qr.szxytkj.cn

[Q15] 查询全部
来源：http://tk.panjiajie.cn

SELECT * FROM users;
来源：http://wm.nicolike.cn

[Q16] 查询指定列
来源：http://pd.521024.cn

SELECT id, name FROM users;
来源：http://vi.jctech888.com.cn

[Q17] 条件查询
来源：http://vr.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tb.muxihuayi.cn

[Q18] 模糊匹配
来源：http://lh.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mg.wgjwhj.cn

[Q19] 范围查询
来源：http://qk.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://od.yuntaijiaju.cn

[Q20] IN 列表
来源：http://ws.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://es.nszjky.cn

[Q21] 空值判断
来源：http://lo.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://va.bjjhwx.cn

[Q22] 排序
来源：http://vr.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fz.lnxyls.cn

[Q23] 分页
来源：http://ez.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gf.newstarts.cn

[Q24] 去重
来源：http://yc.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://ie.hnjuh.cn

[Q25] 只取前 N 条
来源：http://nl.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kb.shtwfgs.cn

[Q26] 计数
来源：http://zd.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://nu.haigaiapp.cn

[Q27] 条件计数
来源：http://iv.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tf.shtwfgs.cn

[Q28] 求和与平均
来源：http://xr.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dg.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://nd.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lt.szsharing.cn

[Q30] 分组统计
来源：http://yr.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vm.newstarts.cn

[Q31] 分组后过滤
来源：http://xc.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zc.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://mk.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gd.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qj.haigaiapp.cn

[Q33] 多列分组
来源：http://yl.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dc.szsharing.cn

[Q34] 每组取第一条
来源：http://lr.hahajie.cn

SELECT * FROM (
来源：http://bc.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iz.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://dl.hnjuh.cn

[Q35] 内连接
来源：http://wa.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ki.yuntaijiaju.cn

[Q36] 左连接
来源：http://ox.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qv.521024.cn

[Q37] 右连接
来源：http://xk.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jb.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gc.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fq.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://nv.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ct.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zr.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tx.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pd.gzmigu.cn

[Q41] 多表连接
来源：http://yq.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ks.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://ki.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://ct.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://qi.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://ux.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wx.shtwfgs.cn

[Q43] 标量子查询
来源：http://ac.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bc.muxihuayi.cn

[Q44] IN 子查询
来源：http://ar.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zo.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://xg.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dc.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wk.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vg.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://ol.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xp.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://nv.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hh.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://rb.huixinmuqiang.cn

[Q49] 更新单行
来源：http://qy.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ki.nszjky.cn

[Q50] 批量更新
来源：http://od.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vb.shxzukj.cn

[Q51] 用子查询更新
来源：http://su.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vh.nicolike.cn

[Q52] 删除指定行
来源：http://yq.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://kz.muxihuayi.cn

[Q53] 按条件删除
来源：http://ct.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oc.asd995.cn

[Q54] 清空表
来源：http://ql.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://hi.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://rs.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pm.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://ag.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://in.bookmarksfly.cn

[Q57] 行号
来源：http://nm.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tj.jctech888.com.cn

[Q58] 累计求和
来源：http://dl.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jd.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://pg.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://he.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://bi.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pl.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rx.huanxung.cn

[Q61] 移动平均
来源：http://ls.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wv.huixiangedu.cn

[Q62] 分组占比
来源：http://xx.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ob.szsharing.cn

[Q63] 开启事务
来源：http://ep.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yd.szsharing.cn

[Q64] 提交事务
来源：http://ab.lnxyls.cn

COMMIT;
来源：http://sp.gzmigu.cn

[Q65] 回滚事务
来源：http://jf.haigaiapp.cn

ROLLBACK;
来源：http://jk.bjjhwx.cn

[Q66] 行锁查询
来源：http://cn.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pc.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://dc.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bq.newstarts.cn

[Q68] 保存点
来源：http://ta.hahajie.cn

SAVEPOINT sp1;
来源：http://jk.szsharing.cn

ROLLBACK TO sp1;
来源：http://ek.hnjuh.cn

[Q69] 查看执行计划
来源：http://ye.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ts.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://hy.panjiajie.cn

ANALYZE TABLE users;
来源：http://ra.shxzukj.cn

[Q71] 查看建表语句
来源：http://st.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eu.shxzukj.cn

[Q72] 查看索引
来源：http://yq.gzmigu.cn

SHOW INDEX FROM users;
来源：http://qi.huanxung.cn

[Q73] 查看表状态
来源：http://mh.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jb.panjiajie.cn

[Q74] 强制使用索引
来源：http://ts.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vo.szsharing.cn

[Q75] 日期格式化
来源：http://yj.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vm.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qy.nicolike.cn

[Q76] 按天统计
来源：http://hz.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ev.haigaiapp.cn

[Q77] 时间加减
来源：http://rl.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mq.colortex.cn

[Q78] 当前时间
来源：http://hy.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://db.szsharing.cn

[Q79] 字符串拼接
来源：http://lh.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bw.haigaiapp.cn

[Q80] 字符串截取
来源：http://gy.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bx.jianghongdianzi.cn

[Q81] 字符串替换
来源：http://dt.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lw.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://vw.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://av.huanxung.cn

[Q83] 大小写转换
来源：http://de.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eu.hahajie.cn

[Q84] 去除首尾空格
来源：http://ku.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://je.huanxung.cn

[Q85] 数值取整
来源：http://gp.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ai.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://zh.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uk.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://bn.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ql.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://gh.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sr.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eo.hahajie.cn

[Q89] 判断表是否存在
来源：http://gb.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ob.panjiajie.cn

[Q90] 生成序号列
来源：http://kc.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vw.haigaiapp.cn

================================================================================
来源：http://vv.521024.cn

R. Bash 专题
来源：http://eh.huixinmuqiang.cn

================================================================================
来源：http://zm.hnjuh.cn

[R01] shebang 与严格模式
来源：http://lo.wgjwhj.cn

#!/usr/bin/env bash
来源：http://wv.chemitech.net.cn

set -euo pipefail
来源：http://ei.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://ce.nicolike.cn

name="Tom"; echo "$name"
来源：http://hb.colortex.cn

[R03] 只读变量
来源：http://hr.huixiangedu.cn

readonly PI=3.14
来源：http://od.shxzskj.cn

[R04] 位置参数
来源：http://id.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sb.jianghongdianzi.cn

[R05] 参数默认值
来源：http://mz.yuexingan06.cn

name="${1:-default}"
来源：http://gj.shxzskj.cn

[R06] 判断命令是否存在
来源：http://da.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iz.huixinmuqiang.cn

[R07] if 判断文件
来源：http://dm.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jm.huixinmuqiang.cn

[R08] 数值比较
来源：http://nh.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://an.yuntaijiaju.cn

[R09] 字符串比较
来源：http://rl.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tk.bookmarksfly.cn

[R10] 正则匹配
来源：http://df.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wn.shxzukj.cn

[R11] case 多分支
来源：http://ph.newstarts.cn

case "$1" in
来源：http://ls.haigaiapp.cn

start) echo "启动" ;;
来源：http://ep.nszjky.cn

stop)  echo "停止" ;;
来源：http://mo.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://yt.muxihuayi.cn

esac
来源：http://ii.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://zb.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://kj.bookmarksfly.cn

[R13] for 计数循环
来源：http://uv.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://nm.nicolike.cn

[R14] C 风格 for
来源：http://wk.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xc.lnxyls.cn

[R15] while 逐行读文件
来源：http://et.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://is.huixinmuqiang.cn

[R16] until 等待条件
来源：http://wq.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iy.shxzskj.cn

[R17] 数组定义与取值
来源：http://av.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pu.haigaiapp.cn

[R18] 遍历数组
来源：http://pc.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ao.panjiajie.cn

[R19] 数组长度
来源：http://mc.gzmigu.cn

echo "${#arr[@]}"
来源：http://yn.szsharing.cn

[R20] 关联数组（字典）
来源：http://ob.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dx.9csxet.cn

[R21] 字符串长度
来源：http://my.bookmarksfly.cn

echo "${#s}"
来源：http://pd.newstarts.cn

[R22] 截取子串
来源：http://ee.szxytkj.cn

echo "${s:0:5}"
来源：http://up.chemitech.net.cn

[R23] 字符串替换
来源：http://pv.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rs.panjiajie.cn

[R24] 大小写转换
来源：http://nx.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ma.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://xv.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hp.colortex.cn

[R26] 命令替换
来源：http://nz.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://yv.yuexingan06.cn

[R27] 算术展开
来源：http://ut.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://ce.szxytkj.cn

[R28] 浮点运算
来源：http://ne.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://ho.szxytkj.cn

[R29] 定义函数
来源：http://ib.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mg.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://aw.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://zb.gzmigu.cn

[R31] 局部变量
来源：http://qh.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://md.hahajie.cn

[R32] 参数个数校验
来源：http://zh.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mh.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://ju.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tk.nszjky.cn

[R34] 退出时清理
来源：http://rp.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ac.szxytkj.cn

[R35] 后台执行并等待
来源：http://qp.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zt.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://pk.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rw.newstarts.cn

[R37] 把输出赋给变量
来源：http://ud.muxihuayi.cn

files=$(ls -1)
来源：http://fx.shxzukj.cn

[R38] 管道串联
来源：http://ts.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://uu.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://za.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://du.shtwfgs.cn

[R40] 追加写日志
来源：http://ln.huanxung.cn

echo "log" >> out.log
来源：http://ie.colortex.cn

[R41] 丢弃输出
来源：http://pk.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://jn.yuntaijiaju.cn

[R42] 输入重定向
来源：http://ue.newstarts.cn

wc -l < a.txt
来源：http://st.hahajie.cn

[R43] 按名字查找文件
来源：http://bu.newstarts.cn

find . -name "*.log" -type f
来源：http://in.huixiangedu.cn

[R44] 按修改时间查找
来源：http://nt.huixiangedu.cn

find . -mtime -7 -type f
来源：http://nl.wgjwhj.cn

[R45] 批量删除
来源：http://ib.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://ti.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://mh.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ck.colortex.cn

[R47] sed 单行替换
来源：http://wa.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ax.521024.cn

[R48] awk 取指定列
来源：http://um.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://rh.szxytkj.cn

[R49] awk 带条件
来源：http://dc.muxihuayi.cn


<!-- 参考信息 -->