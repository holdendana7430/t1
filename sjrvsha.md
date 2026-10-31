代发 wailian999

);
来源：http://id.shxzukj.cn

[Q03] 增加列
来源：http://ob.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ei.gzmigu.cn

[Q04] 修改列类型
来源：http://bd.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://li.huanxung.cn

[Q05] 重命名列
来源：http://ts.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vw.jianghongdianzi.cn

[Q06] 删除列
来源：http://pw.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dz.huixinmuqiang.cn

[Q07] 删除表
来源：http://hu.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://bu.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://od.huixinmuqiang.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ib.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://bg.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cl.jctech888.com.cn

[Q10] 插入单行
来源：http://ay.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://go.muxihuayi.cn

[Q11] 一次插入多行
来源：http://ak.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hb.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://ev.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pf.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fq.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://ae.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fq.shtwfgs.cn

[Q14] 存在则更新（upsert）
来源：http://xb.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zy.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gl.9csxet.cn

[Q15] 查询全部
来源：http://zt.haigaiapp.cn

SELECT * FROM users;
来源：http://eg.hnjuh.cn

[Q16] 查询指定列
来源：http://vx.szsharing.cn

SELECT id, name FROM users;
来源：http://ja.muxihuayi.cn

[Q17] 条件查询
来源：http://fg.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sc.nszjky.cn

[Q18] 模糊匹配
来源：http://zz.szsharing.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xp.asd995.cn

[Q19] 范围查询
来源：http://bi.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ta.lnxyls.cn

[Q20] IN 列表
来源：http://na.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sw.nicolike.cn

[Q21] 空值判断
来源：http://pp.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://th.colortex.cn

[Q22] 排序
来源：http://ws.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cy.521024.cn

[Q23] 分页
来源：http://at.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://np.asd995.cn

[Q24] 去重
来源：http://rw.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://ah.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://oo.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yn.newstarts.cn

[Q26] 计数
来源：http://nc.chemitech.net.cn

SELECT COUNT(*) FROM users;
来源：http://zs.huixiangedu.cn

[Q27] 条件计数
来源：http://jv.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://id.huanxung.cn

[Q28] 求和与平均
来源：http://vs.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gz.szxytkj.cn

[Q29] 最大最小值
来源：http://sr.9csxet.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pb.hahajie.cn

[Q30] 分组统计
来源：http://pl.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wx.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://xb.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oe.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://hb.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vf.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dm.wgjwhj.cn

[Q33] 多列分组
来源：http://lj.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ii.521024.cn

[Q34] 每组取第一条
来源：http://ex.hnjuh.cn

SELECT * FROM (
来源：http://nw.colortex.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lc.shxzukj.cn

) t WHERE rn = 1;
来源：http://rh.szxytkj.cn

[Q35] 内连接
来源：http://wu.bookmarksfly.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xd.huanxung.cn

[Q36] 左连接
来源：http://wi.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fc.jctech888.com.cn

[Q37] 右连接
来源：http://ax.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sv.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://by.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://og.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://kw.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oq.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pq.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sx.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zp.hahajie.cn

[Q41] 多表连接
来源：http://gv.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ea.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://jn.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://re.521024.cn

[Q42] 连接条件附加过滤
来源：http://eq.shtwfgs.cn

SELECT u.name, o.amount FROM users u
来源：http://gi.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ec.gzmigu.cn

[Q43] 标量子查询
来源：http://sc.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eo.521024.cn

[Q44] IN 子查询
来源：http://qm.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xh.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://rn.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cp.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rg.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://on.newstarts.cn

[Q47] 与平均值比较
来源：http://us.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ge.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://al.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://el.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://pn.hnjuh.cn

[Q49] 更新单行
来源：http://hm.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iz.hahajie.cn

[Q50] 批量更新
来源：http://ix.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mp.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://uu.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ug.szsharing.cn

[Q52] 删除指定行
来源：http://ih.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://ld.huanxung.cn

[Q53] 按条件删除
来源：http://ao.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kv.bjjhwx.cn

