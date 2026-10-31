代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://od.hahajie.cn

) t WHERE rn = 1;
来源：http://rq.huixinmuqiang.cn

[Q35] 内连接
来源：http://gm.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cf.nicolike.cn

[Q36] 左连接
来源：http://dj.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ug.szsharing.cn

[Q37] 右连接
来源：http://pn.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nz.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xn.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pb.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://pb.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fs.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ms.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rg.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ys.panjiajie.cn

[Q41] 多表连接
来源：http://dx.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ii.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://vu.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://bb.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://tb.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://ob.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gv.nicolike.cn

[Q43] 标量子查询
来源：http://rr.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uh.nicolike.cn

[Q44] IN 子查询
来源：http://lx.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yt.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://qd.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uq.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xs.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vr.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://jy.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wo.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://oz.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tb.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://ho.shxzskj.cn

[Q49] 更新单行
来源：http://xs.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gu.chemitech.net.cn

[Q50] 批量更新
来源：http://bk.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://js.chemitech.net.cn

[Q51] 用子查询更新
来源：http://zh.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kj.colortex.cn

[Q52] 删除指定行
来源：http://on.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://uk.haigaiapp.cn

[Q53] 按条件删除
来源：http://ap.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zh.colortex.cn

[Q54] 清空表
来源：http://am.colortex.cn

TRUNCATE TABLE logs;
来源：http://ea.nicolike.cn

[Q55] 排名（并列占位）
来源：http://um.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fu.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://ik.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mq.9csxet.cn

[Q57] 行号
来源：http://xm.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ge.huixiangedu.cn

[Q58] 累计求和
来源：http://no.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vp.huixiangedu.cn

[Q59] 分组内累计
来源：http://dl.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ok.jianghongdianzi.cn

[Q60] 取上一行 / 下一行
来源：http://vp.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rm.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oq.nszjky.cn

[Q61] 移动平均
来源：http://rt.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dq.colortex.cn

[Q62] 分组占比
来源：http://pp.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yd.bjjhwx.cn

[Q63] 开启事务
来源：http://ex.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://of.lnxyls.cn

[Q64] 提交事务
来源：http://bl.shxzukj.cn

COMMIT;
来源：http://dz.szxytkj.cn

[Q65] 回滚事务
来源：http://ma.hnjuh.cn

ROLLBACK;
来源：http://vc.521024.cn

[Q66] 行锁查询
来源：http://cw.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hl.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://re.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tt.szxytkj.cn

[Q68] 保存点
来源：http://tg.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://ny.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://yd.shxzskj.cn

[Q69] 查看执行计划
来源：http://ch.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uj.shxzukj.cn

[Q70] 更新统计信息
来源：http://mt.9csxet.cn

ANALYZE TABLE users;
来源：http://qy.huanxung.cn

[Q71] 查看建表语句
来源：http://wg.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mn.bjjhwx.cn

[Q72] 查看索引
来源：http://cr.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://uf.shtwfgs.cn

[Q73] 查看表状态
来源：http://nn.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lx.colortex.cn

[Q74] 强制使用索引
来源：http://qd.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qh.shxzskj.cn

[Q75] 日期格式化
来源：http://cu.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ow.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ql.521024.cn

[Q76] 按天统计
来源：http://kt.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oz.521024.cn

[Q77] 时间加减
来源：http://pw.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://za.haigaiapp.cn

[Q78] 当前时间
来源：http://vb.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ls.shxzukj.cn

[Q79] 字符串拼接
来源：http://bl.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ko.muxihuayi.cn

[Q80] 字符串截取
来源：http://xd.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tz.bjjhwx.cn

[Q81] 字符串替换
来源：http://bg.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zc.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://kv.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ot.panjiajie.cn

[Q83] 大小写转换
来源：http://ej.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lr.lnxyls.cn

[Q84] 去除首尾空格
来源：http://tk.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://es.521024.cn

[Q85] 数值取整
来源：http://vb.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ze.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://ab.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bh.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://qi.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mm.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://yp.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sy.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hh.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://qu.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jh.shtwfgs.cn

[Q90] 生成序号列
来源：http://wt.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sq.jianghongdianzi.cn

