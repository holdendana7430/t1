代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://un.lnxyls.cn

[Q11] 一次插入多行
来源：http://xm.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nc.wgjwhj.cn

[Q12] 插入后取自增 ID
来源：http://fe.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cn.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lh.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://dz.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fq.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://ug.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lk.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qt.haigaiapp.cn

[Q15] 查询全部
来源：http://mf.bjjhwx.cn

SELECT * FROM users;
来源：http://rn.hahajie.cn

[Q16] 查询指定列
来源：http://lt.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://tm.wgjwhj.cn

[Q17] 条件查询
来源：http://xj.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://es.haigaiapp.cn

[Q18] 模糊匹配
来源：http://hc.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xq.wgjwhj.cn

[Q19] 范围查询
来源：http://hw.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ys.nicolike.cn

[Q20] IN 列表
来源：http://ws.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mj.chemitech.net.cn

[Q21] 空值判断
来源：http://tp.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eh.shxzukj.cn

[Q22] 排序
来源：http://sg.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ty.huanxung.cn

[Q23] 分页
来源：http://lf.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ze.asd995.cn

[Q24] 去重
来源：http://mt.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://iv.hahajie.cn

[Q25] 只取前 N 条
来源：http://uo.asd995.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yy.muxihuayi.cn

[Q26] 计数
来源：http://ab.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://og.lnxyls.cn

[Q27] 条件计数
来源：http://zp.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kw.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://rp.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tq.nicolike.cn

[Q29] 最大最小值
来源：http://vy.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://aj.panjiajie.cn

[Q30] 分组统计
来源：http://vg.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uj.yuexingan06.cn

[Q31] 分组后过滤
来源：http://vv.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vl.newstarts.cn

[Q32] 分组拼接字符串
来源：http://qw.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ka.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dl.haigaiapp.cn

[Q33] 多列分组
来源：http://nc.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ns.shxzukj.cn

[Q34] 每组取第一条
来源：http://ho.lnxyls.cn

SELECT * FROM (
来源：http://ex.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://au.wgjwhj.cn

) t WHERE rn = 1;
来源：http://op.hahajie.cn

[Q35] 内连接
来源：http://yz.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zq.yuexingan06.cn

[Q36] 左连接
来源：http://mc.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hq.huixinmuqiang.cn

[Q37] 右连接
来源：http://yv.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zg.muxihuayi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fj.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mc.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://pt.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lg.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rm.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qn.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://or.asd995.cn

[Q41] 多表连接
来源：http://cb.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wr.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://ui.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://ri.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://dy.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://kr.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ki.asd995.cn

[Q43] 标量子查询
来源：http://en.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xu.yuexingan06.cn

[Q44] IN 子查询
来源：http://ei.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ey.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://qn.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tf.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gw.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aw.asd995.cn

[Q47] 与平均值比较
来源：http://nk.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yj.bjjhwx.cn

[Q48] CTE 公用表表达式
来源：http://zd.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ud.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://yr.lnxyls.cn

[Q49] 更新单行
来源：http://xk.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dq.shtwfgs.cn

[Q50] 批量更新
来源：http://ud.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kl.yuexingan06.cn

[Q51] 用子查询更新
来源：http://iu.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qn.huanxung.cn

[Q52] 删除指定行
来源：http://bd.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://sw.hahajie.cn

[Q53] 按条件删除
来源：http://bu.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wo.huixinmuqiang.cn

[Q54] 清空表
来源：http://gb.huanxung.cn

TRUNCATE TABLE logs;
来源：http://or.colortex.cn

[Q55] 排名（并列占位）
来源：http://or.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fp.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://qn.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nw.shxzskj.cn

[Q57] 行号
来源：http://pp.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://en.hnjuh.cn

[Q58] 累计求和
来源：http://qr.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mm.haigaiapp.cn

[Q59] 分组内累计
来源：http://bw.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rk.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://wz.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ep.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gm.huixiangedu.cn

[Q61] 移动平均
来源：http://fo.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ij.chemitech.net.cn

[Q62] 分组占比
来源：http://bp.shxzukj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://my.gzmigu.cn

