代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tk.nszjky.cn

[Q32] 分组拼接字符串
来源：http://dj.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gg.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ow.panjiajie.cn

[Q33] 多列分组
来源：http://rp.lnxyls.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ot.szsharing.cn

[Q34] 每组取第一条
来源：http://rg.bookmarksfly.cn

SELECT * FROM (
来源：http://wo.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yb.szxytkj.cn

) t WHERE rn = 1;
来源：http://ty.huixinmuqiang.cn

[Q35] 内连接
来源：http://vj.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dc.yuntaijiaju.cn

[Q36] 左连接
来源：http://ml.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pt.9csxet.cn

[Q37] 右连接
来源：http://uv.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lc.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yl.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bb.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://jk.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zx.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pd.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dy.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gq.yuntaijiaju.cn

[Q41] 多表连接
来源：http://bg.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dh.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://ax.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://jf.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://xu.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://ob.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://os.shxzskj.cn

[Q43] 标量子查询
来源：http://me.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://be.jctech888.com.cn

[Q44] IN 子查询
来源：http://cx.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pb.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://jy.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yh.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oz.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gl.lnxyls.cn

[Q47] 与平均值比较
来源：http://ip.jianghongdianzi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ho.bjjhwx.cn

[Q48] CTE 公用表表达式
来源：http://ht.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pb.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://ms.huixiangedu.cn

[Q49] 更新单行
来源：http://dh.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hp.yuntaijiaju.cn

[Q50] 批量更新
来源：http://ge.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dj.wgjwhj.cn

[Q51] 用子查询更新
来源：http://vi.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zt.haigaiapp.cn

[Q52] 删除指定行
来源：http://kr.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://ne.hahajie.cn

[Q53] 按条件删除
来源：http://uv.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ot.shxzukj.cn

[Q54] 清空表
来源：http://es.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://mf.nszjky.cn

[Q55] 排名（并列占位）
来源：http://ig.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fk.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://nx.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tj.nszjky.cn

[Q57] 行号
来源：http://jw.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sg.huixinmuqiang.cn

[Q58] 累计求和
来源：http://ob.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cx.huanxung.cn

[Q59] 分组内累计
来源：http://po.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ga.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://wl.shxzukj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kc.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qw.newstarts.cn

[Q61] 移动平均
来源：http://ot.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hc.hnjuh.cn

[Q62] 分组占比
来源：http://wv.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yl.shtwfgs.cn

[Q63] 开启事务
来源：http://by.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://as.huixinmuqiang.cn

[Q64] 提交事务
来源：http://dl.lnxyls.cn

COMMIT;
来源：http://fb.shtwfgs.cn

[Q65] 回滚事务
来源：http://xz.panjiajie.cn

ROLLBACK;
来源：http://ds.nszjky.cn

[Q66] 行锁查询
来源：http://qp.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yf.hnjuh.cn

[Q67] 设置隔离级别
来源：http://yt.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sz.huixiangedu.cn

[Q68] 保存点
来源：http://qg.nicolike.cn

SAVEPOINT sp1;
来源：http://jk.newstarts.cn

ROLLBACK TO sp1;
来源：http://ji.chemitech.net.cn

[Q69] 查看执行计划
来源：http://mq.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zg.huixiangedu.cn

[Q70] 更新统计信息
来源：http://nw.nszjky.cn

ANALYZE TABLE users;
来源：http://qk.asd995.cn

[Q71] 查看建表语句
来源：http://wz.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ae.huixiangedu.cn

[Q72] 查看索引
来源：http://my.shxzukj.cn

SHOW INDEX FROM users;
来源：http://xd.hnjuh.cn

[Q73] 查看表状态
来源：http://bg.haigaiapp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://if.newstarts.cn

[Q74] 强制使用索引
来源：http://gh.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xq.shtwfgs.cn

[Q75] 日期格式化
来源：http://wl.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ma.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mp.lnxyls.cn

[Q76] 按天统计
来源：http://iy.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jy.muxihuayi.cn

[Q77] 时间加减
来源：http://dg.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://me.shtwfgs.cn

[Q78] 当前时间
来源：http://jc.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xk.newstarts.cn

[Q79] 字符串拼接
来源：http://xj.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jt.panjiajie.cn

[Q80] 字符串截取
来源：http://eo.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bk.huanxung.cn

