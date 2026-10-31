代发 wailian999

[Q33] 多列分组
来源：http://yj.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mj.9csxet.cn

[Q34] 每组取第一条
来源：http://mf.huixinmuqiang.cn

SELECT * FROM (
来源：http://my.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ic.nicolike.cn

) t WHERE rn = 1;
来源：http://oo.huanxung.cn

[Q35] 内连接
来源：http://mw.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jh.muxihuayi.cn

[Q36] 左连接
来源：http://dh.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://we.bookmarksfly.cn

[Q37] 右连接
来源：http://wq.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wd.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yy.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cj.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://wh.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rg.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fm.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wb.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sz.chemitech.net.cn

[Q41] 多表连接
来源：http://lm.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qy.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://vj.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://jr.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://gf.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://np.chemitech.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cu.9csxet.cn

[Q43] 标量子查询
来源：http://ch.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wo.szsharing.cn

[Q44] IN 子查询
来源：http://ts.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://co.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://wf.yuexingan06.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://co.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yd.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://il.chemitech.net.cn

[Q47] 与平均值比较
来源：http://wq.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lt.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://yb.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mp.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://od.yuexingan06.cn

[Q49] 更新单行
来源：http://wb.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zl.lnxyls.cn

[Q50] 批量更新
来源：http://dd.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vo.szsharing.cn

[Q51] 用子查询更新
来源：http://cz.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ut.hnjuh.cn

[Q52] 删除指定行
来源：http://va.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://hz.szxytkj.cn

[Q53] 按条件删除
来源：http://bd.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://st.jianghongdianzi.cn

[Q54] 清空表
来源：http://lp.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://iy.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://ar.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qn.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://ht.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mi.haigaiapp.cn

[Q57] 行号
来源：http://ca.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mo.szsharing.cn

[Q58] 累计求和
来源：http://zr.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sg.bjjhwx.cn

[Q59] 分组内累计
来源：http://mv.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ts.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://hx.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kz.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rq.hnjuh.cn

[Q61] 移动平均
来源：http://tq.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ef.szsharing.cn

[Q62] 分组占比
来源：http://ds.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://po.huanxung.cn

[Q63] 开启事务
来源：http://nf.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wz.nszjky.cn

[Q64] 提交事务
来源：http://db.jianghongdianzi.cn

COMMIT;
来源：http://hx.shxzukj.cn

[Q65] 回滚事务
来源：http://re.jianghongdianzi.cn

ROLLBACK;
来源：http://ln.hnjuh.cn

[Q66] 行锁查询
来源：http://eh.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pg.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://dm.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ww.chemitech.net.cn

[Q68] 保存点
来源：http://py.bjjhwx.cn

SAVEPOINT sp1;
来源：http://ay.colortex.cn

ROLLBACK TO sp1;
来源：http://ug.lnxyls.cn

[Q69] 查看执行计划
来源：http://ca.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jq.colortex.cn

[Q70] 更新统计信息
来源：http://nv.panjiajie.cn

ANALYZE TABLE users;
来源：http://ec.newstarts.cn

[Q71] 查看建表语句
来源：http://xw.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xz.chemitech.net.cn

[Q72] 查看索引
来源：http://ez.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://iy.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://ou.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zs.shtwfgs.cn

[Q74] 强制使用索引
来源：http://ej.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kk.newstarts.cn

[Q75] 日期格式化
来源：http://hv.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cs.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dm.haigaiapp.cn

[Q76] 按天统计
来源：http://kz.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ww.muxihuayi.cn

[Q77] 时间加减
来源：http://dp.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fp.9csxet.cn

[Q78] 当前时间
来源：http://kg.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ou.haigaiapp.cn

[Q79] 字符串拼接
来源：http://jj.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lo.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://xn.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ey.szxytkj.cn

[Q81] 字符串替换
来源：http://ge.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mk.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://eq.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fh.panjiajie.cn

[Q83] 大小写转换
来源：http://ut.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xg.szxytkj.cn

[Q84] 去除首尾空格
来源：http://ub.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://wg.521024.cn

[Q85] 数值取整
来源：http://zc.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xn.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://xj.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yp.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://cx.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ln.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://px.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fe.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gg.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://de.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ju.colortex.cn

