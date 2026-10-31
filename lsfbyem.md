代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fe.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://xt.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cm.asd995.cn

[Q12] 插入后取自增 ID
来源：http://kc.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fo.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wk.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://tn.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rk.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://ka.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tr.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://up.shxzskj.cn

[Q15] 查询全部
来源：http://ay.huanxung.cn

SELECT * FROM users;
来源：http://ag.9csxet.cn

[Q16] 查询指定列
来源：http://nm.hahajie.cn

SELECT id, name FROM users;
来源：http://sz.nszjky.cn

[Q17] 条件查询
来源：http://ag.shxzukj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bt.9csxet.cn

[Q18] 模糊匹配
来源：http://re.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nt.yuexingan06.cn

[Q19] 范围查询
来源：http://ev.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jw.hnjuh.cn

[Q20] IN 列表
来源：http://vy.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://va.9csxet.cn

[Q21] 空值判断
来源：http://yk.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aj.jctech888.com.cn

[Q22] 排序
来源：http://ob.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zx.wgjwhj.cn

[Q23] 分页
来源：http://yv.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://om.newstarts.cn

[Q24] 去重
来源：http://wb.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://ki.gzmigu.cn

[Q25] 只取前 N 条
来源：http://yv.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gr.yuntaijiaju.cn

[Q26] 计数
来源：http://nu.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://ci.chemitech.net.cn

[Q27] 条件计数
来源：http://qg.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dr.lnxyls.cn

[Q28] 求和与平均
来源：http://zo.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hd.jctech888.com.cn

[Q29] 最大最小值
来源：http://qu.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ot.szsharing.cn

[Q30] 分组统计
来源：http://kc.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ip.huixiangedu.cn

[Q31] 分组后过滤
来源：http://as.haigaiapp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kd.521024.cn

[Q32] 分组拼接字符串
来源：http://xn.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fl.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vl.521024.cn

[Q33] 多列分组
来源：http://pp.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rt.521024.cn

[Q34] 每组取第一条
来源：http://im.huanxung.cn

SELECT * FROM (
来源：http://ws.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yv.wgjwhj.cn

) t WHERE rn = 1;
来源：http://kp.bjjhwx.cn

[Q35] 内连接
来源：http://om.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yw.haigaiapp.cn

[Q36] 左连接
来源：http://dg.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://id.wgjwhj.cn

[Q37] 右连接
来源：http://db.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ma.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bc.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wm.asd995.cn

[Q39] 自连接（查上下级）
来源：http://cq.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sj.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xi.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lz.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mj.bjjhwx.cn

[Q41] 多表连接
来源：http://vj.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://io.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://mr.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://hm.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://xm.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://hb.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ui.bookmarksfly.cn

[Q43] 标量子查询
来源：http://xl.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cf.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://cu.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ph.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://xn.yuexingan06.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kr.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qw.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bi.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://xj.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vn.asd995.cn

[Q48] CTE 公用表表达式
来源：http://rg.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://th.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://ge.jianghongdianzi.cn

[Q49] 更新单行
来源：http://hy.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lx.panjiajie.cn

[Q50] 批量更新
来源：http://pn.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bu.szxytkj.cn

[Q51] 用子查询更新
来源：http://wo.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bk.panjiajie.cn

[Q52] 删除指定行
来源：http://bi.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://go.panjiajie.cn

[Q53] 按条件删除
来源：http://yq.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yp.huixinmuqiang.cn

[Q54] 清空表
来源：http://hv.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://bh.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://yn.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ot.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://gi.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pt.panjiajie.cn

[Q57] 行号
来源：http://eq.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dk.521024.cn

[Q58] 累计求和
来源：http://be.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jm.bjjhwx.cn

[Q59] 分组内累计
来源：http://zg.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rb.jianghongdianzi.cn

[Q60] 取上一行 / 下一行
来源：http://eh.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ym.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zg.shxzskj.cn

[Q61] 移动平均
来源：http://du.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xy.hnjuh.cn

[Q62] 分组占比
来源：http://wv.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gj.szxytkj.cn

[Q63] 开启事务
来源：http://tf.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vr.yuexingan06.cn

