代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://rw.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rg.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hj.nicolike.cn

[Q15] 查询全部
来源：http://lc.521024.cn

SELECT * FROM users;
来源：http://cy.newstarts.cn

[Q16] 查询指定列
来源：http://jv.haigaiapp.cn

SELECT id, name FROM users;
来源：http://tf.bjjhwx.cn

[Q17] 条件查询
来源：http://yu.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pl.shtwfgs.cn

[Q18] 模糊匹配
来源：http://or.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://il.shxzskj.cn

[Q19] 范围查询
来源：http://ds.shxzukj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xb.lnxyls.cn

[Q20] IN 列表
来源：http://pq.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pl.gzmigu.cn

[Q21] 空值判断
来源：http://wh.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uq.shxzukj.cn

[Q22] 排序
来源：http://cf.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xw.hnjuh.cn

[Q23] 分页
来源：http://ph.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gr.jctech888.com.cn

[Q24] 去重
来源：http://gn.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://er.newstarts.cn

[Q25] 只取前 N 条
来源：http://or.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xe.bookmarksfly.cn

[Q26] 计数
来源：http://iy.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://nw.wgjwhj.cn

[Q27] 条件计数
来源：http://ud.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pg.nicolike.cn

[Q28] 求和与平均
来源：http://jd.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rd.szxytkj.cn

[Q29] 最大最小值
来源：http://xu.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sq.huixinmuqiang.cn

[Q30] 分组统计
来源：http://mv.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cx.gzmigu.cn

[Q31] 分组后过滤
来源：http://eb.bookmarksfly.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://is.asd995.cn

[Q32] 分组拼接字符串
来源：http://tu.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rk.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuexingan06.cn

[Q33] 多列分组
来源：http://ew.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tv.hahajie.cn

[Q34] 每组取第一条
来源：http://gj.chemitech.net.cn

SELECT * FROM (
来源：http://cx.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://la.bjjhwx.cn

) t WHERE rn = 1;
来源：http://mb.jctech888.com.cn

[Q35] 内连接
来源：http://ic.bookmarksfly.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pp.wgjwhj.cn

[Q36] 左连接
来源：http://mn.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hh.jianghongdianzi.cn

[Q37] 右连接
来源：http://zw.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cx.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kb.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uq.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://kj.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qf.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pz.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ho.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rk.shxzskj.cn

[Q41] 多表连接
来源：http://hc.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fk.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://mz.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://ou.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://lt.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://pn.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yk.hnjuh.cn

[Q43] 标量子查询
来源：http://uu.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vv.panjiajie.cn

[Q44] IN 子查询
来源：http://ou.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pp.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://wz.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mi.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bn.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kf.521024.cn

[Q47] 与平均值比较
来源：http://dr.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cd.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://us.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rq.jctech888.com.cn

SELECT * FROM t WHERE c > 5;
来源：http://pc.chemitech.net.cn

[Q49] 更新单行
来源：http://no.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gw.gzmigu.cn

[Q50] 批量更新
来源：http://ys.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dv.bjjhwx.cn

[Q51] 用子查询更新
来源：http://md.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://px.panjiajie.cn

[Q52] 删除指定行
来源：http://qo.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://vv.panjiajie.cn

[Q53] 按条件删除
来源：http://jz.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mh.bjjhwx.cn

[Q54] 清空表
来源：http://uc.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://kz.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://al.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gl.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://yy.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://na.shxzukj.cn

[Q57] 行号
来源：http://pq.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qq.szxytkj.cn

[Q58] 累计求和
来源：http://lw.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zf.asd995.cn

[Q59] 分组内累计
来源：http://oc.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://av.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://dd.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wk.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tw.chemitech.net.cn

[Q61] 移动平均
来源：http://xf.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://it.wgjwhj.cn

[Q62] 分组占比
来源：http://qv.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kj.huixinmuqiang.cn

[Q63] 开启事务
来源：http://lo.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uo.9csxet.cn

[Q64] 提交事务
来源：http://ve.jianghongdianzi.cn

