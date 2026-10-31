代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://ck.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://ap.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qd.nicolike.cn

[Q10] 插入单行
来源：http://tf.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wm.lnxyls.cn

[Q11] 一次插入多行
来源：http://tp.gzmigu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mz.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://uq.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://aw.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://la.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://uh.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gf.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://wo.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xn.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://eo.newstarts.cn

[Q15] 查询全部
来源：http://zq.yuntaijiaju.cn

SELECT * FROM users;
来源：http://rt.szxytkj.cn

[Q16] 查询指定列
来源：http://sy.wgjwhj.cn

SELECT id, name FROM users;
来源：http://yx.muxihuayi.cn

[Q17] 条件查询
来源：http://vv.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wn.asd995.cn

[Q18] 模糊匹配
来源：http://nj.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eh.szxytkj.cn

[Q19] 范围查询
来源：http://ar.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zq.bjjhwx.cn

[Q20] IN 列表
来源：http://ow.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ni.shxzskj.cn

[Q21] 空值判断
来源：http://aw.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wk.521024.cn

[Q22] 排序
来源：http://xc.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qt.huanxung.cn

[Q23] 分页
来源：http://ki.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ke.jianghongdianzi.cn

[Q24] 去重
来源：http://rm.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://tx.gzmigu.cn

[Q25] 只取前 N 条
来源：http://us.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lo.muxihuayi.cn

[Q26] 计数
来源：http://oo.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://uu.panjiajie.cn

[Q27] 条件计数
来源：http://dc.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mu.hnjuh.cn

[Q28] 求和与平均
来源：http://jf.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yw.huixiangedu.cn

[Q29] 最大最小值
来源：http://fo.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zw.9csxet.cn

[Q30] 分组统计
来源：http://nm.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vu.colortex.cn

[Q31] 分组后过滤
来源：http://iw.jctech888.com.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://it.jctech888.com.cn

[Q32] 分组拼接字符串
来源：http://ys.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ir.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nd.yuexingan06.cn

[Q33] 多列分组
来源：http://ey.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ba.jctech888.com.cn

[Q34] 每组取第一条
来源：http://kt.shxzukj.cn

