代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ma.9csxet.cn

[Q28] 求和与平均
来源：http://bo.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ql.muxihuayi.cn

[Q29] 最大最小值
来源：http://dz.asd995.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ku.colortex.cn

[Q30] 分组统计
来源：http://fs.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uh.shxzukj.cn

[Q31] 分组后过滤
来源：http://ry.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dy.szsharing.cn

[Q32] 分组拼接字符串
来源：http://kc.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pn.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eh.huixinmuqiang.cn

[Q33] 多列分组
来源：http://ws.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kx.yuexingan06.cn

[Q34] 每组取第一条
来源：http://ty.szsharing.cn

SELECT * FROM (
来源：http://lo.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ak.hahajie.cn

) t WHERE rn = 1;
来源：http://xs.huixinmuqiang.cn

[Q35] 内连接
来源：http://kj.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fg.shxzskj.cn

[Q36] 左连接
来源：http://rs.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ts.newstarts.cn

[Q37] 右连接
来源：http://rc.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ka.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pm.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zd.asd995.cn

[Q39] 自连接（查上下级）
来源：http://ys.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qc.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wf.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://la.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kj.lnxyls.cn

[Q41] 多表连接
来源：http://qs.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lx.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://uu.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://vb.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://rh.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://jn.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ns.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://fi.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fz.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://gg.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iz.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://sm.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ii.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gk.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://od.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://hs.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yg.asd995.cn

[Q48] CTE 公用表表达式
来源：http://jl.jianghongdianzi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bt.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://jk.huixinmuqiang.cn

[Q49] 更新单行
来源：http://lj.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://op.colortex.cn

[Q50] 批量更新
来源：http://lz.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mg.haigaiapp.cn

[Q51] 用子查询更新
来源：http://wl.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gx.9csxet.cn

[Q52] 删除指定行
来源：http://rc.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://xg.hnjuh.cn

[Q53] 按条件删除
来源：http://nl.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ax.haigaiapp.cn

[Q54] 清空表
来源：http://cn.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://bw.asd995.cn

[Q55] 排名（并列占位）
来源：http://xc.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ku.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://gp.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ih.jctech888.com.cn

[Q57] 行号
来源：http://ne.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yg.hahajie.cn

[Q58] 累计求和
来源：http://pu.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xm.lnxyls.cn

[Q59] 分组内累计
来源：http://jn.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://he.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://zj.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dj.huixinmuqiang.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ym.yuexingan06.cn

[Q61] 移动平均
来源：http://bl.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nu.shxzukj.cn

[Q62] 分组占比
来源：http://sf.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cs.newstarts.cn

[Q63] 开启事务
来源：http://pf.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dw.gzmigu.cn

[Q64] 提交事务
来源：http://br.haigaiapp.cn

COMMIT;
来源：http://wt.colortex.cn

[Q65] 回滚事务
来源：http://ay.colortex.cn

ROLLBACK;
来源：http://yh.yuexingan06.cn

[Q66] 行锁查询
来源：http://lo.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://td.szsharing.cn

[Q67] 设置隔离级别
来源：http://wd.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ph.bjjhwx.cn

[Q68] 保存点
来源：http://ae.shxzukj.cn

SAVEPOINT sp1;
来源：http://sw.nszjky.cn

ROLLBACK TO sp1;
来源：http://xz.panjiajie.cn

[Q69] 查看执行计划
来源：http://qx.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ig.huanxung.cn

[Q70] 更新统计信息
来源：http://eu.asd995.cn

ANALYZE TABLE users;
来源：http://vh.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://xt.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xe.huanxung.cn

[Q72] 查看索引
来源：http://ao.gzmigu.cn

SHOW INDEX FROM users;
来源：http://iw.colortex.cn

[Q73] 查看表状态
来源：http://we.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ie.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://rm.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uq.asd995.cn

[Q75] 日期格式化
来源：http://ok.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ci.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dv.newstarts.cn

[Q76] 按天统计
来源：http://fg.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jl.yuntaijiaju.cn

[Q77] 时间加减
来源：http://lt.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gt.panjiajie.cn

[Q78] 当前时间
来源：http://us.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xn.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://ct.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://al.chemitech.net.cn

