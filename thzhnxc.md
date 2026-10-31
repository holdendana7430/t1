代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://yw.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ti.lnxyls.cn

[Q13] 忽略重复插入
来源：http://fd.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vv.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://jk.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ua.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dn.chemitech.net.cn

[Q15] 查询全部
来源：http://hn.shtwfgs.cn

SELECT * FROM users;
来源：http://uo.nicolike.cn

[Q16] 查询指定列
来源：http://br.nicolike.cn

SELECT id, name FROM users;
来源：http://ph.521024.cn

[Q17] 条件查询
来源：http://wy.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://br.szxytkj.cn

[Q18] 模糊匹配
来源：http://dc.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fm.szsharing.cn

[Q19] 范围查询
来源：http://ly.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ir.szsharing.cn

[Q20] IN 列表
来源：http://cx.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yp.jctech888.com.cn

[Q21] 空值判断
来源：http://oq.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ds.panjiajie.cn

[Q22] 排序
来源：http://rs.panjiajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rm.yuexingan06.cn

[Q23] 分页
来源：http://wf.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mt.muxihuayi.cn

[Q24] 去重
来源：http://si.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://zn.nicolike.cn

[Q25] 只取前 N 条
来源：http://gr.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fp.gzmigu.cn

[Q26] 计数
来源：http://mz.gzmigu.cn

SELECT COUNT(*) FROM users;
来源：http://vl.colortex.cn

[Q27] 条件计数
来源：http://sw.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qf.wgjwhj.cn

[Q28] 求和与平均
来源：http://ep.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xs.hnjuh.cn

[Q29] 最大最小值
来源：http://xt.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dg.szxytkj.cn

[Q30] 分组统计
来源：http://uj.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ib.newstarts.cn

[Q31] 分组后过滤
来源：http://ic.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gn.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://nn.jctech888.com.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eo.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nr.shtwfgs.cn

[Q33] 多列分组
来源：http://yc.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ow.hahajie.cn

[Q34] 每组取第一条
来源：http://mm.yuexingan06.cn

SELECT * FROM (
来源：http://dz.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xp.hahajie.cn

) t WHERE rn = 1;
来源：http://lv.9csxet.cn

[Q35] 内连接
来源：http://mx.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oy.521024.cn

[Q36] 左连接
来源：http://al.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jn.wgjwhj.cn

[Q37] 右连接
来源：http://zg.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://su.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xk.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jv.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://yc.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://me.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://no.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vm.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aj.wgjwhj.cn

[Q41] 多表连接
来源：http://cg.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pp.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://ko.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://nq.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://bl.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://kz.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ci.huanxung.cn

[Q43] 标量子查询
来源：http://ek.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rl.jctech888.com.cn

[Q44] IN 子查询
来源：http://qa.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ri.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://nw.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yj.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://he.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ur.newstarts.cn

[Q47] 与平均值比较
来源：http://of.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://te.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://yv.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vx.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://ds.newstarts.cn

[Q49] 更新单行
来源：http://hz.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dm.nszjky.cn

[Q50] 批量更新
来源：http://ct.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gi.hnjuh.cn

[Q51] 用子查询更新
来源：http://iq.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pk.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://xs.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://wu.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://zt.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hf.gzmigu.cn

[Q54] 清空表
来源：http://wc.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://vp.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://rs.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dl.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://ns.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vt.huixiangedu.cn

[Q57] 行号
来源：http://fd.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zy.huanxung.cn

[Q58] 累计求和
来源：http://ve.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://za.521024.cn

[Q59] 分组内累计
来源：http://sn.yuntaijiaju.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dl.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://lj.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dq.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qc.huanxung.cn

[Q61] 移动平均
来源：http://pl.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qk.bookmarksfly.cn

[Q62] 分组占比
来源：http://pu.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qv.huixinmuqiang.cn

[Q63] 开启事务
来源：http://xp.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xh.yuexingan06.cn

[Q64] 提交事务
来源：http://qy.hahajie.cn

COMMIT;
来源：http://os.haigaiapp.cn

[Q65] 回滚事务
来源：http://ga.bjjhwx.cn

ROLLBACK;
来源：http://df.yuexingan06.cn

