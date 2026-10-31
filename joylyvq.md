代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lo.wgjwhj.cn

[Q24] 去重
来源：http://xd.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://ng.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://ov.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qh.yuexingan06.cn

[Q26] 计数
来源：http://ah.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://su.chemitech.net.cn

[Q27] 条件计数
来源：http://kp.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fa.jctech888.com.cn

[Q28] 求和与平均
来源：http://nf.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://go.lnxyls.cn

[Q29] 最大最小值
来源：http://bg.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://or.muxihuayi.cn

[Q30] 分组统计
来源：http://vu.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ob.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://zk.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://br.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://ue.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ik.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bi.9csxet.cn

[Q33] 多列分组
来源：http://zr.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yf.521024.cn

[Q34] 每组取第一条
来源：http://oz.muxihuayi.cn

SELECT * FROM (
来源：http://lx.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://im.shxzukj.cn

) t WHERE rn = 1;
来源：http://bl.muxihuayi.cn

[Q35] 内连接
来源：http://gl.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://in.jctech888.com.cn

[Q36] 左连接
来源：http://ik.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xv.nszjky.cn

[Q37] 右连接
来源：http://sw.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cv.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dt.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lr.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://zc.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nj.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vi.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xi.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://av.szsharing.cn

[Q41] 多表连接
来源：http://eb.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ux.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://id.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://ii.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://gw.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://hw.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ep.panjiajie.cn

[Q43] 标量子查询
来源：http://in.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tg.9csxet.cn

[Q44] IN 子查询
来源：http://ss.bjjhwx.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wb.521024.cn

[Q45] EXISTS 判断存在
来源：http://qh.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cn.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ko.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qr.chemitech.net.cn

[Q47] 与平均值比较
来源：http://yn.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ab.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://zi.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qk.jctech888.com.cn

SELECT * FROM t WHERE c > 5;
来源：http://ro.bjjhwx.cn

[Q49] 更新单行
来源：http://dw.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fc.shtwfgs.cn

[Q50] 批量更新
来源：http://wg.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://by.wgjwhj.cn

[Q51] 用子查询更新
来源：http://kv.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://am.haigaiapp.cn

[Q52] 删除指定行
来源：http://iy.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://il.muxihuayi.cn

[Q53] 按条件删除
来源：http://ht.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gl.shxzskj.cn

[Q54] 清空表
来源：http://mp.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://kc.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://mh.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mo.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://zz.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wb.jctech888.com.cn

[Q57] 行号
来源：http://as.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yn.asd995.cn

[Q58] 累计求和
来源：http://kx.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gu.szsharing.cn

[Q59] 分组内累计
来源：http://xv.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hx.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://vf.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rf.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hw.gzmigu.cn

[Q61] 移动平均
来源：http://ke.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pl.szsharing.cn

[Q62] 分组占比
来源：http://fd.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xi.jianghongdianzi.cn

[Q63] 开启事务
来源：http://lr.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ge.hnjuh.cn

[Q64] 提交事务
来源：http://li.szxytkj.cn

COMMIT;
来源：http://dm.chemitech.net.cn

[Q65] 回滚事务
来源：http://dq.panjiajie.cn

ROLLBACK;
来源：http://or.haigaiapp.cn

[Q66] 行锁查询
来源：http://cf.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vk.lnxyls.cn

[Q67] 设置隔离级别
来源：http://ie.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xv.9csxet.cn

[Q68] 保存点
来源：http://za.jctech888.com.cn

SAVEPOINT sp1;
来源：http://pi.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://kt.nszjky.cn

[Q69] 查看执行计划
来源：http://pp.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kp.lnxyls.cn

[Q70] 更新统计信息
来源：http://pl.9csxet.cn

ANALYZE TABLE users;
来源：http://zo.haigaiapp.cn

[Q71] 查看建表语句
来源：http://nd.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://im.jianghongdianzi.cn

[Q72] 查看索引
来源：http://kh.shxzukj.cn

SHOW INDEX FROM users;
来源：http://ra.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://nr.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bg.yuntaijiaju.cn

[Q74] 强制使用索引
来源：http://to.lnxyls.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xt.wgjwhj.cn

[Q75] 日期格式化
来源：http://mo.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qu.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fs.lnxyls.cn

