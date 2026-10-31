代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oq.shtwfgs.cn

[Q28] 求和与平均
来源：http://tb.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sa.haigaiapp.cn

[Q29] 最大最小值
来源：http://vq.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fu.huixinmuqiang.cn

[Q30] 分组统计
来源：http://ap.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hf.wgjwhj.cn

[Q31] 分组后过滤
来源：http://eb.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vb.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://mo.colortex.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bn.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hc.panjiajie.cn

[Q33] 多列分组
来源：http://tv.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lf.asd995.cn

[Q34] 每组取第一条
来源：http://uw.panjiajie.cn

SELECT * FROM (
来源：http://yl.nicolike.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wr.asd995.cn

) t WHERE rn = 1;
来源：http://yw.hnjuh.cn

[Q35] 内连接
来源：http://uk.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ke.shxzskj.cn

[Q36] 左连接
来源：http://re.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wx.hnjuh.cn

[Q37] 右连接
来源：http://gu.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pc.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kt.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cf.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://nh.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ks.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://si.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yg.shxzukj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qf.nszjky.cn

[Q41] 多表连接
来源：http://hx.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yv.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://uo.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://al.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://el.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://lb.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gq.521024.cn

[Q43] 标量子查询
来源：http://ze.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qd.nicolike.cn

[Q44] IN 子查询
来源：http://ew.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://em.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://zk.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sf.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ri.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zo.521024.cn

[Q47] 与平均值比较
来源：http://lt.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jr.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://av.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zx.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://ow.jianghongdianzi.cn

[Q49] 更新单行
来源：http://wg.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gh.9csxet.cn

[Q50] 批量更新
来源：http://cy.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fp.hnjuh.cn

[Q51] 用子查询更新
来源：http://uo.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wc.lnxyls.cn

[Q52] 删除指定行
来源：http://gj.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://np.bookmarksfly.cn

[Q53] 按条件删除
来源：http://wh.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bp.huanxung.cn

[Q54] 清空表
来源：http://il.hahajie.cn

TRUNCATE TABLE logs;
来源：http://fc.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://le.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sb.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://ep.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fi.jctech888.com.cn

[Q57] 行号
来源：http://pi.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ps.szsharing.cn

[Q58] 累计求和
来源：http://zy.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://co.521024.cn

[Q59] 分组内累计
来源：http://vy.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jz.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://ei.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uj.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hp.huixiangedu.cn

[Q61] 移动平均
来源：http://mz.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rl.bjjhwx.cn

[Q62] 分组占比
来源：http://md.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://si.szxytkj.cn

[Q63] 开启事务
来源：http://ya.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://th.colortex.cn

[Q64] 提交事务
来源：http://ws.newstarts.cn

COMMIT;
来源：http://bn.shtwfgs.cn

[Q65] 回滚事务
来源：http://yk.bookmarksfly.cn

ROLLBACK;
来源：http://az.haigaiapp.cn

[Q66] 行锁查询
来源：http://eq.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uu.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://ea.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gc.newstarts.cn

[Q68] 保存点
来源：http://hw.asd995.cn

SAVEPOINT sp1;
来源：http://yn.nszjky.cn

ROLLBACK TO sp1;
来源：http://jr.hahajie.cn

[Q69] 查看执行计划
来源：http://ma.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sr.muxihuayi.cn

[Q70] 更新统计信息
来源：http://jp.szsharing.cn

ANALYZE TABLE users;
来源：http://ak.panjiajie.cn

[Q71] 查看建表语句
来源：http://fj.huanxung.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ok.chemitech.net.cn

[Q72] 查看索引
来源：http://so.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://cf.huanxung.cn

[Q73] 查看表状态
来源：http://tu.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rl.bjjhwx.cn

[Q74] 强制使用索引
来源：http://en.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vh.colortex.cn

[Q75] 日期格式化
来源：http://gi.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wq.jianghongdianzi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lm.huixinmuqiang.cn

[Q76] 按天统计
来源：http://td.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fz.huixiangedu.cn

[Q77] 时间加减
来源：http://nh.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jr.wgjwhj.cn

[Q78] 当前时间
来源：http://hx.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pq.colortex.cn

