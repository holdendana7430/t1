代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://mi.panjiajie.cn

[Q07] 删除表
来源：http://tn.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://up.asd995.cn

[Q08] 创建普通索引
来源：http://il.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hd.shxzukj.cn

[Q09] 创建唯一索引
来源：http://kd.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ph.shxzskj.cn

[Q10] 插入单行
来源：http://ge.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jd.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://ay.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cn.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://pg.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hl.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oh.521024.cn

[Q13] 忽略重复插入
来源：http://pw.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uc.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://lq.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hm.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://am.jianghongdianzi.cn

[Q15] 查询全部
来源：http://cq.huixiangedu.cn

SELECT * FROM users;
来源：http://de.szxytkj.cn

[Q16] 查询指定列
来源：http://zp.bjjhwx.cn

SELECT id, name FROM users;
来源：http://at.bookmarksfly.cn

[Q17] 条件查询
来源：http://nn.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vs.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://qy.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ag.huixiangedu.cn

[Q19] 范围查询
来源：http://op.shxzukj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ek.bookmarksfly.cn

[Q20] IN 列表
来源：http://oh.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jf.nszjky.cn

[Q21] 空值判断
来源：http://cl.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://oj.hahajie.cn

[Q22] 排序
来源：http://jo.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wg.szsharing.cn

[Q23] 分页
来源：http://iw.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ic.bjjhwx.cn

[Q24] 去重
来源：http://kk.huixiangedu.cn

SELECT DISTINCT city FROM users;
来源：http://jx.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://as.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hs.asd995.cn

[Q26] 计数
来源：http://gd.521024.cn

SELECT COUNT(*) FROM users;
来源：http://gm.asd995.cn

[Q27] 条件计数
来源：http://rj.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ix.huixiangedu.cn

[Q28] 求和与平均
来源：http://gp.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://or.gzmigu.cn

[Q29] 最大最小值
来源：http://gd.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kq.newstarts.cn

[Q30] 分组统计
来源：http://rc.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ln.nszjky.cn

[Q31] 分组后过滤
来源：http://dn.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wi.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://ol.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vi.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ze.szxytkj.cn

[Q33] 多列分组
来源：http://vz.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bz.bjjhwx.cn

[Q34] 每组取第一条
来源：http://fo.muxihuayi.cn

SELECT * FROM (
来源：http://mw.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lv.wgjwhj.cn

) t WHERE rn = 1;
来源：http://kj.huanxung.cn

[Q35] 内连接
来源：http://yn.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mg.bookmarksfly.cn

[Q36] 左连接
来源：http://en.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kf.hnjuh.cn

[Q37] 右连接
来源：http://vb.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mc.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mt.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://at.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://hd.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://he.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yo.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rm.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://on.nszjky.cn

[Q41] 多表连接
来源：http://pt.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vq.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://fd.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://bf.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://ii.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://du.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ao.hnjuh.cn

[Q43] 标量子查询
来源：http://nw.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jo.szxytkj.cn

[Q44] IN 子查询
来源：http://ht.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nt.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://hc.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nx.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hq.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ct.szsharing.cn

[Q47] 与平均值比较
来源：http://ax.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sq.asd995.cn

[Q48] CTE 公用表表达式
来源：http://an.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gb.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://av.jctech888.com.cn

[Q49] 更新单行
来源：http://bf.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gt.szxytkj.cn

[Q50] 批量更新
来源：http://pk.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wq.521024.cn

[Q51] 用子查询更新
来源：http://we.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bm.huanxung.cn

[Q52] 删除指定行
来源：http://bf.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://tr.nszjky.cn

[Q53] 按条件删除
来源：http://fx.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://da.nicolike.cn

[Q54] 清空表
来源：http://az.9csxet.cn

TRUNCATE TABLE logs;
来源：http://yr.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://aj.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dd.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://wp.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://co.colortex.cn

[Q57] 行号
来源：http://ia.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tc.hnjuh.cn