[Q80] 字符串截取
来源：http://iz.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mk.chemitech.net.cn

[Q81] 字符串替换
来源：http://vv.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zx.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://vj.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ps.bjjhwx.cn

[Q83] 大小写转换
来源：http://nd.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ql.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://fg.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://ij.nicolike.cn

[Q85] 数值取整
来源：http://uv.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://st.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://nx.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zv.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://ri.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lr.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://pz.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://my.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mc.panjiajie.cn

[Q89] 判断表是否存在
来源：http://zj.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jx.asd995.cn

[Q90] 生成序号列
来源：http://up.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vd.lnxyls.cn

================================================================================
来源：http://dl.muxihuayi.cn

R. Bash 专题
来源：http://ai.hahajie.cn

================================================================================
来源：http://kq.lnxyls.cn

[R01] shebang 与严格模式
来源：http://ha.szxytkj.cn

#!/usr/bin/env bash
来源：http://up.chemitech.net.cn

set -euo pipefail
来源：http://vp.nszjky.cn

[R02] 变量赋值与使用
来源：http://ts.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://ac.nszjky.cn

[R03] 只读变量
来源：http://cg.newstarts.cn

readonly PI=3.14
来源：http://bc.chemitech.net.cn

[R04] 位置参数
来源：http://pa.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nj.huixinmuqiang.cn

[R05] 参数默认值
来源：http://kx.nicolike.cn

name="${1:-default}"
来源：http://gl.nszjky.cn

[R06] 判断命令是否存在
来源：http://mi.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yf.shxzskj.cn

[R07] if 判断文件
来源：http://dj.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rm.521024.cn

[R08] 数值比较
来源：http://al.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mk.shtwfgs.cn

[R09] 字符串比较
来源：http://hn.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qx.bookmarksfly.cn

[R10] 正则匹配
来源：http://bt.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zm.9csxet.cn

[R11] case 多分支
来源：http://vm.huanxung.cn

case "$1" in
来源：http://ub.gzmigu.cn

start) echo "启动" ;;
来源：http://ix.asd995.cn

stop)  echo "停止" ;;
来源：http://cs.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://ia.wgjwhj.cn

esac
来源：http://fi.szxytkj.cn

[R12] for 遍历文件
来源：http://py.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://yv.szxytkj.cn

[R13] for 计数循环
来源：http://ve.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://hj.521024.cn

[R14] C 风格 for
来源：http://yq.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ft.shtwfgs.cn

[R15] while 逐行读文件
来源：http://hy.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lc.gzmigu.cn

[R16] until 等待条件
来源：http://ar.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uw.huanxung.cn

[R17] 数组定义与取值
来源：http://dd.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fb.huixinmuqiang.cn

[R18] 遍历数组
来源：http://oc.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fm.newstarts.cn

[R19] 数组长度
来源：http://zl.yuexingan06.cn

echo "${#arr[@]}"
来源：http://qr.bookmarksfly.cn

[R20] 关联数组（字典）
来源：http://uu.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xe.panjiajie.cn

[R21] 字符串长度
来源：http://hr.chemitech.net.cn

echo "${#s}"
来源：http://xp.colortex.cn

[R22] 截取子串
来源：http://wm.yuexingan06.cn

echo "${s:0:5}"
来源：http://dx.chemitech.net.cn

[R23] 字符串替换
来源：http://sy.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wq.521024.cn

[R24] 大小写转换
来源：http://sh.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vz.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://oa.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bf.huixiangedu.cn

[R26] 命令替换
来源：http://fr.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://ko.jianghongdianzi.cn

[R27] 算术展开
来源：http://jn.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://xv.lnxyls.cn

[R28] 浮点运算
来源：http://rh.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://wu.shtwfgs.cn

[R29] 定义函数
来源：http://cu.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bu.panjiajie.cn

[R30] 函数返回状态码
来源：http://tk.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://ul.9csxet.cn

[R31] 局部变量
来源：http://xw.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://hr.huixiangedu.cn

[R32] 参数个数校验
来源：http://wq.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://td.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://lu.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xx.asd995.cn

[R34] 退出时清理
来源：http://yk.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dj.szsharing.cn