================================================================================
来源：http://zz.yuexingan06.cn

R. Bash 专题
来源：http://vz.szsharing.cn

================================================================================
来源：http://hq.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://ha.huanxung.cn

#!/usr/bin/env bash
来源：http://cc.gzmigu.cn

set -euo pipefail
来源：http://et.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://jy.9csxet.cn

name="Tom"; echo "$name"
来源：http://nd.haigaiapp.cn

[R03] 只读变量
来源：http://zc.muxihuayi.cn

readonly PI=3.14
来源：http://qt.chemitech.net.cn

[R04] 位置参数
来源：http://xe.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wj.szxytkj.cn

[R05] 参数默认值
来源：http://yg.nicolike.cn

name="${1:-default}"
来源：http://wb.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://md.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pg.jctech888.com.cn

[R07] if 判断文件
来源：http://ga.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yj.bookmarksfly.cn

[R08] 数值比较
来源：http://jv.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ck.huanxung.cn

[R09] 字符串比较
来源：http://ff.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://by.nszjky.cn

[R10] 正则匹配
来源：http://pl.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ll.jianghongdianzi.cn

[R11] case 多分支
来源：http://fk.szsharing.cn

case "$1" in
来源：http://sx.hahajie.cn

start) echo "启动" ;;
来源：http://df.hahajie.cn

stop)  echo "停止" ;;
来源：http://pa.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://as.yuntaijiaju.cn

esac
来源：http://vf.wgjwhj.cn

[R12] for 遍历文件
来源：http://jl.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://tw.hahajie.cn

[R13] for 计数循环
来源：http://zg.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://sy.szsharing.cn

[R14] C 风格 for
来源：http://oz.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cj.521024.cn

[R15] while 逐行读文件
来源：http://uv.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ss.huixinmuqiang.cn

[R16] until 等待条件
来源：http://hw.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kp.asd995.cn

[R17] 数组定义与取值
来源：http://tp.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zs.colortex.cn

[R18] 遍历数组
来源：http://fa.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ys.bookmarksfly.cn

[R19] 数组长度
来源：http://fi.asd995.cn

echo "${#arr[@]}"
来源：http://yg.hnjuh.cn

[R20] 关联数组（字典）
来源：http://jl.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xi.hahajie.cn

[R21] 字符串长度
来源：http://ph.huixiangedu.cn

echo "${#s}"
来源：http://pe.szsharing.cn

[R22] 截取子串
来源：http://ms.shxzskj.cn

echo "${s:0:5}"
来源：http://xl.huixiangedu.cn

[R23] 字符串替换
来源：http://lf.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://va.9csxet.cn

[R24] 大小写转换
来源：http://qm.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ps.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://rn.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ay.yuntaijiaju.cn

[R26] 命令替换
来源：http://vb.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://fa.chemitech.net.cn

[R27] 算术展开
来源：http://vl.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://sf.shxzukj.cn

[R28] 浮点运算
来源：http://ea.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://gu.gzmigu.cn

[R29] 定义函数
来源：http://ca.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jp.szsharing.cn

[R30] 函数返回状态码
来源：http://gd.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://ju.chemitech.net.cn

[R31] 局部变量
来源：http://dy.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://gz.gzmigu.cn

[R32] 参数个数校验
来源：http://fz.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pt.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://ln.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tg.szsharing.cn

[R34] 退出时清理
来源：http://qm.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://za.lnxyls.cn

[R35] 后台执行并等待
来源：http://vk.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lf.shxzukj.cn

[R36] 并发执行多个任务
来源：http://lu.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kd.nszjky.cn

[R37] 把输出赋给变量
来源：http://tn.yuntaijiaju.cn

files=$(ls -1)
来源：http://hs.yuexingan06.cn

[R38] 管道串联
来源：http://to.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://pz.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://cg.szxytkj.cn

cmd > out.log 2>&1
来源：http://mp.panjiajie.cn

[R40] 追加写日志
来源：http://oi.jianghongdianzi.cn

echo "log" >> out.log
来源：http://ih.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://wf.9csxet.cn

cmd >/dev/null 2>&1
来源：http://zv.bjjhwx.cn

