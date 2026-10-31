代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wy.yuexingan06.cn

[Q18] 模糊匹配
来源：http://zr.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yg.nszjky.cn

[Q19] 范围查询
来源：http://mc.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ys.shxzukj.cn

[Q20] IN 列表
来源：http://lf.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jx.chemitech.net.cn

[Q21] 空值判断
来源：http://jf.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ve.bookmarksfly.cn

[Q22] 排序
来源：http://yp.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zp.huixiangedu.cn

[Q23] 分页
来源：http://qh.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://op.9csxet.cn

[Q24] 去重
来源：http://zn.521024.cn

SELECT DISTINCT city FROM users;
来源：http://ys.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://sr.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ao.huixinmuqiang.cn

[Q26] 计数
来源：http://tt.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://hg.wgjwhj.cn

[Q27] 条件计数
来源：http://pb.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rv.szsharing.cn

[Q28] 求和与平均
来源：http://kn.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://li.nszjky.cn

[Q29] 最大最小值
来源：http://zm.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://no.bookmarksfly.cn

[Q30] 分组统计
来源：http://ov.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ul.chemitech.net.cn

[Q31] 分组后过滤
来源：http://hw.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cl.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://cg.jctech888.com.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://je.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://di.9csxet.cn

[Q33] 多列分组
来源：http://du.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ef.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://nf.hnjuh.cn

SELECT * FROM (
来源：http://eg.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hf.chemitech.net.cn

) t WHERE rn = 1;
来源：http://zg.muxihuayi.cn

[Q35] 内连接
来源：http://ag.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://or.gzmigu.cn

[Q36] 左连接
来源：http://vd.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fg.gzmigu.cn

[Q37] 右连接
来源：http://ct.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xk.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lr.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pa.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://rp.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mf.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zc.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ue.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nf.muxihuayi.cn

[Q41] 多表连接
来源：http://hz.muxihuayi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hs.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://ac.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://sl.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://fn.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://rq.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mo.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://nq.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zl.bookmarksfly.cn

[Q44] IN 子查询
来源：http://yz.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bc.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://wt.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yw.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mm.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qp.huixiangedu.cn

[Q47] 与平均值比较
来源：http://yf.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vv.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://ag.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zb.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://dn.bjjhwx.cn

[Q49] 更新单行
来源：http://kw.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ux.muxihuayi.cn

[Q50] 批量更新
来源：http://is.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pm.nszjky.cn

[Q51] 用子查询更新
来源：http://na.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://db.szxytkj.cn

[Q52] 删除指定行
来源：http://sn.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://xc.colortex.cn

[Q53] 按条件删除
来源：http://wq.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xf.panjiajie.cn

[Q54] 清空表
来源：http://an.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://tg.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://ay.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ac.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://kl.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://in.colortex.cn

[Q57] 行号
来源：http://sk.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eu.shtwfgs.cn

[Q58] 累计求和
来源：http://ab.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sc.yuexingan06.cn

[Q59] 分组内累计
来源：http://sk.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qb.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://tb.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lq.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mq.muxihuayi.cn

[Q61] 移动平均
来源：http://rs.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cj.521024.cn

[Q62] 分组占比
来源：http://fu.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uf.shxzskj.cn

[Q63] 开启事务
来源：http://no.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://em.bookmarksfly.cn

[Q64] 提交事务
来源：http://ld.bookmarksfly.cn

COMMIT;
来源：http://rj.shtwfgs.cn

[Q65] 回滚事务
来源：http://tw.nszjky.cn

ROLLBACK;
来源：http://gl.huanxung.cn

[Q66] 行锁查询
来源：http://aq.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iq.panjiajie.cn

[Q67] 设置隔离级别
来源：http://bh.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hj.bjjhwx.cn

[Q68] 保存点
来源：http://wk.shxzukj.cn

SAVEPOINT sp1;
来源：http://pj.huanxung.cn

ROLLBACK TO sp1;
来源：http://or.gzmigu.cn

[Q69] 查看执行计划
来源：http://yc.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://um.asd995.cn