[Q90] 生成序号列
来源：http://gs.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dq.huanxung.cn

================================================================================
来源：http://ed.panjiajie.cn

R. Bash 专题
来源：http://mw.jctech888.com.cn

================================================================================
来源：http://iy.nicolike.cn

[R01] shebang 与严格模式
来源：http://as.yuexingan06.cn

#!/usr/bin/env bash
来源：http://fa.jianghongdianzi.cn

set -euo pipefail
来源：http://gp.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://iq.shxzukj.cn

name="Tom"; echo "$name"
来源：http://ku.gzmigu.cn

[R03] 只读变量
来源：http://yb.newstarts.cn

readonly PI=3.14
来源：http://hs.shxzskj.cn

[R04] 位置参数
来源：http://mh.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qn.muxihuayi.cn

[R05] 参数默认值
来源：http://nc.shxzukj.cn

name="${1:-default}"
来源：http://lf.521024.cn

[R06] 判断命令是否存在
来源：http://ef.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ah.asd995.cn

[R07] if 判断文件
来源：http://bh.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ff.bookmarksfly.cn

[R08] 数值比较
来源：http://hd.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iq.bookmarksfly.cn

[R09] 字符串比较
来源：http://zy.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aj.hahajie.cn

[R10] 正则匹配
来源：http://sp.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xu.bjjhwx.cn

[R11] case 多分支
来源：http://ij.lnxyls.cn

case "$1" in
来源：http://qd.huanxung.cn

start) echo "启动" ;;
来源：http://pf.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://ux.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://lt.jctech888.com.cn

esac
来源：http://ta.wgjwhj.cn

[R12] for 遍历文件
来源：http://es.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://hc.jianghongdianzi.cn

[R13] for 计数循环
来源：http://tu.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://uq.yuntaijiaju.cn

[R14] C 风格 for
来源：http://hm.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gz.wgjwhj.cn

[R15] while 逐行读文件
来源：http://fb.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lc.nicolike.cn

[R16] until 等待条件
来源：http://yd.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ov.shtwfgs.cn

[R17] 数组定义与取值
来源：http://vf.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://go.jianghongdianzi.cn

[R18] 遍历数组
来源：http://ch.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fz.nszjky.cn

[R19] 数组长度
来源：http://dm.muxihuayi.cn

echo "${#arr[@]}"
来源：http://sc.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://ag.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ab.gzmigu.cn

[R21] 字符串长度
来源：http://yr.lnxyls.cn

echo "${#s}"
来源：http://uj.haigaiapp.cn

[R22] 截取子串
来源：http://ew.9csxet.cn

echo "${s:0:5}"
来源：http://ph.shxzukj.cn

[R23] 字符串替换
来源：http://ih.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zb.bjjhwx.cn

[R24] 大小写转换
来源：http://pv.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yx.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://ua.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kh.nicolike.cn

[R26] 命令替换
来源：http://gb.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://tl.shxzskj.cn

[R27] 算术展开
来源：http://wb.szsharing.cn

echo $((1 + 2 * 3))
来源：http://vg.lnxyls.cn

[R28] 浮点运算
来源：http://uf.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://gp.muxihuayi.cn

[R29] 定义函数
来源：http://mu.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pt.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://sd.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://bg.nicolike.cn

[R31] 局部变量
来源：http://jl.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://sn.muxihuayi.cn

[R32] 参数个数校验
来源：http://wp.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://el.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://ux.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pv.hnjuh.cn

[R34] 退出时清理
来源：http://vn.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ig.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://wg.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ns.asd995.cn

[R36] 并发执行多个任务
来源：http://ci.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ro.newstarts.cn

[R37] 把输出赋给变量
来源：http://vx.jctech888.com.cn

files=$(ls -1)
来源：http://ej.shtwfgs.cn

[R38] 管道串联
来源：http://it.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://lt.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://ib.colortex.cn

cmd > out.log 2>&1
来源：http://gl.chemitech.net.cn

[R40] 追加写日志
来源：http://br.jianghongdianzi.cn

echo "log" >> out.log
来源：http://ma.huixiangedu.cn

