代发 wailian999

[Q33] 多列分组
来源：http://zi.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fu.chemitech.net.cn

[Q34] 每组取第一条
来源：http://ee.haigaiapp.cn

SELECT * FROM (
来源：http://uw.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rv.huixiangedu.cn

) t WHERE rn = 1;
来源：http://uy.colortex.cn

[Q35] 内连接
来源：http://pt.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lc.521024.cn

[Q36] 左连接
来源：http://jf.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ie.panjiajie.cn

[Q37] 右连接
来源：http://dn.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pv.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://id.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ic.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://pt.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gk.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fk.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qt.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fh.newstarts.cn

[Q41] 多表连接
来源：http://hi.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vo.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://yo.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://as.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://un.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://qo.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cm.nicolike.cn

[Q43] 标量子查询
来源：http://qs.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ft.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://xz.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vh.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://tn.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tq.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://co.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wd.haigaiapp.cn

[Q47] 与平均值比较
来源：http://tj.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fg.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://yu.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gj.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://uj.9csxet.cn

[Q49] 更新单行
来源：http://gh.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nb.jctech888.com.cn

[Q50] 批量更新
来源：http://xn.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jf.szxytkj.cn

[Q51] 用子查询更新
来源：http://vy.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gd.nszjky.cn

[Q52] 删除指定行
来源：http://ac.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://vz.hnjuh.cn

[Q53] 按条件删除
来源：http://fz.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wa.hahajie.cn

[Q54] 清空表
来源：http://rp.asd995.cn

TRUNCATE TABLE logs;
来源：http://un.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://ih.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qw.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://jf.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sz.nicolike.cn

[Q57] 行号
来源：http://bx.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rf.nszjky.cn

[Q58] 累计求和
来源：http://sw.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lw.wgjwhj.cn

[Q59] 分组内累计
来源：http://xu.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ay.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://xx.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bx.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ud.huanxung.cn

[Q61] 移动平均
来源：http://vu.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fa.huixiangedu.cn

[Q62] 分组占比
来源：http://my.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dq.haigaiapp.cn

[Q63] 开启事务
来源：http://js.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nm.hahajie.cn

[Q64] 提交事务
来源：http://la.bjjhwx.cn

COMMIT;
来源：http://tq.huanxung.cn

[Q65] 回滚事务
来源：http://if.panjiajie.cn

ROLLBACK;
来源：http://tr.hnjuh.cn

[Q66] 行锁查询
来源：http://ge.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ro.asd995.cn

[Q67] 设置隔离级别
来源：http://ok.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qk.haigaiapp.cn

[Q68] 保存点
来源：http://ya.nicolike.cn

SAVEPOINT sp1;
来源：http://lq.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://wv.szxytkj.cn

[Q69] 查看执行计划
来源：http://gr.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cv.hnjuh.cn

[Q70] 更新统计信息
来源：http://ah.newstarts.cn

ANALYZE TABLE users;
来源：http://zs.9csxet.cn

[Q71] 查看建表语句
来源：http://kk.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://do.yuexingan06.cn

[Q72] 查看索引
来源：http://bn.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://pv.jctech888.com.cn

[Q73] 查看表状态
来源：http://nv.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cl.bjjhwx.cn

[Q74] 强制使用索引
来源：http://an.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ye.colortex.cn

[Q75] 日期格式化
来源：http://pp.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vj.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aq.bookmarksfly.cn

[Q76] 按天统计
来源：http://zl.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ec.nicolike.cn

[Q77] 时间加减
来源：http://ju.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cp.huixinmuqiang.cn

[Q78] 当前时间
来源：http://yb.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ng.asd995.cn

[Q79] 字符串拼接
来源：http://ik.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qx.shxzukj.cn

[Q80] 字符串截取
来源：http://rw.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lx.colortex.cn

[Q81] 字符串替换
来源：http://su.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bt.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://rd.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nt.bookmarksfly.cn

[Q83] 大小写转换
来源：http://fg.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lm.szxytkj.cn

[Q84] 去除首尾空格
来源：http://ya.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://dm.colortex.cn

[Q85] 数值取整
来源：http://pq.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://em.521024.cn

[Q86] 读取 JSON 字段
来源：http://pt.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dk.nszjky.cn

