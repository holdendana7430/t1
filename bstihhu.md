代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ub.521024.cn

[Q26] 计数
来源：http://uw.chemitech.net.cn

SELECT COUNT(*) FROM users;
来源：http://mq.hahajie.cn

[Q27] 条件计数
来源：http://rc.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uw.bjjhwx.cn

[Q28] 求和与平均
来源：http://vx.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jp.hahajie.cn

[Q29] 最大最小值
来源：http://yw.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wn.jianghongdianzi.cn

[Q30] 分组统计
来源：http://lz.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fj.shtwfgs.cn

[Q31] 分组后过滤
来源：http://aq.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bj.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://aq.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ll.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ig.shxzukj.cn

[Q33] 多列分组
来源：http://lx.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://od.shxzskj.cn

[Q34] 每组取第一条
来源：http://fk.yuexingan06.cn

SELECT * FROM (
来源：http://em.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ze.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://nf.wgjwhj.cn

[Q35] 内连接
来源：http://vo.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://re.bjjhwx.cn

[Q36] 左连接
来源：http://qs.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yg.huixinmuqiang.cn

[Q37] 右连接
来源：http://iw.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sa.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zo.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lj.colortex.cn

[Q39] 自连接（查上下级）
来源：http://be.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ip.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://su.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sn.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gq.shtwfgs.cn

[Q41] 多表连接
来源：http://bg.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tz.szxytkj.cn

JOIN users u ON u.id = o.user_id
来源：http://oq.chemitech.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://gc.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://em.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://lg.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vl.shxzukj.cn

[Q43] 标量子查询
来源：http://ak.newstarts.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zo.panjiajie.cn

[Q44] IN 子查询
来源：http://nv.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ed.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://bb.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gs.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pt.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dq.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://wy.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mp.521024.cn

[Q48] CTE 公用表表达式
来源：http://tj.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://du.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://zh.haigaiapp.cn

[Q49] 更新单行
来源：http://ri.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vx.huixiangedu.cn

[Q50] 批量更新
来源：http://lq.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vw.szsharing.cn

[Q51] 用子查询更新
来源：http://kd.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kn.nszjky.cn

[Q52] 删除指定行
来源：http://io.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://oa.gzmigu.cn

[Q53] 按条件删除
来源：http://ky.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ou.jctech888.com.cn

[Q54] 清空表
来源：http://wo.colortex.cn

TRUNCATE TABLE logs;
来源：http://sd.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://fk.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ql.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://fk.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jb.haigaiapp.cn

[Q57] 行号
来源：http://ke.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zj.colortex.cn

[Q58] 累计求和
来源：http://nj.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mz.bjjhwx.cn

[Q59] 分组内累计
来源：http://ou.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fa.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://eg.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jm.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://va.shxzukj.cn

[Q61] 移动平均
来源：http://ph.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bn.huixinmuqiang.cn

[Q62] 分组占比
来源：http://ev.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jo.newstarts.cn

[Q63] 开启事务
来源：http://bv.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ak.gzmigu.cn

[Q64] 提交事务
来源：http://ym.shxzukj.cn

COMMIT;
来源：http://lx.gzmigu.cn

[Q65] 回滚事务
来源：http://sa.nicolike.cn

ROLLBACK;
来源：http://fb.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://ep.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ze.hahajie.cn

[Q67] 设置隔离级别
来源：http://ov.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vb.colortex.cn

[Q68] 保存点
来源：http://pu.hahajie.cn

SAVEPOINT sp1;
来源：http://wz.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://rw.szxytkj.cn

[Q69] 查看执行计划
来源：http://cq.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yy.asd995.cn

[Q70] 更新统计信息
来源：http://is.shxzukj.cn

ANALYZE TABLE users;
来源：http://bp.hahajie.cn

[Q71] 查看建表语句
来源：http://ej.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yf.shtwfgs.cn

[Q72] 查看索引
来源：http://mr.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://ko.yuexingan06.cn

[Q73] 查看表状态
来源：http://sc.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gb.chemitech.net.cn

[Q74] 强制使用索引
来源：http://nl.lnxyls.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://od.nicolike.cn

[Q75] 日期格式化
来源：http://wn.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bp.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iq.bjjhwx.cn

[Q76] 按天统计
来源：http://tl.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ca.colortex.cn

[Q77] 时间加减
来源：http://gy.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hn.colortex.cn

[Q78] 当前时间
来源：http://qs.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ki.nszjky.cn

[Q79] 字符串拼接
来源：http://qh.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rg.colortex.cn

[Q80] 字符串截取
来源：http://dy.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hr.shxzukj.cn

[Q81] 字符串替换
来源：http://py.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ie.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://qs.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vv.nszjky.cn

[Q83] 大小写转换
来源：http://uf.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qz.9csxet.cn

[Q84] 去除首尾空格
来源：http://cd.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://xc.bjjhwx.cn

[Q85] 数值取整
来源：http://wy.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dj.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://da.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://be.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://to.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qf.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://li.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sw.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yk.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://mj.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fi.bjjhwx.cn

[Q90] 生成序号列
来源：http://ql.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://we.gzmigu.cn

================================================================================
来源：http://cc.huixinmuqiang.cn

R. Bash 专题
来源：http://nq.szsharing.cn

================================================================================
来源：http://tn.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://zj.gzmigu.cn

#!/usr/bin/env bash
来源：http://ri.gzmigu.cn

set -euo pipefail
来源：http://mt.asd995.cn

[R02] 变量赋值与使用
来源：http://gy.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://id.bookmarksfly.cn

[R03] 只读变量
来源：http://yw.wgjwhj.cn

readonly PI=3.14
来源：http://dk.chemitech.net.cn

[R04] 位置参数
来源：http://ri.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://be.gzmigu.cn

[R05] 参数默认值
来源：http://gy.lnxyls.cn

name="${1:-default}"
来源：http://zr.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://ne.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jf.chemitech.net.cn

[R07] if 判断文件
来源：http://sn.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rd.asd995.cn

[R08] 数值比较
来源：http://pv.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uo.panjiajie.cn

[R09] 字符串比较
来源：http://gz.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ky.asd995.cn

[R10] 正则匹配
来源：http://yh.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wd.jctech888.com.cn

[R11] case 多分支
来源：http://hn.shtwfgs.cn

case "$1" in
来源：http://ky.hahajie.cn

start) echo "启动" ;;
来源：http://qx.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://yq.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://yp.shxzukj.cn