[Q66] 行锁查询
来源：http://bj.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fc.lnxyls.cn

[Q67] 设置隔离级别
来源：http://dq.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qs.muxihuayi.cn

[Q68] 保存点
来源：http://ls.muxihuayi.cn

SAVEPOINT sp1;
来源：http://vw.huanxung.cn

ROLLBACK TO sp1;
来源：http://hu.yuexingan06.cn

[Q69] 查看执行计划
来源：http://aw.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vx.huixiangedu.cn

[Q70] 更新统计信息
来源：http://tr.colortex.cn

ANALYZE TABLE users;
来源：http://qb.wgjwhj.cn

[Q71] 查看建表语句
来源：http://ko.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qw.huixiangedu.cn

[Q72] 查看索引
来源：http://qc.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://on.muxihuayi.cn

[Q73] 查看表状态
来源：http://gn.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fs.muxihuayi.cn

[Q74] 强制使用索引
来源：http://qg.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xd.521024.cn

[Q75] 日期格式化
来源：http://sp.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pl.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mr.hahajie.cn

[Q76] 按天统计
来源：http://vq.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rm.hnjuh.cn

[Q77] 时间加减
来源：http://mv.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pn.haigaiapp.cn

[Q78] 当前时间
来源：http://dg.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://on.nszjky.cn

[Q79] 字符串拼接
来源：http://is.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yj.haigaiapp.cn

[Q80] 字符串截取
来源：http://zm.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kh.shxzukj.cn

[Q81] 字符串替换
来源：http://kp.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cd.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://lo.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yg.bjjhwx.cn

[Q83] 大小写转换
来源：http://wo.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yr.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://nr.521024.cn

SELECT TRIM(name) FROM users;
来源：http://qs.panjiajie.cn

[Q85] 数值取整
来源：http://ro.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ia.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://ew.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://be.szsharing.cn

[Q87] JSON 字段做条件
来源：http://gn.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xb.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://fr.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://af.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oo.lnxyls.cn

[Q89] 判断表是否存在
来源：http://tj.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wk.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://dp.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cg.shxzukj.cn

================================================================================
来源：http://jr.bjjhwx.cn

R. Bash 专题
来源：http://iw.asd995.cn

================================================================================
来源：http://ry.nicolike.cn

[R01] shebang 与严格模式
来源：http://lr.muxihuayi.cn

#!/usr/bin/env bash
来源：http://lt.nicolike.cn

set -euo pipefail
来源：http://aj.newstarts.cn

[R02] 变量赋值与使用
来源：http://py.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://jf.huanxung.cn

[R03] 只读变量
来源：http://cn.yuexingan06.cn

readonly PI=3.14
来源：http://sc.colortex.cn

[R04] 位置参数
来源：http://cg.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yb.bookmarksfly.cn

[R05] 参数默认值
来源：http://in.gzmigu.cn

name="${1:-default}"
来源：http://tj.szxytkj.cn

[R06] 判断命令是否存在
来源：http://gz.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lf.hahajie.cn

[R07] if 判断文件
来源：http://bv.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gk.colortex.cn

[R08] 数值比较
来源：http://xc.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://il.haigaiapp.cn

[R09] 字符串比较
来源：http://xs.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ag.jctech888.com.cn

[R10] 正则匹配
来源：http://oc.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ki.hahajie.cn

[R11] case 多分支
来源：http://io.newstarts.cn

case "$1" in
来源：http://sk.shxzskj.cn

start) echo "启动" ;;
来源：http://lz.szsharing.cn

stop)  echo "停止" ;;
来源：http://zg.huixinmuqiang.cn

*)     echo "未知命令" ;;
来源：http://ww.jctech888.com.cn

esac
来源：http://ke.shtwfgs.cn

[R12] for 遍历文件
来源：http://za.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://xk.huixinmuqiang.cn

[R13] for 计数循环
来源：http://sb.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://xd.huixiangedu.cn

[R14] C 风格 for
来源：http://qb.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xt.hahajie.cn

[R15] while 逐行读文件
来源：http://al.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kk.bookmarksfly.cn

[R16] until 等待条件
来源：http://kr.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yz.chemitech.net.cn

[R17] 数组定义与取值
来源：http://wz.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kj.szxytkj.cn