[Q70] 更新统计信息
来源：http://vr.szsharing.cn

ANALYZE TABLE users;
来源：http://ud.newstarts.cn

[Q71] 查看建表语句
来源：http://gj.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tk.gzmigu.cn

[Q72] 查看索引
来源：http://za.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://tx.jctech888.com.cn

[Q73] 查看表状态
来源：http://fi.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tf.colortex.cn

[Q74] 强制使用索引
来源：http://tf.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kx.gzmigu.cn

[Q75] 日期格式化
来源：http://yz.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uj.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gc.yuexingan06.cn

[Q76] 按天统计
来源：http://yy.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xx.asd995.cn

[Q77] 时间加减
来源：http://wm.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ws.gzmigu.cn

[Q78] 当前时间
来源：http://ww.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fz.hahajie.cn

[Q79] 字符串拼接
来源：http://ie.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tq.szxytkj.cn

[Q80] 字符串截取
来源：http://vm.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gv.muxihuayi.cn

[Q81] 字符串替换
来源：http://zc.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vi.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://lb.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zy.gzmigu.cn

[Q83] 大小写转换
来源：http://zj.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sd.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://lp.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://pt.szxytkj.cn

[Q85] 数值取整
来源：http://xf.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nn.521024.cn

[Q86] 读取 JSON 字段
来源：http://dh.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sq.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://nt.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dl.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://yw.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oz.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cg.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://lo.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zb.shtwfgs.cn

[Q90] 生成序号列
来源：http://pk.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pg.shxzukj.cn

================================================================================
来源：http://lq.huixiangedu.cn

R. Bash 专题
来源：http://dl.haigaiapp.cn

================================================================================
来源：http://pr.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://os.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://fz.lnxyls.cn

set -euo pipefail
来源：http://nn.colortex.cn

[R02] 变量赋值与使用
来源：http://rf.9csxet.cn

name="Tom"; echo "$name"
来源：http://aq.muxihuayi.cn

[R03] 只读变量
来源：http://op.lnxyls.cn

readonly PI=3.14
来源：http://ny.gzmigu.cn

[R04] 位置参数
来源：http://qw.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nr.jianghongdianzi.cn

[R05] 参数默认值
来源：http://ac.newstarts.cn

name="${1:-default}"
来源：http://um.9csxet.cn

[R06] 判断命令是否存在
来源：http://jj.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rf.muxihuayi.cn

[R07] if 判断文件
来源：http://id.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rh.bookmarksfly.cn

[R08] 数值比较
来源：http://mc.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ox.521024.cn

[R09] 字符串比较
来源：http://tm.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cu.nicolike.cn

[R10] 正则匹配
来源：http://fo.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://np.gzmigu.cn

[R11] case 多分支
来源：http://bv.9csxet.cn

case "$1" in
来源：http://hn.bjjhwx.cn

start) echo "启动" ;;
来源：http://lj.asd995.cn

stop)  echo "停止" ;;
来源：http://aj.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://ep.bjjhwx.cn

esac
来源：http://ax.szxytkj.cn

[R12] for 遍历文件
来源：http://mo.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://ww.521024.cn

[R13] for 计数循环
来源：http://ym.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://ds.szxytkj.cn

[R14] C 风格 for
来源：http://dp.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nu.bjjhwx.cn

[R15] while 逐行读文件
来源：http://oo.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rl.jctech888.com.cn

[R16] until 等待条件
来源：http://rw.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ht.huanxung.cn

[R17] 数组定义与取值
来源：http://hr.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xr.wgjwhj.cn

[R18] 遍历数组
来源：http://pf.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mx.szxytkj.cn

[R19] 数组长度
来源：http://td.gzmigu.cn

echo "${#arr[@]}"
来源：http://kz.lnxyls.cn

[R20] 关联数组（字典）
来源：http://go.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lg.shxzukj.cn

[R21] 字符串长度
来源：http://cp.shtwfgs.cn

echo "${#s}"
来源：http://gs.muxihuayi.cn

[R22] 截取子串
来源：http://qc.muxihuayi.cn