[Q79] 字符串拼接
来源：http://tm.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ns.521024.cn

[Q80] 字符串截取
来源：http://hf.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jb.nszjky.cn

[Q81] 字符串替换
来源：http://jb.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fl.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://jl.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://di.muxihuayi.cn

[Q83] 大小写转换
来源：http://tv.szsharing.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eu.huanxung.cn

[Q84] 去除首尾空格
来源：http://wr.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://su.gzmigu.cn

[Q85] 数值取整
来源：http://cb.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wv.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://zr.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iw.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://ci.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ep.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://ht.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ep.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://io.newstarts.cn

[Q89] 判断表是否存在
来源：http://nb.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yg.asd995.cn

[Q90] 生成序号列
来源：http://rf.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pp.asd995.cn

================================================================================
来源：http://yq.lnxyls.cn

R. Bash 专题
来源：http://yj.yuntaijiaju.cn

================================================================================
来源：http://vn.hnjuh.cn

[R01] shebang 与严格模式
来源：http://nq.huanxung.cn

#!/usr/bin/env bash
来源：http://hd.shtwfgs.cn

set -euo pipefail
来源：http://qb.nicolike.cn

[R02] 变量赋值与使用
来源：http://iv.shxzukj.cn

name="Tom"; echo "$name"
来源：http://qe.jctech888.com.cn

[R03] 只读变量
来源：http://fv.muxihuayi.cn

readonly PI=3.14
来源：http://qi.521024.cn

[R04] 位置参数
来源：http://ru.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vl.521024.cn

[R05] 参数默认值
来源：http://ho.bookmarksfly.cn

name="${1:-default}"
来源：http://jv.nicolike.cn

[R06] 判断命令是否存在
来源：http://vc.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://po.bookmarksfly.cn

[R07] if 判断文件
来源：http://cp.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rv.shxzskj.cn

[R08] 数值比较
来源：http://pe.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pw.muxihuayi.cn

[R09] 字符串比较
来源：http://sl.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://on.haigaiapp.cn

[R10] 正则匹配
来源：http://hg.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ub.huixinmuqiang.cn

[R11] case 多分支
来源：http://ww.chemitech.net.cn

case "$1" in
来源：http://kt.huixiangedu.cn

start) echo "启动" ;;
来源：http://tc.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://gu.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://yl.shxzskj.cn

esac
来源：http://qk.shxzukj.cn

[R12] for 遍历文件
来源：http://nd.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://kr.bookmarksfly.cn

[R13] for 计数循环
来源：http://pm.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://ud.yuexingan06.cn

[R14] C 风格 for
来源：http://vk.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cf.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://kh.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sj.shxzukj.cn

[R16] until 等待条件
来源：http://om.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qr.9csxet.cn

[R17] 数组定义与取值
来源：http://qv.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jl.jctech888.com.cn

[R18] 遍历数组
来源：http://zu.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dx.panjiajie.cn

[R19] 数组长度
来源：http://bi.colortex.cn

echo "${#arr[@]}"
来源：http://qv.shxzskj.cn

[R20] 关联数组（字典）
来源：http://vp.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ct.shxzskj.cn

[R21] 字符串长度
来源：http://jl.shtwfgs.cn

echo "${#s}"
来源：http://nq.muxihuayi.cn

[R22] 截取子串
来源：http://ks.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://vx.shtwfgs.cn

[R23] 字符串替换
来源：http://sw.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fe.shtwfgs.cn

[R24] 大小写转换
来源：http://bd.nszjky.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dm.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://lu.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zw.huixiangedu.cn

[R26] 命令替换
来源：http://ld.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://tv.shxzskj.cn

[R27] 算术展开
来源：http://wg.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://xa.colortex.cn

[R28] 浮点运算
来源：http://rc.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://sh.haigaiapp.cn

[R29] 定义函数
来源：http://bi.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qb.yuexingan06.cn

[R30] 函数返回状态码
来源：http://vr.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://iq.szxytkj.cn

[R31] 局部变量
来源：http://wj.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://po.lnxyls.cn

[R32] 参数个数校验
来源：http://zu.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://um.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://iy.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://og.bookmarksfly.cn

