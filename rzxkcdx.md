代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ey.gzmigu.cn

[Q18] 模糊匹配
来源：http://cd.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rm.jctech888.com.cn

[Q19] 范围查询
来源：http://wg.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uv.wgjwhj.cn

[Q20] IN 列表
来源：http://di.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lx.521024.cn

[Q21] 空值判断
来源：http://fr.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pd.panjiajie.cn

[Q22] 排序
来源：http://ad.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wt.shtwfgs.cn

[Q23] 分页
来源：http://jp.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dg.nszjky.cn

[Q24] 去重
来源：http://os.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://kn.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://sd.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ga.huixinmuqiang.cn

[Q26] 计数
来源：http://jz.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://jk.chemitech.net.cn

[Q27] 条件计数
来源：http://uq.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yf.hnjuh.cn

[Q28] 求和与平均
来源：http://ay.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kh.yuntaijiaju.cn

[Q29] 最大最小值
来源：http://ju.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://va.shxzskj.cn

[Q30] 分组统计
来源：http://oc.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vl.lnxyls.cn

[Q31] 分组后过滤
来源：http://fi.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cc.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://rh.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jo.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://og.yuexingan06.cn

[Q33] 多列分组
来源：http://zi.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qw.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://iq.haigaiapp.cn

SELECT * FROM (
来源：http://fm.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lm.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://is.panjiajie.cn

[Q35] 内连接
来源：http://pa.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kh.huixinmuqiang.cn

[Q36] 左连接
来源：http://ek.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rk.9csxet.cn

[Q37] 右连接
来源：http://xy.panjiajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cf.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zh.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lx.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://ky.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qm.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dj.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bx.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mn.shxzukj.cn

[Q41] 多表连接
来源：http://ha.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://am.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://sx.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://tp.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://fy.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://pg.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jg.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://ak.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xp.nszjky.cn

[Q44] IN 子查询
来源：http://yx.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cz.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://hi.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mc.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yj.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://es.haigaiapp.cn

[Q47] 与平均值比较
来源：http://ax.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cz.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://ch.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bs.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://mn.yuntaijiaju.cn

[Q49] 更新单行
来源：http://ky.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qf.huixinmuqiang.cn

[Q50] 批量更新
来源：http://vj.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://df.szsharing.cn

[Q51] 用子查询更新
来源：http://zo.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mk.asd995.cn

[Q52] 删除指定行
来源：http://tv.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://qo.bjjhwx.cn

[Q53] 按条件删除
来源：http://en.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rg.yuexingan06.cn

[Q54] 清空表
来源：http://do.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://vo.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://hh.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pv.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://mz.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ab.shxzukj.cn

[Q57] 行号
来源：http://vv.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dv.yuexingan06.cn

[Q58] 累计求和
来源：http://xd.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dp.wgjwhj.cn

[Q59] 分组内累计
来源：http://dd.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ix.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://nu.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kq.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yj.yuexingan06.cn

[Q61] 移动平均
来源：http://cp.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ag.9csxet.cn

[Q62] 分组占比
来源：http://cy.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oy.bookmarksfly.cn

[Q63] 开启事务
来源：http://en.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ab.521024.cn

[Q64] 提交事务
来源：http://cj.nicolike.cn

COMMIT;
来源：http://ry.bookmarksfly.cn

[Q65] 回滚事务
来源：http://uy.gzmigu.cn

ROLLBACK;
来源：http://an.gzmigu.cn

[Q66] 行锁查询
来源：http://wh.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ll.hnjuh.cn

[Q67] 设置隔离级别
来源：http://sr.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hu.asd995.cn

[Q68] 保存点
来源：http://ue.jianghongdianzi.cn

SAVEPOINT sp1;
来源：http://xw.asd995.cn

ROLLBACK TO sp1;
来源：http://dc.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://zw.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gm.chemitech.net.cn

[Q70] 更新统计信息
来源：http://ls.huixiangedu.cn

ANALYZE TABLE users;
来源：http://jx.asd995.cn

[Q71] 查看建表语句
来源：http://ka.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lu.panjiajie.cn

[Q72] 查看索引
来源：http://je.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://sf.colortex.cn

[Q73] 查看表状态
来源：http://oz.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ra.lnxyls.cn

[Q74] 强制使用索引
来源：http://mh.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zl.521024.cn

[Q75] 日期格式化
来源：http://it.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ik.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nh.huixiangedu.cn

[Q76] 按天统计
来源：http://hd.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zz.huanxung.cn

[Q77] 时间加减
来源：http://ds.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jw.huixiangedu.cn

[Q78] 当前时间
来源：http://dc.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gc.asd995.cn

[Q79] 字符串拼接
来源：http://wi.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qj.bookmarksfly.cn

[Q80] 字符串截取
来源：http://ac.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://au.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://fh.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://au.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://fw.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fn.gzmigu.cn

[Q83] 大小写转换
来源：http://xl.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bx.lnxyls.cn

[Q84] 去除首尾空格
来源：http://bq.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://lg.newstarts.cn

[Q85] 数值取整
来源：http://zu.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://la.521024.cn

[Q86] 读取 JSON 字段
来源：http://pv.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jr.9csxet.cn

[Q87] JSON 字段做条件
来源：http://at.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xo.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://hn.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ro.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ww.gzmigu.cn

[Q89] 判断表是否存在
来源：http://qi.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fi.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://zq.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://az.nicolike.cn

================================================================================
来源：http://vp.colortex.cn

R. Bash 专题
来源：http://tr.hnjuh.cn

================================================================================
来源：http://xm.nszjky.cn

[R01] shebang 与严格模式
来源：http://vy.colortex.cn

#!/usr/bin/env bash
来源：http://mq.huixiangedu.cn

set -euo pipefail
来源：http://nh.nicolike.cn

[R02] 变量赋值与使用
来源：http://nt.szxytkj.cn

name="Tom"; echo "$name"
来源：http://hm.haigaiapp.cn

[R03] 只读变量
来源：http://bk.huanxung.cn

readonly PI=3.14
来源：http://af.huixiangedu.cn

[R04] 位置参数
来源：http://on.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cl.szxytkj.cn

[R05] 参数默认值
来源：http://mm.muxihuayi.cn

name="${1:-default}"
来源：http://fk.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://fw.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cj.muxihuayi.cn

[R07] if 判断文件
来源：http://sz.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uj.shtwfgs.cn

[R08] 数值比较
来源：http://vf.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qc.lnxyls.cn

[R09] 字符串比较
来源：http://kd.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nw.bookmarksfly.cn

[R10] 正则匹配
来源：http://cp.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fn.colortex.cn

[R11] case 多分支
来源：http://vu.hahajie.cn

case "$1" in
来源：http://og.huixiangedu.cn

start) echo "启动" ;;
来源：http://ih.hnjuh.cn