[R18] 遍历数组
来源：http://nf.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mu.shtwfgs.cn

[R19] 数组长度
来源：http://gt.yuexingan06.cn

echo "${#arr[@]}"
来源：http://xb.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://vp.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ws.521024.cn

[R21] 字符串长度
来源：http://qj.muxihuayi.cn

echo "${#s}"
来源：http://iw.shxzukj.cn

[R22] 截取子串
来源：http://ge.gzmigu.cn

echo "${s:0:5}"
来源：http://wx.nicolike.cn

[R23] 字符串替换
来源：http://uc.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mq.nicolike.cn

[R24] 大小写转换
来源：http://yd.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jk.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://wg.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://iu.yuexingan06.cn

[R26] 命令替换
来源：http://xw.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://qb.szsharing.cn

[R27] 算术展开
来源：http://xu.nszjky.cn

echo $((1 + 2 * 3))
来源：http://qo.szsharing.cn

[R28] 浮点运算
来源：http://pv.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://cq.shtwfgs.cn

[R29] 定义函数
来源：http://jf.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ew.nszjky.cn

[R30] 函数返回状态码
来源：http://ki.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://uw.bjjhwx.cn

[R31] 局部变量
来源：http://oj.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://ew.hnjuh.cn

[R32] 参数个数校验
来源：http://zf.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hi.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://sm.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mc.521024.cn

[R34] 退出时清理
来源：http://hw.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bh.bjjhwx.cn

[R35] 后台执行并等待
来源：http://kf.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oo.huanxung.cn

[R36] 并发执行多个任务
来源：http://tj.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xm.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://iv.shxzskj.cn

files=$(ls -1)
来源：http://lj.asd995.cn

[R38] 管道串联
来源：http://oo.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://nc.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://vn.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://ht.hahajie.cn

[R40] 追加写日志
来源：http://ez.jianghongdianzi.cn

echo "log" >> out.log
来源：http://tz.szsharing.cn

[R41] 丢弃输出
来源：http://rs.huanxung.cn

cmd >/dev/null 2>&1
来源：http://mk.huixiangedu.cn

[R42] 输入重定向
来源：http://hn.nicolike.cn

wc -l < a.txt
来源：http://lm.haigaiapp.cn

[R43] 按名字查找文件
来源：http://jv.shtwfgs.cn

find . -name "*.log" -type f
来源：http://xg.wgjwhj.cn

[R44] 按修改时间查找
来源：http://iu.muxihuayi.cn

find . -mtime -7 -type f
来源：http://ea.panjiajie.cn

[R45] 批量删除
来源：http://yz.nszjky.cn

find . -name "*.tmp" -delete
来源：http://jm.shxzskj.cn

[R46] 递归替换文件内容
来源：http://fd.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pd.wgjwhj.cn

[R47] sed 单行替换
来源：http://zk.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ut.chemitech.net.cn

[R48] awk 取指定列
来源：http://lw.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://rd.asd995.cn

[R49] awk 带条件
来源：http://yn.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wq.jianghongdianzi.cn

[R50] awk 求和
来源：http://kh.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hk.chemitech.net.cn

[R51] 排序去重取前几
来源：http://eb.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zi.nszjky.cn

[R52] 统计行数
来源：http://fp.hahajie.cn

wc -l a.txt
来源：http://kk.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://kx.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xv.colortex.cn

[R54] 比较两个文件
来源：http://ha.huanxung.cn

diff a.txt b.txt
来源：http://ld.hnjuh.cn

[R55] 压缩与解压
来源：http://cg.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bh.shxzukj.cn

[R56] 远程拷贝
来源：http://mi.muxihuayi.cn

scp file user@host:/path/
来源：http://fi.shxzskj.cn

[R57] 远程执行命令
来源：http://pu.huanxung.cn

ssh user@host 'uptime'
来源：http://ce.shxzskj.cn

[R58] 下载文件
来源：http://dj.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ud.lnxyls.cn

[R59] 发 POST JSON
来源：http://pc.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vp.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://nj.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xn.panjiajie.cn

[R61] 磁盘占用
来源：http://mg.jianghongdianzi.cn


<!-- 参考信息 -->