代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://zb.asd995.cn

[Q09] 创建唯一索引
来源：http://iv.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://go.bjjhwx.cn

[Q10] 插入单行
来源：http://px.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bi.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://pc.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ir.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://qb.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vv.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zq.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://vq.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ad.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://ex.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ot.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bz.bookmarksfly.cn

[Q15] 查询全部
来源：http://ca.huanxung.cn

SELECT * FROM users;
来源：http://ot.muxihuayi.cn

[Q16] 查询指定列
来源：http://xg.asd995.cn

SELECT id, name FROM users;
来源：http://cu.hahajie.cn

[Q17] 条件查询
来源：http://mr.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vk.9csxet.cn

[Q18] 模糊匹配
来源：http://wl.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://px.szsharing.cn

[Q19] 范围查询
来源：http://vq.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ul.szsharing.cn

[Q20] IN 列表
来源：http://kd.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pr.lnxyls.cn

[Q21] 空值判断
来源：http://lb.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bp.yuntaijiaju.cn

[Q22] 排序
来源：http://td.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ox.huanxung.cn

[Q23] 分页
来源：http://cv.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ng.szxytkj.cn

[Q24] 去重
来源：http://rj.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://vr.shxzskj.cn

[Q25] 只取前 N 条
来源：http://qt.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zu.shxzukj.cn

[Q26] 计数
来源：http://hh.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://am.hahajie.cn

[Q27] 条件计数
来源：http://cl.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fx.bjjhwx.cn

[Q28] 求和与平均
来源：http://jh.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rs.lnxyls.cn

[Q29] 最大最小值
来源：http://jg.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pe.newstarts.cn

[Q30] 分组统计
来源：http://gf.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fh.hnjuh.cn

[Q31] 分组后过滤
来源：http://ps.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dw.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://nd.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ak.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pc.huanxung.cn

[Q33] 多列分组
来源：http://hf.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://us.newstarts.cn

[Q34] 每组取第一条
来源：http://yx.bookmarksfly.cn

SELECT * FROM (
来源：http://zu.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rr.szxytkj.cn

) t WHERE rn = 1;
来源：http://pr.haigaiapp.cn

[Q35] 内连接
来源：http://mv.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lw.colortex.cn

[Q36] 左连接
来源：http://qb.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://um.bookmarksfly.cn

[Q37] 右连接
来源：http://jx.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://un.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wx.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://op.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://kr.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ev.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nu.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ys.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ho.jctech888.com.cn

[Q41] 多表连接
来源：http://us.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ya.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://vn.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://au.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://jr.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://xy.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nt.haigaiapp.cn

[Q43] 标量子查询
来源：http://ul.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ts.haigaiapp.cn

[Q44] IN 子查询
来源：http://yw.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pk.521024.cn

[Q45] EXISTS 判断存在
来源：http://ye.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dy.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ms.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fy.lnxyls.cn

[Q47] 与平均值比较
来源：http://em.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ti.colortex.cn

[Q48] CTE 公用表表达式
来源：http://jb.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ce.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://rj.shtwfgs.cn

[Q49] 更新单行
来源：http://ek.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ol.521024.cn

[Q50] 批量更新
来源：http://kq.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rw.szsharing.cn

[Q51] 用子查询更新
来源：http://tn.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zl.panjiajie.cn

[Q52] 删除指定行
来源：http://mw.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://ou.bjjhwx.cn

[Q53] 按条件删除
来源：http://zq.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zx.szsharing.cn

[Q54] 清空表
来源：http://pk.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://gn.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://yy.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qs.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://fv.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hg.521024.cn

[Q57] 行号
来源：http://nm.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mk.wgjwhj.cn

[Q58] 累计求和
来源：http://au.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aq.jctech888.com.cn

[Q59] 分组内累计
来源：http://th.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ym.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://qy.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ob.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fp.nicolike.cn

[Q61] 移动平均
来源：http://su.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dw.bookmarksfly.cn

[Q62] 分组占比
来源：http://ey.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ym.huixinmuqiang.cn