[Q63] 开启事务
来源：http://om.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ss.yuntaijiaju.cn

[Q64] 提交事务
来源：http://ip.panjiajie.cn

COMMIT;
来源：http://bn.nszjky.cn

[Q65] 回滚事务
来源：http://yd.bookmarksfly.cn

ROLLBACK;
来源：http://fr.gzmigu.cn

[Q66] 行锁查询
来源：http://zv.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xu.hnjuh.cn

[Q67] 设置隔离级别
来源：http://dx.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fn.nszjky.cn

[Q68] 保存点
来源：http://jd.hnjuh.cn

SAVEPOINT sp1;
来源：http://xp.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://nh.szsharing.cn

[Q69] 查看执行计划
来源：http://up.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bf.bjjhwx.cn

[Q70] 更新统计信息
来源：http://yi.wgjwhj.cn

ANALYZE TABLE users;
来源：http://dv.wgjwhj.cn

[Q71] 查看建表语句
来源：http://rw.huanxung.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ou.shtwfgs.cn

[Q72] 查看索引
来源：http://be.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://gk.muxihuayi.cn

[Q73] 查看表状态
来源：http://ry.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wn.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://zh.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lr.newstarts.cn

[Q75] 日期格式化
来源：http://va.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gt.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dq.panjiajie.cn

[Q76] 按天统计
来源：http://ja.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rs.colortex.cn

[Q77] 时间加减
来源：http://lz.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wo.szxytkj.cn

[Q78] 当前时间
来源：http://hf.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yv.wgjwhj.cn

[Q79] 字符串拼接
来源：http://rf.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yj.bookmarksfly.cn

[Q80] 字符串截取
来源：http://uf.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jg.szsharing.cn

[Q81] 字符串替换
来源：http://vk.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gd.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://rk.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bb.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://nq.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ja.hnjuh.cn

[Q84] 去除首尾空格
来源：http://ee.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://qo.shxzukj.cn

[Q85] 数值取整
来源：http://un.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yv.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://dz.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ly.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://zf.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lb.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://vh.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nq.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gc.huanxung.cn

[Q89] 判断表是否存在
来源：http://cl.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ng.wgjwhj.cn

[Q90] 生成序号列
来源：http://ua.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ut.shtwfgs.cn

================================================================================
来源：http://ha.shtwfgs.cn

R. Bash 专题
来源：http://xe.colortex.cn

================================================================================
来源：http://mg.nicolike.cn

[R01] shebang 与严格模式
来源：http://ue.nszjky.cn

#!/usr/bin/env bash
来源：http://of.shxzukj.cn

set -euo pipefail
来源：http://eg.hnjuh.cn

[R02] 变量赋值与使用
来源：http://wv.lnxyls.cn

name="Tom"; echo "$name"
来源：http://le.chemitech.net.cn

[R03] 只读变量
来源：http://ky.hahajie.cn

readonly PI=3.14
来源：http://sp.wgjwhj.cn

[R04] 位置参数
来源：http://ys.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vm.yuexingan06.cn

[R05] 参数默认值
来源：http://pc.nszjky.cn

name="${1:-default}"
来源：http://qp.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://mr.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ry.shtwfgs.cn

[R07] if 判断文件
来源：http://al.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ou.lnxyls.cn

[R08] 数值比较
来源：http://zh.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xg.bjjhwx.cn

[R09] 字符串比较
来源：http://vh.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hd.gzmigu.cn

[R10] 正则匹配
来源：http://ah.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ia.hahajie.cn

[R11] case 多分支
来源：http://gk.jianghongdianzi.cn

case "$1" in
来源：http://pp.newstarts.cn

start) echo "启动" ;;
来源：http://pw.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://kp.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://zz.jianghongdianzi.cn

esac
来源：http://ke.nszjky.cn

[R12] for 遍历文件
来源：http://xh.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://rz.bjjhwx.cn

[R13] for 计数循环
来源：http://gn.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://kz.nicolike.cn

[R14] C 风格 for
来源：http://aq.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bo.haigaiapp.cn

[R15] while 逐行读文件
来源：http://mj.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ty.chemitech.net.cn

[R16] until 等待条件
来源：http://zk.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zm.gzmigu.cn