stop)  echo "停止" ;;
来源：http://np.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://iz.shxzskj.cn

esac
来源：http://nv.shxzskj.cn

[R12] for 遍历文件
来源：http://uu.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://rd.hahajie.cn

[R13] for 计数循环
来源：http://mt.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://lp.shtwfgs.cn

[R14] C 风格 for
来源：http://ip.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://du.huanxung.cn

[R15] while 逐行读文件
来源：http://lf.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ux.hahajie.cn

[R16] until 等待条件
来源：http://xv.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xi.hahajie.cn

[R17] 数组定义与取值
来源：http://wu.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jt.shxzskj.cn

[R18] 遍历数组
来源：http://pu.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pp.huanxung.cn

[R19] 数组长度
来源：http://ys.nszjky.cn

echo "${#arr[@]}"
来源：http://yx.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://jf.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ru.muxihuayi.cn

[R21] 字符串长度
来源：http://ev.jianghongdianzi.cn

echo "${#s}"
来源：http://gb.chemitech.net.cn

[R22] 截取子串
来源：http://oz.asd995.cn

echo "${s:0:5}"
来源：http://vj.panjiajie.cn

[R23] 字符串替换
来源：http://vw.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mf.hnjuh.cn

[R24] 大小写转换
来源：http://qg.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ir.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://zm.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ey.nszjky.cn

