代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yj.wgjwhj.cn

[Q28] 求和与平均
来源：http://hl.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bk.9csxet.cn

[Q29] 最大最小值
来源：http://cj.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vl.hnjuh.cn

[Q30] 分组统计
来源：http://ov.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pl.shxzukj.cn

[Q31] 分组后过滤
来源：http://js.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cp.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://cw.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yq.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pk.shxzukj.cn

[Q33] 多列分组
来源：http://nl.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xd.shxzskj.cn

[Q34] 每组取第一条
来源：http://if.yuexingan06.cn

SELECT * FROM (
来源：http://dt.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tt.huanxung.cn

) t WHERE rn = 1;
来源：http://og.nszjky.cn

[Q35] 内连接
来源：http://sp.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://py.huanxung.cn

[Q36] 左连接
来源：http://th.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cz.szxytkj.cn

[Q37] 右连接
来源：http://sg.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ao.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sl.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qo.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://qj.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ko.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xh.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://os.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://do.haigaiapp.cn

[Q41] 多表连接
来源：http://do.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qv.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://tc.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://he.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://qm.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://so.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ah.shtwfgs.cn

[Q43] 标量子查询
来源：http://xh.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ao.lnxyls.cn

[Q44] IN 子查询
来源：http://ep.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mx.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://xx.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sc.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://de.lnxyls.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tz.colortex.cn

[Q47] 与平均值比较
来源：http://rf.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sv.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://hm.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yy.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://xr.haigaiapp.cn

[Q49] 更新单行
来源：http://dq.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ef.bookmarksfly.cn

[Q50] 批量更新
来源：http://bt.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mh.huanxung.cn

[Q51] 用子查询更新
来源：http://wn.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yk.huixiangedu.cn

[Q52] 删除指定行
来源：http://xr.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://jp.shtwfgs.cn

[Q53] 按条件删除
来源：http://ep.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vo.hnjuh.cn

[Q54] 清空表
来源：http://mt.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://xn.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://ox.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ln.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://mx.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pg.chemitech.net.cn

[Q57] 行号
来源：http://tn.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xy.muxihuayi.cn

[Q58] 累计求和
来源：http://rr.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://os.hahajie.cn

[Q59] 分组内累计
来源：http://rr.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nh.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://lc.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rq.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yp.shxzukj.cn

[Q61] 移动平均
来源：http://qd.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hb.wgjwhj.cn

[Q62] 分组占比
来源：http://ub.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gk.wgjwhj.cn

[Q63] 开启事务
来源：http://mi.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ki.bjjhwx.cn

[Q64] 提交事务
来源：http://me.yuntaijiaju.cn

COMMIT;
来源：http://fg.wgjwhj.cn

[Q65] 回滚事务
来源：http://rv.nicolike.cn

ROLLBACK;
来源：http://vm.gzmigu.cn

[Q66] 行锁查询
来源：http://vv.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yw.szsharing.cn

[Q67] 设置隔离级别
来源：http://jp.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tf.hahajie.cn

[Q68] 保存点
来源：http://gg.colortex.cn

SAVEPOINT sp1;
来源：http://ry.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://az.szsharing.cn

[Q69] 查看执行计划
来源：http://mq.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nn.huixiangedu.cn

[Q70] 更新统计信息
来源：http://xw.shxzukj.cn

ANALYZE TABLE users;
来源：http://ud.newstarts.cn

[Q71] 查看建表语句
来源：http://ku.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xw.wgjwhj.cn

[Q72] 查看索引
来源：http://bb.shxzukj.cn

SHOW INDEX FROM users;
来源：http://qr.jctech888.com.cn

[Q73] 查看表状态
来源：http://rk.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ht.chemitech.net.cn

[Q74] 强制使用索引
来源：http://jc.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cj.wgjwhj.cn

[Q75] 日期格式化
来源：http://mh.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rp.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://an.jctech888.com.cn

[Q76] 按天统计
来源：http://qj.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://od.panjiajie.cn

[Q77] 时间加减
来源：http://bt.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mk.shxzskj.cn

[Q78] 当前时间
来源：http://nm.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ih.hahajie.cn

[Q79] 字符串拼接
来源：http://xp.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tt.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://nr.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ea.szsharing.cn

