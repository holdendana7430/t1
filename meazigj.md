代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://mj.colortex.cn

[Q09] 创建唯一索引
来源：http://ji.huixiangedu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fr.szxytkj.cn

[Q10] 插入单行
来源：http://eb.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xl.huixiangedu.cn

[Q11] 一次插入多行
来源：http://eo.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mb.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://qm.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ak.nicolike.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://no.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://pr.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pk.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://wo.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xq.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fv.gzmigu.cn

[Q15] 查询全部
来源：http://na.szsharing.cn

SELECT * FROM users;
来源：http://qx.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://ck.huanxung.cn

SELECT id, name FROM users;
来源：http://tw.hnjuh.cn

[Q17] 条件查询
来源：http://sa.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ma.hnjuh.cn

[Q18] 模糊匹配
来源：http://vm.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fk.bjjhwx.cn

[Q19] 范围查询
来源：http://qw.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bc.nicolike.cn

[Q20] IN 列表
来源：http://ad.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fc.lnxyls.cn

[Q21] 空值判断
来源：http://wy.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ek.nszjky.cn

[Q22] 排序
来源：http://zp.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ov.huixiangedu.cn

[Q23] 分页
来源：http://oq.haigaiapp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ov.bjjhwx.cn

[Q24] 去重
来源：http://ls.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://nc.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://zq.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bw.bookmarksfly.cn

[Q26] 计数
来源：http://qt.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://gz.gzmigu.cn

[Q27] 条件计数
来源：http://yo.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sj.gzmigu.cn

[Q28] 求和与平均
来源：http://qg.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bi.wgjwhj.cn

[Q29] 最大最小值
来源：http://dh.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zn.huanxung.cn

[Q30] 分组统计
来源：http://wu.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://se.szsharing.cn

[Q31] 分组后过滤
来源：http://mt.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://at.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://kc.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fx.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://or.bjjhwx.cn

[Q33] 多列分组
来源：http://rm.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iy.colortex.cn

[Q34] 每组取第一条
来源：http://yd.hahajie.cn

SELECT * FROM (
来源：http://wk.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ri.gzmigu.cn

) t WHERE rn = 1;
来源：http://zh.yuntaijiaju.cn

[Q35] 内连接
来源：http://st.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ge.szxytkj.cn

[Q36] 左连接
来源：http://vb.asd995.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zo.nicolike.cn

[Q37] 右连接
来源：http://rm.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xc.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pm.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yp.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://ip.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zz.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ji.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sp.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ia.muxihuayi.cn

[Q41] 多表连接
来源：http://iy.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iz.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://bp.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://xm.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://ej.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://yy.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hv.panjiajie.cn

[Q43] 标量子查询
来源：http://as.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://im.521024.cn

[Q44] IN 子查询
来源：http://ta.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bf.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://ts.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hw.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://is.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jt.shtwfgs.cn

[Q47] 与平均值比较
来源：http://hw.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gs.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://fr.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ug.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://ao.gzmigu.cn

[Q49] 更新单行
来源：http://wg.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ck.huanxung.cn

[Q50] 批量更新
来源：http://un.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aa.szsharing.cn

[Q51] 用子查询更新
来源：http://vi.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zj.huanxung.cn

[Q52] 删除指定行
来源：http://xu.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://vu.bjjhwx.cn

[Q53] 按条件删除
来源：http://sj.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iq.asd995.cn

[Q54] 清空表
来源：http://eh.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://vy.nszjky.cn

[Q55] 排名（并列占位）
来源：http://ti.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kn.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://ej.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nh.newstarts.cn

[Q57] 行号
来源：http://mo.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ih.jctech888.com.cn

[Q58] 累计求和
来源：http://cl.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wx.muxihuayi.cn

[Q59] 分组内累计
来源：http://cm.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ai.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://us.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://af.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lr.shxzukj.cn

[Q61] 移动平均
来源：http://kn.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kj.asd995.cn

[Q62] 分组占比
来源：http://mb.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mk.shxzskj.cn

[Q63] 开启事务
来源：http://ap.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gm.nszjky.cn

