代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pi.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://et.asd995.cn

[Q35] 内连接
来源：http://gp.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lk.chemitech.net.cn

[Q36] 左连接
来源：http://il.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xy.shxzskj.cn

[Q37] 右连接
来源：http://tw.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bj.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vk.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bf.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://bs.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fq.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ee.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hm.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sc.bookmarksfly.cn

[Q41] 多表连接
来源：http://ul.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uj.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://wk.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://sh.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://zm.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://ef.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://np.bookmarksfly.cn

[Q43] 标量子查询
来源：http://tk.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ww.shxzskj.cn

[Q44] IN 子查询
来源：http://qf.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yn.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://ii.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tw.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://iu.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jy.szxytkj.cn

[Q47] 与平均值比较
来源：http://in.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ta.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://rb.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ag.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://rc.szsharing.cn

[Q49] 更新单行
来源：http://mw.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sd.huixinmuqiang.cn

[Q50] 批量更新
来源：http://ie.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pz.huixiangedu.cn

[Q51] 用子查询更新
来源：http://ia.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rw.gzmigu.cn

[Q52] 删除指定行
来源：http://vw.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://wv.wgjwhj.cn

[Q53] 按条件删除
来源：http://na.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yx.colortex.cn

[Q54] 清空表
来源：http://vf.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://uo.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://pk.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xe.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://iq.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ms.panjiajie.cn

[Q57] 行号
来源：http://ra.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://at.huanxung.cn

[Q58] 累计求和
来源：http://xg.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fe.haigaiapp.cn

[Q59] 分组内累计
来源：http://nu.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sb.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://md.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wj.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wo.9csxet.cn

[Q61] 移动平均
来源：http://zi.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ec.chemitech.net.cn

[Q62] 分组占比
来源：http://jd.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hp.yuntaijiaju.cn

[Q63] 开启事务
来源：http://nh.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qu.panjiajie.cn

[Q64] 提交事务
来源：http://uy.yuexingan06.cn

COMMIT;
来源：http://xo.shxzskj.cn

[Q65] 回滚事务
来源：http://kt.panjiajie.cn

ROLLBACK;
来源：http://dk.bjjhwx.cn

[Q66] 行锁查询
来源：http://ch.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tt.hnjuh.cn

[Q67] 设置隔离级别
来源：http://tz.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ww.gzmigu.cn

[Q68] 保存点
来源：http://fa.newstarts.cn

SAVEPOINT sp1;
来源：http://ow.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://qr.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://az.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iq.newstarts.cn

[Q70] 更新统计信息
来源：http://fy.muxihuayi.cn

ANALYZE TABLE users;
来源：http://ch.huixiangedu.cn

[Q71] 查看建表语句
来源：http://qa.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ql.yuexingan06.cn

[Q72] 查看索引
来源：http://tj.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://jg.muxihuayi.cn

[Q73] 查看表状态
来源：http://hj.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cz.chemitech.net.cn

[Q74] 强制使用索引
来源：http://bp.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zq.colortex.cn

[Q75] 日期格式化
来源：http://on.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://us.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mv.haigaiapp.cn

[Q76] 按天统计
来源：http://yg.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bg.gzmigu.cn

[Q77] 时间加减
来源：http://jo.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pv.9csxet.cn

[Q78] 当前时间
来源：http://qz.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bu.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://qf.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fr.hahajie.cn

[Q80] 字符串截取
来源：http://eg.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://av.huixiangedu.cn

[Q81] 字符串替换
来源：http://yf.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wj.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://cf.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ng.bookmarksfly.cn

[Q83] 大小写转换
来源：http://aa.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bj.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://eh.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://bz.panjiajie.cn

[Q85] 数值取整
来源：http://mr.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mr.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://tx.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yh.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://gr.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://af.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://ud.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://up.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kd.gzmigu.cn

[Q89] 判断表是否存在
来源：http://ox.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://um.hnjuh.cn

[Q90] 生成序号列
来源：http://zl.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pn.yuntaijiaju.cn

================================================================================
来源：http://sq.gzmigu.cn

R. Bash 专题
来源：http://xh.yuexingan06.cn

================================================================================
来源：http://ht.szsharing.cn

