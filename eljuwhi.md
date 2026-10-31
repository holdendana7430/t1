代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xj.jctech888.com.cn

[Q24] 去重
来源：http://nm.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://am.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://sz.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://om.chemitech.net.cn

[Q26] 计数
来源：http://wm.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://rh.newstarts.cn

[Q27] 条件计数
来源：http://wt.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yg.gzmigu.cn

[Q28] 求和与平均
来源：http://yt.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hb.shxzskj.cn

[Q29] 最大最小值
来源：http://cd.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gf.bjjhwx.cn

[Q30] 分组统计
来源：http://db.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qr.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://cg.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ur.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://on.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xc.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fv.jianghongdianzi.cn

[Q33] 多列分组
来源：http://gl.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://do.hnjuh.cn

[Q34] 每组取第一条
来源：http://qy.szxytkj.cn

SELECT * FROM (
来源：http://xl.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ab.szxytkj.cn

) t WHERE rn = 1;
来源：http://kc.521024.cn

[Q35] 内连接
来源：http://ci.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lm.colortex.cn

[Q36] 左连接
来源：http://eg.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lo.bookmarksfly.cn

[Q37] 右连接
来源：http://dq.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bb.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://so.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nk.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://cz.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ac.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lm.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://aj.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lf.hnjuh.cn

[Q41] 多表连接
来源：http://bb.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tz.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://no.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://ae.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://pp.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://jc.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ev.colortex.cn

[Q43] 标量子查询
来源：http://zh.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gu.hnjuh.cn

[Q44] IN 子查询
来源：http://tb.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xa.521024.cn

[Q45] EXISTS 判断存在
来源：http://ku.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://up.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bm.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bm.panjiajie.cn

[Q47] 与平均值比较
来源：http://fl.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uq.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://jk.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nb.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://mw.9csxet.cn

[Q49] 更新单行
来源：http://mx.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fe.szxytkj.cn

[Q50] 批量更新
来源：http://kz.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hm.asd995.cn

[Q51] 用子查询更新
来源：http://yh.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jk.asd995.cn

[Q52] 删除指定行
来源：http://lj.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://dz.asd995.cn

[Q53] 按条件删除
来源：http://of.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vl.hahajie.cn

[Q54] 清空表
来源：http://oj.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://ea.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://nd.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rh.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://rm.huixiangedu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oe.hnjuh.cn

[Q57] 行号
来源：http://fs.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ds.gzmigu.cn

[Q58] 累计求和
来源：http://sf.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ac.lnxyls.cn

[Q59] 分组内累计
来源：http://vh.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ca.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://dd.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cv.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xl.gzmigu.cn

[Q61] 移动平均
来源：http://bt.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://br.bjjhwx.cn

[Q62] 分组占比
来源：http://om.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eb.shtwfgs.cn

[Q63] 开启事务
来源：http://zi.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bm.jianghongdianzi.cn

[Q64] 提交事务
来源：http://hi.gzmigu.cn

COMMIT;
来源：http://ha.haigaiapp.cn

[Q65] 回滚事务
来源：http://us.bookmarksfly.cn

ROLLBACK;
来源：http://uc.lnxyls.cn

[Q66] 行锁查询
来源：http://ci.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gf.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://mw.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jz.hahajie.cn

[Q68] 保存点
来源：http://ke.jianghongdianzi.cn

SAVEPOINT sp1;
来源：http://zz.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://gc.lnxyls.cn

[Q69] 查看执行计划
来源：http://mk.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ye.asd995.cn

[Q70] 更新统计信息
来源：http://mz.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://ih.haigaiapp.cn

[Q71] 查看建表语句
来源：http://se.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xp.521024.cn

[Q72] 查看索引
来源：http://tj.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://nq.shtwfgs.cn

[Q73] 查看表状态
来源：http://pr.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ln.bjjhwx.cn

[Q74] 强制使用索引
来源：http://pl.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bz.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://uf.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kq.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pm.muxihuayi.cn