esac
来源：http://fh.hnjuh.cn

[R12] for 遍历文件
来源：http://gw.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://rn.huanxung.cn

[R13] for 计数循环
来源：http://xr.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://ll.jctech888.com.cn

[R14] C 风格 for
来源：http://ty.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kx.panjiajie.cn

[R15] while 逐行读文件
来源：http://qd.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aa.gzmigu.cn

[R16] until 等待条件
来源：http://yy.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ab.muxihuayi.cn

[R17] 数组定义与取值
来源：http://kv.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wd.panjiajie.cn

[R18] 遍历数组
来源：http://gt.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cy.shxzskj.cn

[R19] 数组长度
来源：http://tf.asd995.cn

echo "${#arr[@]}"
来源：http://qb.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://ab.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dv.huanxung.cn

[R21] 字符串长度
来源：http://qb.shtwfgs.cn

echo "${#s}"
来源：http://en.jctech888.com.cn

[R22] 截取子串
来源：http://qx.wgjwhj.cn

echo "${s:0:5}"
来源：http://dw.huixiangedu.cn

[R23] 字符串替换
来源：http://yf.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sm.bjjhwx.cn

[R24] 大小写转换
来源：http://mj.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ty.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://xq.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sq.lnxyls.cn

[R26] 命令替换
来源：http://pz.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://ej.shtwfgs.cn

[R27] 算术展开
来源：http://sy.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://cz.szxytkj.cn

[R28] 浮点运算
来源：http://dy.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://yd.huanxung.cn

[R29] 定义函数
来源：http://pt.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iy.colortex.cn

[R30] 函数返回状态码
来源：http://zy.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://pw.9csxet.cn