[R42] 输入重定向
来源：http://vz.haigaiapp.cn

wc -l < a.txt
来源：http://np.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://rl.yuexingan06.cn

find . -name "*.log" -type f
来源：http://ai.shxzukj.cn

[R44] 按修改时间查找
来源：http://po.hahajie.cn

find . -mtime -7 -type f
来源：http://iu.szsharing.cn

[R45] 批量删除
来源：http://lj.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://mv.hnjuh.cn

[R46] 递归替换文件内容
来源：http://xy.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fb.haigaiapp.cn

[R47] sed 单行替换
来源：http://pe.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ks.chemitech.net.cn

[R48] awk 取指定列
来源：http://dc.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://dt.hahajie.cn

[R49] awk 带条件
来源：http://hr.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ii.wgjwhj.cn

[R50] awk 求和
来源：http://wc.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://en.haigaiapp.cn

[R51] 排序去重取前几
来源：http://an.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ln.jianghongdianzi.cn

[R52] 统计行数
来源：http://du.colortex.cn

wc -l a.txt
来源：http://cy.521024.cn

[R53] 查看文件头与实时尾
来源：http://no.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jk.haigaiapp.cn

[R54] 比较两个文件
来源：http://bg.gzmigu.cn

diff a.txt b.txt
来源：http://ll.shxzskj.cn

[R55] 压缩与解压
来源：http://gp.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gp.huixiangedu.cn

[R56] 远程拷贝
来源：http://ri.hahajie.cn

scp file user@host:/path/
来源：http://ea.gzmigu.cn

[R57] 远程执行命令
来源：http://xv.newstarts.cn

ssh user@host 'uptime'
来源：http://ep.hnjuh.cn

[R58] 下载文件
来源：http://iv.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yv.521024.cn

[R59] 发 POST JSON
来源：http://lk.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qu.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://wc.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kh.521024.cn

[R61] 磁盘占用
来源：http://sj.yuntaijiaju.cn

df -h;  du -sh *
来源：http://oz.szsharing.cn

[R62] 找最占空间的文件
来源：http://hs.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://sg.huixiangedu.cn

[R63] 内存与进程
来源：http://cw.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://cc.521024.cn

[R64] 结束进程
来源：http://ju.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://we.chemitech.net.cn

[R65] 查看端口占用
来源：http://ho.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zz.shtwfgs.cn

[R66] 定时任务
来源：http://re.nszjky.cn

crontab -e;  crontab -l
来源：http://ql.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://ep.asd995.cn

openssl rand -hex 16
来源：http://oq.521024.cn

[R68] 计算文件校验值
来源：http://ca.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ic.shtwfgs.cn

[R69] 生成随机密码
来源：http://gx.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://io.hahajie.cn

[R70] 时间戳与互转
来源：http://kp.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://bx.huixiangedu.cn

[R71] 日期格式化
来源：http://va.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zg.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://ru.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://el.yuntaijiaju.cn

[R73] 分割大日志
来源：http://py.wgjwhj.cn

split -l 1000 big.log part_
来源：http://xb.newstarts.cn

[R74] 批量重命名
来源：http://su.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pz.shxzukj.cn

[R75] 导出环境变量
来源：http://rq.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://mm.bookmarksfly.cn

[R76] 使用临时文件
来源：http://va.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qn.nszjky.cn

[R77] 读取用户输入
来源：http://dy.jctech888.com.cn

read -rp "请输入: " ans
来源：http://ba.hahajie.cn

[R78] 交互式菜单
来源：http://jq.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tl.szxytkj.cn

[R79] 解析命令行选项
来源：http://fa.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tg.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://op.wgjwhj.cn

time ./run.sh
来源：http://tj.chemitech.net.cn

================================================================================
来源：http://eg.lnxyls.cn

S. C / C++ 专题
来源：http://ly.chemitech.net.cn

================================================================================
来源：http://cc.muxihuayi.cn

[S01] C：Hello World
来源：http://vx.lnxyls.cn

#include <stdio.h>
来源：http://vi.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nn.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://si.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://zf.shxzskj.cn

[S03] C：读入整数
来源：http://kj.shxzukj.cn


<!-- 参考信息 -->