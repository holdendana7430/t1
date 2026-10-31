代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ej.haigaiapp.cn

[Q05] 重命名列
来源：http://ez.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vp.muxihuayi.cn

[Q06] 删除列
来源：http://dl.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kk.bjjhwx.cn

[Q07] 删除表
来源：http://uo.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://tr.yuexingan06.cn

[Q08] 创建普通索引
来源：http://cc.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jz.panjiajie.cn

[Q09] 创建唯一索引
来源：http://an.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eu.yuntaijiaju.cn

[Q10] 插入单行
来源：http://qf.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ik.newstarts.cn

[Q11] 一次插入多行
来源：http://zv.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xd.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://ls.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yf.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jp.asd995.cn

[Q13] 忽略重复插入
来源：http://tl.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gr.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://as.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ti.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vx.colortex.cn

[Q15] 查询全部
来源：http://kj.gzmigu.cn

SELECT * FROM users;
来源：http://aq.newstarts.cn

[Q16] 查询指定列
来源：http://jp.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://kq.bjjhwx.cn

[Q17] 条件查询
来源：http://vb.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ux.nszjky.cn

[Q18] 模糊匹配
来源：http://bh.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wo.wgjwhj.cn

[Q19] 范围查询
来源：http://kk.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ls.panjiajie.cn

[Q20] IN 列表
来源：http://bz.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qu.hahajie.cn

[Q21] 空值判断
来源：http://ha.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vh.gzmigu.cn

[Q22] 排序
来源：http://ic.newstarts.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ji.huanxung.cn

[Q23] 分页
来源：http://es.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hn.shxzskj.cn

[Q24] 去重
来源：http://fs.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://iw.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://ep.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gt.panjiajie.cn

[Q26] 计数
来源：http://ti.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://np.newstarts.cn

[Q27] 条件计数
来源：http://af.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xa.haigaiapp.cn

[Q28] 求和与平均
来源：http://vl.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pd.haigaiapp.cn

[Q29] 最大最小值
来源：http://om.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cv.haigaiapp.cn

[Q30] 分组统计
来源：http://av.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sw.szxytkj.cn

[Q31] 分组后过滤
来源：http://ox.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pc.colortex.cn

[Q32] 分组拼接字符串
来源：http://je.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fv.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zx.huanxung.cn

[Q33] 多列分组
来源：http://ww.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qr.shxzskj.cn

[Q34] 每组取第一条
来源：http://hc.jianghongdianzi.cn

SELECT * FROM (
来源：http://yu.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fc.muxihuayi.cn

) t WHERE rn = 1;
来源：http://wf.bjjhwx.cn

[Q35] 内连接
来源：http://br.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wi.haigaiapp.cn

[Q36] 左连接
来源：http://tr.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vt.jctech888.com.cn

[Q37] 右连接
来源：http://vu.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pw.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://et.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wb.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://fh.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xk.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lm.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hv.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pb.yuexingan06.cn

[Q41] 多表连接
来源：http://hs.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qn.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://zd.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://mw.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://qc.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://ul.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qk.hnjuh.cn

[Q43] 标量子查询
来源：http://kf.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ge.muxihuayi.cn

[Q44] IN 子查询
来源：http://xz.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ku.colortex.cn

[Q45] EXISTS 判断存在
来源：http://kw.huixiangedu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rq.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vc.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bh.nicolike.cn

[Q47] 与平均值比较
来源：http://up.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ix.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://zz.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xz.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://da.nicolike.cn

[Q49] 更新单行
来源：http://ci.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lv.jianghongdianzi.cn

[Q50] 批量更新
来源：http://zf.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ij.asd995.cn

[Q51] 用子查询更新
来源：http://yn.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ok.9csxet.cn

[Q52] 删除指定行
来源：http://om.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://ke.shxzukj.cn

[Q53] 按条件删除
来源：http://bp.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://de.gzmigu.cn

[Q54] 清空表
来源：http://sb.nicolike.cn

TRUNCATE TABLE logs;
来源：http://sh.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://av.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vw.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://aj.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fl.panjiajie.cn

