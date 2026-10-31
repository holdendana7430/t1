代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://ma.9csxet.cn

[Q09] 创建唯一索引
来源：http://li.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://um.szsharing.cn

[Q10] 插入单行
来源：http://mh.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ja.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://zk.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zz.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://fi.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pg.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oq.521024.cn

[Q13] 忽略重复插入
来源：http://xn.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mb.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://ct.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rt.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zk.bookmarksfly.cn

[Q15] 查询全部
来源：http://yz.shxzskj.cn

SELECT * FROM users;
来源：http://ne.9csxet.cn

[Q16] 查询指定列
来源：http://vx.szxytkj.cn

SELECT id, name FROM users;
来源：http://xc.jctech888.com.cn

[Q17] 条件查询
来源：http://tc.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pg.bjjhwx.cn

[Q18] 模糊匹配
来源：http://yw.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gc.huanxung.cn

[Q19] 范围查询
来源：http://ww.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ed.wgjwhj.cn

[Q20] IN 列表
来源：http://zc.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qi.9csxet.cn

[Q21] 空值判断
来源：http://xx.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sf.gzmigu.cn

[Q22] 排序
来源：http://bb.panjiajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vp.yuntaijiaju.cn

[Q23] 分页
来源：http://uc.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kz.colortex.cn

[Q24] 去重
来源：http://qm.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://sc.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://ph.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aa.wgjwhj.cn

[Q26] 计数
来源：http://cw.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://gv.shxzukj.cn

[Q27] 条件计数
来源：http://lf.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iu.szsharing.cn

[Q28] 求和与平均
来源：http://jn.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yy.colortex.cn

[Q29] 最大最小值
来源：http://ga.asd995.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zx.newstarts.cn

[Q30] 分组统计
来源：http://gc.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qs.huanxung.cn

[Q31] 分组后过滤
来源：http://tg.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xl.newstarts.cn

[Q32] 分组拼接字符串
来源：http://cg.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wg.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://od.hahajie.cn

[Q33] 多列分组
来源：http://tk.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://de.colortex.cn

[Q34] 每组取第一条
来源：http://yt.yuexingan06.cn

SELECT * FROM (
来源：http://jz.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dq.muxihuayi.cn

) t WHERE rn = 1;
来源：http://uz.hahajie.cn

[Q35] 内连接
来源：http://gd.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ao.huixiangedu.cn

[Q36] 左连接
来源：http://ku.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yn.521024.cn

[Q37] 右连接
来源：http://be.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kd.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dn.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ii.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://xw.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ym.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kc.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ru.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ic.jctech888.com.cn

[Q41] 多表连接
来源：http://ek.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ie.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://re.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://qd.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://vp.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://lj.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xj.huixiangedu.cn

[Q43] 标量子查询
来源：http://oy.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vp.bookmarksfly.cn

[Q44] IN 子查询
来源：http://fx.lnxyls.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yr.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://fi.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://co.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cp.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cm.szxytkj.cn

[Q47] 与平均值比较
来源：http://pj.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ih.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://cp.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oc.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://hv.hnjuh.cn

[Q49] 更新单行
来源：http://jc.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ph.nicolike.cn

[Q50] 批量更新
来源：http://ki.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sp.colortex.cn

[Q51] 用子查询更新
来源：http://co.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vk.szsharing.cn

[Q52] 删除指定行
来源：http://rq.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://cz.szsharing.cn

[Q53] 按条件删除
来源：http://ts.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vy.shxzskj.cn

[Q54] 清空表
来源：http://it.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://sf.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://gd.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rg.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://yx.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rd.bjjhwx.cn

[Q57] 行号
来源：http://ol.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cn.bookmarksfly.cn

[Q58] 累计求和
来源：http://sn.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vo.shtwfgs.cn

[Q59] 分组内累计
来源：http://eu.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bm.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://nr.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qf.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yj.shxzskj.cn

[Q61] 移动平均
来源：http://vx.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gn.panjiajie.cn

[Q62] 分组占比
来源：http://uw.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yq.yuexingan06.cn