[Q63] 开启事务
来源：http://xh.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jh.bjjhwx.cn

[Q64] 提交事务
来源：http://ug.hnjuh.cn

COMMIT;
来源：http://ht.shxzskj.cn

[Q65] 回滚事务
来源：http://zc.nicolike.cn

ROLLBACK;
来源：http://cg.shxzukj.cn

[Q66] 行锁查询
来源：http://yp.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ja.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://yw.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cr.huixinmuqiang.cn

[Q68] 保存点
来源：http://hh.huanxung.cn

SAVEPOINT sp1;
来源：http://od.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://sd.yuexingan06.cn

[Q69] 查看执行计划
来源：http://kw.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vb.9csxet.cn

[Q70] 更新统计信息
来源：http://un.panjiajie.cn

ANALYZE TABLE users;
来源：http://lk.shtwfgs.cn

[Q71] 查看建表语句
来源：http://xh.huanxung.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xh.jianghongdianzi.cn

[Q72] 查看索引
来源：http://qf.szsharing.cn

SHOW INDEX FROM users;
来源：http://in.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://un.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nt.shtwfgs.cn

[Q74] 强制使用索引
来源：http://th.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vi.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://jv.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ip.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fw.hahajie.cn

[Q76] 按天统计
来源：http://yi.shtwfgs.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qw.haigaiapp.cn

[Q77] 时间加减
来源：http://oq.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gf.huixiangedu.cn

[Q78] 当前时间
来源：http://pt.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pw.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://cp.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xr.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://rm.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wk.newstarts.cn

[Q81] 字符串替换
来源：http://re.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gw.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://se.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sa.hnjuh.cn

[Q83] 大小写转换
来源：http://tq.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xx.hnjuh.cn

[Q84] 去除首尾空格
来源：http://tn.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://ca.asd995.cn

[Q85] 数值取整
来源：http://ku.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hk.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://fb.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ry.hahajie.cn

[Q87] JSON 字段做条件
来源：http://fy.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lo.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://di.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yp.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wv.hnjuh.cn

[Q89] 判断表是否存在
来源：http://my.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uw.yuexingan06.cn

[Q90] 生成序号列
来源：http://qe.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://md.jianghongdianzi.cn

================================================================================
来源：http://lx.521024.cn

R. Bash 专题
来源：http://rk.asd995.cn

================================================================================
来源：http://ce.szxytkj.cn

[R01] shebang 与严格模式
来源：http://ue.szsharing.cn

#!/usr/bin/env bash
来源：http://fm.bookmarksfly.cn

set -euo pipefail
来源：http://do.panjiajie.cn

[R02] 变量赋值与使用
来源：http://bk.szsharing.cn

name="Tom"; echo "$name"
来源：http://bg.szxytkj.cn

[R03] 只读变量
来源：http://vi.bookmarksfly.cn

readonly PI=3.14
来源：http://fl.colortex.cn

[R04] 位置参数
来源：http://ae.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lc.bjjhwx.cn

[R05] 参数默认值
来源：http://yk.bjjhwx.cn

name="${1:-default}"
来源：http://dz.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://df.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xn.chemitech.net.cn

[R07] if 判断文件
来源：http://wv.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gt.bookmarksfly.cn

[R08] 数值比较
来源：http://qt.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://th.yuntaijiaju.cn

[R09] 字符串比较
来源：http://nq.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ig.gzmigu.cn

[R10] 正则匹配
来源：http://pd.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ma.gzmigu.cn

[R11] case 多分支
来源：http://dg.shtwfgs.cn

case "$1" in
来源：http://ow.bookmarksfly.cn

start) echo "启动" ;;
来源：http://ls.szxytkj.cn

stop)  echo "停止" ;;
来源：http://cp.521024.cn

*)     echo "未知命令" ;;
来源：http://nt.huanxung.cn

esac
来源：http://ym.szsharing.cn

[R12] for 遍历文件
来源：http://dj.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://kj.chemitech.net.cn

