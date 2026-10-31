代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://mn.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hf.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://fu.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ci.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://yq.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fe.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vf.yuexingan06.cn

[Q15] 查询全部
来源：http://ir.shxzukj.cn

SELECT * FROM users;
来源：http://yl.newstarts.cn

[Q16] 查询指定列
来源：http://ik.jctech888.com.cn

SELECT id, name FROM users;
来源：http://zc.yuntaijiaju.cn

[Q17] 条件查询
来源：http://yy.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wq.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://yr.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://di.hnjuh.cn

[Q19] 范围查询
来源：http://np.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kk.9csxet.cn

[Q20] IN 列表
来源：http://an.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dm.wgjwhj.cn

[Q21] 空值判断
来源：http://jb.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fj.asd995.cn

[Q22] 排序
来源：http://zv.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ik.lnxyls.cn

[Q23] 分页
来源：http://oi.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ma.bookmarksfly.cn

[Q24] 去重
来源：http://gz.huixiangedu.cn

SELECT DISTINCT city FROM users;
来源：http://lp.newstarts.cn

[Q25] 只取前 N 条
来源：http://yl.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cl.huixinmuqiang.cn

[Q26] 计数
来源：http://lh.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://op.colortex.cn

[Q27] 条件计数
来源：http://kb.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cd.shxzukj.cn

[Q28] 求和与平均
来源：http://xw.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mq.huixinmuqiang.cn

[Q29] 最大最小值
来源：http://vb.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://do.hnjuh.cn

[Q30] 分组统计
来源：http://pk.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vj.bjjhwx.cn

[Q31] 分组后过滤
来源：http://kx.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cs.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://zy.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ga.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nq.nicolike.cn

[Q33] 多列分组
来源：http://zt.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://op.szxytkj.cn

[Q34] 每组取第一条
来源：http://cx.hnjuh.cn

SELECT * FROM (
来源：http://kb.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nh.lnxyls.cn

) t WHERE rn = 1;
来源：http://hm.bjjhwx.cn

[Q35] 内连接
来源：http://ga.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://he.colortex.cn

[Q36] 左连接
来源：http://hn.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kd.nicolike.cn

[Q37] 右连接
来源：http://sd.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gf.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xb.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fz.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://fj.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yo.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cv.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vl.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://er.hnjuh.cn

[Q41] 多表连接
来源：http://sv.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vi.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://ze.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://ga.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://yo.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://zt.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lo.9csxet.cn

[Q43] 标量子查询
来源：http://ht.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gx.huixiangedu.cn

[Q44] IN 子查询
来源：http://mq.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ax.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://he.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bs.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ba.lnxyls.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sa.newstarts.cn

[Q47] 与平均值比较
来源：http://sc.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rr.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://dw.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yf.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://fs.shxzskj.cn

[Q49] 更新单行
来源：http://og.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ch.nicolike.cn

[Q50] 批量更新
来源：http://yy.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xr.wgjwhj.cn

[Q51] 用子查询更新
来源：http://zp.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lo.newstarts.cn

[Q52] 删除指定行
来源：http://mm.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://wg.huanxung.cn

[Q53] 按条件删除
来源：http://bd.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zc.huixinmuqiang.cn

[Q54] 清空表
来源：http://re.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://yw.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://cl.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lm.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://fe.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vo.nicolike.cn

[Q57] 行号
来源：http://ys.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ia.huanxung.cn

[Q58] 累计求和
来源：http://ld.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vq.panjiajie.cn

[Q59] 分组内累计
来源：http://od.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zq.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://xl.shxzukj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yj.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://la.shxzukj.cn

[Q61] 移动平均
来源：http://yv.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tz.521024.cn

[Q62] 分组占比
来源：http://ku.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pj.hnjuh.cn

[Q63] 开启事务
来源：http://uy.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tz.szxytkj.cn

[Q64] 提交事务
来源：http://ff.hnjuh.cn

COMMIT;
来源：http://ne.asd995.cn