[Q81] 字符串替换
来源：http://wt.yuexingan06.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sm.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://hq.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cx.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://sj.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bd.jctech888.com.cn

[Q84] 去除首尾空格
来源：http://bx.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://pj.yuexingan06.cn

[Q85] 数值取整
来源：http://nq.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iv.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://xs.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tn.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://ix.panjiajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://la.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://ol.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bs.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hg.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://ub.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tz.szxytkj.cn

[Q90] 生成序号列
来源：http://jo.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ih.panjiajie.cn

================================================================================
来源：http://vq.haigaiapp.cn

R. Bash 专题
来源：http://lh.colortex.cn

================================================================================
来源：http://zh.nicolike.cn

[R01] shebang 与严格模式
来源：http://be.yuexingan06.cn

#!/usr/bin/env bash
来源：http://qj.521024.cn

set -euo pipefail
来源：http://mr.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://xn.newstarts.cn

name="Tom"; echo "$name"
来源：http://zr.hahajie.cn

[R03] 只读变量
来源：http://ds.huixiangedu.cn

readonly PI=3.14
来源：http://vo.521024.cn

[R04] 位置参数
来源：http://vj.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cm.colortex.cn

[R05] 参数默认值
来源：http://ua.huixiangedu.cn

name="${1:-default}"
来源：http://rm.nszjky.cn

[R06] 判断命令是否存在
来源：http://gi.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://av.lnxyls.cn

[R07] if 判断文件
来源：http://uo.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nm.nicolike.cn

[R08] 数值比较
来源：http://sp.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://at.wgjwhj.cn

[R09] 字符串比较
来源：http://jv.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dt.huanxung.cn

[R10] 正则匹配
来源：http://va.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bx.shxzskj.cn

[R11] case 多分支
来源：http://sx.jctech888.com.cn

case "$1" in
来源：http://kj.yuexingan06.cn

start) echo "启动" ;;
来源：http://be.nszjky.cn

stop)  echo "停止" ;;
来源：http://ye.newstarts.cn

*)     echo "未知命令" ;;
来源：http://iy.jianghongdianzi.cn

esac
来源：http://ju.szsharing.cn

[R12] for 遍历文件
来源：http://wg.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://ve.huixiangedu.cn

[R13] for 计数循环
来源：http://un.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://kg.shxzukj.cn

[R14] C 风格 for
来源：http://zq.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lh.521024.cn

[R15] while 逐行读文件
来源：http://vq.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iu.muxihuayi.cn

[R16] until 等待条件
来源：http://sy.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oc.hnjuh.cn

[R17] 数组定义与取值
来源：http://js.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gn.shxzukj.cn

[R18] 遍历数组
来源：http://lz.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bh.nszjky.cn

[R19] 数组长度
来源：http://sc.newstarts.cn

echo "${#arr[@]}"
来源：http://qm.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://lp.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jf.szsharing.cn

[R21] 字符串长度
来源：http://sw.nszjky.cn

echo "${#s}"
来源：http://fy.huixiangedu.cn

[R22] 截取子串
来源：http://qd.521024.cn

echo "${s:0:5}"
来源：http://bs.shxzskj.cn

[R23] 字符串替换
来源：http://yd.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ai.chemitech.net.cn

[R24] 大小写转换
来源：http://kj.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mt.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://hs.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xs.newstarts.cn

[R26] 命令替换
来源：http://at.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://sj.bjjhwx.cn

[R27] 算术展开
来源：http://hw.hahajie.cn

echo $((1 + 2 * 3))
来源：http://lg.huixiangedu.cn

[R28] 浮点运算
来源：http://rw.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://bc.muxihuayi.cn

[R29] 定义函数
来源：http://ea.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qq.haigaiapp.cn

[R30] 函数返回状态码
来源：http://vw.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://dp.hnjuh.cn

[R31] 局部变量
来源：http://fw.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://gf.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://hh.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ly.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://cq.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ea.shxzskj.cn

[R34] 退出时清理
来源：http://rf.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bl.colortex.cn

[R35] 后台执行并等待
来源：http://jz.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dz.hahajie.cn

[R36] 并发执行多个任务
来源：http://mq.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fs.szxytkj.cn

[R37] 把输出赋给变量
来源：http://ii.9csxet.cn