[Q64] 提交事务
来源：http://an.panjiajie.cn

COMMIT;
来源：http://ad.bjjhwx.cn

[Q65] 回滚事务
来源：http://js.shtwfgs.cn

ROLLBACK;
来源：http://ty.hnjuh.cn

[Q66] 行锁查询
来源：http://un.colortex.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bt.521024.cn

[Q67] 设置隔离级别
来源：http://qm.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oc.shxzskj.cn

[Q68] 保存点
来源：http://bv.szxytkj.cn

SAVEPOINT sp1;
来源：http://pc.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://ig.colortex.cn

[Q69] 查看执行计划
来源：http://jq.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cv.shtwfgs.cn

[Q70] 更新统计信息
来源：http://mz.shxzukj.cn

ANALYZE TABLE users;
来源：http://ei.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://ra.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pa.muxihuayi.cn

[Q72] 查看索引
来源：http://xo.shxzukj.cn

SHOW INDEX FROM users;
来源：http://hg.bjjhwx.cn

[Q73] 查看表状态
来源：http://nt.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gc.haigaiapp.cn

[Q74] 强制使用索引
来源：http://po.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.bjjhwx.cn

[Q75] 日期格式化
来源：http://ky.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cz.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ex.wgjwhj.cn

[Q76] 按天统计
来源：http://sm.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sv.shxzukj.cn

[Q77] 时间加减
来源：http://zy.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://us.wgjwhj.cn

[Q78] 当前时间
来源：http://jt.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nx.szxytkj.cn

[Q79] 字符串拼接
来源：http://ll.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sx.huanxung.cn

[Q80] 字符串截取
来源：http://oy.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xx.szsharing.cn

[Q81] 字符串替换
来源：http://oo.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dm.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://kl.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wu.panjiajie.cn

[Q83] 大小写转换
来源：http://hn.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ia.szsharing.cn

[Q84] 去除首尾空格
来源：http://pd.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://bh.jctech888.com.cn

[Q85] 数值取整
来源：http://eb.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://im.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://vb.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gf.9csxet.cn

[Q87] JSON 字段做条件
来源：http://sp.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bx.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://aw.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xc.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://by.9csxet.cn

[Q89] 判断表是否存在
来源：http://jj.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wp.9csxet.cn

[Q90] 生成序号列
来源：http://pf.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mf.9csxet.cn

================================================================================
来源：http://qp.521024.cn

R. Bash 专题
来源：http://bs.wgjwhj.cn

================================================================================
来源：http://pv.newstarts.cn

[R01] shebang 与严格模式
来源：http://kn.nicolike.cn

#!/usr/bin/env bash
来源：http://fr.panjiajie.cn

set -euo pipefail
来源：http://nf.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://um.gzmigu.cn

name="Tom"; echo "$name"
来源：http://qi.huanxung.cn

[R03] 只读变量
来源：http://id.shxzskj.cn

readonly PI=3.14
来源：http://ld.wgjwhj.cn

[R04] 位置参数
来源：http://mi.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fc.hahajie.cn

[R05] 参数默认值
来源：http://bk.lnxyls.cn

name="${1:-default}"
来源：http://ly.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://aq.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ub.shtwfgs.cn

[R07] if 判断文件
来源：http://aj.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ph.shxzskj.cn

[R08] 数值比较
来源：http://lv.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ir.wgjwhj.cn

[R09] 字符串比较
来源：http://hh.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xr.jctech888.com.cn

[R10] 正则匹配
来源：http://pc.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ao.huixiangedu.cn

[R11] case 多分支
来源：http://ah.hahajie.cn

case "$1" in
来源：http://rk.shxzukj.cn

start) echo "启动" ;;
来源：http://cb.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://sa.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://jx.shxzskj.cn

esac
来源：http://sm.chemitech.net.cn

[R12] for 遍历文件
来源：http://bn.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://lo.wgjwhj.cn

[R13] for 计数循环
来源：http://zf.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://pm.9csxet.cn

[R14] C 风格 for
来源：http://oq.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fh.colortex.cn

[R15] while 逐行读文件
来源：http://cu.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://om.521024.cn

