代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://bf.bjjhwx.cn

[Q22] 排序
来源：http://pf.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pb.521024.cn

[Q23] 分页
来源：http://mq.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://da.yuntaijiaju.cn

[Q24] 去重
来源：http://pn.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://di.newstarts.cn

[Q25] 只取前 N 条
来源：http://dr.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ki.huixinmuqiang.cn

[Q26] 计数
来源：http://ja.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://ot.yuexingan06.cn

[Q27] 条件计数
来源：http://gs.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fw.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://rs.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xr.nszjky.cn

[Q29] 最大最小值
来源：http://hy.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mt.haigaiapp.cn

[Q30] 分组统计
来源：http://ru.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gz.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://ej.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gw.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://iu.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iy.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://or.9csxet.cn

[Q33] 多列分组
来源：http://nl.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gb.bjjhwx.cn

[Q34] 每组取第一条
来源：http://my.jianghongdianzi.cn

SELECT * FROM (
来源：http://bk.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qo.muxihuayi.cn

) t WHERE rn = 1;
来源：http://kf.bjjhwx.cn

[Q35] 内连接
来源：http://zp.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rn.huixinmuqiang.cn

[Q36] 左连接
来源：http://vk.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ll.szxytkj.cn

[Q37] 右连接
来源：http://ea.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bl.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hi.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jz.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://zx.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://du.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dx.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vn.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fs.huixinmuqiang.cn

[Q41] 多表连接
来源：http://qf.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://th.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://am.chemitech.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://oe.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://sh.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://dd.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vk.yuexingan06.cn

[Q43] 标量子查询
来源：http://iu.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jm.nicolike.cn

[Q44] IN 子查询
来源：http://fo.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://in.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://qx.yuexingan06.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aj.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nl.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gw.huanxung.cn

[Q47] 与平均值比较
来源：http://xs.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ht.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://ex.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dv.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://vk.shxzskj.cn

[Q49] 更新单行
来源：http://my.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xs.colortex.cn

[Q50] 批量更新
来源：http://rc.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zr.hnjuh.cn

[Q51] 用子查询更新
来源：http://vb.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xl.lnxyls.cn

[Q52] 删除指定行
来源：http://yx.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://du.bjjhwx.cn

[Q53] 按条件删除
来源：http://st.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ko.yuexingan06.cn

[Q54] 清空表
来源：http://qv.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://oh.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://yy.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jf.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://kd.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sj.huixiangedu.cn

[Q57] 行号
来源：http://wl.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ng.yuexingan06.cn

[Q58] 累计求和
来源：http://xz.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://rx.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jv.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://gr.gzmigu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://in.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lm.lnxyls.cn

[Q61] 移动平均
来源：http://jb.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zi.asd995.cn

[Q62] 分组占比
来源：http://kn.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bx.nszjky.cn

[Q63] 开启事务
来源：http://es.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qo.chemitech.net.cn

[Q64] 提交事务
来源：http://en.szxytkj.cn

COMMIT;
来源：http://vh.shxzukj.cn

[Q65] 回滚事务
来源：http://pl.shtwfgs.cn

ROLLBACK;
来源：http://cb.chemitech.net.cn

[Q66] 行锁查询
来源：http://la.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fg.hnjuh.cn

[Q67] 设置隔离级别
来源：http://oq.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cm.colortex.cn

[Q68] 保存点
来源：http://co.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://zj.shxzskj.cn

ROLLBACK TO sp1;
来源：http://mv.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://ux.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dq.hahajie.cn

[Q70] 更新统计信息
来源：http://ha.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://ep.huanxung.cn

[Q71] 查看建表语句
来源：http://dk.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yg.gzmigu.cn

[Q72] 查看索引
来源：http://xm.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://vp.szxytkj.cn

[Q73] 查看表状态
来源：http://no.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qt.huixiangedu.cn

[Q74] 强制使用索引
来源：http://js.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hu.nszjky.cn