[R01] shebang 与严格模式
来源：http://xb.muxihuayi.cn

#!/usr/bin/env bash
来源：http://kr.9csxet.cn

set -euo pipefail
来源：http://wh.szsharing.cn

[R02] 变量赋值与使用
来源：http://fw.gzmigu.cn

name="Tom"; echo "$name"
来源：http://ie.chemitech.net.cn

[R03] 只读变量
来源：http://rg.huixiangedu.cn

readonly PI=3.14
来源：http://ao.huixinmuqiang.cn

[R04] 位置参数
来源：http://mn.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hr.panjiajie.cn

[R05] 参数默认值
来源：http://ox.shtwfgs.cn

name="${1:-default}"
来源：http://hc.hahajie.cn

[R06] 判断命令是否存在
来源：http://bm.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tz.jianghongdianzi.cn

[R07] if 判断文件
来源：http://ec.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pk.yuexingan06.cn

[R08] 数值比较
来源：http://wb.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xv.lnxyls.cn

[R09] 字符串比较
来源：http://zd.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jq.szxytkj.cn

[R10] 正则匹配
来源：http://hd.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uo.521024.cn

[R11] case 多分支
来源：http://hm.jctech888.com.cn

case "$1" in
来源：http://zp.colortex.cn

start) echo "启动" ;;
来源：http://nv.9csxet.cn

stop)  echo "停止" ;;
来源：http://ac.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://kd.wgjwhj.cn

esac
来源：http://ku.wgjwhj.cn

[R12] for 遍历文件
来源：http://fa.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://lj.jianghongdianzi.cn

[R13] for 计数循环
来源：http://ac.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://ky.wgjwhj.cn

[R14] C 风格 for
来源：http://pf.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yr.shxzskj.cn

[R15] while 逐行读文件
来源：http://lp.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ex.yuntaijiaju.cn

[R16] until 等待条件
来源：http://ql.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qm.shxzskj.cn

[R17] 数组定义与取值
来源：http://lf.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hm.lnxyls.cn

[R18] 遍历数组
来源：http://yh.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bm.asd995.cn

[R19] 数组长度
来源：http://an.newstarts.cn

echo "${#arr[@]}"
来源：http://ox.huanxung.cn

[R20] 关联数组（字典）
来源：http://bv.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nb.shtwfgs.cn

[R21] 字符串长度
来源：http://cp.bookmarksfly.cn

echo "${#s}"
来源：http://we.szxytkj.cn

[R22] 截取子串
来源：http://dn.newstarts.cn

echo "${s:0:5}"
来源：http://rj.gzmigu.cn

[R23] 字符串替换
来源：http://qh.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rv.muxihuayi.cn

[R24] 大小写转换
来源：http://eu.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xh.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://sk.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eb.asd995.cn

[R26] 命令替换
来源：http://rm.521024.cn

now=$(date +%F); echo "$now"
来源：http://ov.521024.cn

[R27] 算术展开
来源：http://ql.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://du.shtwfgs.cn

[R28] 浮点运算
来源：http://vb.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://nu.huixiangedu.cn

[R29] 定义函数
来源：http://vd.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yp.9csxet.cn

[R30] 函数返回状态码
来源：http://rm.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://qb.shtwfgs.cn

[R31] 局部变量
来源：http://be.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://jw.szsharing.cn

[R32] 参数个数校验
来源：http://fa.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ml.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://tr.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://al.newstarts.cn

[R34] 退出时清理
来源：http://uf.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zx.gzmigu.cn

[R35] 后台执行并等待
来源：http://oj.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wd.huanxung.cn

[R36] 并发执行多个任务
来源：http://kx.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cu.hnjuh.cn

[R37] 把输出赋给变量
来源：http://qp.shxzukj.cn

files=$(ls -1)
来源：http://xj.9csxet.cn

[R38] 管道串联
来源：http://pq.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://vr.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://ys.huanxung.cn

cmd > out.log 2>&1
来源：http://sa.nszjky.cn

[R40] 追加写日志
来源：http://fz.szsharing.cn

echo "log" >> out.log
来源：http://fx.yuexingan06.cn

[R41] 丢弃输出
来源：http://sn.asd995.cn