[R13] for 计数循环
来源：http://eh.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://bd.chemitech.net.cn

[R14] C 风格 for
来源：http://uk.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qz.haigaiapp.cn

[R15] while 逐行读文件
来源：http://kg.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yi.asd995.cn

[R16] until 等待条件
来源：http://dj.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gg.jctech888.com.cn

[R17] 数组定义与取值
来源：http://gr.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dz.hahajie.cn

[R18] 遍历数组
来源：http://tx.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xu.haigaiapp.cn

[R19] 数组长度
来源：http://lu.gzmigu.cn

echo "${#arr[@]}"
来源：http://kx.nicolike.cn

[R20] 关联数组（字典）
来源：http://ke.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://it.jianghongdianzi.cn

[R21] 字符串长度
来源：http://ev.newstarts.cn

echo "${#s}"
来源：http://vi.bookmarksfly.cn

[R22] 截取子串
来源：http://ty.gzmigu.cn

echo "${s:0:5}"
来源：http://cb.jctech888.com.cn

[R23] 字符串替换
来源：http://dc.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gy.gzmigu.cn

[R24] 大小写转换
来源：http://mm.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lo.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://ou.lnxyls.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zu.muxihuayi.cn

[R26] 命令替换
来源：http://uo.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://en.muxihuayi.cn

[R27] 算术展开
来源：http://fm.huanxung.cn

echo $((1 + 2 * 3))
来源：http://ph.shxzukj.cn

[R28] 浮点运算
来源：http://so.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://qt.bookmarksfly.cn

[R29] 定义函数
来源：http://jo.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yg.yuntaijiaju.cn

[R30] 函数返回状态码
来源：http://sr.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://uq.shtwfgs.cn

[R31] 局部变量
来源：http://co.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://sj.hnjuh.cn

[R32] 参数个数校验
来源：http://gu.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kj.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://hj.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vg.lnxyls.cn

[R34] 退出时清理
来源：http://jv.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://am.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://tp.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dy.huanxung.cn

[R36] 并发执行多个任务
来源：http://ij.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fb.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://pt.chemitech.net.cn

files=$(ls -1)
来源：http://cr.shtwfgs.cn

[R38] 管道串联
来源：http://lw.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://ey.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://qj.newstarts.cn

cmd > out.log 2>&1
来源：http://mj.colortex.cn

[R40] 追加写日志
来源：http://zx.muxihuayi.cn

echo "log" >> out.log
来源：http://tb.nszjky.cn

[R41] 丢弃输出
来源：http://um.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://qz.jctech888.com.cn

[R42] 输入重定向
来源：http://nl.nicolike.cn

wc -l < a.txt
来源：http://yy.szxytkj.cn

[R43] 按名字查找文件
来源：http://nj.huanxung.cn

find . -name "*.log" -type f
来源：http://lj.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://uh.chemitech.net.cn

find . -mtime -7 -type f
来源：http://ii.shxzskj.cn

[R45] 批量删除
来源：http://pq.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://he.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://nn.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yc.hahajie.cn

[R47] sed 单行替换
来源：http://fg.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://eg.521024.cn

[R48] awk 取指定列
来源：http://tq.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://go.hahajie.cn

[R49] awk 带条件
来源：http://hx.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ua.hahajie.cn

[R50] awk 求和
来源：http://zg.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ro.shtwfgs.cn

[R51] 排序去重取前几
来源：http://bf.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hy.jianghongdianzi.cn

[R52] 统计行数
来源：http://ul.shxzukj.cn

wc -l a.txt
来源：http://zu.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://en.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wb.lnxyls.cn

[R54] 比较两个文件
来源：http://ij.wgjwhj.cn

diff a.txt b.txt
来源：http://yb.huanxung.cn

[R55] 压缩与解压
来源：http://tk.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ov.shxzukj.cn

[R56] 远程拷贝
来源：http://up.shxzskj.cn

scp file user@host:/path/
来源：http://kq.lnxyls.cn

[R57] 远程执行命令
来源：http://yb.colortex.cn


<!-- 参考信息 -->