SELECT * FROM (
来源：http://mo.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ak.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://vj.shxzskj.cn

[Q35] 内连接
来源：http://wx.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xl.shtwfgs.cn

[Q36] 左连接
来源：http://zi.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sh.jctech888.com.cn

[Q37] 右连接
来源：http://yz.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bi.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hj.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ee.gzmigu.cn

[Q39] 自连接（查上下级）
来源：http://tq.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pr.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lx.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jp.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ae.newstarts.cn

[Q41] 多表连接
来源：http://vn.muxihuayi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fn.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://ra.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://zb.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://fb.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://de.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gq.hnjuh.cn

[Q43] 标量子查询
来源：http://qs.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://no.bjjhwx.cn

[Q44] IN 子查询
来源：http://mf.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dn.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://tm.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jx.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ht.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://di.haigaiapp.cn

[Q47] 与平均值比较
来源：http://du.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bd.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://mi.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mv.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://ij.lnxyls.cn

[Q49] 更新单行
来源：http://aj.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fp.yuntaijiaju.cn

[Q50] 批量更新
来源：http://os.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wi.szxytkj.cn

[Q51] 用子查询更新
来源：http://hu.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yl.521024.cn

[Q52] 删除指定行
来源：http://da.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://rl.chemitech.net.cn

[Q53] 按条件删除
来源：http://uv.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gf.szsharing.cn

[Q54] 清空表
来源：http://ge.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://qo.521024.cn

[Q55] 排名（并列占位）
来源：http://am.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://it.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://om.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cm.szsharing.cn

[Q57] 行号
来源：http://tz.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dq.bjjhwx.cn

[Q58] 累计求和
来源：http://cn.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gg.szxytkj.cn

[Q59] 分组内累计
来源：http://mc.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ia.huixiangedu.cn

[Q60] 取上一行 / 下一行
来源：http://rt.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tk.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://we.yuexingan06.cn

[Q61] 移动平均
来源：http://jt.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fr.bjjhwx.cn

[Q62] 分组占比
来源：http://yk.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zu.chemitech.net.cn

[Q63] 开启事务
来源：http://dm.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hu.huanxung.cn

[Q64] 提交事务
来源：http://vx.panjiajie.cn

COMMIT;
来源：http://gm.shxzukj.cn

[Q65] 回滚事务
来源：http://bs.shtwfgs.cn

ROLLBACK;
来源：http://an.shxzukj.cn

[Q66] 行锁查询
来源：http://qe.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nt.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://vw.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ge.lnxyls.cn

[Q68] 保存点
来源：http://bf.szxytkj.cn

SAVEPOINT sp1;
来源：http://qp.521024.cn

ROLLBACK TO sp1;
来源：http://yj.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://tc.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ao.wgjwhj.cn

[Q70] 更新统计信息
来源：http://tk.shxzskj.cn

ANALYZE TABLE users;
来源：http://im.asd995.cn

[Q71] 查看建表语句
来源：http://oa.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ez.szsharing.cn

[Q72] 查看索引
来源：http://vj.hnjuh.cn

SHOW INDEX FROM users;
来源：http://nf.yuexingan06.cn

[Q73] 查看表状态
来源：http://sw.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rp.muxihuayi.cn

[Q74] 强制使用索引
来源：http://bt.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fv.wgjwhj.cn

[Q75] 日期格式化
来源：http://cx.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cj.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://po.huixiangedu.cn

[Q76] 按天统计
来源：http://sn.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://in.shxzskj.cn

[Q77] 时间加减
来源：http://pf.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gm.shxzskj.cn

[Q78] 当前时间
来源：http://zu.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ya.huanxung.cn

[Q79] 字符串拼接
来源：http://yr.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oo.asd995.cn

[Q80] 字符串截取
来源：http://kv.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fp.panjiajie.cn

[Q81] 字符串替换
来源：http://vq.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://za.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://kf.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://py.bookmarksfly.cn

[Q83] 大小写转换
来源：http://vh.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://al.jctech888.com.cn

[Q84] 去除首尾空格
来源：http://if.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://sj.colortex.cn

[Q85] 数值取整
来源：http://bi.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ig.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://do.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sm.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://fo.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ig.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://vn.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zq.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bs.lnxyls.cn

[Q89] 判断表是否存在
来源：http://lg.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hr.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://sn.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ge.9csxet.cn

================================================================================
来源：http://ng.lnxyls.cn

R. Bash 专题
来源：http://vs.szxytkj.cn

================================================================================
来源：http://jl.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://om.huixiangedu.cn

#!/usr/bin/env bash
来源：http://ti.hnjuh.cn

set -euo pipefail
来源：http://vh.gzmigu.cn

[R02] 变量赋值与使用
来源：http://bx.9csxet.cn

name="Tom"; echo "$name"
来源：http://pl.shtwfgs.cn

[R03] 只读变量
来源：http://lz.shxzukj.cn

readonly PI=3.14
来源：http://ah.shtwfgs.cn

[R04] 位置参数
来源：http://rp.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qd.huixiangedu.cn

[R05] 参数默认值
来源：http://at.9csxet.cn

name="${1:-default}"
来源：http://bt.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://os.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fg.lnxyls.cn

[R07] if 判断文件
来源：http://uk.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ai.szsharing.cn

[R08] 数值比较
来源：http://na.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yz.lnxyls.cn

[R09] 字符串比较
来源：http://dc.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jq.521024.cn

[R10] 正则匹配
来源：http://da.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nr.huixiangedu.cn

[R11] case 多分支
来源：http://pc.newstarts.cn

case "$1" in
来源：http://hc.hnjuh.cn

start) echo "启动" ;;
来源：http://te.panjiajie.cn

stop)  echo "停止" ;;
来源：http://ht.nszjky.cn

*)     echo "未知命令" ;;
来源：http://cz.shtwfgs.cn

esac
来源：http://uv.521024.cn

[R12] for 遍历文件
来源：http://ev.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://pm.shxzskj.cn