[Q58] 累计求和
来源：http://ow.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iy.lnxyls.cn

[Q59] 分组内累计
来源：http://dx.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vh.521024.cn

[Q60] 取上一行 / 下一行
来源：http://wm.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lq.hnjuh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ah.bjjhwx.cn

[Q61] 移动平均
来源：http://nu.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ls.hahajie.cn

[Q62] 分组占比
来源：http://hv.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://na.lnxyls.cn

[Q63] 开启事务
来源：http://xc.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vk.shxzukj.cn

[Q64] 提交事务
来源：http://if.wgjwhj.cn

COMMIT;
来源：http://tb.szxytkj.cn

[Q65] 回滚事务
来源：http://ey.shtwfgs.cn

ROLLBACK;
来源：http://gx.muxihuayi.cn

[Q66] 行锁查询
来源：http://yg.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ok.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://ps.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://aw.huixinmuqiang.cn

[Q68] 保存点
来源：http://ar.nicolike.cn

SAVEPOINT sp1;
来源：http://kn.nicolike.cn

ROLLBACK TO sp1;
来源：http://ic.haigaiapp.cn

[Q69] 查看执行计划
来源：http://xv.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cn.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://nk.huixiangedu.cn

ANALYZE TABLE users;
来源：http://zh.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://ov.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mh.shxzukj.cn

[Q72] 查看索引
来源：http://cs.nszjky.cn

SHOW INDEX FROM users;
来源：http://ju.haigaiapp.cn

[Q73] 查看表状态
来源：http://ug.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sc.muxihuayi.cn

[Q74] 强制使用索引
来源：http://se.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xf.shtwfgs.cn

[Q75] 日期格式化
来源：http://jw.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vf.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vu.szxytkj.cn

[Q76] 按天统计
来源：http://ch.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xu.newstarts.cn

[Q77] 时间加减
来源：http://gs.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kw.huanxung.cn

[Q78] 当前时间
来源：http://op.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://la.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://cl.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gu.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://ug.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nt.nicolike.cn

[Q81] 字符串替换
来源：http://fd.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dt.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://jb.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dl.huixiangedu.cn

[Q83] 大小写转换
来源：http://aa.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bx.panjiajie.cn

[Q84] 去除首尾空格
来源：http://cp.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://dg.asd995.cn

[Q85] 数值取整
来源：http://th.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eh.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://uv.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ii.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://yk.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://if.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://ch.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ou.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xo.lnxyls.cn

[Q89] 判断表是否存在
来源：http://tv.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dm.muxihuayi.cn

[Q90] 生成序号列
来源：http://kz.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ss.panjiajie.cn

================================================================================
来源：http://hj.gzmigu.cn

R. Bash 专题
来源：http://fc.colortex.cn

================================================================================
来源：http://qt.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://on.lnxyls.cn

#!/usr/bin/env bash
来源：http://zv.gzmigu.cn

set -euo pipefail
来源：http://xz.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://zy.lnxyls.cn

name="Tom"; echo "$name"
来源：http://df.lnxyls.cn

[R03] 只读变量
来源：http://ef.asd995.cn

readonly PI=3.14
来源：http://re.shtwfgs.cn

[R04] 位置参数
来源：http://ao.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wx.shxzukj.cn

[R05] 参数默认值
来源：http://ss.wgjwhj.cn

name="${1:-default}"
来源：http://me.lnxyls.cn

[R06] 判断命令是否存在
来源：http://dh.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gu.colortex.cn

[R07] if 判断文件
来源：http://us.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qs.colortex.cn

[R08] 数值比较
来源：http://ch.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zy.huanxung.cn

[R09] 字符串比较
来源：http://gm.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fb.lnxyls.cn

[R10] 正则匹配
来源：http://vu.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rx.bjjhwx.cn

[R11] case 多分支
来源：http://di.haigaiapp.cn

case "$1" in
来源：http://iw.bookmarksfly.cn

start) echo "启动" ;;
来源：http://ys.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://tx.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://af.lnxyls.cn