COMMIT;
来源：http://bn.shtwfgs.cn

[Q65] 回滚事务
来源：http://gz.muxihuayi.cn

ROLLBACK;
来源：http://cp.hahajie.cn

[Q66] 行锁查询
来源：http://ey.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ma.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://tf.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qm.nszjky.cn

[Q68] 保存点
来源：http://ui.chemitech.net.cn

SAVEPOINT sp1;
来源：http://to.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://rl.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://sj.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vo.szsharing.cn

[Q70] 更新统计信息
来源：http://wg.nicolike.cn

ANALYZE TABLE users;
来源：http://iw.szxytkj.cn

[Q71] 查看建表语句
来源：http://sz.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jx.haigaiapp.cn

[Q72] 查看索引
来源：http://ne.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://ep.shxzukj.cn

[Q73] 查看表状态
来源：http://dn.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ah.shxzskj.cn

[Q74] 强制使用索引
来源：http://vw.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wq.panjiajie.cn

[Q75] 日期格式化
来源：http://id.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cy.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nr.szxytkj.cn

[Q76] 按天统计
来源：http://lx.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://se.hnjuh.cn

[Q77] 时间加减
来源：http://eb.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xb.hahajie.cn

[Q78] 当前时间
来源：http://ek.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vp.huanxung.cn

[Q79] 字符串拼接
来源：http://ve.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ct.shtwfgs.cn

[Q80] 字符串截取
来源：http://zk.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uy.bookmarksfly.cn

[Q81] 字符串替换
来源：http://yq.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gs.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://ha.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://te.huixiangedu.cn

[Q83] 大小写转换
来源：http://kg.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vf.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://za.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://cz.bjjhwx.cn

[Q85] 数值取整
来源：http://ap.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ri.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://el.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dm.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://bd.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://is.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://zo.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://th.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ua.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://xw.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://co.nicolike.cn

[Q90] 生成序号列
来源：http://xj.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lt.huixinmuqiang.cn

================================================================================
来源：http://gu.gzmigu.cn

R. Bash 专题
来源：http://sb.chemitech.net.cn

================================================================================
来源：http://ef.hnjuh.cn

[R01] shebang 与严格模式
来源：http://bo.colortex.cn

#!/usr/bin/env bash
来源：http://mg.shtwfgs.cn

set -euo pipefail
来源：http://ad.nicolike.cn

[R02] 变量赋值与使用
来源：http://um.shxzskj.cn

name="Tom"; echo "$name"
来源：http://er.521024.cn

[R03] 只读变量
来源：http://fw.panjiajie.cn

readonly PI=3.14
来源：http://fg.hahajie.cn

[R04] 位置参数
来源：http://qx.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ys.jctech888.com.cn

[R05] 参数默认值
来源：http://ss.hnjuh.cn

name="${1:-default}"
来源：http://xh.asd995.cn

[R06] 判断命令是否存在
来源：http://mc.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nm.jctech888.com.cn

[R07] if 判断文件
来源：http://pd.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hk.9csxet.cn

[R08] 数值比较
来源：http://re.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://um.asd995.cn

[R09] 字符串比较
来源：http://oy.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pv.gzmigu.cn

[R10] 正则匹配
来源：http://sq.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fn.asd995.cn

[R11] case 多分支
来源：http://ny.chemitech.net.cn

case "$1" in
来源：http://cq.szxytkj.cn

start) echo "启动" ;;
来源：http://st.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://xq.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://sw.szxytkj.cn

esac
来源：http://dl.gzmigu.cn

[R12] for 遍历文件
来源：http://fi.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://fr.nszjky.cn

[R13] for 计数循环
来源：http://hl.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://qu.shtwfgs.cn

[R14] C 风格 for
来源：http://wm.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pa.gzmigu.cn

[R15] while 逐行读文件
来源：http://dw.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vj.nicolike.cn

[R16] until 等待条件
来源：http://om.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ck.wgjwhj.cn

[R17] 数组定义与取值
来源：http://gd.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ay.szsharing.cn