[Q76] 按天统计
来源：http://yr.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qs.huixiangedu.cn

[Q77] 时间加减
来源：http://xl.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xt.shxzukj.cn

[Q78] 当前时间
来源：http://ja.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pf.gzmigu.cn

[Q79] 字符串拼接
来源：http://hx.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fy.szxytkj.cn

[Q80] 字符串截取
来源：http://rp.jianghongdianzi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rn.gzmigu.cn

[Q81] 字符串替换
来源：http://kr.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://it.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://hi.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wv.yuexingan06.cn

[Q83] 大小写转换
来源：http://gi.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gc.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://nx.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://fl.muxihuayi.cn

[Q85] 数值取整
来源：http://ts.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rl.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://dt.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://go.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://im.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ru.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://ld.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ht.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://th.gzmigu.cn

[Q89] 判断表是否存在
来源：http://bc.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mv.yuexingan06.cn

[Q90] 生成序号列
来源：http://vl.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ge.hnjuh.cn

================================================================================
来源：http://og.hahajie.cn

R. Bash 专题
来源：http://oz.gzmigu.cn

================================================================================
来源：http://ln.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://xp.huanxung.cn

#!/usr/bin/env bash
来源：http://wt.nicolike.cn

set -euo pipefail
来源：http://ej.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://el.szxytkj.cn

name="Tom"; echo "$name"
来源：http://zq.shxzukj.cn

[R03] 只读变量
来源：http://gd.lnxyls.cn

readonly PI=3.14
来源：http://du.newstarts.cn

[R04] 位置参数
来源：http://ag.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pm.9csxet.cn

[R05] 参数默认值
来源：http://al.yuexingan06.cn

name="${1:-default}"
来源：http://ej.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://zh.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ja.yuntaijiaju.cn

[R07] if 判断文件
来源：http://zz.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ve.wgjwhj.cn

[R08] 数值比较
来源：http://vd.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fc.haigaiapp.cn

[R09] 字符串比较
来源：http://yz.nszjky.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qi.shxzukj.cn

[R10] 正则匹配
来源：http://zj.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ek.yuntaijiaju.cn

[R11] case 多分支
来源：http://ky.asd995.cn

case "$1" in
来源：http://wa.nicolike.cn

start) echo "启动" ;;
来源：http://yy.nszjky.cn

stop)  echo "停止" ;;
来源：http://pg.szsharing.cn

*)     echo "未知命令" ;;
来源：http://pb.nicolike.cn

esac
来源：http://ud.panjiajie.cn

[R12] for 遍历文件
来源：http://py.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://ai.haigaiapp.cn

[R13] for 计数循环
来源：http://ls.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://sm.nicolike.cn

[R14] C 风格 for
来源：http://wp.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pc.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://ek.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ji.huixinmuqiang.cn

[R16] until 等待条件
来源：http://jf.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hp.bjjhwx.cn

[R17] 数组定义与取值
来源：http://ww.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mf.jctech888.com.cn

[R18] 遍历数组
来源：http://fv.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vr.hnjuh.cn

[R19] 数组长度
来源：http://ad.hahajie.cn

echo "${#arr[@]}"
来源：http://ei.huanxung.cn

[R20] 关联数组（字典）
来源：http://xf.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zr.panjiajie.cn

[R21] 字符串长度
来源：http://rj.panjiajie.cn

echo "${#s}"
来源：http://en.panjiajie.cn

[R22] 截取子串
来源：http://oi.hnjuh.cn

echo "${s:0:5}"
来源：http://ra.shtwfgs.cn

[R23] 字符串替换
来源：http://fi.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yl.bookmarksfly.cn

[R24] 大小写转换
来源：http://kf.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gu.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://dx.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bf.jianghongdianzi.cn

[R26] 命令替换
来源：http://bw.colortex.cn

now=$(date +%F); echo "$now"
来源：http://mr.hahajie.cn

[R27] 算术展开
来源：http://rt.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://iz.521024.cn

[R28] 浮点运算
来源：http://uo.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://yg.nicolike.cn

[R29] 定义函数
来源：http://xd.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jp.nszjky.cn

[R30] 函数返回状态码
来源：http://pt.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://un.hnjuh.cn