[R16] until 等待条件
来源：http://sh.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vx.asd995.cn

[R17] 数组定义与取值
来源：http://gi.huanxung.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ov.521024.cn

[R18] 遍历数组
来源：http://cl.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xw.haigaiapp.cn

[R19] 数组长度
来源：http://vd.hahajie.cn

echo "${#arr[@]}"
来源：http://qz.newstarts.cn

[R20] 关联数组（字典）
来源：http://hl.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kv.szsharing.cn

[R21] 字符串长度
来源：http://cs.bjjhwx.cn

echo "${#s}"
来源：http://zs.9csxet.cn

[R22] 截取子串
来源：http://cv.huanxung.cn

echo "${s:0:5}"
来源：http://jm.9csxet.cn

[R23] 字符串替换
来源：http://gi.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iy.newstarts.cn

[R24] 大小写转换
来源：http://qr.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zt.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://po.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://li.9csxet.cn

[R26] 命令替换
来源：http://un.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://hs.bookmarksfly.cn

[R27] 算术展开
来源：http://qn.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://uo.yuntaijiaju.cn

[R28] 浮点运算
来源：http://bz.521024.cn

echo "scale=2; 10/3" | bc
来源：http://gp.szsharing.cn

[R29] 定义函数
来源：http://he.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://em.bjjhwx.cn

[R30] 函数返回状态码
来源：http://ub.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://kq.yuntaijiaju.cn

[R31] 局部变量
来源：http://gy.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://lo.colortex.cn

[R32] 参数个数校验
来源：http://cv.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iw.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://pd.szxytkj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vg.huanxung.cn

[R34] 退出时清理
来源：http://la.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pw.newstarts.cn

[R35] 后台执行并等待
来源：http://sj.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ja.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://jg.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tz.9csxet.cn

[R37] 把输出赋给变量
来源：http://ez.panjiajie.cn

files=$(ls -1)
来源：http://zt.huixinmuqiang.cn

[R38] 管道串联
来源：http://bm.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://gl.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://ln.yuexingan06.cn

cmd > out.log 2>&1
来源：http://xu.jianghongdianzi.cn

[R40] 追加写日志
来源：http://bj.huanxung.cn

echo "log" >> out.log
来源：http://jk.haigaiapp.cn

[R41] 丢弃输出
来源：http://ak.9csxet.cn

cmd >/dev/null 2>&1
来源：http://ao.chemitech.net.cn

[R42] 输入重定向
来源：http://xz.shxzukj.cn

wc -l < a.txt
来源：http://km.wgjwhj.cn

[R43] 按名字查找文件
来源：http://wf.colortex.cn

find . -name "*.log" -type f
来源：http://yw.muxihuayi.cn

[R44] 按修改时间查找
来源：http://bi.newstarts.cn

find . -mtime -7 -type f
来源：http://wz.szxytkj.cn

[R45] 批量删除
来源：http://vn.nicolike.cn

find . -name "*.tmp" -delete
来源：http://yx.gzmigu.cn

[R46] 递归替换文件内容
来源：http://pw.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gd.hahajie.cn

[R47] sed 单行替换
来源：http://ab.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oo.asd995.cn

[R48] awk 取指定列
来源：http://no.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://ho.huixinmuqiang.cn

[R49] awk 带条件
来源：http://hn.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uw.bjjhwx.cn

[R50] awk 求和
来源：http://jp.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tj.shtwfgs.cn

[R51] 排序去重取前几
来源：http://tc.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wb.szsharing.cn

[R52] 统计行数
来源：http://ap.gzmigu.cn

wc -l a.txt
来源：http://kr.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://ko.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ud.newstarts.cn

[R54] 比较两个文件
来源：http://bu.haigaiapp.cn

diff a.txt b.txt
来源：http://gd.chemitech.net.cn

[R55] 压缩与解压
来源：http://wb.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://co.szsharing.cn

[R56] 远程拷贝
来源：http://mo.nicolike.cn

scp file user@host:/path/
来源：http://sx.panjiajie.cn

[R57] 远程执行命令
来源：http://dz.colortex.cn


<!-- 参考信息 -->