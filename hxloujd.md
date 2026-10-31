代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://cb.nicolike.cn

[Q22] 排序
来源：http://wf.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://em.colortex.cn

[Q23] 分页
来源：http://lb.jianghongdianzi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ez.haigaiapp.cn

[Q24] 去重
来源：http://qa.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://uu.panjiajie.cn

[Q25] 只取前 N 条
来源：http://hr.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bc.shxzukj.cn

[Q26] 计数
来源：http://hl.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://rf.haigaiapp.cn

[Q27] 条件计数
来源：http://os.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rg.huixiangedu.cn

[Q28] 求和与平均
来源：http://ut.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xq.szxytkj.cn

[Q29] 最大最小值
来源：http://xt.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zt.chemitech.net.cn

[Q30] 分组统计
来源：http://bc.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xm.yuexingan06.cn

[Q31] 分组后过滤
来源：http://av.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ak.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://rn.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mb.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://px.huixinmuqiang.cn

[Q33] 多列分组
来源：http://da.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://py.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://tf.jctech888.com.cn

SELECT * FROM (
来源：http://aq.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cn.lnxyls.cn

) t WHERE rn = 1;
来源：http://wa.jianghongdianzi.cn

[Q35] 内连接
来源：http://sn.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mr.hahajie.cn

[Q36] 左连接
来源：http://an.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://or.bookmarksfly.cn

[Q37] 右连接
来源：http://md.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jq.muxihuayi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ll.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hg.colortex.cn

[Q39] 自连接（查上下级）
来源：http://ul.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qz.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oo.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dw.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pl.yuexingan06.cn

[Q41] 多表连接
来源：http://zy.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ed.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://sc.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://os.colortex.cn

[Q42] 连接条件附加过滤
来源：http://rq.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://ak.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ls.nszjky.cn

[Q43] 标量子查询
来源：http://rs.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ty.szxytkj.cn

[Q44] IN 子查询
来源：http://vt.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uv.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://ul.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zk.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kw.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jr.shxzukj.cn

[Q47] 与平均值比较
来源：http://pe.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mh.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://aj.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ic.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://bb.jianghongdianzi.cn

[Q49] 更新单行
来源：http://lq.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wy.szxytkj.cn

[Q50] 批量更新
来源：http://nu.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uk.colortex.cn

[Q51] 用子查询更新
来源：http://cs.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ht.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://pm.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://vx.muxihuayi.cn

[Q53] 按条件删除
来源：http://mp.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jw.huanxung.cn

[Q54] 清空表
来源：http://ma.9csxet.cn

TRUNCATE TABLE logs;
来源：http://au.hahajie.cn

[Q55] 排名（并列占位）
来源：http://uv.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yo.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://yi.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yo.szsharing.cn

[Q57] 行号
来源：http://il.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ut.huixinmuqiang.cn

[Q58] 累计求和
来源：http://yk.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cb.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://sr.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nj.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://sm.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ty.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://my.jctech888.com.cn

[Q61] 移动平均
来源：http://ll.hnjuh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ez.shxzskj.cn

[Q62] 分组占比
来源：http://lu.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nu.bjjhwx.cn

[Q63] 开启事务
来源：http://kc.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ph.gzmigu.cn

[Q64] 提交事务
来源：http://jg.chemitech.net.cn

COMMIT;
来源：http://rp.yuexingan06.cn

[Q65] 回滚事务
来源：http://ux.newstarts.cn

ROLLBACK;
来源：http://bn.colortex.cn

[Q66] 行锁查询
来源：http://il.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cw.huanxung.cn

[Q67] 设置隔离级别
来源：http://ud.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hf.bookmarksfly.cn

[Q68] 保存点
来源：http://ir.panjiajie.cn

SAVEPOINT sp1;
来源：http://wp.hnjuh.cn

ROLLBACK TO sp1;
来源：http://wj.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://iy.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://na.yuexingan06.cn

[Q70] 更新统计信息
来源：http://yx.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://we.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://aq.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fx.nicolike.cn

[Q72] 查看索引
来源：http://uu.huanxung.cn

SHOW INDEX FROM users;
来源：http://lb.huixiangedu.cn

