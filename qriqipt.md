代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fv.huanxung.cn

[Q28] 求和与平均
来源：http://dt.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jv.yuntaijiaju.cn

[Q29] 最大最小值
来源：http://gd.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tb.wgjwhj.cn

[Q30] 分组统计
来源：http://hs.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vx.gzmigu.cn

[Q31] 分组后过滤
来源：http://pq.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hs.nszjky.cn

[Q32] 分组拼接字符串
来源：http://bc.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xz.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://de.jianghongdianzi.cn

[Q33] 多列分组
来源：http://ta.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pj.nicolike.cn

[Q34] 每组取第一条
来源：http://kb.jctech888.com.cn

SELECT * FROM (
来源：http://na.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hx.nicolike.cn

) t WHERE rn = 1;
来源：http://ni.muxihuayi.cn

[Q35] 内连接
来源：http://pj.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://li.huixinmuqiang.cn

[Q36] 左连接
来源：http://gu.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hp.szsharing.cn

[Q37] 右连接
来源：http://go.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ts.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vm.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://le.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://gb.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ln.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lz.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://he.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zg.huixinmuqiang.cn

[Q41] 多表连接
来源：http://ov.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hf.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://de.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://lo.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://aw.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://ky.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mf.shxzskj.cn

[Q43] 标量子查询
来源：http://ri.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://av.yuexingan06.cn

[Q44] IN 子查询
来源：http://kc.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tt.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://eu.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gx.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uk.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://us.shtwfgs.cn

[Q47] 与平均值比较
来源：http://ha.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lc.521024.cn

[Q48] CTE 公用表表达式
来源：http://fo.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://av.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://gj.lnxyls.cn

[Q49] 更新单行
来源：http://bm.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fn.shtwfgs.cn

[Q50] 批量更新
来源：http://ov.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://so.hnjuh.cn

[Q51] 用子查询更新
来源：http://rs.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yv.colortex.cn

[Q52] 删除指定行
来源：http://sh.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://rr.chemitech.net.cn

[Q53] 按条件删除
来源：http://lt.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jm.lnxyls.cn

[Q54] 清空表
来源：http://mx.newstarts.cn

TRUNCATE TABLE logs;
来源：http://bf.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://rv.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sl.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://ao.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://us.szsharing.cn

[Q57] 行号
来源：http://ec.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zb.bookmarksfly.cn

[Q58] 累计求和
来源：http://gf.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ot.panjiajie.cn

[Q59] 分组内累计
来源：http://gc.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tp.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://ru.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ty.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jb.bookmarksfly.cn

[Q61] 移动平均
来源：http://fu.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lw.panjiajie.cn

[Q62] 分组占比
来源：http://qf.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cs.shtwfgs.cn

[Q63] 开启事务
来源：http://hn.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tz.huixinmuqiang.cn

[Q64] 提交事务
来源：http://lu.bjjhwx.cn

COMMIT;
来源：http://yi.jctech888.com.cn

[Q65] 回滚事务
来源：http://ue.panjiajie.cn

ROLLBACK;
来源：http://gw.yuexingan06.cn

[Q66] 行锁查询
来源：http://xg.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hv.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://xc.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wb.newstarts.cn

[Q68] 保存点
来源：http://ud.jianghongdianzi.cn

SAVEPOINT sp1;
来源：http://cu.9csxet.cn

ROLLBACK TO sp1;
来源：http://xw.nszjky.cn

[Q69] 查看执行计划
来源：http://uk.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bq.asd995.cn

[Q70] 更新统计信息
来源：http://wo.wgjwhj.cn

ANALYZE TABLE users;
来源：http://kr.muxihuayi.cn

[Q71] 查看建表语句
来源：http://ow.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oq.bjjhwx.cn

[Q72] 查看索引
来源：http://ht.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://pt.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://ly.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tu.chemitech.net.cn

[Q74] 强制使用索引
来源：http://ba.lnxyls.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eg.hahajie.cn

[Q75] 日期格式化
来源：http://xp.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cf.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://si.wgjwhj.cn

[Q76] 按天统计
来源：http://iq.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tl.szsharing.cn

[Q77] 时间加减
来源：http://cn.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ds.hnjuh.cn