esac
来源：http://ca.haigaiapp.cn

[R12] for 遍历文件
来源：http://gg.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://xh.newstarts.cn

[R13] for 计数循环
来源：http://gk.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://op.bjjhwx.cn

[R14] C 风格 for
来源：http://qh.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oz.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://ju.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tv.shtwfgs.cn

[R16] until 等待条件
来源：http://ui.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zx.jctech888.com.cn

[R17] 数组定义与取值
来源：http://uf.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jw.bookmarksfly.cn

[R18] 遍历数组
来源：http://mn.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ii.shxzukj.cn

[R19] 数组长度
来源：http://nf.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://wk.nicolike.cn

[R20] 关联数组（字典）
来源：http://xn.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hc.nszjky.cn

[R21] 字符串长度
来源：http://lq.shxzukj.cn

echo "${#s}"
来源：http://pc.9csxet.cn

[R22] 截取子串
来源：http://oe.yuexingan06.cn

echo "${s:0:5}"
来源：http://nv.shxzukj.cn

[R23] 字符串替换
来源：http://jx.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ky.yuexingan06.cn

[R24] 大小写转换
来源：http://uq.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tx.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://kp.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bb.szsharing.cn

[R26] 命令替换
来源：http://yr.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://hc.chemitech.net.cn

[R27] 算术展开
来源：http://yu.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://ag.newstarts.cn

[R28] 浮点运算
来源：http://wr.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://pt.huixinmuqiang.cn

[R29] 定义函数
来源：http://ki.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zj.panjiajie.cn

[R30] 函数返回状态码
来源：http://bp.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://yh.nszjky.cn

[R31] 局部变量
来源：http://bg.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://eh.bjjhwx.cn

[R32] 参数个数校验
来源：http://iy.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rr.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://tr.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uv.chemitech.net.cn

[R34] 退出时清理
来源：http://ur.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tl.chemitech.net.cn

[R35] 后台执行并等待
来源：http://ed.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ou.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://ql.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uk.nicolike.cn

[R37] 把输出赋给变量
来源：http://cl.shtwfgs.cn

files=$(ls -1)
来源：http://gq.huixinmuqiang.cn

[R38] 管道串联
来源：http://sl.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://pu.521024.cn

[R39] 重定向标准输出与错误
来源：http://ad.jctech888.com.cn

cmd > out.log 2>&1
来源：http://qt.muxihuayi.cn

[R40] 追加写日志
来源：http://qy.shxzukj.cn

echo "log" >> out.log
来源：http://gt.9csxet.cn

[R41] 丢弃输出
来源：http://lu.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://jd.muxihuayi.cn

[R42] 输入重定向
来源：http://sc.muxihuayi.cn

wc -l < a.txt
来源：http://al.asd995.cn

[R43] 按名字查找文件
来源：http://th.wgjwhj.cn

find . -name "*.log" -type f
来源：http://nw.nicolike.cn

[R44] 按修改时间查找
来源：http://qd.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://vy.colortex.cn

[R45] 批量删除
来源：http://hi.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://fi.hnjuh.cn

[R46] 递归替换文件内容
来源：http://bf.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kz.shtwfgs.cn

[R47] sed 单行替换
来源：http://cv.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mq.huixiangedu.cn

[R48] awk 取指定列
来源：http://wa.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://cg.chemitech.net.cn

[R49] awk 带条件
来源：http://is.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ra.panjiajie.cn

[R50] awk 求和
来源：http://ha.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cl.9csxet.cn

[R51] 排序去重取前几
来源：http://hd.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ma.muxihuayi.cn

[R52] 统计行数
来源：http://xi.asd995.cn

wc -l a.txt
来源：http://zr.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://rs.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tl.hahajie.cn

[R54] 比较两个文件
来源：http://tv.huixiangedu.cn

diff a.txt b.txt
来源：http://qp.gzmigu.cn

[R55] 压缩与解压
来源：http://uz.nicolike.cn


<!-- 参考信息 -->