[R13] for 计数循环
来源：http://vr.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://zs.bookmarksfly.cn

[R14] C 风格 for
来源：http://zk.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mc.nszjky.cn

[R15] while 逐行读文件
来源：http://ot.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://je.huixiangedu.cn

[R16] until 等待条件
来源：http://xr.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://od.bjjhwx.cn

[R17] 数组定义与取值
来源：http://cc.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wc.bjjhwx.cn

[R18] 遍历数组
来源：http://na.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oq.wgjwhj.cn

[R19] 数组长度
来源：http://kd.szsharing.cn

echo "${#arr[@]}"
来源：http://ao.nicolike.cn

[R20] 关联数组（字典）
来源：http://qh.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qg.colortex.cn

[R21] 字符串长度
来源：http://bq.haigaiapp.cn

echo "${#s}"
来源：http://xb.nicolike.cn

[R22] 截取子串
来源：http://oz.shtwfgs.cn

echo "${s:0:5}"
来源：http://ys.gzmigu.cn

[R23] 字符串替换
来源：http://qa.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xb.shxzskj.cn

[R24] 大小写转换
来源：http://ki.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lc.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://oh.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wu.nicolike.cn

[R26] 命令替换
来源：http://hc.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://xf.haigaiapp.cn

[R27] 算术展开
来源：http://gr.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://bj.yuexingan06.cn

[R28] 浮点运算
来源：http://hq.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://kx.huixinmuqiang.cn

[R29] 定义函数
来源：http://bg.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sv.chemitech.net.cn

[R30] 函数返回状态码
来源：http://gh.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://bz.shtwfgs.cn

[R31] 局部变量
来源：http://vm.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://uy.hahajie.cn

[R32] 参数个数校验
来源：http://oh.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qy.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://ur.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xq.521024.cn

[R34] 退出时清理
来源：http://np.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rd.huixiangedu.cn

[R35] 后台执行并等待
来源：http://iy.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hp.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://fh.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qr.szsharing.cn

[R37] 把输出赋给变量
来源：http://ba.lnxyls.cn

files=$(ls -1)
来源：http://pv.panjiajie.cn

[R38] 管道串联
来源：http://zs.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://uq.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://sm.521024.cn

cmd > out.log 2>&1
来源：http://fp.shtwfgs.cn

[R40] 追加写日志
来源：http://ua.huixiangedu.cn

echo "log" >> out.log
来源：http://ev.colortex.cn

[R41] 丢弃输出
来源：http://gb.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://bs.yuntaijiaju.cn

[R42] 输入重定向
来源：http://ik.jianghongdianzi.cn

wc -l < a.txt
来源：http://es.chemitech.net.cn

[R43] 按名字查找文件
来源：http://cv.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://ai.nicolike.cn

[R44] 按修改时间查找
来源：http://cc.szxytkj.cn

find . -mtime -7 -type f
来源：http://eq.huixiangedu.cn

[R45] 批量删除
来源：http://lz.szsharing.cn

find . -name "*.tmp" -delete
来源：http://ch.nicolike.cn

[R46] 递归替换文件内容
来源：http://hz.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tm.gzmigu.cn

[R47] sed 单行替换
来源：http://kr.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zf.panjiajie.cn

[R48] awk 取指定列
来源：http://ez.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://ko.hahajie.cn

[R49] awk 带条件
来源：http://nw.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yu.nszjky.cn

[R50] awk 求和
来源：http://lm.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bo.wgjwhj.cn

[R51] 排序去重取前几
来源：http://xh.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gw.muxihuayi.cn

[R52] 统计行数
来源：http://bl.muxihuayi.cn

wc -l a.txt
来源：http://sv.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://lw.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uk.shxzukj.cn

[R54] 比较两个文件
来源：http://cf.haigaiapp.cn

diff a.txt b.txt
来源：http://mv.szxytkj.cn

[R55] 压缩与解压
来源：http://kn.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tk.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://kj.chemitech.net.cn

scp file user@host:/path/
来源：http://fl.haigaiapp.cn

[R57] 远程执行命令
来源：http://xl.szsharing.cn


<!-- 参考信息 -->