[Q73] 查看表状态
来源：http://kw.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gb.huanxung.cn

[Q74] 强制使用索引
来源：http://nv.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xx.bookmarksfly.cn

[Q75] 日期格式化
来源：http://ny.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fx.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dr.panjiajie.cn

[Q76] 按天统计
来源：http://zy.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uv.colortex.cn

[Q77] 时间加减
来源：http://ej.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dr.huanxung.cn

[Q78] 当前时间
来源：http://gf.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rk.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://qf.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ub.haigaiapp.cn

[Q80] 字符串截取
来源：http://as.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uu.9csxet.cn

[Q81] 字符串替换
来源：http://eg.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cs.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://za.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bj.shxzskj.cn

[Q83] 大小写转换
来源：http://aq.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://af.shxzukj.cn

[Q84] 去除首尾空格
来源：http://ut.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://gl.huixiangedu.cn

[Q85] 数值取整
来源：http://pl.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eu.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://vn.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ci.asd995.cn

[Q87] JSON 字段做条件
来源：http://dc.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wy.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://yk.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://it.huixinmuqiang.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tu.panjiajie.cn

[Q89] 判断表是否存在
来源：http://fk.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yw.haigaiapp.cn

[Q90] 生成序号列
来源：http://qo.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sy.huixiangedu.cn

================================================================================
来源：http://bd.wgjwhj.cn

R. Bash 专题
来源：http://mg.nicolike.cn

================================================================================
来源：http://qk.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://zc.chemitech.net.cn

#!/usr/bin/env bash
来源：http://wv.chemitech.net.cn

set -euo pipefail
来源：http://ao.9csxet.cn

[R02] 变量赋值与使用
来源：http://ty.nszjky.cn

name="Tom"; echo "$name"
来源：http://el.yuntaijiaju.cn

[R03] 只读变量
来源：http://ab.shxzskj.cn

readonly PI=3.14
来源：http://mo.9csxet.cn

[R04] 位置参数
来源：http://vd.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nr.newstarts.cn

[R05] 参数默认值
来源：http://nr.asd995.cn

name="${1:-default}"
来源：http://ed.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://nc.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kf.hnjuh.cn

[R07] if 判断文件
来源：http://bg.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ia.panjiajie.cn

[R08] 数值比较
来源：http://th.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xs.521024.cn

[R09] 字符串比较
来源：http://ir.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zh.yuexingan06.cn

[R10] 正则匹配
来源：http://dz.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dk.bookmarksfly.cn

[R11] case 多分支
来源：http://jt.gzmigu.cn

case "$1" in
来源：http://cj.hahajie.cn

start) echo "启动" ;;
来源：http://db.asd995.cn

stop)  echo "停止" ;;
来源：http://jp.newstarts.cn

*)     echo "未知命令" ;;
来源：http://bu.haigaiapp.cn

esac
来源：http://pt.9csxet.cn

[R12] for 遍历文件
来源：http://cp.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://ly.521024.cn

[R13] for 计数循环
来源：http://qm.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://fu.asd995.cn

[R14] C 风格 for
来源：http://ts.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wf.wgjwhj.cn

[R15] while 逐行读文件
来源：http://su.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ih.huanxung.cn

[R16] until 等待条件
来源：http://pi.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xu.szsharing.cn

[R17] 数组定义与取值
来源：http://eh.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bh.newstarts.cn

[R18] 遍历数组
来源：http://fe.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yz.nicolike.cn

[R19] 数组长度
来源：http://vb.szxytkj.cn

echo "${#arr[@]}"
来源：http://hb.shxzukj.cn

[R20] 关联数组（字典）
来源：http://ji.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lp.newstarts.cn

[R21] 字符串长度
来源：http://kp.gzmigu.cn

echo "${#s}"
来源：http://iz.szxytkj.cn

[R22] 截取子串
来源：http://hf.huanxung.cn

echo "${s:0:5}"
来源：http://sc.chemitech.net.cn

[R23] 字符串替换
来源：http://da.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lt.hnjuh.cn

[R24] 大小写转换
来源：http://gb.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vb.521024.cn