[Q78] 当前时间
来源：http://pr.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yw.muxihuayi.cn

[Q79] 字符串拼接
来源：http://kb.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://td.colortex.cn

[Q80] 字符串截取
来源：http://wf.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jl.gzmigu.cn

[Q81] 字符串替换
来源：http://zz.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sm.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://yw.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sc.huixiangedu.cn

[Q83] 大小写转换
来源：http://cr.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://px.9csxet.cn

[Q84] 去除首尾空格
来源：http://fc.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://lk.nszjky.cn

[Q85] 数值取整
来源：http://ar.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ef.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://vk.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fr.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://lb.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://by.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://po.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pi.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cq.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://td.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jb.colortex.cn

[Q90] 生成序号列
来源：http://xu.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uo.shxzskj.cn

================================================================================
来源：http://lx.shtwfgs.cn

R. Bash 专题
来源：http://bt.yuntaijiaju.cn

================================================================================
来源：http://qh.newstarts.cn

[R01] shebang 与严格模式
来源：http://lx.gzmigu.cn

#!/usr/bin/env bash
来源：http://cw.asd995.cn

set -euo pipefail
来源：http://ad.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://dr.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://af.muxihuayi.cn

[R03] 只读变量
来源：http://ju.jctech888.com.cn

readonly PI=3.14
来源：http://vu.colortex.cn

[R04] 位置参数
来源：http://eo.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yl.huixiangedu.cn

[R05] 参数默认值
来源：http://ha.yuexingan06.cn

name="${1:-default}"
来源：http://al.huanxung.cn

[R06] 判断命令是否存在
来源：http://mb.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tk.newstarts.cn

[R07] if 判断文件
来源：http://ye.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gf.newstarts.cn

[R08] 数值比较
来源：http://sb.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rv.colortex.cn

[R09] 字符串比较
来源：http://yz.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ef.9csxet.cn

[R10] 正则匹配
来源：http://de.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kd.yuexingan06.cn

[R11] case 多分支
来源：http://om.yuntaijiaju.cn

case "$1" in
来源：http://hw.nicolike.cn

start) echo "启动" ;;
来源：http://tl.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://gk.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://xe.newstarts.cn

esac
来源：http://bn.shtwfgs.cn

[R12] for 遍历文件
来源：http://mw.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://tk.shxzukj.cn

[R13] for 计数循环
来源：http://dz.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://sm.yuntaijiaju.cn

[R14] C 风格 for
来源：http://kt.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wd.newstarts.cn

[R15] while 逐行读文件
来源：http://jw.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rc.lnxyls.cn

[R16] until 等待条件
来源：http://sn.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pi.521024.cn

[R17] 数组定义与取值
来源：http://ai.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://at.nicolike.cn

[R18] 遍历数组
来源：http://jv.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nl.shtwfgs.cn

[R19] 数组长度
来源：http://sj.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://ox.panjiajie.cn

[R20] 关联数组（字典）
来源：http://gt.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zu.panjiajie.cn

[R21] 字符串长度
来源：http://oy.shtwfgs.cn

echo "${#s}"
来源：http://dr.lnxyls.cn

[R22] 截取子串
来源：http://ra.chemitech.net.cn

echo "${s:0:5}"
来源：http://yz.jctech888.com.cn

[R23] 字符串替换
来源：http://ur.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kx.chemitech.net.cn

[R24] 大小写转换
来源：http://sh.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gp.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://jf.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ps.jianghongdianzi.cn

[R26] 命令替换
来源：http://kb.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://tb.huanxung.cn

[R27] 算术展开
来源：http://ev.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://ph.521024.cn

[R28] 浮点运算
来源：http://zr.huixiangedu.cn

echo "scale=2; 10/3" | bc
来源：http://ff.nicolike.cn

[R29] 定义函数
来源：http://wh.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oh.hnjuh.cn

[R30] 函数返回状态码
来源：http://kx.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://rn.nicolike.cn

[R31] 局部变量
来源：http://zf.nszjky.cn

f() { local x=1; echo "$x"; }
来源：http://wk.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://qs.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hd.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://sr.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ks.gzmigu.cn

[R34] 退出时清理
来源：http://eq.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lm.hnjuh.cn