[Q63] 开启事务
来源：http://xh.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hq.jctech888.com.cn

[Q64] 提交事务
来源：http://hz.hnjuh.cn

COMMIT;
来源：http://un.asd995.cn

[Q65] 回滚事务
来源：http://sd.lnxyls.cn

ROLLBACK;
来源：http://xb.hnjuh.cn

[Q66] 行锁查询
来源：http://in.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lq.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://mt.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kg.9csxet.cn

[Q68] 保存点
来源：http://rd.bjjhwx.cn

SAVEPOINT sp1;
来源：http://in.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://pr.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://fr.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gs.panjiajie.cn

[Q70] 更新统计信息
来源：http://dq.shxzukj.cn

ANALYZE TABLE users;
来源：http://rf.panjiajie.cn

[Q71] 查看建表语句
来源：http://gp.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://se.chemitech.net.cn

[Q72] 查看索引
来源：http://ck.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://vi.haigaiapp.cn

[Q73] 查看表状态
来源：http://hi.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://da.szsharing.cn

[Q74] 强制使用索引
来源：http://od.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rf.nszjky.cn

[Q75] 日期格式化
来源：http://ij.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://do.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shxzukj.cn

[Q76] 按天统计
来源：http://fj.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zt.panjiajie.cn

[Q77] 时间加减
来源：http://iw.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kq.colortex.cn

[Q78] 当前时间
来源：http://ik.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ne.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://vu.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ne.yuexingan06.cn

[Q80] 字符串截取
来源：http://te.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kc.panjiajie.cn

[Q81] 字符串替换
来源：http://vh.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cb.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://sz.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vr.shtwfgs.cn

[Q83] 大小写转换
来源：http://aa.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zy.9csxet.cn

[Q84] 去除首尾空格
来源：http://ss.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://on.shxzukj.cn

[Q85] 数值取整
来源：http://mg.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yz.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://wu.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ev.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://qj.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mn.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://co.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hx.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lw.szsharing.cn

[Q89] 判断表是否存在
来源：http://lt.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jy.nicolike.cn

[Q90] 生成序号列
来源：http://cq.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ic.newstarts.cn

================================================================================
来源：http://eo.muxihuayi.cn

R. Bash 专题
来源：http://pm.panjiajie.cn

================================================================================
来源：http://ga.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://ic.shtwfgs.cn

#!/usr/bin/env bash
来源：http://yq.nszjky.cn

set -euo pipefail
来源：http://us.521024.cn

[R02] 变量赋值与使用
来源：http://mm.szxytkj.cn

name="Tom"; echo "$name"
来源：http://le.haigaiapp.cn

[R03] 只读变量
来源：http://ka.asd995.cn

readonly PI=3.14
来源：http://hd.wgjwhj.cn

[R04] 位置参数
来源：http://gc.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zj.yuntaijiaju.cn

[R05] 参数默认值
来源：http://rb.colortex.cn

name="${1:-default}"
来源：http://fx.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://je.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ie.jianghongdianzi.cn

[R07] if 判断文件
来源：http://gt.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ml.muxihuayi.cn

[R08] 数值比较
来源：http://bx.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jc.9csxet.cn

[R09] 字符串比较
来源：http://sv.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fl.yuexingan06.cn

[R10] 正则匹配
来源：http://fy.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://md.nszjky.cn

[R11] case 多分支
来源：http://fu.gzmigu.cn

case "$1" in
来源：http://kl.shxzskj.cn

start) echo "启动" ;;
来源：http://lm.szsharing.cn

stop)  echo "停止" ;;
来源：http://nq.huanxung.cn

*)     echo "未知命令" ;;
来源：http://hl.asd995.cn

esac
来源：http://xu.muxihuayi.cn

[R12] for 遍历文件
来源：http://xa.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://ya.colortex.cn

[R13] for 计数循环
来源：http://ld.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://ei.huixiangedu.cn

[R14] C 风格 for
来源：http://jt.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sw.szsharing.cn

[R15] while 逐行读文件
来源：http://xy.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ak.hahajie.cn