[R25] 去后缀 / 去前缀
来源：http://nt.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://td.shtwfgs.cn

[R26] 命令替换
来源：http://id.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://uc.colortex.cn

[R27] 算术展开
来源：http://da.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://ae.shxzskj.cn

[R28] 浮点运算
来源：http://rn.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://me.muxihuayi.cn

[R29] 定义函数
来源：http://ox.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lp.shxzskj.cn

[R30] 函数返回状态码
来源：http://jw.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://al.muxihuayi.cn

[R31] 局部变量
来源：http://vy.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://zk.yuexingan06.cn

[R32] 参数个数校验
来源：http://er.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ze.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://tr.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://in.shtwfgs.cn

[R34] 退出时清理
来源：http://xq.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ta.yuexingan06.cn

[R35] 后台执行并等待
来源：http://wd.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lh.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://hf.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qy.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://sd.asd995.cn

files=$(ls -1)
来源：http://ue.nszjky.cn

[R38] 管道串联
来源：http://ne.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://eo.asd995.cn

[R39] 重定向标准输出与错误
来源：http://tr.huixiangedu.cn

cmd > out.log 2>&1
来源：http://jh.hnjuh.cn

[R40] 追加写日志
来源：http://ln.jctech888.com.cn

echo "log" >> out.log
来源：http://an.shtwfgs.cn

[R41] 丢弃输出
来源：http://yh.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://gl.521024.cn

[R42] 输入重定向
来源：http://ln.yuexingan06.cn

wc -l < a.txt
来源：http://zz.muxihuayi.cn

[R43] 按名字查找文件
来源：http://aa.newstarts.cn

find . -name "*.log" -type f
来源：http://py.chemitech.net.cn

[R44] 按修改时间查找
来源：http://hs.shtwfgs.cn

find . -mtime -7 -type f
来源：http://im.panjiajie.cn

[R45] 批量删除
来源：http://cl.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://lb.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://kh.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ew.jctech888.com.cn

[R47] sed 单行替换
来源：http://zo.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yu.nszjky.cn

[R48] awk 取指定列
来源：http://pv.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://cs.newstarts.cn

[R49] awk 带条件
来源：http://iy.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lo.hahajie.cn

[R50] awk 求和
来源：http://nh.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xv.panjiajie.cn

[R51] 排序去重取前几
来源：http://zd.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ya.bjjhwx.cn

[R52] 统计行数
来源：http://te.9csxet.cn

wc -l a.txt
来源：http://uc.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://fp.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eu.szxytkj.cn

[R54] 比较两个文件
来源：http://lp.huanxung.cn

diff a.txt b.txt
来源：http://rk.nicolike.cn

[R55] 压缩与解压
来源：http://vx.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://my.nszjky.cn

[R56] 远程拷贝
来源：http://rj.asd995.cn

scp file user@host:/path/
来源：http://xg.newstarts.cn

[R57] 远程执行命令
来源：http://ue.bjjhwx.cn

ssh user@host 'uptime'
来源：http://te.muxihuayi.cn

[R58] 下载文件
来源：http://jo.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ny.asd995.cn

[R59] 发 POST JSON
来源：http://ua.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xs.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://vk.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rb.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://oe.hnjuh.cn

df -h;  du -sh *
来源：http://wl.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://zo.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://ou.asd995.cn

[R63] 内存与进程
来源：http://bm.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://rd.chemitech.net.cn

[R64] 结束进程
来源：http://dv.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://gl.9csxet.cn

[R65] 查看端口占用
来源：http://zh.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fd.asd995.cn

[R66] 定时任务
来源：http://il.muxihuayi.cn

crontab -e;  crontab -l
来源：http://ef.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://zz.szsharing.cn

openssl rand -hex 16
来源：http://fj.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://bg.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vz.jctech888.com.cn

[R69] 生成随机密码
来源：http://ve.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://db.szxytkj.cn

[R70] 时间戳与互转
来源：http://pf.hahajie.cn

date +%s;  date -d @1700000000
来源：http://ap.nicolike.cn

[R71] 日期格式化
来源：http://dh.panjiajie.cn


<!-- 参考信息 -->