代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jm.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://uo.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cr.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hp.gzmigu.cn

[Q33] 多列分组
来源：http://ou.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wq.nszjky.cn

[Q34] 每组取第一条
来源：http://jh.bjjhwx.cn

SELECT * FROM (
来源：http://nr.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wl.huanxung.cn

) t WHERE rn = 1;
来源：http://zs.9csxet.cn

[Q35] 内连接
来源：http://sa.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ed.jctech888.com.cn

[Q36] 左连接
来源：http://zm.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aw.yuexingan06.cn

[Q37] 右连接
来源：http://rx.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mi.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gk.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pw.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://zo.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dm.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qv.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://se.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://um.szxytkj.cn

[Q41] 多表连接
来源：http://eb.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bd.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://cr.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://pt.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://ju.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://zc.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uz.huanxung.cn

[Q43] 标量子查询
来源：http://yl.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qn.hnjuh.cn

[Q44] IN 子查询
来源：http://al.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yi.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://al.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vp.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xf.wgjwhj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oq.lnxyls.cn

[Q47] 与平均值比较
来源：http://in.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vy.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://xu.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sq.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://pk.huanxung.cn

[Q49] 更新单行
来源：http://ma.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ty.shxzskj.cn

[Q50] 批量更新
来源：http://pc.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://af.shxzskj.cn

[Q51] 用子查询更新
来源：http://yr.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tt.9csxet.cn

[Q52] 删除指定行
来源：http://zi.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://qe.hnjuh.cn

[Q53] 按条件删除
来源：http://pv.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dq.jctech888.com.cn

[Q54] 清空表
来源：http://vk.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://lj.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://vd.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zf.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://dl.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://et.asd995.cn

[Q57] 行号
来源：http://nv.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xq.szxytkj.cn

[Q58] 累计求和
来源：http://vv.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wq.jctech888.com.cn

[Q59] 分组内累计
来源：http://gt.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qj.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://js.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://at.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yv.newstarts.cn

[Q61] 移动平均
来源：http://pj.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ab.yuexingan06.cn

[Q62] 分组占比
来源：http://uj.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eu.hnjuh.cn

[Q63] 开启事务
来源：http://nl.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uc.gzmigu.cn

[Q64] 提交事务
来源：http://uj.szxytkj.cn

COMMIT;
来源：http://qt.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://st.nicolike.cn

ROLLBACK;
来源：http://vt.haigaiapp.cn

[Q66] 行锁查询
来源：http://ix.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ur.shxzskj.cn

[Q67] 设置隔离级别
来源：http://zj.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ug.9csxet.cn

[Q68] 保存点
来源：http://bd.muxihuayi.cn

SAVEPOINT sp1;
来源：http://mj.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://np.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://vp.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tq.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://zf.9csxet.cn

ANALYZE TABLE users;
来源：http://we.jctech888.com.cn

[Q71] 查看建表语句
来源：http://ti.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bd.szxytkj.cn

[Q72] 查看索引
来源：http://rj.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://zj.bookmarksfly.cn

[Q73] 查看表状态
来源：http://nm.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vc.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://um.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://on.shxzukj.cn

[Q75] 日期格式化
来源：http://vv.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ly.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://om.chemitech.net.cn

[Q76] 按天统计
来源：http://on.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qn.wgjwhj.cn

[Q77] 时间加减
来源：http://ni.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zk.szxytkj.cn

[Q78] 当前时间
来源：http://oo.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eh.hnjuh.cn

[Q79] 字符串拼接
来源：http://fy.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://st.colortex.cn

[Q80] 字符串截取
来源：http://cu.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tf.szxytkj.cn

[Q81] 字符串替换
来源：http://xd.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://co.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://rg.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lp.nszjky.cn

[Q83] 大小写转换
来源：http://vi.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://so.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://dt.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://ad.nicolike.cn

[Q85] 数值取整
来源：http://dh.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tm.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://su.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lt.szsharing.cn