[Q87] JSON 字段做条件
来源：http://wg.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hk.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://nt.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ku.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lz.nszjky.cn

[Q89] 判断表是否存在
来源：http://ef.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jg.shtwfgs.cn

[Q90] 生成序号列
来源：http://wx.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jh.shxzukj.cn

================================================================================
来源：http://cp.shxzskj.cn

R. Bash 专题
来源：http://yu.nszjky.cn

================================================================================
来源：http://fx.hnjuh.cn

[R01] shebang 与严格模式
来源：http://lt.yuexingan06.cn

#!/usr/bin/env bash
来源：http://nm.yuntaijiaju.cn

set -euo pipefail
来源：http://xa.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://mw.hahajie.cn

name="Tom"; echo "$name"
来源：http://mh.521024.cn

[R03] 只读变量
来源：http://xz.521024.cn

readonly PI=3.14
来源：http://zr.hahajie.cn

[R04] 位置参数
来源：http://cm.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ej.newstarts.cn

[R05] 参数默认值
来源：http://bq.newstarts.cn

name="${1:-default}"
来源：http://hs.nicolike.cn

[R06] 判断命令是否存在
来源：http://vb.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hk.panjiajie.cn

[R07] if 判断文件
来源：http://xm.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bj.shxzukj.cn

[R08] 数值比较
来源：http://ia.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://io.bookmarksfly.cn

[R09] 字符串比较
来源：http://er.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://or.yuntaijiaju.cn

[R10] 正则匹配
来源：http://he.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ea.lnxyls.cn

[R11] case 多分支
来源：http://dz.shxzukj.cn

case "$1" in
来源：http://dm.nszjky.cn

start) echo "启动" ;;
来源：http://yg.gzmigu.cn

stop)  echo "停止" ;;
来源：http://bv.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://ko.huixinmuqiang.cn

esac
来源：http://ch.chemitech.net.cn

[R12] for 遍历文件
来源：http://mu.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://fd.wgjwhj.cn

[R13] for 计数循环
来源：http://rc.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://mn.muxihuayi.cn

[R14] C 风格 for
来源：http://yd.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rq.panjiajie.cn

[R15] while 逐行读文件
来源：http://hb.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ey.nszjky.cn

[R16] until 等待条件
来源：http://rs.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mo.hnjuh.cn

[R17] 数组定义与取值
来源：http://yl.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pv.szxytkj.cn

[R18] 遍历数组
来源：http://al.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aj.yuntaijiaju.cn

[R19] 数组长度
来源：http://ri.huixiangedu.cn

echo "${#arr[@]}"
来源：http://ii.shxzukj.cn

[R20] 关联数组（字典）
来源：http://sr.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sc.nicolike.cn

[R21] 字符串长度
来源：http://ii.521024.cn

echo "${#s}"
来源：http://kw.haigaiapp.cn

[R22] 截取子串
来源：http://ey.bookmarksfly.cn

echo "${s:0:5}"
来源：http://yr.shxzskj.cn

[R23] 字符串替换
来源：http://es.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ge.nicolike.cn

[R24] 大小写转换
来源：http://ih.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rv.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://ja.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sj.szxytkj.cn

[R26] 命令替换
来源：http://hc.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://ve.chemitech.net.cn

[R27] 算术展开
来源：http://ox.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://df.newstarts.cn

[R28] 浮点运算
来源：http://nk.521024.cn

echo "scale=2; 10/3" | bc
来源：http://bc.chemitech.net.cn

[R29] 定义函数
来源：http://tw.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ag.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://vi.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://wd.shxzukj.cn

[R31] 局部变量
来源：http://dt.521024.cn

f() { local x=1; echo "$x"; }
来源：http://iu.shxzukj.cn

[R32] 参数个数校验
来源：http://ko.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xa.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://lx.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gg.521024.cn

[R34] 退出时清理
来源：http://jy.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wq.wgjwhj.cn

[R35] 后台执行并等待
来源：http://aq.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://la.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://ab.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vd.hnjuh.cn

[R37] 把输出赋给变量
来源：http://af.huanxung.cn

files=$(ls -1)
来源：http://nb.nicolike.cn

[R38] 管道串联
来源：http://po.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://nd.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://by.gzmigu.cn

cmd > out.log 2>&1
来源：http://dx.chemitech.net.cn