[R16] until 等待条件
来源：http://hm.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ld.nszjky.cn

[R17] 数组定义与取值
来源：http://hu.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lz.hnjuh.cn

[R18] 遍历数组
来源：http://zm.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://we.yuexingan06.cn

[R19] 数组长度
来源：http://et.hahajie.cn

echo "${#arr[@]}"
来源：http://vn.newstarts.cn

[R20] 关联数组（字典）
来源：http://kf.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xi.jianghongdianzi.cn

[R21] 字符串长度
来源：http://wq.yuntaijiaju.cn

echo "${#s}"
来源：http://sa.shtwfgs.cn

[R22] 截取子串
来源：http://yq.lnxyls.cn

echo "${s:0:5}"
来源：http://lv.bookmarksfly.cn

[R23] 字符串替换
来源：http://mw.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ki.szsharing.cn

[R24] 大小写转换
来源：http://rr.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xt.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://wj.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ic.hnjuh.cn

[R26] 命令替换
来源：http://xm.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://kf.gzmigu.cn

[R27] 算术展开
来源：http://ec.9csxet.cn

echo $((1 + 2 * 3))
来源：http://rf.asd995.cn

[R28] 浮点运算
来源：http://mf.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://dv.szxytkj.cn

[R29] 定义函数
来源：http://xk.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ng.shtwfgs.cn

[R30] 函数返回状态码
来源：http://rk.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://et.nszjky.cn

[R31] 局部变量
来源：http://yh.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://mw.shtwfgs.cn

[R32] 参数个数校验
来源：http://zt.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gx.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://fw.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wn.shtwfgs.cn

[R34] 退出时清理
来源：http://dq.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://su.chemitech.net.cn

[R35] 后台执行并等待
来源：http://au.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kd.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://zh.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jp.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://ce.huixiangedu.cn

files=$(ls -1)
来源：http://wn.szsharing.cn

[R38] 管道串联
来源：http://am.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://ny.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://ov.muxihuayi.cn

cmd > out.log 2>&1
来源：http://gh.newstarts.cn

[R40] 追加写日志
来源：http://hk.jianghongdianzi.cn

echo "log" >> out.log
来源：http://jo.bookmarksfly.cn

[R41] 丢弃输出
来源：http://ua.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://ql.jianghongdianzi.cn

[R42] 输入重定向
来源：http://ff.shtwfgs.cn

wc -l < a.txt
来源：http://cr.nszjky.cn

[R43] 按名字查找文件
来源：http://zi.lnxyls.cn

find . -name "*.log" -type f
来源：http://sy.szsharing.cn

[R44] 按修改时间查找
来源：http://xk.bjjhwx.cn

find . -mtime -7 -type f
来源：http://zv.asd995.cn

[R45] 批量删除
来源：http://pw.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://tz.nszjky.cn

[R46] 递归替换文件内容
来源：http://bb.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vu.wgjwhj.cn

[R47] sed 单行替换
来源：http://hb.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wv.huanxung.cn

[R48] awk 取指定列
来源：http://mc.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://mo.lnxyls.cn

[R49] awk 带条件
来源：http://yz.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nj.colortex.cn

[R50] awk 求和
来源：http://vh.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sw.shtwfgs.cn

[R51] 排序去重取前几
来源：http://yo.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eh.szsharing.cn

[R52] 统计行数
来源：http://ta.wgjwhj.cn

wc -l a.txt
来源：http://hk.colortex.cn

[R53] 查看文件头与实时尾
来源：http://ub.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://es.shxzukj.cn

[R54] 比较两个文件
来源：http://jl.shxzskj.cn

diff a.txt b.txt
来源：http://vo.huanxung.cn

[R55] 压缩与解压
来源：http://xz.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://av.shxzukj.cn

[R56] 远程拷贝
来源：http://sv.bookmarksfly.cn

scp file user@host:/path/
来源：http://wy.huixiangedu.cn

[R57] 远程执行命令
来源：http://cq.hahajie.cn


<!-- 参考信息 -->