[R34] 退出时清理
来源：http://do.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hd.yuexingan06.cn

[R35] 后台执行并等待
来源：http://mc.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nl.hahajie.cn

[R36] 并发执行多个任务
来源：http://yh.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lx.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://lr.panjiajie.cn

files=$(ls -1)
来源：http://vn.newstarts.cn

[R38] 管道串联
来源：http://kd.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://bs.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://ot.shtwfgs.cn

cmd > out.log 2>&1
来源：http://zj.521024.cn

[R40] 追加写日志
来源：http://xb.yuexingan06.cn

echo "log" >> out.log
来源：http://bi.newstarts.cn

[R41] 丢弃输出
来源：http://ib.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://iv.hahajie.cn

[R42] 输入重定向
来源：http://ik.521024.cn

wc -l < a.txt
来源：http://ql.newstarts.cn

[R43] 按名字查找文件
来源：http://kr.hnjuh.cn

find . -name "*.log" -type f
来源：http://oy.shxzukj.cn

[R44] 按修改时间查找
来源：http://bn.haigaiapp.cn

find . -mtime -7 -type f
来源：http://hx.521024.cn

[R45] 批量删除
来源：http://rw.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://fw.521024.cn

[R46] 递归替换文件内容
来源：http://ub.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uj.nicolike.cn

[R47] sed 单行替换
来源：http://hm.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nd.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://aw.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://fe.9csxet.cn

[R49] awk 带条件
来源：http://cd.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fp.bookmarksfly.cn

[R50] awk 求和
来源：http://bx.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ym.wgjwhj.cn

[R51] 排序去重取前几
来源：http://gn.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rs.szsharing.cn

[R52] 统计行数
来源：http://td.521024.cn

wc -l a.txt
来源：http://xx.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://as.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://if.hahajie.cn

[R54] 比较两个文件
来源：http://wq.szxytkj.cn

diff a.txt b.txt
来源：http://gt.muxihuayi.cn

[R55] 压缩与解压
来源：http://gj.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xw.shxzskj.cn

[R56] 远程拷贝
来源：http://sm.asd995.cn

scp file user@host:/path/
来源：http://jf.hahajie.cn

[R57] 远程执行命令
来源：http://fi.szxytkj.cn

ssh user@host 'uptime'
来源：http://ak.9csxet.cn

[R58] 下载文件
来源：http://ki.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oa.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://uw.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lg.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://ej.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mi.gzmigu.cn

[R61] 磁盘占用
来源：http://aa.yuntaijiaju.cn

df -h;  du -sh *
来源：http://dp.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://cb.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://pi.yuexingan06.cn

[R63] 内存与进程
来源：http://ao.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://oc.yuntaijiaju.cn

[R64] 结束进程
来源：http://gm.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://zq.huanxung.cn

[R65] 查看端口占用
来源：http://kj.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ru.wgjwhj.cn

[R66] 定时任务
来源：http://qs.szsharing.cn

crontab -e;  crontab -l
来源：http://jf.hahajie.cn

[R67] 生成随机十六进制串
来源：http://qd.szxytkj.cn

openssl rand -hex 16
来源：http://md.wgjwhj.cn

[R68] 计算文件校验值
来源：http://hl.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gu.wgjwhj.cn

[R69] 生成随机密码
来源：http://ec.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://pl.521024.cn

[R70] 时间戳与互转
来源：http://ws.9csxet.cn

date +%s;  date -d @1700000000
来源：http://ei.panjiajie.cn

[R71] 日期格式化
来源：http://lf.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mb.asd995.cn

[R72] 等待端口就绪
来源：http://sv.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ur.haigaiapp.cn

[R73] 分割大日志
来源：http://xw.nszjky.cn

split -l 1000 big.log part_
来源：http://bp.bjjhwx.cn

[R74] 批量重命名
来源：http://aj.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sm.huixiangedu.cn

[R75] 导出环境变量
来源：http://wu.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://kd.panjiajie.cn

[R76] 使用临时文件
来源：http://eh.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://su.bookmarksfly.cn

[R77] 读取用户输入
来源：http://hn.521024.cn


<!-- 参考信息 -->