[R35] 后台执行并等待
来源：http://jq.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zk.szxytkj.cn

[R36] 并发执行多个任务
来源：http://iq.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ph.9csxet.cn

[R37] 把输出赋给变量
来源：http://yo.panjiajie.cn

files=$(ls -1)
来源：http://bk.bookmarksfly.cn

[R38] 管道串联
来源：http://vq.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://vn.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://ho.newstarts.cn

cmd > out.log 2>&1
来源：http://cz.asd995.cn

[R40] 追加写日志
来源：http://rh.panjiajie.cn

echo "log" >> out.log
来源：http://kn.521024.cn

[R41] 丢弃输出
来源：http://ys.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://gc.yuexingan06.cn

[R42] 输入重定向
来源：http://ev.jianghongdianzi.cn

wc -l < a.txt
来源：http://dy.huanxung.cn

[R43] 按名字查找文件
来源：http://qd.haigaiapp.cn

find . -name "*.log" -type f
来源：http://up.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://qu.muxihuayi.cn

find . -mtime -7 -type f
来源：http://yw.chemitech.net.cn

[R45] 批量删除
来源：http://di.newstarts.cn

find . -name "*.tmp" -delete
来源：http://jf.shxzukj.cn

[R46] 递归替换文件内容
来源：http://hu.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cv.muxihuayi.cn

[R47] sed 单行替换
来源：http://mm.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bv.haigaiapp.cn

[R48] awk 取指定列
来源：http://yy.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://ye.panjiajie.cn

[R49] awk 带条件
来源：http://bo.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lz.asd995.cn

[R50] awk 求和
来源：http://vm.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ki.muxihuayi.cn

[R51] 排序去重取前几
来源：http://bu.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wq.colortex.cn

[R52] 统计行数
来源：http://ln.521024.cn

wc -l a.txt
来源：http://zq.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://qi.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zt.jctech888.com.cn

[R54] 比较两个文件
来源：http://tp.szxytkj.cn

diff a.txt b.txt
来源：http://yp.bookmarksfly.cn

[R55] 压缩与解压
来源：http://la.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dy.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://en.yuexingan06.cn

scp file user@host:/path/
来源：http://mx.muxihuayi.cn

[R57] 远程执行命令
来源：http://oj.asd995.cn

ssh user@host 'uptime'
来源：http://il.nszjky.cn

[R58] 下载文件
来源：http://sw.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dd.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://ov.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ts.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://hq.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yz.9csxet.cn

[R61] 磁盘占用
来源：http://bc.jianghongdianzi.cn

df -h;  du -sh *
来源：http://xi.szsharing.cn

[R62] 找最占空间的文件
来源：http://fl.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://qj.jctech888.com.cn

[R63] 内存与进程
来源：http://yh.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://xf.colortex.cn

[R64] 结束进程
来源：http://hj.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://is.nszjky.cn

[R65] 查看端口占用
来源：http://tk.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gt.chemitech.net.cn

[R66] 定时任务
来源：http://yp.gzmigu.cn

crontab -e;  crontab -l
来源：http://he.colortex.cn

[R67] 生成随机十六进制串
来源：http://kc.shxzskj.cn

openssl rand -hex 16
来源：http://by.haigaiapp.cn

[R68] 计算文件校验值
来源：http://sn.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gb.shxzskj.cn

[R69] 生成随机密码
来源：http://ge.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://tu.shxzukj.cn

[R70] 时间戳与互转
来源：http://ju.9csxet.cn

date +%s;  date -d @1700000000
来源：http://ly.lnxyls.cn

[R71] 日期格式化
来源：http://ol.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://aq.colortex.cn

[R72] 等待端口就绪
来源：http://wu.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fe.colortex.cn

[R73] 分割大日志
来源：http://bx.gzmigu.cn

split -l 1000 big.log part_
来源：http://wl.bookmarksfly.cn

[R74] 批量重命名
来源：http://of.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://av.shxzskj.cn

[R75] 导出环境变量
来源：http://ht.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://bo.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://rd.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gq.gzmigu.cn

[R77] 读取用户输入
来源：http://ye.bjjhwx.cn


<!-- 参考信息 -->