[R40] 追加写日志
来源：http://qv.huanxung.cn

echo "log" >> out.log
来源：http://zx.huixiangedu.cn

[R41] 丢弃输出
来源：http://cd.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://jr.huixiangedu.cn

[R42] 输入重定向
来源：http://hv.521024.cn

wc -l < a.txt
来源：http://mw.szxytkj.cn

[R43] 按名字查找文件
来源：http://zl.shxzukj.cn

find . -name "*.log" -type f
来源：http://fn.wgjwhj.cn

[R44] 按修改时间查找
来源：http://uz.bjjhwx.cn

find . -mtime -7 -type f
来源：http://gs.gzmigu.cn

[R45] 批量删除
来源：http://ob.hahajie.cn

find . -name "*.tmp" -delete
来源：http://ni.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://ac.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rt.colortex.cn

[R47] sed 单行替换
来源：http://jq.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jf.bjjhwx.cn

[R48] awk 取指定列
来源：http://ba.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://jx.haigaiapp.cn

[R49] awk 带条件
来源：http://rf.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xb.shxzskj.cn

[R50] awk 求和
来源：http://bi.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ob.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://gu.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pv.shxzukj.cn

[R52] 统计行数
来源：http://tw.shtwfgs.cn

wc -l a.txt
来源：http://vg.521024.cn

[R53] 查看文件头与实时尾
来源：http://ww.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vz.shxzukj.cn

[R54] 比较两个文件
来源：http://hl.haigaiapp.cn

diff a.txt b.txt
来源：http://fk.bjjhwx.cn

[R55] 压缩与解压
来源：http://le.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zr.panjiajie.cn

[R56] 远程拷贝
来源：http://ax.9csxet.cn

scp file user@host:/path/
来源：http://fw.jctech888.com.cn

[R57] 远程执行命令
来源：http://ug.9csxet.cn

ssh user@host 'uptime'
来源：http://qh.gzmigu.cn

[R58] 下载文件
来源：http://lm.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bf.9csxet.cn

[R59] 发 POST JSON
来源：http://og.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nc.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://vr.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ey.muxihuayi.cn

[R61] 磁盘占用
来源：http://gw.wgjwhj.cn

df -h;  du -sh *
来源：http://kn.521024.cn

[R62] 找最占空间的文件
来源：http://ws.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://uq.shxzukj.cn

[R63] 内存与进程
来源：http://vn.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://vj.bookmarksfly.cn

[R64] 结束进程
来源：http://cf.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://qc.huixiangedu.cn

[R65] 查看端口占用
来源：http://ac.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tm.hnjuh.cn

[R66] 定时任务
来源：http://nw.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://bw.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://cf.haigaiapp.cn

openssl rand -hex 16
来源：http://yy.chemitech.net.cn

[R68] 计算文件校验值
来源：http://fn.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oh.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://js.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://gv.huanxung.cn

[R70] 时间戳与互转
来源：http://rj.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://to.muxihuayi.cn

[R71] 日期格式化
来源：http://qs.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vr.gzmigu.cn

[R72] 等待端口就绪
来源：http://uj.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://th.chemitech.net.cn

[R73] 分割大日志
来源：http://db.wgjwhj.cn

split -l 1000 big.log part_
来源：http://hg.nszjky.cn

[R74] 批量重命名
来源：http://sa.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dv.shxzskj.cn

[R75] 导出环境变量
来源：http://vj.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://te.panjiajie.cn

[R76] 使用临时文件
来源：http://aq.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wj.szsharing.cn

[R77] 读取用户输入
来源：http://mv.lnxyls.cn

read -rp "请输入: " ans
来源：http://em.muxihuayi.cn

[R78] 交互式菜单
来源：http://hw.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ay.szxytkj.cn

[R79] 解析命令行选项
来源：http://fm.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://na.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://rh.newstarts.cn

time ./run.sh
来源：http://xh.bjjhwx.cn

================================================================================
来源：http://vx.hnjuh.cn

S. C / C++ 专题
来源：http://pu.bjjhwx.cn

================================================================================
来源：http://nj.lnxyls.cn

[S01] C：Hello World
来源：http://ug.9csxet.cn

#include <stdio.h>
来源：http://to.521024.cn


<!-- 参考信息 -->