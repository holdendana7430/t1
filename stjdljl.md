代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fn.asd995.cn

) t WHERE rn = 1;
来源：http://gz.muxihuayi.cn

[Q35] 内连接
来源：http://pf.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vl.shxzukj.cn

[Q36] 左连接
来源：http://hm.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yn.jctech888.com.cn

[Q37] 右连接
来源：http://zi.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yo.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://aj.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cg.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://ol.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oz.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xd.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rr.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sa.szxytkj.cn

[Q41] 多表连接
来源：http://as.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yb.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://nw.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://si.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://yb.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://is.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vb.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://gp.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nf.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://kc.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sp.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://lj.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kv.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sb.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ux.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://wt.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tg.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://ir.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cb.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://tk.szxytkj.cn

[Q49] 更新单行
来源：http://fu.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tq.shtwfgs.cn

[Q50] 批量更新
来源：http://nk.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xr.haigaiapp.cn

[Q51] 用子查询更新
来源：http://ae.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ws.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://iy.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://hg.jctech888.com.cn

[Q53] 按条件删除
来源：http://bz.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dl.muxihuayi.cn

[Q54] 清空表
来源：http://mw.colortex.cn

TRUNCATE TABLE logs;
来源：http://pp.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://rd.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cq.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://zl.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ga.shxzukj.cn

[Q57] 行号
来源：http://pc.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kl.shxzskj.cn

[Q58] 累计求和
来源：http://cn.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gs.nicolike.cn

[Q59] 分组内累计
来源：http://dk.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gk.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://wv.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qk.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wq.huanxung.cn

[Q61] 移动平均
来源：http://az.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pb.521024.cn

[Q62] 分组占比
来源：http://ld.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wc.shtwfgs.cn

[Q63] 开启事务
来源：http://wb.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ev.hnjuh.cn

[Q64] 提交事务
来源：http://rb.yuexingan06.cn

COMMIT;
来源：http://jl.hnjuh.cn

[Q65] 回滚事务
来源：http://oi.gzmigu.cn

ROLLBACK;
来源：http://zo.yuexingan06.cn

[Q66] 行锁查询
来源：http://go.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nf.gzmigu.cn

[Q67] 设置隔离级别
来源：http://ig.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ry.muxihuayi.cn

[Q68] 保存点
来源：http://ej.521024.cn

SAVEPOINT sp1;
来源：http://oa.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://ln.huanxung.cn

[Q69] 查看执行计划
来源：http://ni.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pt.bjjhwx.cn

[Q70] 更新统计信息
来源：http://at.nszjky.cn

ANALYZE TABLE users;
来源：http://jr.wgjwhj.cn

[Q71] 查看建表语句
来源：http://vi.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oc.szsharing.cn

[Q72] 查看索引
来源：http://or.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://cl.szxytkj.cn

[Q73] 查看表状态
来源：http://bb.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hw.gzmigu.cn

[Q74] 强制使用索引
来源：http://be.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wu.jctech888.com.cn

[Q75] 日期格式化
来源：http://fa.szsharing.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lo.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bg.9csxet.cn

[Q76] 按天统计
来源：http://ru.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ej.9csxet.cn

[Q77] 时间加减
来源：http://nv.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xx.hahajie.cn

[Q78] 当前时间
来源：http://zq.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://se.panjiajie.cn

[Q79] 字符串拼接
来源：http://kh.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lw.asd995.cn

[Q80] 字符串截取
来源：http://el.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uw.jctech888.com.cn

[Q81] 字符串替换
来源：http://yx.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ux.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://nf.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dp.yuexingan06.cn

[Q83] 大小写转换
来源：http://pp.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wj.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://zy.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://cs.chemitech.net.cn

[Q85] 数值取整
来源：http://bt.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rr.colortex.cn

[Q86] 读取 JSON 字段
来源：http://bb.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uq.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://la.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qn.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://xq.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pn.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yj.szsharing.cn

[Q89] 判断表是否存在
来源：http://dn.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ns.huanxung.cn

[Q90] 生成序号列
来源：http://em.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qx.panjiajie.cn

================================================================================
来源：http://ve.nszjky.cn