[R31] 局部变量
来源：http://rx.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://hz.nicolike.cn

[R32] 参数个数校验
来源：http://kc.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ca.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://nt.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zz.yuexingan06.cn

[R34] 退出时清理
来源：http://pr.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bt.nicolike.cn

[R35] 后台执行并等待
来源：http://bt.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dq.huanxung.cn

[R36] 并发执行多个任务
来源：http://ui.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wn.colortex.cn

[R37] 把输出赋给变量
来源：http://gg.hnjuh.cn

files=$(ls -1)
来源：http://zc.hnjuh.cn

[R38] 管道串联
来源：http://ga.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://xs.521024.cn

[R39] 重定向标准输出与错误
来源：http://so.nicolike.cn

cmd > out.log 2>&1
来源：http://jk.huixinmuqiang.cn

[R40] 追加写日志
来源：http://ly.shtwfgs.cn

echo "log" >> out.log
来源：http://em.bjjhwx.cn

[R41] 丢弃输出
来源：http://nq.9csxet.cn

cmd >/dev/null 2>&1
来源：http://xq.nszjky.cn

[R42] 输入重定向
来源：http://yy.lnxyls.cn

wc -l < a.txt
来源：http://hk.shxzskj.cn

[R43] 按名字查找文件
来源：http://di.szxytkj.cn

find . -name "*.log" -type f
来源：http://jc.asd995.cn

[R44] 按修改时间查找
来源：http://jb.wgjwhj.cn

find . -mtime -7 -type f
来源：http://tb.haigaiapp.cn

[R45] 批量删除
来源：http://jd.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://cg.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://ke.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gd.lnxyls.cn

[R47] sed 单行替换
来源：http://zd.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qy.nszjky.cn

[R48] awk 取指定列
来源：http://fy.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://zz.bookmarksfly.cn

[R49] awk 带条件
来源：http://bi.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cf.muxihuayi.cn

[R50] awk 求和
来源：http://in.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fi.asd995.cn

[R51] 排序去重取前几
来源：http://jx.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://go.nszjky.cn

[R52] 统计行数
来源：http://cq.nicolike.cn

wc -l a.txt
来源：http://um.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://lh.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ui.chemitech.net.cn

[R54] 比较两个文件
来源：http://rf.chemitech.net.cn

diff a.txt b.txt
来源：http://fa.hnjuh.cn

[R55] 压缩与解压
来源：http://ly.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wh.9csxet.cn

[R56] 远程拷贝
来源：http://of.colortex.cn

scp file user@host:/path/
来源：http://ps.bjjhwx.cn

[R57] 远程执行命令
来源：http://ui.shxzukj.cn

ssh user@host 'uptime'
来源：http://hd.asd995.cn

[R58] 下载文件
来源：http://oa.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fm.nicolike.cn

[R59] 发 POST JSON
来源：http://ua.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rz.521024.cn

[R60] 只看 HTTP 状态码
来源：http://xk.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lz.szsharing.cn

[R61] 磁盘占用
来源：http://zb.shxzskj.cn

df -h;  du -sh *
来源：http://ee.hnjuh.cn

[R62] 找最占空间的文件
来源：http://nd.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://fd.hahajie.cn

[R63] 内存与进程
来源：http://hn.asd995.cn

free -h;  ps aux | grep nginx
来源：http://ys.jianghongdianzi.cn

[R64] 结束进程
来源：http://uv.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://ei.jctech888.com.cn

[R65] 查看端口占用
来源：http://re.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rn.shtwfgs.cn

[R66] 定时任务
来源：http://is.9csxet.cn

crontab -e;  crontab -l
来源：http://bm.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://yd.muxihuayi.cn

openssl rand -hex 16
来源：http://ws.asd995.cn

[R68] 计算文件校验值
来源：http://lv.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pu.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://hr.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://fc.shxzskj.cn

[R70] 时间戳与互转
来源：http://wf.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://ma.bjjhwx.cn

[R71] 日期格式化
来源：http://my.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zl.chemitech.net.cn

[R72] 等待端口就绪
来源：http://qa.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qj.521024.cn

[R73] 分割大日志
来源：http://qd.asd995.cn


<!-- 参考信息 -->