[Q54] 清空表
来源：http://md.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://jg.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://uj.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mu.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://qi.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sj.asd995.cn

[Q57] 行号
来源：http://yj.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ut.jianghongdianzi.cn

[Q58] 累计求和
来源：http://yo.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hi.jctech888.com.cn

[Q59] 分组内累计
来源：http://wc.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yr.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://ri.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://va.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vj.nicolike.cn

[Q61] 移动平均
来源：http://je.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ck.colortex.cn

[Q62] 分组占比
来源：http://sb.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qo.521024.cn

[Q63] 开启事务
来源：http://pa.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kl.nicolike.cn

[Q64] 提交事务
来源：http://kt.bjjhwx.cn

COMMIT;
来源：http://ek.bookmarksfly.cn

[Q65] 回滚事务
来源：http://uz.newstarts.cn

ROLLBACK;
来源：http://ws.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://ve.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://to.521024.cn

[Q67] 设置隔离级别
来源：http://en.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://za.huixiangedu.cn

[Q68] 保存点
来源：http://mb.lnxyls.cn

SAVEPOINT sp1;
来源：http://lm.521024.cn

ROLLBACK TO sp1;
来源：http://ra.chemitech.net.cn

[Q69] 查看执行计划
来源：http://pw.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sj.chemitech.net.cn

[Q70] 更新统计信息
来源：http://hk.wgjwhj.cn

ANALYZE TABLE users;
来源：http://tm.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://sh.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ja.chemitech.net.cn

[Q72] 查看索引
来源：http://qn.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://lo.lnxyls.cn

[Q73] 查看表状态
来源：http://af.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hf.hnjuh.cn

[Q74] 强制使用索引
来源：http://dp.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pk.shxzskj.cn

[Q75] 日期格式化
来源：http://gz.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zn.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pq.nszjky.cn

[Q76] 按天统计
来源：http://we.shtwfgs.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://re.hnjuh.cn

[Q77] 时间加减
来源：http://it.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://px.muxihuayi.cn

[Q78] 当前时间
来源：http://lj.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cj.szsharing.cn

[Q79] 字符串拼接
来源：http://wi.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bd.panjiajie.cn

[Q80] 字符串截取
来源：http://tf.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pv.panjiajie.cn

[Q81] 字符串替换
来源：http://qd.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nd.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://ft.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zn.nszjky.cn

[Q83] 大小写转换
来源：http://ns.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cp.huanxung.cn

[Q84] 去除首尾空格
来源：http://fz.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://gd.lnxyls.cn

[Q85] 数值取整
来源：http://ev.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lt.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://hk.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dd.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://xc.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eo.521024.cn

[Q88] 行转列（条件聚合）
来源：http://do.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gq.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hs.asd995.cn

[Q89] 判断表是否存在
来源：http://yy.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lh.colortex.cn

[Q90] 生成序号列
来源：http://ea.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ge.muxihuayi.cn

================================================================================
来源：http://yu.colortex.cn

R. Bash 专题
来源：http://wc.huixinmuqiang.cn

================================================================================
来源：http://ia.shxzukj.cn

[R01] shebang 与严格模式
来源：http://qe.muxihuayi.cn

#!/usr/bin/env bash
来源：http://gg.muxihuayi.cn

set -euo pipefail
来源：http://hj.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://bz.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://hr.newstarts.cn

[R03] 只读变量
来源：http://xh.521024.cn

readonly PI=3.14
来源：http://ny.haigaiapp.cn

[R04] 位置参数
来源：http://xq.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fb.huixiangedu.cn

[R05] 参数默认值
来源：http://se.huanxung.cn

name="${1:-default}"
来源：http://mw.newstarts.cn

[R06] 判断命令是否存在
来源：http://wr.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hg.jianghongdianzi.cn

[R07] if 判断文件
来源：http://us.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vb.colortex.cn

[R08] 数值比较
来源：http://mq.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cj.colortex.cn

[R09] 字符串比较
来源：http://db.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qb.colortex.cn