[Q57] 行号
来源：http://dl.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lj.bjjhwx.cn

[Q58] 累计求和
来源：http://jy.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ne.colortex.cn

[Q59] 分组内累计
来源：http://ey.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rz.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://hx.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cl.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qt.szsharing.cn

[Q61] 移动平均
来源：http://tm.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ux.shtwfgs.cn

[Q62] 分组占比
来源：http://fn.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cz.wgjwhj.cn

[Q63] 开启事务
来源：http://jb.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xn.bjjhwx.cn

[Q64] 提交事务
来源：http://zf.bjjhwx.cn

COMMIT;
来源：http://cj.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://rs.huixinmuqiang.cn

ROLLBACK;
来源：http://cf.shxzukj.cn

[Q66] 行锁查询
来源：http://jq.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ar.colortex.cn

[Q67] 设置隔离级别
来源：http://ws.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uo.shtwfgs.cn

[Q68] 保存点
来源：http://to.nszjky.cn

SAVEPOINT sp1;
来源：http://iz.colortex.cn

ROLLBACK TO sp1;
来源：http://dh.huixiangedu.cn

[Q69] 查看执行计划
来源：http://qr.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zb.chemitech.net.cn

[Q70] 更新统计信息
来源：http://nm.panjiajie.cn

ANALYZE TABLE users;
来源：http://sr.wgjwhj.cn

[Q71] 查看建表语句
来源：http://dk.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vs.gzmigu.cn

[Q72] 查看索引
来源：http://az.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://zm.chemitech.net.cn

[Q73] 查看表状态
来源：http://xb.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nr.bjjhwx.cn

[Q74] 强制使用索引
来源：http://dz.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vs.bjjhwx.cn

[Q75] 日期格式化
来源：http://bk.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lm.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wh.newstarts.cn

[Q76] 按天统计
来源：http://iv.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rj.szsharing.cn

[Q77] 时间加减
来源：http://ua.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gq.shtwfgs.cn

[Q78] 当前时间
来源：http://dz.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sj.shxzukj.cn

[Q79] 字符串拼接
来源：http://vx.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oq.jctech888.com.cn

[Q80] 字符串截取
来源：http://md.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zm.lnxyls.cn

[Q81] 字符串替换
来源：http://zz.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ft.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://yx.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ju.yuexingan06.cn

[Q83] 大小写转换
来源：http://ho.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ul.nicolike.cn

[Q84] 去除首尾空格
来源：http://yr.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://rg.hahajie.cn

[Q85] 数值取整
来源：http://dz.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ot.521024.cn

[Q86] 读取 JSON 字段
来源：http://uq.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fc.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://pz.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://he.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://da.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://su.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sx.hnjuh.cn

[Q89] 判断表是否存在
来源：http://nv.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uk.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://pb.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kn.hahajie.cn

================================================================================
来源：http://hx.muxihuayi.cn

R. Bash 专题
来源：http://mh.panjiajie.cn

================================================================================
来源：http://fa.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://xz.shxzskj.cn

#!/usr/bin/env bash
来源：http://gi.yuexingan06.cn

set -euo pipefail
来源：http://sj.gzmigu.cn

[R02] 变量赋值与使用
来源：http://kq.hahajie.cn

name="Tom"; echo "$name"
来源：http://wd.hnjuh.cn

[R03] 只读变量
来源：http://zr.hahajie.cn

readonly PI=3.14
来源：http://ka.huixiangedu.cn

[R04] 位置参数
来源：http://yz.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qj.newstarts.cn

[R05] 参数默认值
来源：http://wm.521024.cn

name="${1:-default}"
来源：http://dx.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://gx.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://au.hnjuh.cn

[R07] if 判断文件
来源：http://yz.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nx.hnjuh.cn

[R08] 数值比较
来源：http://jv.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fu.bjjhwx.cn

[R09] 字符串比较
来源：http://ci.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qk.huixinmuqiang.cn

[R10] 正则匹配
来源：http://lc.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ju.shtwfgs.cn

[R11] case 多分支
来源：http://hl.yuexingan06.cn