[Q87] JSON 字段做条件
来源：http://nq.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hw.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://yc.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bk.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tm.shxzskj.cn

[Q89] 判断表是否存在
来源：http://xq.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://af.wgjwhj.cn

[Q90] 生成序号列
来源：http://gq.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ya.szxytkj.cn

================================================================================
来源：http://hu.gzmigu.cn

R. Bash 专题
来源：http://by.szxytkj.cn

================================================================================
来源：http://xd.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://nq.9csxet.cn

#!/usr/bin/env bash
来源：http://rx.szxytkj.cn

set -euo pipefail
来源：http://va.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://yy.szsharing.cn

name="Tom"; echo "$name"
来源：http://qx.bookmarksfly.cn

[R03] 只读变量
来源：http://am.hnjuh.cn

readonly PI=3.14
来源：http://mi.yuntaijiaju.cn

[R04] 位置参数
来源：http://uj.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lb.shtwfgs.cn

[R05] 参数默认值
来源：http://lv.shtwfgs.cn

name="${1:-default}"
来源：http://pu.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://cc.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bh.jctech888.com.cn

[R07] if 判断文件
来源：http://op.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://os.huixinmuqiang.cn

[R08] 数值比较
来源：http://ic.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jl.bjjhwx.cn

[R09] 字符串比较
来源：http://tt.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rd.szsharing.cn

[R10] 正则匹配
来源：http://ft.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://at.9csxet.cn

[R11] case 多分支
来源：http://pw.jianghongdianzi.cn

case "$1" in
来源：http://zi.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://jj.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://os.gzmigu.cn

*)     echo "未知命令" ;;
来源：http://kv.shxzskj.cn

esac
来源：http://ey.gzmigu.cn

[R12] for 遍历文件
来源：http://cp.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://xm.jctech888.com.cn

[R13] for 计数循环
来源：http://qo.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://ls.hnjuh.cn

[R14] C 风格 for
来源：http://cy.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qx.asd995.cn

[R15] while 逐行读文件
来源：http://qa.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xh.shxzukj.cn

[R16] until 等待条件
来源：http://su.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ck.newstarts.cn

[R17] 数组定义与取值
来源：http://bz.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://md.huixinmuqiang.cn

[R18] 遍历数组
来源：http://iy.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://we.panjiajie.cn

[R19] 数组长度
来源：http://du.muxihuayi.cn

echo "${#arr[@]}"
来源：http://ia.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://uh.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oo.bjjhwx.cn

[R21] 字符串长度
来源：http://nk.bookmarksfly.cn

echo "${#s}"
来源：http://sw.bjjhwx.cn

[R22] 截取子串
来源：http://ag.shtwfgs.cn

echo "${s:0:5}"
来源：http://fn.lnxyls.cn

[R23] 字符串替换
来源：http://em.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wd.bookmarksfly.cn

[R24] 大小写转换
来源：http://zh.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jc.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://zm.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vj.chemitech.net.cn

[R26] 命令替换
来源：http://bh.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://fh.521024.cn

[R27] 算术展开
来源：http://ar.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://ei.hahajie.cn

[R28] 浮点运算
来源：http://as.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://xw.shtwfgs.cn

[R29] 定义函数
来源：http://fq.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ic.yuexingan06.cn

[R30] 函数返回状态码
来源：http://dd.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://eg.asd995.cn

[R31] 局部变量
来源：http://vb.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://ep.gzmigu.cn

[R32] 参数个数校验
来源：http://yq.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nb.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://ht.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oi.lnxyls.cn

[R34] 退出时清理
来源：http://cw.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://di.muxihuayi.cn

[R35] 后台执行并等待
来源：http://si.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wk.gzmigu.cn

[R36] 并发执行多个任务
来源：http://cc.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pv.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://qw.yuntaijiaju.cn

files=$(ls -1)
来源：http://jn.yuexingan06.cn