[R35] 后台执行并等待
来源：http://kx.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mj.lnxyls.cn

[R36] 并发执行多个任务
来源：http://pg.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hs.huanxung.cn

[R37] 把输出赋给变量
来源：http://en.yuntaijiaju.cn

files=$(ls -1)
来源：http://ta.bookmarksfly.cn

[R38] 管道串联
来源：http://mh.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://sj.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://ln.szsharing.cn

cmd > out.log 2>&1
来源：http://hu.colortex.cn

[R40] 追加写日志
来源：http://sn.szxytkj.cn

echo "log" >> out.log
来源：http://fm.hnjuh.cn

[R41] 丢弃输出
来源：http://io.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://xq.nszjky.cn

[R42] 输入重定向
来源：http://pz.shtwfgs.cn

wc -l < a.txt
来源：http://fg.nszjky.cn

[R43] 按名字查找文件
来源：http://zw.chemitech.net.cn

find . -name "*.log" -type f
来源：http://ag.lnxyls.cn

[R44] 按修改时间查找
来源：http://ez.shxzskj.cn

find . -mtime -7 -type f
来源：http://eb.shtwfgs.cn

[R45] 批量删除
来源：http://wu.hahajie.cn

find . -name "*.tmp" -delete
来源：http://xm.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://xw.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://po.newstarts.cn

[R47] sed 单行替换
来源：http://cm.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qg.bjjhwx.cn

[R48] awk 取指定列
来源：http://yc.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://ke.asd995.cn

[R49] awk 带条件
来源：http://nx.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ga.gzmigu.cn

[R50] awk 求和
来源：http://za.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ke.szxytkj.cn

[R51] 排序去重取前几
来源：http://vc.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lg.huixiangedu.cn

[R52] 统计行数
来源：http://ok.muxihuayi.cn

wc -l a.txt
来源：http://st.asd995.cn

[R53] 查看文件头与实时尾
来源：http://ga.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ww.nicolike.cn

[R54] 比较两个文件
来源：http://yu.colortex.cn

diff a.txt b.txt
来源：http://hq.bookmarksfly.cn

[R55] 压缩与解压
来源：http://ei.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://on.gzmigu.cn

[R56] 远程拷贝
来源：http://tc.9csxet.cn

scp file user@host:/path/
来源：http://cd.szxytkj.cn

[R57] 远程执行命令
来源：http://sd.hahajie.cn

ssh user@host 'uptime'
来源：http://ib.shtwfgs.cn

[R58] 下载文件
来源：http://kj.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bp.shxzukj.cn

[R59] 发 POST JSON
来源：http://jg.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jh.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://lp.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rw.chemitech.net.cn

[R61] 磁盘占用
来源：http://ju.haigaiapp.cn

df -h;  du -sh *
来源：http://pv.gzmigu.cn

[R62] 找最占空间的文件
来源：http://za.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://br.yuntaijiaju.cn

[R63] 内存与进程
来源：http://us.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://gm.wgjwhj.cn

[R64] 结束进程
来源：http://ez.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://yx.huixiangedu.cn

[R65] 查看端口占用
来源：http://gp.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yn.yuexingan06.cn

[R66] 定时任务
来源：http://ds.chemitech.net.cn

crontab -e;  crontab -l
来源：http://ym.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://ck.9csxet.cn

openssl rand -hex 16
来源：http://zk.nszjky.cn

[R68] 计算文件校验值
来源：http://rn.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oh.gzmigu.cn

[R69] 生成随机密码
来源：http://ei.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://yw.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://hh.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://yy.bjjhwx.cn

[R71] 日期格式化
来源：http://nw.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ym.panjiajie.cn

[R72] 等待端口就绪
来源：http://xy.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ow.newstarts.cn

[R73] 分割大日志
来源：http://im.huanxung.cn

split -l 1000 big.log part_
来源：http://gu.shxzukj.cn

[R74] 批量重命名
来源：http://rb.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ov.bookmarksfly.cn

[R75] 导出环境变量
来源：http://cc.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://ro.shxzukj.cn

[R76] 使用临时文件
来源：http://be.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kj.szxytkj.cn

[R77] 读取用户输入
来源：http://lj.yuexingan06.cn


<!-- 参考信息 -->