[Q65] 回滚事务
来源：http://bz.szsharing.cn

ROLLBACK;
来源：http://cn.panjiajie.cn

[Q66] 行锁查询
来源：http://gf.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yb.hahajie.cn

[Q67] 设置隔离级别
来源：http://mf.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wx.panjiajie.cn

[Q68] 保存点
来源：http://ld.asd995.cn

SAVEPOINT sp1;
来源：http://jc.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://vd.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://xo.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://za.wgjwhj.cn

[Q70] 更新统计信息
来源：http://fh.nicolike.cn

ANALYZE TABLE users;
来源：http://si.asd995.cn

[Q71] 查看建表语句
来源：http://ao.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yk.shtwfgs.cn

[Q72] 查看索引
来源：http://tv.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://yu.haigaiapp.cn

[Q73] 查看表状态
来源：http://fo.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ca.huanxung.cn

[Q74] 强制使用索引
来源：http://bj.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xz.chemitech.net.cn

[Q75] 日期格式化
来源：http://yo.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yf.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pe.jianghongdianzi.cn

[Q76] 按天统计
来源：http://wg.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xg.nszjky.cn

[Q77] 时间加减
来源：http://mf.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tv.colortex.cn

[Q78] 当前时间
来源：http://al.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ya.hnjuh.cn

[Q79] 字符串拼接
来源：http://fn.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yz.chemitech.net.cn

[Q80] 字符串截取
来源：http://xf.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vz.shxzskj.cn

[Q81] 字符串替换
来源：http://ep.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ld.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://oi.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ag.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://qm.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zo.newstarts.cn

[Q84] 去除首尾空格
来源：http://qc.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://eo.yuntaijiaju.cn

[Q85] 数值取整
来源：http://be.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://of.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://wf.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://my.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://ta.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zm.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://hg.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oz.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ic.hnjuh.cn

[Q89] 判断表是否存在
来源：http://tq.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nz.9csxet.cn

[Q90] 生成序号列
来源：http://bn.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vc.shxzukj.cn

================================================================================
来源：http://mg.shxzukj.cn

R. Bash 专题
来源：http://uw.szxytkj.cn

================================================================================
来源：http://zw.521024.cn

[R01] shebang 与严格模式
来源：http://gx.jctech888.com.cn

#!/usr/bin/env bash
来源：http://zp.9csxet.cn

set -euo pipefail
来源：http://jt.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://dt.szxytkj.cn

name="Tom"; echo "$name"
来源：http://fh.shtwfgs.cn

[R03] 只读变量
来源：http://ow.wgjwhj.cn

readonly PI=3.14
来源：http://ql.muxihuayi.cn

[R04] 位置参数
来源：http://mo.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qx.colortex.cn

[R05] 参数默认值
来源：http://xb.521024.cn

name="${1:-default}"
来源：http://ye.szxytkj.cn

[R06] 判断命令是否存在
来源：http://gk.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ly.nicolike.cn

[R07] if 判断文件
来源：http://yj.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uh.shxzukj.cn

[R08] 数值比较
来源：http://je.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://at.jianghongdianzi.cn

[R09] 字符串比较
来源：http://et.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dd.colortex.cn

[R10] 正则匹配
来源：http://km.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rj.521024.cn

[R11] case 多分支
来源：http://bi.jianghongdianzi.cn

case "$1" in
来源：http://qb.szsharing.cn

start) echo "启动" ;;
来源：http://xy.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://af.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://zt.shtwfgs.cn

esac
来源：http://sk.panjiajie.cn

[R12] for 遍历文件
来源：http://yo.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://hv.shtwfgs.cn

[R13] for 计数循环
来源：http://sq.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://jp.bookmarksfly.cn

[R14] C 风格 for
来源：http://mr.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ha.521024.cn

[R15] while 逐行读文件
来源：http://jl.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tf.nicolike.cn

[R16] until 等待条件
来源：http://nf.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rm.521024.cn