[R17] 数组定义与取值
来源：http://qi.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cu.colortex.cn

[R18] 遍历数组
来源：http://ag.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kd.gzmigu.cn

[R19] 数组长度
来源：http://bo.shxzskj.cn

echo "${#arr[@]}"
来源：http://nt.asd995.cn

[R20] 关联数组（字典）
来源：http://tn.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hg.jianghongdianzi.cn

[R21] 字符串长度
来源：http://dj.yuexingan06.cn

echo "${#s}"
来源：http://mm.newstarts.cn

[R22] 截取子串
来源：http://oj.panjiajie.cn

echo "${s:0:5}"
来源：http://fs.szxytkj.cn

[R23] 字符串替换
来源：http://jc.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ry.jianghongdianzi.cn

[R24] 大小写转换
来源：http://yp.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gk.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://fo.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mt.muxihuayi.cn

[R26] 命令替换
来源：http://bq.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://xd.szxytkj.cn

[R27] 算术展开
来源：http://yf.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://jy.jctech888.com.cn

[R28] 浮点运算
来源：http://ua.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://nu.hnjuh.cn

[R29] 定义函数
来源：http://xk.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ur.gzmigu.cn

[R30] 函数返回状态码
来源：http://pw.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://em.huanxung.cn

[R31] 局部变量
来源：http://yc.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://cc.haigaiapp.cn

[R32] 参数个数校验
来源：http://si.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mv.521024.cn

[R33] 捕获错误并提示行号
来源：http://nw.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vb.huixiangedu.cn

[R34] 退出时清理
来源：http://mq.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sz.shxzskj.cn

[R35] 后台执行并等待
来源：http://sv.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xa.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://vj.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kg.newstarts.cn

[R37] 把输出赋给变量
来源：http://vl.521024.cn

files=$(ls -1)
来源：http://ea.chemitech.net.cn

[R38] 管道串联
来源：http://zr.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://ya.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://fd.newstarts.cn

cmd > out.log 2>&1
来源：http://vq.lnxyls.cn

[R40] 追加写日志
来源：http://sp.asd995.cn

echo "log" >> out.log
来源：http://rp.nicolike.cn

[R41] 丢弃输出
来源：http://cp.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://dd.shtwfgs.cn

[R42] 输入重定向
来源：http://xk.9csxet.cn

wc -l < a.txt
来源：http://te.wgjwhj.cn

[R43] 按名字查找文件
来源：http://ut.colortex.cn

find . -name "*.log" -type f
来源：http://ea.shtwfgs.cn

[R44] 按修改时间查找
来源：http://yd.bjjhwx.cn

find . -mtime -7 -type f
来源：http://bq.bookmarksfly.cn

[R45] 批量删除
来源：http://co.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://jc.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://uh.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://re.hahajie.cn

[R47] sed 单行替换
来源：http://ac.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://az.wgjwhj.cn

[R48] awk 取指定列
来源：http://xv.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://vk.huixiangedu.cn

[R49] awk 带条件
来源：http://oa.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://at.wgjwhj.cn

[R50] awk 求和
来源：http://sh.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vn.521024.cn

[R51] 排序去重取前几
来源：http://ad.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hf.huixinmuqiang.cn

[R52] 统计行数
来源：http://rl.shtwfgs.cn

wc -l a.txt
来源：http://py.asd995.cn

[R53] 查看文件头与实时尾
来源：http://hq.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pj.hnjuh.cn

[R54] 比较两个文件
来源：http://qt.newstarts.cn

diff a.txt b.txt
来源：http://kf.szsharing.cn

[R55] 压缩与解压
来源：http://jk.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qg.shxzukj.cn

[R56] 远程拷贝
来源：http://ie.shxzukj.cn

scp file user@host:/path/
来源：http://ih.jctech888.com.cn

[R57] 远程执行命令
来源：http://cw.jctech888.com.cn

ssh user@host 'uptime'
来源：http://bq.521024.cn

[R58] 下载文件
来源：http://my.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eb.shxzskj.cn

[R59] 发 POST JSON
来源：http://wc.nicolike.cn


<!-- 参考信息 -->