[R38] 管道串联
来源：http://no.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://gb.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://cn.nszjky.cn

cmd > out.log 2>&1
来源：http://jm.jianghongdianzi.cn

[R40] 追加写日志
来源：http://bv.nszjky.cn

echo "log" >> out.log
来源：http://kc.newstarts.cn

[R41] 丢弃输出
来源：http://yc.521024.cn

cmd >/dev/null 2>&1
来源：http://nw.yuexingan06.cn

[R42] 输入重定向
来源：http://bc.hnjuh.cn

wc -l < a.txt
来源：http://fv.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://si.hnjuh.cn

find . -name "*.log" -type f
来源：http://xw.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://qy.hnjuh.cn

find . -mtime -7 -type f
来源：http://zm.huanxung.cn

[R45] 批量删除
来源：http://pz.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://zp.shxzukj.cn

[R46] 递归替换文件内容
来源：http://tk.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hu.muxihuayi.cn

[R47] sed 单行替换
来源：http://om.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ro.huixiangedu.cn

[R48] awk 取指定列
来源：http://fv.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://hq.nicolike.cn

[R49] awk 带条件
来源：http://jn.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pn.nicolike.cn

[R50] awk 求和
来源：http://go.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ka.521024.cn

[R51] 排序去重取前几
来源：http://pw.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ua.jianghongdianzi.cn

[R52] 统计行数
来源：http://aj.chemitech.net.cn

wc -l a.txt
来源：http://fo.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://de.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://im.asd995.cn

[R54] 比较两个文件
来源：http://wx.szxytkj.cn

diff a.txt b.txt
来源：http://hr.jctech888.com.cn

[R55] 压缩与解压
来源：http://vv.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ik.hnjuh.cn

[R56] 远程拷贝
来源：http://hb.yuntaijiaju.cn

scp file user@host:/path/
来源：http://ab.haigaiapp.cn

[R57] 远程执行命令
来源：http://lc.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://wm.haigaiapp.cn

[R58] 下载文件
来源：http://ol.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ie.bjjhwx.cn

[R59] 发 POST JSON
来源：http://ka.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jd.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://ci.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://et.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://jz.asd995.cn

df -h;  du -sh *
来源：http://yv.asd995.cn

[R62] 找最占空间的文件
来源：http://jx.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://wg.szxytkj.cn

[R63] 内存与进程
来源：http://ua.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://nk.hahajie.cn

[R64] 结束进程
来源：http://ze.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://zb.nicolike.cn

[R65] 查看端口占用
来源：http://sd.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hd.colortex.cn

[R66] 定时任务
来源：http://mo.muxihuayi.cn

crontab -e;  crontab -l
来源：http://us.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://cd.wgjwhj.cn

openssl rand -hex 16
来源：http://ir.colortex.cn

[R68] 计算文件校验值
来源：http://rl.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fp.bjjhwx.cn

[R69] 生成随机密码
来源：http://tw.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://go.szsharing.cn

[R70] 时间戳与互转
来源：http://cg.nszjky.cn

date +%s;  date -d @1700000000
来源：http://ow.huixinmuqiang.cn

[R71] 日期格式化
来源：http://jn.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://az.bjjhwx.cn

[R72] 等待端口就绪
来源：http://tj.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uu.wgjwhj.cn

[R73] 分割大日志
来源：http://kv.shxzukj.cn

split -l 1000 big.log part_
来源：http://kn.colortex.cn

[R74] 批量重命名
来源：http://qg.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sb.huixiangedu.cn

[R75] 导出环境变量
来源：http://ko.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://xp.hnjuh.cn

[R76] 使用临时文件
来源：http://oa.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xs.panjiajie.cn

[R77] 读取用户输入
来源：http://jj.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://vi.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://go.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ox.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://nc.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zv.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://mo.asd995.cn

time ./run.sh
来源：http://oj.jctech888.com.cn

================================================================================
来源：http://vv.nicolike.cn


<!-- 参考信息 -->