files=$(ls -1)
来源：http://hk.521024.cn

[R38] 管道串联
来源：http://pi.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://qk.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://li.shxzukj.cn

cmd > out.log 2>&1
来源：http://ye.9csxet.cn

[R40] 追加写日志
来源：http://aq.huanxung.cn

echo "log" >> out.log
来源：http://je.hahajie.cn

[R41] 丢弃输出
来源：http://gt.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://hy.colortex.cn

[R42] 输入重定向
来源：http://zj.wgjwhj.cn

wc -l < a.txt
来源：http://oi.shxzukj.cn

[R43] 按名字查找文件
来源：http://yv.gzmigu.cn

find . -name "*.log" -type f
来源：http://qq.newstarts.cn

[R44] 按修改时间查找
来源：http://cn.bjjhwx.cn

find . -mtime -7 -type f
来源：http://da.hnjuh.cn

[R45] 批量删除
来源：http://cu.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://vx.newstarts.cn

[R46] 递归替换文件内容
来源：http://go.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://og.huanxung.cn

[R47] sed 单行替换
来源：http://jl.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kk.shxzukj.cn

[R48] awk 取指定列
来源：http://ju.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://ku.asd995.cn

[R49] awk 带条件
来源：http://lx.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://an.chemitech.net.cn

[R50] awk 求和
来源：http://fu.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gg.panjiajie.cn

[R51] 排序去重取前几
来源：http://rs.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zw.nicolike.cn

[R52] 统计行数
来源：http://ph.shtwfgs.cn

wc -l a.txt
来源：http://oo.521024.cn

[R53] 查看文件头与实时尾
来源：http://ra.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xs.yuexingan06.cn

[R54] 比较两个文件
来源：http://sj.panjiajie.cn

diff a.txt b.txt
来源：http://lm.hahajie.cn

[R55] 压缩与解压
来源：http://ax.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zf.colortex.cn

[R56] 远程拷贝
来源：http://cc.yuntaijiaju.cn

scp file user@host:/path/
来源：http://uu.jctech888.com.cn

[R57] 远程执行命令
来源：http://iu.9csxet.cn

ssh user@host 'uptime'
来源：http://ni.hnjuh.cn

[R58] 下载文件
来源：http://yk.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fl.jctech888.com.cn

[R59] 发 POST JSON
来源：http://dz.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gw.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://mj.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zh.panjiajie.cn

[R61] 磁盘占用
来源：http://tm.nicolike.cn

df -h;  du -sh *
来源：http://ow.szsharing.cn

[R62] 找最占空间的文件
来源：http://df.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://fg.huixinmuqiang.cn

[R63] 内存与进程
来源：http://tt.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://ww.hnjuh.cn

[R64] 结束进程
来源：http://ri.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://ab.shxzskj.cn

[R65] 查看端口占用
来源：http://py.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yf.szsharing.cn

[R66] 定时任务
来源：http://hp.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://lh.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://nt.shxzskj.cn

openssl rand -hex 16
来源：http://mb.nicolike.cn

[R68] 计算文件校验值
来源：http://mc.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hq.lnxyls.cn

[R69] 生成随机密码
来源：http://yd.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://gs.szsharing.cn

[R70] 时间戳与互转
来源：http://ab.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://uo.colortex.cn

[R71] 日期格式化
来源：http://wr.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xm.chemitech.net.cn

[R72] 等待端口就绪
来源：http://gn.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cp.bookmarksfly.cn

[R73] 分割大日志
来源：http://ai.panjiajie.cn

split -l 1000 big.log part_
来源：http://zu.bjjhwx.cn

[R74] 批量重命名
来源：http://sf.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pk.lnxyls.cn

[R75] 导出环境变量
来源：http://jj.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://jc.lnxyls.cn

[R76] 使用临时文件
来源：http://gf.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nn.9csxet.cn

[R77] 读取用户输入
来源：http://yv.szxytkj.cn

read -rp "请输入: " ans
来源：http://xo.wgjwhj.cn

[R78] 交互式菜单
来源：http://tx.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bn.nszjky.cn

[R79] 解析命令行选项
来源：http://po.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ke.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://ox.jianghongdianzi.cn

time ./run.sh
来源：http://xh.bookmarksfly.cn

================================================================================
来源：http://ns.muxihuayi.cn


<!-- 参考信息 -->