[R18] 遍历数组
来源：http://cq.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dl.nicolike.cn

[R19] 数组长度
来源：http://de.yuexingan06.cn

echo "${#arr[@]}"
来源：http://vr.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://kd.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nq.bookmarksfly.cn

[R21] 字符串长度
来源：http://lj.hahajie.cn

echo "${#s}"
来源：http://cj.huixiangedu.cn

[R22] 截取子串
来源：http://nx.9csxet.cn

echo "${s:0:5}"
来源：http://ex.asd995.cn

[R23] 字符串替换
来源：http://hg.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pt.shxzukj.cn

[R24] 大小写转换
来源：http://qx.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://af.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://zz.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kx.colortex.cn

[R26] 命令替换
来源：http://mf.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://wx.huixinmuqiang.cn

[R27] 算术展开
来源：http://tr.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://ek.chemitech.net.cn

[R28] 浮点运算
来源：http://va.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://ml.gzmigu.cn

[R29] 定义函数
来源：http://fm.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://le.hahajie.cn

[R30] 函数返回状态码
来源：http://cz.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://ba.asd995.cn

[R31] 局部变量
来源：http://dd.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://sg.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://tz.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aa.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://ou.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kq.wgjwhj.cn

[R34] 退出时清理
来源：http://sd.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zw.haigaiapp.cn

[R35] 后台执行并等待
来源：http://ib.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sc.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://nm.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://id.lnxyls.cn

[R37] 把输出赋给变量
来源：http://sd.szsharing.cn

files=$(ls -1)
来源：http://to.jianghongdianzi.cn

[R38] 管道串联
来源：http://ex.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://qu.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://vv.shtwfgs.cn

cmd > out.log 2>&1
来源：http://pi.yuntaijiaju.cn

[R40] 追加写日志
来源：http://mv.nicolike.cn

echo "log" >> out.log
来源：http://nq.szsharing.cn

[R41] 丢弃输出
来源：http://re.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://kb.newstarts.cn

[R42] 输入重定向
来源：http://hi.muxihuayi.cn

wc -l < a.txt
来源：http://ua.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://rw.yuexingan06.cn

find . -name "*.log" -type f
来源：http://vi.asd995.cn

[R44] 按修改时间查找
来源：http://pd.panjiajie.cn

find . -mtime -7 -type f
来源：http://jg.chemitech.net.cn

[R45] 批量删除
来源：http://mo.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://yz.huanxung.cn

[R46] 递归替换文件内容
来源：http://lk.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jc.muxihuayi.cn

[R47] sed 单行替换
来源：http://cl.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vd.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://mo.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://na.huixinmuqiang.cn

[R49] awk 带条件
来源：http://ne.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kc.szsharing.cn

[R50] awk 求和
来源：http://eo.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cx.jctech888.com.cn

[R51] 排序去重取前几
来源：http://yv.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://er.yuexingan06.cn

[R52] 统计行数
来源：http://va.hnjuh.cn

wc -l a.txt
来源：http://tf.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://kn.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://se.jctech888.com.cn

[R54] 比较两个文件
来源：http://xz.nicolike.cn

diff a.txt b.txt
来源：http://ha.szxytkj.cn

[R55] 压缩与解压
来源：http://ra.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kz.panjiajie.cn

[R56] 远程拷贝
来源：http://zg.huanxung.cn

scp file user@host:/path/
来源：http://fv.chemitech.net.cn

[R57] 远程执行命令
来源：http://vj.nszjky.cn

ssh user@host 'uptime'
来源：http://wx.panjiajie.cn

[R58] 下载文件
来源：http://mp.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tz.chemitech.net.cn

[R59] 发 POST JSON
来源：http://qc.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cb.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://fy.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yj.szxytkj.cn

[R61] 磁盘占用
来源：http://lc.szsharing.cn

df -h;  du -sh *
来源：http://va.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://wn.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://pk.colortex.cn

[R63] 内存与进程
来源：http://ea.colortex.cn


<!-- 参考信息 -->