[Q64] 提交事务
来源：http://sg.newstarts.cn

COMMIT;
来源：http://td.yuexingan06.cn

[Q65] 回滚事务
来源：http://le.hnjuh.cn

ROLLBACK;
来源：http://ox.9csxet.cn

[Q66] 行锁查询
来源：http://pr.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qo.9csxet.cn

[Q67] 设置隔离级别
来源：http://fs.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ro.yuntaijiaju.cn

[Q68] 保存点
来源：http://lq.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://pv.szxytkj.cn

ROLLBACK TO sp1;
来源：http://lz.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://iz.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pd.huanxung.cn

[Q70] 更新统计信息
来源：http://hs.521024.cn

ANALYZE TABLE users;
来源：http://vq.bjjhwx.cn

[Q71] 查看建表语句
来源：http://ob.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fd.chemitech.net.cn

[Q72] 查看索引
来源：http://qc.9csxet.cn

SHOW INDEX FROM users;
来源：http://wx.nszjky.cn

[Q73] 查看表状态
来源：http://kr.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xu.bjjhwx.cn

[Q74] 强制使用索引
来源：http://kf.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cl.huixiangedu.cn

[Q75] 日期格式化
来源：http://kb.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kr.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://il.bookmarksfly.cn

[Q76] 按天统计
来源：http://xh.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hb.asd995.cn

[Q77] 时间加减
来源：http://vt.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fi.haigaiapp.cn

[Q78] 当前时间
来源：http://dz.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ys.nicolike.cn

[Q79] 字符串拼接
来源：http://ps.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pz.bookmarksfly.cn

[Q80] 字符串截取
来源：http://nq.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bn.newstarts.cn

[Q81] 字符串替换
来源：http://jq.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oq.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://nv.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://va.gzmigu.cn

[Q83] 大小写转换
来源：http://mq.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iu.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://kq.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://wb.szxytkj.cn

[Q85] 数值取整
来源：http://ny.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cb.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://wv.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xt.newstarts.cn

[Q87] JSON 字段做条件
来源：http://vh.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ka.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://av.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ii.huixinmuqiang.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lc.9csxet.cn

[Q89] 判断表是否存在
来源：http://rd.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ij.muxihuayi.cn

[Q90] 生成序号列
来源：http://rn.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://un.lnxyls.cn

================================================================================
来源：http://eu.hahajie.cn

R. Bash 专题
来源：http://cm.huixinmuqiang.cn

================================================================================
来源：http://gy.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://gv.muxihuayi.cn

#!/usr/bin/env bash
来源：http://uq.yuntaijiaju.cn

set -euo pipefail
来源：http://xt.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://xu.newstarts.cn

name="Tom"; echo "$name"
来源：http://ul.gzmigu.cn

[R03] 只读变量
来源：http://nw.nicolike.cn

readonly PI=3.14
来源：http://vq.nszjky.cn

[R04] 位置参数
来源：http://ej.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hu.haigaiapp.cn

[R05] 参数默认值
来源：http://bc.jianghongdianzi.cn

name="${1:-default}"
来源：http://mo.shxzukj.cn

[R06] 判断命令是否存在
来源：http://zy.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sk.newstarts.cn

[R07] if 判断文件
来源：http://na.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vb.shxzskj.cn

[R08] 数值比较
来源：http://fv.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mp.shxzukj.cn

[R09] 字符串比较
来源：http://hd.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bh.nszjky.cn

[R10] 正则匹配
来源：http://xi.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bm.asd995.cn

[R11] case 多分支
来源：http://ll.huixiangedu.cn

case "$1" in
来源：http://fs.szxytkj.cn

start) echo "启动" ;;
来源：http://qv.hnjuh.cn

stop)  echo "停止" ;;
来源：http://zi.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://lh.shxzskj.cn

esac
来源：http://tl.bjjhwx.cn

[R12] for 遍历文件
来源：http://ij.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://mw.9csxet.cn

[R13] for 计数循环
来源：http://xt.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://zs.huixiangedu.cn

[R14] C 风格 for
来源：http://kl.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://su.hahajie.cn

[R15] while 逐行读文件
来源：http://nt.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://by.shxzukj.cn