cmd >/dev/null 2>&1
来源：http://yz.colortex.cn

[R42] 输入重定向
来源：http://hw.bookmarksfly.cn

wc -l < a.txt
来源：http://lq.shtwfgs.cn

[R43] 按名字查找文件
来源：http://tq.521024.cn

find . -name "*.log" -type f
来源：http://kj.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://hd.asd995.cn

find . -mtime -7 -type f
来源：http://kk.szxytkj.cn

[R45] 批量删除
来源：http://js.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://qg.gzmigu.cn

[R46] 递归替换文件内容
来源：http://av.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qt.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://fb.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yb.szsharing.cn

[R48] awk 取指定列
来源：http://ve.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://ds.gzmigu.cn

[R49] awk 带条件
来源：http://ir.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bn.chemitech.net.cn

[R50] awk 求和
来源：http://vh.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vz.haigaiapp.cn

[R51] 排序去重取前几
来源：http://uu.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dd.chemitech.net.cn

[R52] 统计行数
来源：http://md.huixiangedu.cn

wc -l a.txt
来源：http://tk.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://nm.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mw.jctech888.com.cn

[R54] 比较两个文件
来源：http://qr.hahajie.cn

diff a.txt b.txt
来源：http://av.chemitech.net.cn

[R55] 压缩与解压
来源：http://qk.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gl.szsharing.cn

[R56] 远程拷贝
来源：http://xz.yuntaijiaju.cn

scp file user@host:/path/
来源：http://ov.bjjhwx.cn

[R57] 远程执行命令
来源：http://ey.shtwfgs.cn

ssh user@host 'uptime'
来源：http://sr.panjiajie.cn

[R58] 下载文件
来源：http://kx.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://im.jctech888.com.cn

[R59] 发 POST JSON
来源：http://fm.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ph.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://ji.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fm.bookmarksfly.cn

[R61] 磁盘占用
来源：http://ro.asd995.cn

df -h;  du -sh *
来源：http://ry.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://gl.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://hh.colortex.cn

[R63] 内存与进程
来源：http://bx.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://ll.jctech888.com.cn

[R64] 结束进程
来源：http://rq.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://ls.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://ac.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ej.shxzukj.cn

[R66] 定时任务
来源：http://zb.lnxyls.cn

crontab -e;  crontab -l
来源：http://oa.huanxung.cn

[R67] 生成随机十六进制串
来源：http://vj.bjjhwx.cn

openssl rand -hex 16
来源：http://eo.521024.cn

[R68] 计算文件校验值
来源：http://ch.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nh.hnjuh.cn

[R69] 生成随机密码
来源：http://ql.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://se.hnjuh.cn

[R70] 时间戳与互转
来源：http://it.huanxung.cn

date +%s;  date -d @1700000000
来源：http://ay.bookmarksfly.cn

[R71] 日期格式化
来源：http://of.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qn.shxzukj.cn

[R72] 等待端口就绪
来源：http://kq.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zu.shtwfgs.cn

[R73] 分割大日志
来源：http://kp.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://ek.huanxung.cn

[R74] 批量重命名
来源：http://ox.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ql.bjjhwx.cn

[R75] 导出环境变量
来源：http://pn.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://dv.hahajie.cn

[R76] 使用临时文件
来源：http://cw.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wf.shxzukj.cn

[R77] 读取用户输入
来源：http://ho.lnxyls.cn

read -rp "请输入: " ans
来源：http://gf.shxzukj.cn

[R78] 交互式菜单
来源：http://xt.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tu.shxzskj.cn

[R79] 解析命令行选项
来源：http://mh.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sk.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://ja.nicolike.cn

time ./run.sh
来源：http://xe.wgjwhj.cn

================================================================================
来源：http://fb.yuexingan06.cn

S. C / C++ 专题
来源：http://np.nicolike.cn

================================================================================
来源：http://ta.szsharing.cn

[S01] C：Hello World
来源：http://hr.muxihuayi.cn

#include <stdio.h>
来源：http://mv.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nw.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://xi.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://br.nszjky.cn

[S03] C：读入整数
来源：http://wx.muxihuayi.cn


<!-- 参考信息 -->