[Q81] 字符串替换
来源：http://gl.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://or.asd995.cn

[Q82] 字符长度与字节长度
来源：http://kv.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lp.haigaiapp.cn

[Q83] 大小写转换
来源：http://ms.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lf.lnxyls.cn

[Q84] 去除首尾空格
来源：http://np.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://sg.wgjwhj.cn

[Q85] 数值取整
来源：http://tk.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://he.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://ad.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://an.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://no.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eh.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://on.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lh.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ww.shxzukj.cn

[Q89] 判断表是否存在
来源：http://ef.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wb.nszjky.cn

[Q90] 生成序号列
来源：http://gv.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ct.bookmarksfly.cn

================================================================================
来源：http://hu.shxzskj.cn

R. Bash 专题
来源：http://qr.huixinmuqiang.cn

================================================================================
来源：http://eu.szsharing.cn

[R01] shebang 与严格模式
来源：http://lp.shtwfgs.cn

#!/usr/bin/env bash
来源：http://zs.panjiajie.cn

set -euo pipefail
来源：http://oz.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://go.hnjuh.cn

name="Tom"; echo "$name"
来源：http://jj.hnjuh.cn

[R03] 只读变量
来源：http://uk.nicolike.cn

readonly PI=3.14
来源：http://kj.panjiajie.cn

[R04] 位置参数
来源：http://em.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://je.521024.cn

[R05] 参数默认值
来源：http://yf.shxzukj.cn

name="${1:-default}"
来源：http://bp.nszjky.cn

[R06] 判断命令是否存在
来源：http://ok.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ns.haigaiapp.cn

[R07] if 判断文件
来源：http://ku.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yd.wgjwhj.cn

[R08] 数值比较
来源：http://ft.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gk.huanxung.cn

[R09] 字符串比较
来源：http://eb.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tg.shtwfgs.cn

[R10] 正则匹配
来源：http://uy.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zt.hahajie.cn

[R11] case 多分支
来源：http://eq.bookmarksfly.cn

case "$1" in
来源：http://es.bookmarksfly.cn

start) echo "启动" ;;
来源：http://xu.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://pq.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://vt.huanxung.cn

esac
来源：http://hp.colortex.cn

[R12] for 遍历文件
来源：http://tm.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://au.szsharing.cn

[R13] for 计数循环
来源：http://no.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://tv.hnjuh.cn

[R14] C 风格 for
来源：http://aw.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ky.gzmigu.cn

[R15] while 逐行读文件
来源：http://yv.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uz.yuexingan06.cn

[R16] until 等待条件
来源：http://hi.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://je.muxihuayi.cn

[R17] 数组定义与取值
来源：http://ir.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wg.wgjwhj.cn

[R18] 遍历数组
来源：http://dx.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ib.huixinmuqiang.cn

[R19] 数组长度
来源：http://yg.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://xp.panjiajie.cn

[R20] 关联数组（字典）
来源：http://yu.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hu.huanxung.cn

[R21] 字符串长度
来源：http://fj.huixiangedu.cn

echo "${#s}"
来源：http://ac.huixiangedu.cn

[R22] 截取子串
来源：http://em.lnxyls.cn

echo "${s:0:5}"
来源：http://bs.bjjhwx.cn

[R23] 字符串替换
来源：http://fe.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ze.colortex.cn

[R24] 大小写转换
来源：http://it.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ug.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://jx.lnxyls.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://og.panjiajie.cn

[R26] 命令替换
来源：http://kz.colortex.cn

now=$(date +%F); echo "$now"
来源：http://cq.lnxyls.cn

[R27] 算术展开
来源：http://sp.huanxung.cn

echo $((1 + 2 * 3))
来源：http://id.newstarts.cn

[R28] 浮点运算
来源：http://yx.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://sm.hahajie.cn

[R29] 定义函数
来源：http://el.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://na.bjjhwx.cn

[R30] 函数返回状态码
来源：http://uu.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://ga.huanxung.cn

[R31] 局部变量
来源：http://yo.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://zz.muxihuayi.cn

[R32] 参数个数校验
来源：http://gd.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hu.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://in.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eu.nszjky.cn