[Q76] 按天统计
来源：http://qn.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kr.bookmarksfly.cn

[Q77] 时间加减
来源：http://xm.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ty.jctech888.com.cn

[Q78] 当前时间
来源：http://cz.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pt.nszjky.cn

[Q79] 字符串拼接
来源：http://kr.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zu.huanxung.cn

[Q80] 字符串截取
来源：http://ur.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vb.wgjwhj.cn

[Q81] 字符串替换
来源：http://fv.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wh.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://kw.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dz.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://ic.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ad.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://up.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://go.jianghongdianzi.cn

[Q85] 数值取整
来源：http://yn.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ui.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://xx.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wd.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://ov.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kn.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://fm.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tv.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wj.newstarts.cn

[Q89] 判断表是否存在
来源：http://et.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://br.gzmigu.cn

[Q90] 生成序号列
来源：http://az.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ta.huixinmuqiang.cn

================================================================================
来源：http://zn.shtwfgs.cn

R. Bash 专题
来源：http://vp.chemitech.net.cn

================================================================================
来源：http://xg.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://qs.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://fb.szxytkj.cn

set -euo pipefail
来源：http://sb.nszjky.cn

[R02] 变量赋值与使用
来源：http://kz.shxzukj.cn

name="Tom"; echo "$name"
来源：http://iz.yuntaijiaju.cn

[R03] 只读变量
来源：http://fn.colortex.cn

readonly PI=3.14
来源：http://fh.hahajie.cn

[R04] 位置参数
来源：http://em.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rn.jctech888.com.cn

[R05] 参数默认值
来源：http://xz.hnjuh.cn

name="${1:-default}"
来源：http://cu.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://th.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gs.chemitech.net.cn

[R07] if 判断文件
来源：http://sq.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hy.panjiajie.cn

[R08] 数值比较
来源：http://od.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jk.9csxet.cn

[R09] 字符串比较
来源：http://ut.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mj.9csxet.cn

[R10] 正则匹配
来源：http://qx.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pi.huanxung.cn

[R11] case 多分支
来源：http://yk.shtwfgs.cn

case "$1" in
来源：http://jz.nszjky.cn

start) echo "启动" ;;
来源：http://np.gzmigu.cn

stop)  echo "停止" ;;
来源：http://jd.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://ez.panjiajie.cn

esac
来源：http://zu.panjiajie.cn

[R12] for 遍历文件
来源：http://qh.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://ho.shxzukj.cn

[R13] for 计数循环
来源：http://mv.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://to.lnxyls.cn

[R14] C 风格 for
来源：http://kc.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zx.shtwfgs.cn

[R15] while 逐行读文件
来源：http://ba.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://on.asd995.cn

[R16] until 等待条件
来源：http://rz.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://if.panjiajie.cn

[R17] 数组定义与取值
来源：http://hr.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tn.yuexingan06.cn

[R18] 遍历数组
来源：http://pv.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://so.huixinmuqiang.cn

[R19] 数组长度
来源：http://tm.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://up.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://lq.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tt.asd995.cn

[R21] 字符串长度
来源：http://xd.bjjhwx.cn

echo "${#s}"
来源：http://uy.bookmarksfly.cn

[R22] 截取子串
来源：http://ze.shtwfgs.cn

echo "${s:0:5}"
来源：http://vy.bjjhwx.cn

[R23] 字符串替换
来源：http://go.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mu.newstarts.cn

[R24] 大小写转换
来源：http://cw.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ow.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://qz.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gd.chemitech.net.cn

[R26] 命令替换
来源：http://hb.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://gi.panjiajie.cn

[R27] 算术展开
来源：http://mg.huanxung.cn

echo $((1 + 2 * 3))
来源：http://nu.jianghongdianzi.cn

[R28] 浮点运算
来源：http://zq.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://fq.huixinmuqiang.cn

[R29] 定义函数
来源：http://ty.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bk.haigaiapp.cn