[Q75] 日期格式化
来源：http://qh.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jq.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hf.521024.cn

[Q76] 按天统计
来源：http://kk.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oj.jctech888.com.cn

[Q77] 时间加减
来源：http://gk.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://te.bookmarksfly.cn

[Q78] 当前时间
来源：http://tq.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cp.gzmigu.cn

[Q79] 字符串拼接
来源：http://gd.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lj.muxihuayi.cn

[Q80] 字符串截取
来源：http://te.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ul.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://yl.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ur.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://qp.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ip.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://hv.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qp.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://zd.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://wi.hnjuh.cn

[Q85] 数值取整
来源：http://ou.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ha.asd995.cn

[Q86] 读取 JSON 字段
来源：http://sk.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wq.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://ma.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vk.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://nz.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sb.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fv.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://al.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nc.shtwfgs.cn

[Q90] 生成序号列
来源：http://ug.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yb.chemitech.net.cn

================================================================================
来源：http://se.shxzskj.cn

R. Bash 专题
来源：http://cz.wgjwhj.cn

================================================================================
来源：http://iw.asd995.cn

[R01] shebang 与严格模式
来源：http://mj.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://ji.panjiajie.cn

set -euo pipefail
来源：http://ac.shxzukj.cn

[R02] 变量赋值与使用
来源：http://dh.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://ic.nicolike.cn

[R03] 只读变量
来源：http://pn.wgjwhj.cn

readonly PI=3.14
来源：http://la.hnjuh.cn

[R04] 位置参数
来源：http://zs.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gs.huixinmuqiang.cn

[R05] 参数默认值
来源：http://xq.colortex.cn

name="${1:-default}"
来源：http://la.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://ks.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yk.jctech888.com.cn

[R07] if 判断文件
来源：http://bu.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wo.jianghongdianzi.cn

[R08] 数值比较
来源：http://yr.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cd.hnjuh.cn

[R09] 字符串比较
来源：http://pk.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vn.haigaiapp.cn

[R10] 正则匹配
来源：http://tf.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fi.yuntaijiaju.cn

[R11] case 多分支
来源：http://rf.yuntaijiaju.cn

case "$1" in
来源：http://my.yuexingan06.cn

start) echo "启动" ;;
来源：http://og.colortex.cn

stop)  echo "停止" ;;
来源：http://uk.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://bg.huixinmuqiang.cn

esac
来源：http://ff.huanxung.cn

[R12] for 遍历文件
来源：http://bu.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://ms.yuntaijiaju.cn

[R13] for 计数循环
来源：http://tv.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://zm.szxytkj.cn

[R14] C 风格 for
来源：http://do.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lt.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://qw.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yc.shtwfgs.cn

[R16] until 等待条件
来源：http://px.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wc.szsharing.cn

[R17] 数组定义与取值
来源：http://zn.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://au.wgjwhj.cn

[R18] 遍历数组
来源：http://ce.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vh.yuexingan06.cn

[R19] 数组长度
来源：http://yx.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://qe.gzmigu.cn

[R20] 关联数组（字典）
来源：http://nf.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ja.huixinmuqiang.cn

[R21] 字符串长度
来源：http://nj.huixinmuqiang.cn

echo "${#s}"
来源：http://va.huixinmuqiang.cn

[R22] 截取子串
来源：http://po.lnxyls.cn

echo "${s:0:5}"
来源：http://nt.yuexingan06.cn

[R23] 字符串替换
来源：http://wl.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xs.panjiajie.cn

[R24] 大小写转换
来源：http://sa.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rm.521024.cn

[R25] 去后缀 / 去前缀
来源：http://fo.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kf.521024.cn

[R26] 命令替换
来源：http://gw.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://pp.yuexingan06.cn

[R27] 算术展开
来源：http://aj.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://sf.muxihuayi.cn

[R28] 浮点运算
来源：http://zx.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://sl.yuntaijiaju.cn