R. Bash 专题
来源：http://ml.huixiangedu.cn

================================================================================
来源：http://vl.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://nq.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://wa.yuntaijiaju.cn

set -euo pipefail
来源：http://nd.hnjuh.cn

[R02] 变量赋值与使用
来源：http://so.521024.cn

name="Tom"; echo "$name"
来源：http://ck.chemitech.net.cn

[R03] 只读变量
来源：http://dj.bjjhwx.cn

readonly PI=3.14
来源：http://hk.muxihuayi.cn

[R04] 位置参数
来源：http://ho.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ix.colortex.cn

[R05] 参数默认值
来源：http://yh.hahajie.cn

name="${1:-default}"
来源：http://eq.panjiajie.cn

[R06] 判断命令是否存在
来源：http://uz.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ob.huixiangedu.cn

[R07] if 判断文件
来源：http://xz.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lm.newstarts.cn

[R08] 数值比较
来源：http://sk.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kl.chemitech.net.cn

[R09] 字符串比较
来源：http://mn.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vm.yuexingan06.cn

[R10] 正则匹配
来源：http://pr.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rp.wgjwhj.cn

[R11] case 多分支
来源：http://fu.bookmarksfly.cn

case "$1" in
来源：http://ol.szxytkj.cn

start) echo "启动" ;;
来源：http://qa.gzmigu.cn

stop)  echo "停止" ;;
来源：http://mc.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://lj.jianghongdianzi.cn

esac
来源：http://uy.bjjhwx.cn

[R12] for 遍历文件
来源：http://ys.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://ne.shxzskj.cn

[R13] for 计数循环
来源：http://pg.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://hc.wgjwhj.cn

[R14] C 风格 for
来源：http://uq.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gg.hnjuh.cn

[R15] while 逐行读文件
来源：http://xr.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ll.szsharing.cn

[R16] until 等待条件
来源：http://mv.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://na.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://mn.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ig.bookmarksfly.cn

[R18] 遍历数组
来源：http://rt.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ur.chemitech.net.cn

[R19] 数组长度
来源：http://od.gzmigu.cn

echo "${#arr[@]}"
来源：http://tm.szsharing.cn

[R20] 关联数组（字典）
来源：http://ii.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aw.nicolike.cn

[R21] 字符串长度
来源：http://tk.chemitech.net.cn

echo "${#s}"
来源：http://km.shxzukj.cn

[R22] 截取子串
来源：http://ec.bjjhwx.cn

echo "${s:0:5}"
来源：http://se.huixiangedu.cn

[R23] 字符串替换
来源：http://yv.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kk.hahajie.cn

[R24] 大小写转换
来源：http://vy.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dw.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://to.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mm.yuexingan06.cn

[R26] 命令替换
来源：http://ax.521024.cn

now=$(date +%F); echo "$now"
来源：http://kk.yuntaijiaju.cn

[R27] 算术展开
来源：http://ys.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://ks.huixinmuqiang.cn

[R28] 浮点运算
来源：http://vi.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://wf.wgjwhj.cn

[R29] 定义函数
来源：http://sq.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lm.lnxyls.cn

[R30] 函数返回状态码
来源：http://cr.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://ya.newstarts.cn

[R31] 局部变量
来源：http://by.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://bw.haigaiapp.cn

[R32] 参数个数校验
来源：http://hr.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zz.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://lh.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lt.huixinmuqiang.cn

[R34] 退出时清理
来源：http://ah.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://og.huixiangedu.cn

[R35] 后台执行并等待
来源：http://ht.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://em.9csxet.cn

[R36] 并发执行多个任务
来源：http://ol.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jw.nicolike.cn

[R37] 把输出赋给变量
来源：http://xs.jianghongdianzi.cn

files=$(ls -1)
来源：http://lh.jianghongdianzi.cn

[R38] 管道串联
来源：http://iy.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://si.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://al.nszjky.cn

cmd > out.log 2>&1
来源：http://yl.gzmigu.cn

[R40] 追加写日志
来源：http://kx.9csxet.cn

echo "log" >> out.log
来源：http://lg.muxihuayi.cn