[R30] 函数返回状态码
来源：http://of.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://jc.jctech888.com.cn

[R31] 局部变量
来源：http://jf.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://vh.9csxet.cn

[R32] 参数个数校验
来源：http://jz.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://id.asd995.cn

[R33] 捕获错误并提示行号
来源：http://gl.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mi.lnxyls.cn

[R34] 退出时清理
来源：http://wh.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://iz.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://gq.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qk.newstarts.cn

[R36] 并发执行多个任务
来源：http://rj.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pc.9csxet.cn

[R37] 把输出赋给变量
来源：http://te.panjiajie.cn

files=$(ls -1)
来源：http://tn.huixinmuqiang.cn

[R38] 管道串联
来源：http://oj.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://gx.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://md.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://uf.jctech888.com.cn

[R40] 追加写日志
来源：http://qa.newstarts.cn

echo "log" >> out.log
来源：http://ub.wgjwhj.cn

[R41] 丢弃输出
来源：http://dl.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://nx.yuntaijiaju.cn

[R42] 输入重定向
来源：http://hv.szsharing.cn

wc -l < a.txt
来源：http://lj.shxzukj.cn

[R43] 按名字查找文件
来源：http://eq.shxzukj.cn

find . -name "*.log" -type f
来源：http://ws.szsharing.cn

[R44] 按修改时间查找
来源：http://yu.9csxet.cn

find . -mtime -7 -type f
来源：http://tg.huixiangedu.cn

[R45] 批量删除
来源：http://hx.huanxung.cn

find . -name "*.tmp" -delete
来源：http://pr.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://md.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ol.nicolike.cn

[R47] sed 单行替换
来源：http://ie.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bd.shxzskj.cn

[R48] awk 取指定列
来源：http://pj.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://hq.yuntaijiaju.cn

[R49] awk 带条件
来源：http://vk.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nh.yuntaijiaju.cn

[R50] awk 求和
来源：http://an.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ar.yuexingan06.cn

[R51] 排序去重取前几
来源：http://ek.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wu.521024.cn

[R52] 统计行数
来源：http://fd.haigaiapp.cn

wc -l a.txt
来源：http://ly.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://ma.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ov.shtwfgs.cn

[R54] 比较两个文件
来源：http://vh.hnjuh.cn

diff a.txt b.txt
来源：http://bq.shxzskj.cn

[R55] 压缩与解压
来源：http://wk.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gk.shtwfgs.cn

[R56] 远程拷贝
来源：http://ki.panjiajie.cn

scp file user@host:/path/
来源：http://ae.newstarts.cn

[R57] 远程执行命令
来源：http://kk.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://ta.colortex.cn

[R58] 下载文件
来源：http://ak.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qw.asd995.cn

[R59] 发 POST JSON
来源：http://tw.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://it.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://fb.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jk.haigaiapp.cn

[R61] 磁盘占用
来源：http://ag.jianghongdianzi.cn

df -h;  du -sh *
来源：http://xc.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://fg.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://co.yuexingan06.cn

[R63] 内存与进程
来源：http://zk.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://ob.szxytkj.cn

[R64] 结束进程
来源：http://cm.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://vz.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://wx.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://og.asd995.cn

[R66] 定时任务
来源：http://ty.huanxung.cn

crontab -e;  crontab -l
来源：http://yb.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://kj.panjiajie.cn

openssl rand -hex 16
来源：http://xu.yuexingan06.cn

[R68] 计算文件校验值
来源：http://ar.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vw.huixiangedu.cn

[R69] 生成随机密码
来源：http://ow.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://fn.muxihuayi.cn

[R70] 时间戳与互转
来源：http://ab.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://pe.yuexingan06.cn

[R71] 日期格式化
来源：http://gu.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rt.muxihuayi.cn

[R72] 等待端口就绪
来源：http://jn.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ej.haigaiapp.cn

[R73] 分割大日志
来源：http://vp.panjiajie.cn


<!-- 参考信息 -->