[R29] 定义函数
来源：http://nw.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uy.wgjwhj.cn

[R30] 函数返回状态码
来源：http://cc.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://ac.hnjuh.cn

[R31] 局部变量
来源：http://cu.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://nc.shxzukj.cn

[R32] 参数个数校验
来源：http://dw.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oq.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://bp.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ou.bjjhwx.cn

[R34] 退出时清理
来源：http://lb.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yh.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://kr.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zv.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://py.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ga.szsharing.cn

[R37] 把输出赋给变量
来源：http://ny.nicolike.cn

files=$(ls -1)
来源：http://qt.hahajie.cn

[R38] 管道串联
来源：http://pe.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://cd.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://os.shxzukj.cn

cmd > out.log 2>&1
来源：http://dl.colortex.cn

[R40] 追加写日志
来源：http://xq.yuntaijiaju.cn

echo "log" >> out.log
来源：http://ys.bjjhwx.cn

[R41] 丢弃输出
来源：http://yy.huanxung.cn

cmd >/dev/null 2>&1
来源：http://hs.jctech888.com.cn

[R42] 输入重定向
来源：http://ek.9csxet.cn

wc -l < a.txt
来源：http://qg.9csxet.cn

[R43] 按名字查找文件
来源：http://eb.szxytkj.cn

find . -name "*.log" -type f
来源：http://ed.gzmigu.cn

[R44] 按修改时间查找
来源：http://al.huanxung.cn

find . -mtime -7 -type f
来源：http://on.shxzskj.cn

[R45] 批量删除
来源：http://er.9csxet.cn

find . -name "*.tmp" -delete
来源：http://hh.nszjky.cn

[R46] 递归替换文件内容
来源：http://ux.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sn.yuexingan06.cn

[R47] sed 单行替换
来源：http://fb.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pv.chemitech.net.cn

[R48] awk 取指定列
来源：http://wa.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://nd.bookmarksfly.cn

[R49] awk 带条件
来源：http://rk.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ic.shxzskj.cn

[R50] awk 求和
来源：http://xf.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ky.muxihuayi.cn

[R51] 排序去重取前几
来源：http://cz.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qf.521024.cn

[R52] 统计行数
来源：http://hi.nicolike.cn

wc -l a.txt
来源：http://nh.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://tc.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uc.muxihuayi.cn

[R54] 比较两个文件
来源：http://dp.szsharing.cn

diff a.txt b.txt
来源：http://ql.bjjhwx.cn

[R55] 压缩与解压
来源：http://sm.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ul.hnjuh.cn

[R56] 远程拷贝
来源：http://cl.shtwfgs.cn

scp file user@host:/path/
来源：http://qy.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://vs.shtwfgs.cn

ssh user@host 'uptime'
来源：http://fq.newstarts.cn

[R58] 下载文件
来源：http://kc.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sd.nicolike.cn

[R59] 发 POST JSON
来源：http://ad.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xw.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://wm.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rg.wgjwhj.cn

[R61] 磁盘占用
来源：http://hq.shxzukj.cn

df -h;  du -sh *
来源：http://rz.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://wp.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://rp.gzmigu.cn

[R63] 内存与进程
来源：http://rd.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://jq.haigaiapp.cn

[R64] 结束进程
来源：http://nq.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://bh.chemitech.net.cn

[R65] 查看端口占用
来源：http://fp.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vw.hnjuh.cn

[R66] 定时任务
来源：http://yg.colortex.cn

crontab -e;  crontab -l
来源：http://sa.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://ra.9csxet.cn

openssl rand -hex 16
来源：http://nb.hahajie.cn

[R68] 计算文件校验值
来源：http://be.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dp.huanxung.cn

[R69] 生成随机密码
来源：http://tj.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://te.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://pz.colortex.cn

date +%s;  date -d @1700000000
来源：http://ai.jianghongdianzi.cn

[R71] 日期格式化
来源：http://yq.haigaiapp.cn


<!-- 参考信息 -->