[R10] 正则匹配
来源：http://wu.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qe.nszjky.cn

[R11] case 多分支
来源：http://fv.szxytkj.cn

case "$1" in
来源：http://js.colortex.cn

start) echo "启动" ;;
来源：http://ex.hahajie.cn

stop)  echo "停止" ;;
来源：http://vl.colortex.cn

*)     echo "未知命令" ;;
来源：http://an.huixiangedu.cn

esac
来源：http://ii.asd995.cn

[R12] for 遍历文件
来源：http://ye.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://wa.asd995.cn

[R13] for 计数循环
来源：http://hd.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://gp.hnjuh.cn

[R14] C 风格 for
来源：http://ek.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mi.shxzukj.cn

[R15] while 逐行读文件
来源：http://bc.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nz.newstarts.cn

[R16] until 等待条件
来源：http://xo.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ia.huanxung.cn

[R17] 数组定义与取值
来源：http://am.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bg.panjiajie.cn

[R18] 遍历数组
来源：http://sv.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bn.521024.cn

[R19] 数组长度
来源：http://zg.muxihuayi.cn

echo "${#arr[@]}"
来源：http://cp.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://pv.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ev.szsharing.cn

[R21] 字符串长度
来源：http://jd.yuntaijiaju.cn

echo "${#s}"
来源：http://hq.huixinmuqiang.cn

[R22] 截取子串
来源：http://nm.nicolike.cn

echo "${s:0:5}"
来源：http://fy.lnxyls.cn

[R23] 字符串替换
来源：http://vc.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uf.521024.cn

[R24] 大小写转换
来源：http://tr.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bu.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://we.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ky.yuexingan06.cn

[R26] 命令替换
来源：http://js.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://lx.hahajie.cn

[R27] 算术展开
来源：http://hc.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://aa.newstarts.cn

[R28] 浮点运算
来源：http://ho.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://xb.nszjky.cn

[R29] 定义函数
来源：http://sd.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dq.gzmigu.cn

[R30] 函数返回状态码
来源：http://ly.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://mq.hnjuh.cn

[R31] 局部变量
来源：http://jj.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://zk.gzmigu.cn

[R32] 参数个数校验
来源：http://su.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lb.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://vi.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pd.hahajie.cn

[R34] 退出时清理
来源：http://bk.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ud.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://lu.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xr.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://jx.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rk.hahajie.cn

[R37] 把输出赋给变量
来源：http://kz.hahajie.cn

files=$(ls -1)
来源：http://ll.newstarts.cn

[R38] 管道串联
来源：http://pv.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://bw.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://hz.nicolike.cn

cmd > out.log 2>&1
来源：http://vo.haigaiapp.cn

[R40] 追加写日志
来源：http://ve.bjjhwx.cn

echo "log" >> out.log
来源：http://xt.bookmarksfly.cn

[R41] 丢弃输出
来源：http://dx.nicolike.cn

cmd >/dev/null 2>&1
来源：http://cr.huixinmuqiang.cn

[R42] 输入重定向
来源：http://ro.huixinmuqiang.cn

wc -l < a.txt
来源：http://an.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://yh.9csxet.cn

find . -name "*.log" -type f
来源：http://pg.newstarts.cn

[R44] 按修改时间查找
来源：http://yo.hahajie.cn

find . -mtime -7 -type f
来源：http://zh.wgjwhj.cn

[R45] 批量删除
来源：http://be.colortex.cn

find . -name "*.tmp" -delete
来源：http://xj.9csxet.cn

[R46] 递归替换文件内容
来源：http://pg.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jk.newstarts.cn

[R47] sed 单行替换
来源：http://hf.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://og.hahajie.cn

[R48] awk 取指定列
来源：http://vz.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://up.shxzukj.cn

[R49] awk 带条件
来源：http://jh.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zo.szsharing.cn

[R50] awk 求和
来源：http://nl.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rc.wgjwhj.cn

[R51] 排序去重取前几
来源：http://dx.bjjhwx.cn


<!-- 参考信息 -->