case "$1" in
来源：http://kf.521024.cn

start) echo "启动" ;;
来源：http://cp.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://bi.hahajie.cn

*)     echo "未知命令" ;;
来源：http://cy.huixinmuqiang.cn

esac
来源：http://gp.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://nt.bjjhwx.cn

for f in *.txt; do echo "$f"; done
来源：http://vh.521024.cn

[R13] for 计数循环
来源：http://kt.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://dx.jianghongdianzi.cn

[R14] C 风格 for
来源：http://ha.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vd.asd995.cn

[R15] while 逐行读文件
来源：http://vs.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://un.newstarts.cn

[R16] until 等待条件
来源：http://yj.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rw.szxytkj.cn

[R17] 数组定义与取值
来源：http://zo.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ab.szsharing.cn

[R18] 遍历数组
来源：http://da.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ar.shxzukj.cn

[R19] 数组长度
来源：http://wt.wgjwhj.cn

echo "${#arr[@]}"
来源：http://fp.newstarts.cn

[R20] 关联数组（字典）
来源：http://zw.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sd.huixiangedu.cn

[R21] 字符串长度
来源：http://qm.521024.cn

echo "${#s}"
来源：http://ou.huixiangedu.cn

[R22] 截取子串
来源：http://ed.shxzskj.cn

echo "${s:0:5}"
来源：http://iy.newstarts.cn

[R23] 字符串替换
来源：http://dr.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ny.lnxyls.cn

[R24] 大小写转换
来源：http://xi.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kz.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://yb.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hs.panjiajie.cn

[R26] 命令替换
来源：http://pp.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://mb.hnjuh.cn

[R27] 算术展开
来源：http://hw.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://ul.panjiajie.cn

[R28] 浮点运算
来源：http://hq.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://yx.szsharing.cn

[R29] 定义函数
来源：http://ni.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bg.haigaiapp.cn

[R30] 函数返回状态码
来源：http://av.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://kf.wgjwhj.cn

[R31] 局部变量
来源：http://od.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://dr.lnxyls.cn

[R32] 参数个数校验
来源：http://uu.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nt.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://nl.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hs.nszjky.cn

[R34] 退出时清理
来源：http://so.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lm.asd995.cn

[R35] 后台执行并等待
来源：http://fq.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lw.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://kn.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xt.hnjuh.cn

[R37] 把输出赋给变量
来源：http://ed.9csxet.cn

files=$(ls -1)
来源：http://zt.chemitech.net.cn

[R38] 管道串联
来源：http://po.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://he.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://ut.wgjwhj.cn

cmd > out.log 2>&1
来源：http://ns.yuexingan06.cn

[R40] 追加写日志
来源：http://li.bjjhwx.cn

echo "log" >> out.log
来源：http://nc.gzmigu.cn

[R41] 丢弃输出
来源：http://dx.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://hw.chemitech.net.cn

[R42] 输入重定向
来源：http://vi.wgjwhj.cn

wc -l < a.txt
来源：http://ro.hnjuh.cn

[R43] 按名字查找文件
来源：http://nq.colortex.cn

find . -name "*.log" -type f
来源：http://zt.huanxung.cn

[R44] 按修改时间查找
来源：http://bd.shtwfgs.cn

find . -mtime -7 -type f
来源：http://il.bookmarksfly.cn

[R45] 批量删除
来源：http://wy.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://om.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://gb.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jo.newstarts.cn

[R47] sed 单行替换
来源：http://te.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sf.nicolike.cn

[R48] awk 取指定列
来源：http://vf.521024.cn

awk '{print $1, $3}' a.txt
来源：http://wz.yuexingan06.cn

[R49] awk 带条件
来源：http://bz.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://um.9csxet.cn

[R50] awk 求和
来源：http://uo.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://az.chemitech.net.cn

[R51] 排序去重取前几
来源：http://cl.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lp.asd995.cn

[R52] 统计行数
来源：http://lb.asd995.cn

wc -l a.txt
来源：http://zn.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://fs.muxihuayi.cn


<!-- 参考信息 -->