[R17] 数组定义与取值
来源：http://bt.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gp.jianghongdianzi.cn

[R18] 遍历数组
来源：http://rs.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ws.jianghongdianzi.cn

[R19] 数组长度
来源：http://uv.shtwfgs.cn

echo "${#arr[@]}"
来源：http://hg.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://by.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fc.chemitech.net.cn

[R21] 字符串长度
来源：http://hh.muxihuayi.cn

echo "${#s}"
来源：http://ej.jianghongdianzi.cn

[R22] 截取子串
来源：http://lg.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://ow.huanxung.cn

[R23] 字符串替换
来源：http://jx.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hl.huixinmuqiang.cn

[R24] 大小写转换
来源：http://dj.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ea.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://gx.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ik.colortex.cn

[R26] 命令替换
来源：http://yl.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://ws.jianghongdianzi.cn

[R27] 算术展开
来源：http://sh.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://lj.jctech888.com.cn

[R28] 浮点运算
来源：http://ji.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://qk.colortex.cn

[R29] 定义函数
来源：http://jx.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eo.huixiangedu.cn

[R30] 函数返回状态码
来源：http://ai.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://ul.newstarts.cn

[R31] 局部变量
来源：http://ki.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://zq.wgjwhj.cn

[R32] 参数个数校验
来源：http://fa.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yl.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://zk.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aw.nszjky.cn

[R34] 退出时清理
来源：http://ou.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ea.asd995.cn

[R35] 后台执行并等待
来源：http://pv.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uh.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://dq.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bp.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://qt.newstarts.cn

files=$(ls -1)
来源：http://ud.chemitech.net.cn

[R38] 管道串联
来源：http://dq.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://ab.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://kk.szsharing.cn

cmd > out.log 2>&1
来源：http://vf.nszjky.cn

[R40] 追加写日志
来源：http://zz.jctech888.com.cn

echo "log" >> out.log
来源：http://rs.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://to.asd995.cn

cmd >/dev/null 2>&1
来源：http://mn.jianghongdianzi.cn

[R42] 输入重定向
来源：http://kq.szxytkj.cn

wc -l < a.txt
来源：http://nl.bjjhwx.cn

[R43] 按名字查找文件
来源：http://tf.colortex.cn

find . -name "*.log" -type f
来源：http://lp.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://wm.9csxet.cn

find . -mtime -7 -type f
来源：http://xu.nicolike.cn

[R45] 批量删除
来源：http://bp.szsharing.cn

find . -name "*.tmp" -delete
来源：http://zj.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://vj.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iv.lnxyls.cn

[R47] sed 单行替换
来源：http://ys.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wl.shtwfgs.cn

[R48] awk 取指定列
来源：http://cb.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://ea.yuntaijiaju.cn

[R49] awk 带条件
来源：http://gu.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wz.chemitech.net.cn

[R50] awk 求和
来源：http://xj.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jq.huixiangedu.cn

[R51] 排序去重取前几
来源：http://bz.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ow.wgjwhj.cn

[R52] 统计行数
来源：http://xk.hahajie.cn

wc -l a.txt
来源：http://un.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://ic.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pg.gzmigu.cn

[R54] 比较两个文件
来源：http://ty.szxytkj.cn

diff a.txt b.txt
来源：http://ac.yuexingan06.cn

[R55] 压缩与解压
来源：http://xc.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zu.hnjuh.cn

[R56] 远程拷贝
来源：http://mj.nicolike.cn

scp file user@host:/path/
来源：http://lq.wgjwhj.cn

[R57] 远程执行命令
来源：http://hz.bjjhwx.cn

ssh user@host 'uptime'
来源：http://wg.chemitech.net.cn

[R58] 下载文件
来源：http://en.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://br.yuexingan06.cn

[R59] 发 POST JSON
来源：http://ma.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ng.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://xi.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bf.lnxyls.cn

[R61] 磁盘占用
来源：http://pa.shxzskj.cn


<!-- 参考信息 -->