[R34] 退出时清理
来源：http://kh.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zf.521024.cn

[R35] 后台执行并等待
来源：http://dk.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fp.shxzskj.cn

[R36] 并发执行多个任务
来源：http://zb.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://up.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://qi.shxzukj.cn

files=$(ls -1)
来源：http://fe.lnxyls.cn

[R38] 管道串联
来源：http://ki.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://ap.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://an.huanxung.cn

cmd > out.log 2>&1
来源：http://sd.colortex.cn

[R40] 追加写日志
来源：http://oa.jctech888.com.cn

echo "log" >> out.log
来源：http://mk.bjjhwx.cn

[R41] 丢弃输出
来源：http://wi.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://kx.huixiangedu.cn

[R42] 输入重定向
来源：http://no.9csxet.cn

wc -l < a.txt
来源：http://yh.bjjhwx.cn

[R43] 按名字查找文件
来源：http://rj.szsharing.cn

find . -name "*.log" -type f
来源：http://nj.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://wh.nicolike.cn

find . -mtime -7 -type f
来源：http://hc.jctech888.com.cn

[R45] 批量删除
来源：http://cj.521024.cn

find . -name "*.tmp" -delete
来源：http://ye.521024.cn

[R46] 递归替换文件内容
来源：http://vw.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://in.jctech888.com.cn

[R47] sed 单行替换
来源：http://xr.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ja.muxihuayi.cn

[R48] awk 取指定列
来源：http://vq.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://hi.hahajie.cn

[R49] awk 带条件
来源：http://zz.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ma.huixiangedu.cn

[R50] awk 求和
来源：http://ym.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nt.haigaiapp.cn

[R51] 排序去重取前几
来源：http://qb.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dz.bjjhwx.cn

[R52] 统计行数
来源：http://fo.shxzukj.cn

wc -l a.txt
来源：http://es.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://vt.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qf.521024.cn

[R54] 比较两个文件
来源：http://wf.hnjuh.cn

diff a.txt b.txt
来源：http://ow.panjiajie.cn

[R55] 压缩与解压
来源：http://qt.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kk.bjjhwx.cn

[R56] 远程拷贝
来源：http://qr.shtwfgs.cn

scp file user@host:/path/
来源：http://lc.nszjky.cn

[R57] 远程执行命令
来源：http://wj.huanxung.cn

ssh user@host 'uptime'
来源：http://on.huixinmuqiang.cn

[R58] 下载文件
来源：http://cn.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ja.newstarts.cn

[R59] 发 POST JSON
来源：http://cq.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vy.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://hf.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ni.shxzskj.cn

[R61] 磁盘占用
来源：http://pi.huixiangedu.cn

df -h;  du -sh *
来源：http://fx.9csxet.cn

[R62] 找最占空间的文件
来源：http://hw.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://ry.szsharing.cn

[R63] 内存与进程
来源：http://bf.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://lr.newstarts.cn

[R64] 结束进程
来源：http://nm.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://mz.shxzskj.cn

[R65] 查看端口占用
来源：http://yf.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fb.wgjwhj.cn

[R66] 定时任务
来源：http://az.yuexingan06.cn

crontab -e;  crontab -l
来源：http://op.newstarts.cn

[R67] 生成随机十六进制串
来源：http://yc.huanxung.cn

openssl rand -hex 16
来源：http://up.shtwfgs.cn

[R68] 计算文件校验值
来源：http://oh.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cm.haigaiapp.cn

[R69] 生成随机密码
来源：http://fl.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://po.nszjky.cn

[R70] 时间戳与互转
来源：http://sz.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://dh.huixiangedu.cn

[R71] 日期格式化
来源：http://fd.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vg.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://yt.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cm.gzmigu.cn

[R73] 分割大日志
来源：http://qx.521024.cn

split -l 1000 big.log part_
来源：http://rf.haigaiapp.cn

[R74] 批量重命名
来源：http://eb.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://do.szxytkj.cn

[R75] 导出环境变量
来源：http://oo.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://zb.panjiajie.cn

[R76] 使用临时文件
来源：http://yv.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gi.chemitech.net.cn

[R77] 读取用户输入
来源：http://bp.shtwfgs.cn


<!-- 参考信息 -->