[R16] until 等待条件
来源：http://fn.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zi.gzmigu.cn

[R17] 数组定义与取值
来源：http://mt.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ws.yuexingan06.cn

[R18] 遍历数组
来源：http://dq.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rp.bjjhwx.cn

[R19] 数组长度
来源：http://fn.jctech888.com.cn

echo "${#arr[@]}"
来源：http://ik.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://zy.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sy.nicolike.cn

[R21] 字符串长度
来源：http://xq.newstarts.cn

echo "${#s}"
来源：http://is.9csxet.cn

[R22] 截取子串
来源：http://jo.szsharing.cn

echo "${s:0:5}"
来源：http://zz.huixiangedu.cn

[R23] 字符串替换
来源：http://mz.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wl.hahajie.cn

[R24] 大小写转换
来源：http://kc.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fv.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://rp.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tq.lnxyls.cn

[R26] 命令替换
来源：http://wc.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://ls.nszjky.cn

[R27] 算术展开
来源：http://oj.szsharing.cn

echo $((1 + 2 * 3))
来源：http://kh.gzmigu.cn

[R28] 浮点运算
来源：http://wd.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://rs.szxytkj.cn

[R29] 定义函数
来源：http://zt.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hl.yuexingan06.cn

[R30] 函数返回状态码
来源：http://za.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://fs.nszjky.cn

[R31] 局部变量
来源：http://ql.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://qe.chemitech.net.cn

[R32] 参数个数校验
来源：http://ff.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aa.muxihuayi.cn

[R33] 捕获错误并提示行号
来源：http://ze.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wp.haigaiapp.cn

[R34] 退出时清理
来源：http://xk.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ai.szxytkj.cn

[R35] 后台执行并等待
来源：http://qk.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://si.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://kw.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lm.huanxung.cn

[R37] 把输出赋给变量
来源：http://sf.chemitech.net.cn

files=$(ls -1)
来源：http://xm.chemitech.net.cn

[R38] 管道串联
来源：http://po.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://nl.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://tt.521024.cn

cmd > out.log 2>&1
来源：http://nw.panjiajie.cn

[R40] 追加写日志
来源：http://dz.jianghongdianzi.cn

echo "log" >> out.log
来源：http://nh.lnxyls.cn

[R41] 丢弃输出
来源：http://zk.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://gc.panjiajie.cn

[R42] 输入重定向
来源：http://vi.bookmarksfly.cn

wc -l < a.txt
来源：http://vo.hahajie.cn

[R43] 按名字查找文件
来源：http://as.jctech888.com.cn

find . -name "*.log" -type f
来源：http://ae.gzmigu.cn

[R44] 按修改时间查找
来源：http://uc.521024.cn

find . -mtime -7 -type f
来源：http://jg.huixiangedu.cn

[R45] 批量删除
来源：http://lv.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://us.szxytkj.cn

[R46] 递归替换文件内容
来源：http://wr.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ka.nszjky.cn

[R47] sed 单行替换
来源：http://ne.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ej.shtwfgs.cn

[R48] awk 取指定列
来源：http://do.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://up.gzmigu.cn

[R49] awk 带条件
来源：http://xv.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://si.shxzukj.cn

[R50] awk 求和
来源：http://cu.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://my.wgjwhj.cn

[R51] 排序去重取前几
来源：http://kd.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pk.jctech888.com.cn

[R52] 统计行数
来源：http://kx.huixiangedu.cn

wc -l a.txt
来源：http://fs.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://wy.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xm.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://ei.bjjhwx.cn

diff a.txt b.txt
来源：http://ym.gzmigu.cn

[R55] 压缩与解压
来源：http://kv.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bh.bookmarksfly.cn

[R56] 远程拷贝
来源：http://cd.yuntaijiaju.cn

scp file user@host:/path/
来源：http://cy.yuexingan06.cn

[R57] 远程执行命令
来源：http://nk.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://hx.hahajie.cn

[R58] 下载文件
来源：http://at.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fq.gzmigu.cn

[R59] 发 POST JSON
来源：http://di.asd995.cn


<!-- 参考信息 -->