echo "${s:0:5}"
来源：http://de.bookmarksfly.cn

[R23] 字符串替换
来源：http://yr.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ar.nszjky.cn

[R24] 大小写转换
来源：http://aw.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ym.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://wr.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nc.asd995.cn

[R26] 命令替换
来源：http://wp.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://rc.szxytkj.cn

[R27] 算术展开
来源：http://ak.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://rj.bjjhwx.cn

[R28] 浮点运算
来源：http://ev.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://yp.521024.cn

[R29] 定义函数
来源：http://zf.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ur.shtwfgs.cn

[R30] 函数返回状态码
来源：http://cw.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://ou.muxihuayi.cn

[R31] 局部变量
来源：http://qd.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://ek.newstarts.cn

[R32] 参数个数校验
来源：http://cg.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wv.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://wo.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uq.hahajie.cn

[R34] 退出时清理
来源：http://bc.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ta.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://mo.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mz.hahajie.cn

[R36] 并发执行多个任务
来源：http://re.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tt.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://hv.huixiangedu.cn

files=$(ls -1)
来源：http://dp.szxytkj.cn

[R38] 管道串联
来源：http://io.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://ul.521024.cn

[R39] 重定向标准输出与错误
来源：http://rq.shxzukj.cn

cmd > out.log 2>&1
来源：http://lt.jctech888.com.cn

[R40] 追加写日志
来源：http://sk.gzmigu.cn

echo "log" >> out.log
来源：http://xo.yuexingan06.cn

[R41] 丢弃输出
来源：http://km.szsharing.cn

cmd >/dev/null 2>&1
来源：http://hw.panjiajie.cn

[R42] 输入重定向
来源：http://nc.lnxyls.cn

wc -l < a.txt
来源：http://mj.colortex.cn

[R43] 按名字查找文件
来源：http://xi.shxzukj.cn

find . -name "*.log" -type f
来源：http://hb.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://gs.haigaiapp.cn

find . -mtime -7 -type f
来源：http://ww.yuntaijiaju.cn

[R45] 批量删除
来源：http://qi.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://cf.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://tl.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xk.gzmigu.cn

[R47] sed 单行替换
来源：http://hg.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ce.lnxyls.cn

[R48] awk 取指定列
来源：http://ro.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://wg.wgjwhj.cn

[R49] awk 带条件
来源：http://vs.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://je.newstarts.cn

[R50] awk 求和
来源：http://ur.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gr.shxzskj.cn

[R51] 排序去重取前几
来源：http://uk.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uj.lnxyls.cn

[R52] 统计行数
来源：http://la.shtwfgs.cn

wc -l a.txt
来源：http://iy.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://gk.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://py.huixiangedu.cn

[R54] 比较两个文件
来源：http://de.lnxyls.cn

diff a.txt b.txt
来源：http://hy.nicolike.cn

[R55] 压缩与解压
来源：http://wj.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gs.panjiajie.cn

[R56] 远程拷贝
来源：http://xt.9csxet.cn

scp file user@host:/path/
来源：http://kd.haigaiapp.cn

[R57] 远程执行命令
来源：http://hw.nszjky.cn

ssh user@host 'uptime'
来源：http://ot.lnxyls.cn

[R58] 下载文件
来源：http://nx.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://go.szxytkj.cn

[R59] 发 POST JSON
来源：http://af.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pc.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://am.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ex.chemitech.net.cn

[R61] 磁盘占用
来源：http://di.szsharing.cn

df -h;  du -sh *
来源：http://np.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://lw.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://ws.szsharing.cn

[R63] 内存与进程
来源：http://lk.colortex.cn

free -h;  ps aux | grep nginx
来源：http://al.newstarts.cn

[R64] 结束进程
来源：http://ml.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://ei.szxytkj.cn

[R65] 查看端口占用
来源：http://qd.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mk.shxzukj.cn

[R66] 定时任务
来源：http://jz.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://xs.huanxung.cn

[R67] 生成随机十六进制串
来源：http://bv.shxzukj.cn


<!-- 参考信息 -->