[R26] 命令替换
来源：http://uc.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://jo.lnxyls.cn

[R27] 算术展开
来源：http://bl.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://sr.bjjhwx.cn

[R28] 浮点运算
来源：http://fz.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://yx.asd995.cn

[R29] 定义函数
来源：http://fm.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ba.9csxet.cn

[R30] 函数返回状态码
来源：http://vo.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://tk.bookmarksfly.cn

[R31] 局部变量
来源：http://jy.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://sz.shxzukj.cn

[R32] 参数个数校验
来源：http://yc.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cz.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://yn.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cn.lnxyls.cn

[R34] 退出时清理
来源：http://sd.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jv.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://mn.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sd.hahajie.cn

[R36] 并发执行多个任务
来源：http://og.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wy.521024.cn

[R37] 把输出赋给变量
来源：http://wk.jctech888.com.cn

files=$(ls -1)
来源：http://ug.colortex.cn

[R38] 管道串联
来源：http://sv.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://gx.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://oj.szsharing.cn

cmd > out.log 2>&1
来源：http://vj.szsharing.cn

[R40] 追加写日志
来源：http://nb.jianghongdianzi.cn

echo "log" >> out.log
来源：http://ut.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://nj.asd995.cn

cmd >/dev/null 2>&1
来源：http://gm.9csxet.cn

[R42] 输入重定向
来源：http://ug.colortex.cn

wc -l < a.txt
来源：http://su.szsharing.cn

[R43] 按名字查找文件
来源：http://mo.wgjwhj.cn

find . -name "*.log" -type f
来源：http://li.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://tg.nicolike.cn

find . -mtime -7 -type f
来源：http://ej.chemitech.net.cn

[R45] 批量删除
来源：http://rb.szsharing.cn

find . -name "*.tmp" -delete
来源：http://nc.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://sr.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kr.9csxet.cn

[R47] sed 单行替换
来源：http://kw.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mf.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://fn.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://ir.shxzukj.cn

[R49] awk 带条件
来源：http://ez.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xd.lnxyls.cn

[R50] awk 求和
来源：http://iu.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rp.szxytkj.cn

[R51] 排序去重取前几
来源：http://ob.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dl.gzmigu.cn

[R52] 统计行数
来源：http://fy.muxihuayi.cn

wc -l a.txt
来源：http://ey.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://js.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sc.9csxet.cn

[R54] 比较两个文件
来源：http://jp.jctech888.com.cn

diff a.txt b.txt
来源：http://vs.asd995.cn

[R55] 压缩与解压
来源：http://rx.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qe.szxytkj.cn

[R56] 远程拷贝
来源：http://dw.nszjky.cn

scp file user@host:/path/
来源：http://yh.lnxyls.cn

[R57] 远程执行命令
来源：http://ri.colortex.cn

ssh user@host 'uptime'
来源：http://yk.hnjuh.cn

[R58] 下载文件
来源：http://kx.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fu.asd995.cn

[R59] 发 POST JSON
来源：http://ip.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zw.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://ag.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kc.yuexingan06.cn

[R61] 磁盘占用
来源：http://vw.newstarts.cn

df -h;  du -sh *
来源：http://bn.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://uh.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://ut.asd995.cn

[R63] 内存与进程
来源：http://vu.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://sh.asd995.cn

[R64] 结束进程
来源：http://qp.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://iq.yuexingan06.cn

[R65] 查看端口占用
来源：http://mf.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rn.gzmigu.cn

[R66] 定时任务
来源：http://jp.colortex.cn

crontab -e;  crontab -l
来源：http://te.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://di.szsharing.cn


<!-- 参考信息 -->