[R31] 局部变量
来源：http://jg.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://hk.huanxung.cn

[R32] 参数个数校验
来源：http://sn.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://it.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://if.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://es.szsharing.cn

[R34] 退出时清理
来源：http://rr.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xd.lnxyls.cn

[R35] 后台执行并等待
来源：http://wk.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yf.shxzukj.cn

[R36] 并发执行多个任务
来源：http://me.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oa.gzmigu.cn

[R37] 把输出赋给变量
来源：http://hw.gzmigu.cn

files=$(ls -1)
来源：http://mj.jctech888.com.cn

[R38] 管道串联
来源：http://ah.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://gz.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://ot.yuexingan06.cn

cmd > out.log 2>&1
来源：http://ki.yuexingan06.cn

[R40] 追加写日志
来源：http://zl.yuexingan06.cn

echo "log" >> out.log
来源：http://fp.lnxyls.cn

[R41] 丢弃输出
来源：http://kh.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://qu.yuexingan06.cn

[R42] 输入重定向
来源：http://hu.panjiajie.cn

wc -l < a.txt
来源：http://xq.shxzskj.cn

[R43] 按名字查找文件
来源：http://th.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://rj.nszjky.cn

[R44] 按修改时间查找
来源：http://ht.gzmigu.cn

find . -mtime -7 -type f
来源：http://dt.panjiajie.cn

[R45] 批量删除
来源：http://ih.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://ms.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://xl.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ox.haigaiapp.cn

[R47] sed 单行替换
来源：http://mq.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cp.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://et.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://jp.nszjky.cn

[R49] awk 带条件
来源：http://yt.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lv.colortex.cn

[R50] awk 求和
来源：http://ew.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fz.9csxet.cn

[R51] 排序去重取前几
来源：http://cl.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yd.521024.cn

[R52] 统计行数
来源：http://gy.gzmigu.cn

wc -l a.txt
来源：http://pv.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://qp.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://it.shtwfgs.cn

[R54] 比较两个文件
来源：http://vd.colortex.cn

diff a.txt b.txt
来源：http://kg.muxihuayi.cn

[R55] 压缩与解压
来源：http://mt.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mf.szxytkj.cn

[R56] 远程拷贝
来源：http://kr.hahajie.cn

scp file user@host:/path/
来源：http://ru.chemitech.net.cn

[R57] 远程执行命令
来源：http://ln.521024.cn

ssh user@host 'uptime'
来源：http://zf.521024.cn

[R58] 下载文件
来源：http://ob.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://op.hahajie.cn

[R59] 发 POST JSON
来源：http://bz.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ni.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://qd.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fn.hnjuh.cn

[R61] 磁盘占用
来源：http://os.muxihuayi.cn

df -h;  du -sh *
来源：http://eq.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://sn.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://vt.wgjwhj.cn

[R63] 内存与进程
来源：http://kk.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://yu.jianghongdianzi.cn

[R64] 结束进程
来源：http://en.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://fu.hnjuh.cn

[R65] 查看端口占用
来源：http://st.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rw.yuexingan06.cn

[R66] 定时任务
来源：http://ev.panjiajie.cn

crontab -e;  crontab -l
来源：http://lx.521024.cn

[R67] 生成随机十六进制串
来源：http://ap.wgjwhj.cn

openssl rand -hex 16
来源：http://xe.521024.cn

[R68] 计算文件校验值
来源：http://sq.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://at.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://hz.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://rl.chemitech.net.cn

[R70] 时间戳与互转
来源：http://sy.nicolike.cn

date +%s;  date -d @1700000000
来源：http://iu.chemitech.net.cn

[R71] 日期格式化
来源：http://uj.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ji.szsharing.cn

[R72] 等待端口就绪
来源：http://kl.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uw.wgjwhj.cn

[R73] 分割大日志
来源：http://xn.nicolike.cn

split -l 1000 big.log part_
来源：http://bx.colortex.cn

[R74] 批量重命名
来源：http://zg.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://us.panjiajie.cn

[R75] 导出环境变量
来源：http://zb.gzmigu.cn


<!-- 参考信息 -->