[R41] 丢弃输出
来源：http://bq.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://kl.shtwfgs.cn

[R42] 输入重定向
来源：http://uf.huixiangedu.cn

wc -l < a.txt
来源：http://gb.9csxet.cn

[R43] 按名字查找文件
来源：http://qh.asd995.cn

find . -name "*.log" -type f
来源：http://cy.shxzskj.cn

[R44] 按修改时间查找
来源：http://yc.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://ar.hahajie.cn

[R45] 批量删除
来源：http://cs.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://cm.shxzukj.cn

[R46] 递归替换文件内容
来源：http://vm.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ut.wgjwhj.cn

[R47] sed 单行替换
来源：http://ly.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://iu.huanxung.cn

[R48] awk 取指定列
来源：http://rv.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://zz.haigaiapp.cn

[R49] awk 带条件
来源：http://cb.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sb.colortex.cn

[R50] awk 求和
来源：http://cm.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ve.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://yh.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ui.jianghongdianzi.cn

[R52] 统计行数
来源：http://gj.yuexingan06.cn

wc -l a.txt
来源：http://ks.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://db.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mr.colortex.cn

[R54] 比较两个文件
来源：http://du.bjjhwx.cn

diff a.txt b.txt
来源：http://ju.bjjhwx.cn

[R55] 压缩与解压
来源：http://gw.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nq.bookmarksfly.cn

[R56] 远程拷贝
来源：http://ri.hahajie.cn

scp file user@host:/path/
来源：http://mc.panjiajie.cn

[R57] 远程执行命令
来源：http://lb.wgjwhj.cn

ssh user@host 'uptime'
来源：http://ht.bookmarksfly.cn

[R58] 下载文件
来源：http://ee.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ly.hahajie.cn

[R59] 发 POST JSON
来源：http://zo.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wa.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://rf.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jx.colortex.cn

[R61] 磁盘占用
来源：http://fp.nszjky.cn

df -h;  du -sh *
来源：http://sw.colortex.cn

[R62] 找最占空间的文件
来源：http://bh.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://hf.huixiangedu.cn

[R63] 内存与进程
来源：http://sx.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://pv.gzmigu.cn

[R64] 结束进程
来源：http://qm.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://ww.521024.cn

[R65] 查看端口占用
来源：http://ug.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wc.bookmarksfly.cn

[R66] 定时任务
来源：http://xu.hahajie.cn

crontab -e;  crontab -l
来源：http://at.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://qa.huanxung.cn

openssl rand -hex 16
来源：http://bi.newstarts.cn

[R68] 计算文件校验值
来源：http://xx.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bm.jctech888.com.cn

[R69] 生成随机密码
来源：http://oa.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://ln.asd995.cn

[R70] 时间戳与互转
来源：http://bs.9csxet.cn

date +%s;  date -d @1700000000
来源：http://ut.521024.cn

[R71] 日期格式化
来源：http://lw.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ut.szsharing.cn

[R72] 等待端口就绪
来源：http://dp.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lp.hnjuh.cn

[R73] 分割大日志
来源：http://na.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://zu.521024.cn

[R74] 批量重命名
来源：http://ox.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://el.haigaiapp.cn

[R75] 导出环境变量
来源：http://xy.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://ug.nszjky.cn

[R76] 使用临时文件
来源：http://be.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jc.nicolike.cn

[R77] 读取用户输入
来源：http://ue.szxytkj.cn

read -rp "请输入: " ans
来源：http://zl.hnjuh.cn

[R78] 交互式菜单
来源：http://od.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pi.panjiajie.cn

[R79] 解析命令行选项
来源：http://xc.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ub.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://gk.szsharing.cn

time ./run.sh
来源：http://ab.wgjwhj.cn

================================================================================
来源：http://za.gzmigu.cn

S. C / C++ 专题
来源：http://vi.nszjky.cn

================================================================================
来源：http://uu.shtwfgs.cn

[S01] C：Hello World
来源：http://ho.jctech888.com.cn

#include <stdio.h>
来源：http://kz.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pk.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://uh.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://jz.9csxet.cn

[S03] C：读入整数
来源：http://jm.shxzukj.cn


<!-- 参考信息 -->