[R41] 丢弃输出
来源：http://cu.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://jc.nszjky.cn

[R42] 输入重定向
来源：http://fr.shxzukj.cn

wc -l < a.txt
来源：http://bx.newstarts.cn

[R43] 按名字查找文件
来源：http://iy.szsharing.cn

find . -name "*.log" -type f
来源：http://ci.huixiangedu.cn

[R44] 按修改时间查找
来源：http://jj.521024.cn

find . -mtime -7 -type f
来源：http://ew.shxzskj.cn

[R45] 批量删除
来源：http://rs.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://if.gzmigu.cn

[R46] 递归替换文件内容
来源：http://ye.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qv.gzmigu.cn

[R47] sed 单行替换
来源：http://dd.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xt.gzmigu.cn

[R48] awk 取指定列
来源：http://dq.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://yj.shxzskj.cn

[R49] awk 带条件
来源：http://vz.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://al.colortex.cn

[R50] awk 求和
来源：http://wo.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ws.muxihuayi.cn

[R51] 排序去重取前几
来源：http://cw.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://js.szxytkj.cn

[R52] 统计行数
来源：http://hf.huixinmuqiang.cn

wc -l a.txt
来源：http://vc.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://ob.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ba.nszjky.cn

[R54] 比较两个文件
来源：http://av.huixiangedu.cn

diff a.txt b.txt
来源：http://um.huanxung.cn

[R55] 压缩与解压
来源：http://mt.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gq.huixiangedu.cn

[R56] 远程拷贝
来源：http://un.hahajie.cn

scp file user@host:/path/
来源：http://lg.gzmigu.cn

[R57] 远程执行命令
来源：http://rb.colortex.cn

ssh user@host 'uptime'
来源：http://zq.hnjuh.cn

[R58] 下载文件
来源：http://xj.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vj.muxihuayi.cn

[R59] 发 POST JSON
来源：http://rn.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kg.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://xm.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yn.wgjwhj.cn

[R61] 磁盘占用
来源：http://xg.shxzukj.cn

df -h;  du -sh *
来源：http://om.9csxet.cn

[R62] 找最占空间的文件
来源：http://ep.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://is.hahajie.cn

[R63] 内存与进程
来源：http://ei.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://rx.jianghongdianzi.cn

[R64] 结束进程
来源：http://pt.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://cr.hahajie.cn

[R65] 查看端口占用
来源：http://xj.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nw.lnxyls.cn

[R66] 定时任务
来源：http://jg.nszjky.cn

crontab -e;  crontab -l
来源：http://tu.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://do.jianghongdianzi.cn

openssl rand -hex 16
来源：http://iw.nicolike.cn

[R68] 计算文件校验值
来源：http://cc.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vp.huixiangedu.cn

[R69] 生成随机密码
来源：http://ns.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://bv.hahajie.cn

[R70] 时间戳与互转
来源：http://df.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://jy.shtwfgs.cn

[R71] 日期格式化
来源：http://vk.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://or.hahajie.cn

[R72] 等待端口就绪
来源：http://tk.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pv.nicolike.cn

[R73] 分割大日志
来源：http://db.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://ib.jianghongdianzi.cn

[R74] 批量重命名
来源：http://uu.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yu.gzmigu.cn

[R75] 导出环境变量
来源：http://pw.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://gt.nszjky.cn

[R76] 使用临时文件
来源：http://mi.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://km.panjiajie.cn

[R77] 读取用户输入
来源：http://me.nicolike.cn

read -rp "请输入: " ans
来源：http://wu.yuexingan06.cn

[R78] 交互式菜单
来源：http://wq.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sh.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://gn.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tc.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://gc.yuntaijiaju.cn

time ./run.sh
来源：http://pp.jianghongdianzi.cn

================================================================================
来源：http://cj.yuexingan06.cn

S. C / C++ 专题
来源：http://ds.muxihuayi.cn

================================================================================
来源：http://qq.jctech888.com.cn

[S01] C：Hello World
来源：http://yf.newstarts.cn

#include <stdio.h>
来源：http://ks.hnjuh.cn


<!-- 参考信息 -->