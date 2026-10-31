代发 wailian999

[Q36] 左连接
来源：http://to.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ny.nicolike.cn

[Q37] 右连接
来源：http://gp.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rr.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kf.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://me.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://oy.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hl.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tw.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ez.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ld.szsharing.cn

[Q41] 多表连接
来源：http://qv.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kr.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://wk.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://gd.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://dq.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://au.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dm.haigaiapp.cn

[Q43] 标量子查询
来源：http://kx.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ix.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://vg.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rb.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://ms.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mp.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://la.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vs.asd995.cn

[Q47] 与平均值比较
来源：http://nx.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://aj.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://xg.jianghongdianzi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://st.szxytkj.cn

SELECT * FROM t WHERE c > 5;
来源：http://ro.yuexingan06.cn

[Q49] 更新单行
来源：http://zj.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ro.521024.cn

[Q50] 批量更新
来源：http://kj.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jf.asd995.cn

[Q51] 用子查询更新
来源：http://eq.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rh.9csxet.cn

[Q52] 删除指定行
来源：http://pl.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://jk.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://ia.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zw.shtwfgs.cn

[Q54] 清空表
来源：http://em.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://el.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://qi.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oz.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://xl.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nd.newstarts.cn

[Q57] 行号
来源：http://wr.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yv.gzmigu.cn

[Q58] 累计求和
来源：http://jl.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tj.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://bx.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fx.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://yf.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wh.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ym.wgjwhj.cn

[Q61] 移动平均
来源：http://pp.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sw.szxytkj.cn

[Q62] 分组占比
来源：http://ww.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ox.nicolike.cn

[Q63] 开启事务
来源：http://az.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://em.bookmarksfly.cn

[Q64] 提交事务
来源：http://nz.colortex.cn

COMMIT;
来源：http://se.jctech888.com.cn

[Q65] 回滚事务
来源：http://lh.szsharing.cn

ROLLBACK;
来源：http://nj.bjjhwx.cn

[Q66] 行锁查询
来源：http://mu.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hy.szxytkj.cn

[Q67] 设置隔离级别
来源：http://zv.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://py.yuntaijiaju.cn

[Q68] 保存点
来源：http://ay.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://oa.nszjky.cn

ROLLBACK TO sp1;
来源：http://uo.muxihuayi.cn

[Q69] 查看执行计划
来源：http://ro.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jl.hnjuh.cn

[Q70] 更新统计信息
来源：http://mk.jctech888.com.cn

ANALYZE TABLE users;
来源：http://px.hahajie.cn

[Q71] 查看建表语句
来源：http://by.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sa.muxihuayi.cn

[Q72] 查看索引
来源：http://sk.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://ih.hahajie.cn

[Q73] 查看表状态
来源：http://dr.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jj.muxihuayi.cn

[Q74] 强制使用索引
来源：http://vd.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xt.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://lq.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ka.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ou.huanxung.cn

[Q76] 按天统计
来源：http://su.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fz.yuexingan06.cn

[Q77] 时间加减
来源：http://uu.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dx.newstarts.cn

[Q78] 当前时间
来源：http://be.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yi.shxzskj.cn

[Q79] 字符串拼接
来源：http://dp.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yb.nszjky.cn

[Q80] 字符串截取
来源：http://ck.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jc.hnjuh.cn

[Q81] 字符串替换
来源：http://mg.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tb.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://tf.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qq.chemitech.net.cn

[Q83] 大小写转换
来源：http://fw.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kv.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://ed.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://vq.huixinmuqiang.cn

[Q85] 数值取整
来源：http://ko.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sj.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://jn.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gn.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://ld.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ha.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://ia.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vh.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://du.shxzukj.cn

[Q89] 判断表是否存在
来源：http://ei.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hy.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://vm.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jl.jianghongdianzi.cn

================================================================================
来源：http://zv.haigaiapp.cn

R. Bash 专题
来源：http://ku.huixinmuqiang.cn

================================================================================
来源：http://jw.colortex.cn

[R01] shebang 与严格模式
来源：http://pg.huixiangedu.cn

#!/usr/bin/env bash
来源：http://tb.bookmarksfly.cn

set -euo pipefail
来源：http://js.nicolike.cn

[R02] 变量赋值与使用
来源：http://us.shxzskj.cn

name="Tom"; echo "$name"
来源：http://ri.shtwfgs.cn

[R03] 只读变量
来源：http://qf.newstarts.cn

readonly PI=3.14
来源：http://re.szsharing.cn

[R04] 位置参数
来源：http://ap.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rx.yuexingan06.cn

[R05] 参数默认值
来源：http://rz.haigaiapp.cn

name="${1:-default}"
来源：http://ol.asd995.cn

[R06] 判断命令是否存在
来源：http://dl.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lq.haigaiapp.cn

[R07] if 判断文件
来源：http://re.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ek.muxihuayi.cn

[R08] 数值比较
来源：http://mu.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://le.9csxet.cn

[R09] 字符串比较
来源：http://za.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bn.bookmarksfly.cn

[R10] 正则匹配
来源：http://is.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rt.yuexingan06.cn

[R11] case 多分支
来源：http://at.newstarts.cn

case "$1" in
来源：http://of.nszjky.cn

start) echo "启动" ;;
来源：http://uo.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://xt.szsharing.cn

*)     echo "未知命令" ;;
来源：http://vs.nszjky.cn

esac
来源：http://ct.nszjky.cn

[R12] for 遍历文件
来源：http://nv.shxzskj.cn

for f in *.txt; do echo "$f"; done
来源：http://nx.wgjwhj.cn

[R13] for 计数循环
来源：http://jq.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://dd.shtwfgs.cn

[R14] C 风格 for
来源：http://is.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://de.lnxyls.cn

[R15] while 逐行读文件
来源：http://rs.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xr.haigaiapp.cn

[R16] until 等待条件
来源：http://me.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nl.521024.cn

[R17] 数组定义与取值
来源：http://wy.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xt.shxzskj.cn

[R18] 遍历数组
来源：http://ok.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bv.muxihuayi.cn

[R19] 数组长度
来源：http://pr.hnjuh.cn

echo "${#arr[@]}"
来源：http://zm.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://cp.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pz.colortex.cn

[R21] 字符串长度
来源：http://bx.nicolike.cn

echo "${#s}"
来源：http://qf.nicolike.cn

[R22] 截取子串
来源：http://on.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://ij.jctech888.com.cn

[R23] 字符串替换
来源：http://yc.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://np.colortex.cn

[R24] 大小写转换
来源：http://cy.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mr.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://pn.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://to.jianghongdianzi.cn

[R26] 命令替换
来源：http://yl.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://kv.yuntaijiaju.cn

[R27] 算术展开
来源：http://qn.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://ne.bookmarksfly.cn

[R28] 浮点运算
来源：http://st.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://sk.jianghongdianzi.cn

[R29] 定义函数
来源：http://br.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sp.gzmigu.cn

[R30] 函数返回状态码
来源：http://lf.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://tw.yuntaijiaju.cn

[R31] 局部变量
来源：http://kx.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://sn.bjjhwx.cn

[R32] 参数个数校验
来源：http://kx.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jh.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://gy.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://la.muxihuayi.cn

[R34] 退出时清理
来源：http://pc.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hc.shtwfgs.cn

[R35] 后台执行并等待
来源：http://cy.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vp.hnjuh.cn

[R36] 并发执行多个任务
来源：http://lz.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gn.shxzukj.cn

[R37] 把输出赋给变量
来源：http://eg.lnxyls.cn

files=$(ls -1)
来源：http://lz.muxihuayi.cn

[R38] 管道串联
来源：http://qm.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://rk.asd995.cn

[R39] 重定向标准输出与错误
来源：http://uv.shxzskj.cn

cmd > out.log 2>&1
来源：http://bq.shxzukj.cn

[R40] 追加写日志
来源：http://fm.hahajie.cn

echo "log" >> out.log
来源：http://lz.yuexingan06.cn

[R41] 丢弃输出
来源：http://qt.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://ud.huanxung.cn

[R42] 输入重定向
来源：http://ut.newstarts.cn

wc -l < a.txt
来源：http://gb.shtwfgs.cn

[R43] 按名字查找文件
来源：http://qu.hahajie.cn

find . -name "*.log" -type f
来源：http://wg.wgjwhj.cn

[R44] 按修改时间查找
来源：http://ud.shxzskj.cn

find . -mtime -7 -type f
来源：http://rs.yuexingan06.cn

[R45] 批量删除
来源：http://zu.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://lg.szsharing.cn

[R46] 递归替换文件内容
来源：http://cf.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ux.nicolike.cn

[R47] sed 单行替换
来源：http://mn.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vq.haigaiapp.cn

[R48] awk 取指定列
来源：http://ud.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://en.wgjwhj.cn

[R49] awk 带条件
来源：http://gz.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://id.shxzskj.cn

[R50] awk 求和
来源：http://le.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kh.muxihuayi.cn

[R51] 排序去重取前几
来源：http://yx.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qt.jctech888.com.cn

[R52] 统计行数
来源：http://pe.lnxyls.cn

wc -l a.txt
来源：http://pu.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://og.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ed.lnxyls.cn

[R54] 比较两个文件
来源：http://ts.hahajie.cn

diff a.txt b.txt
来源：http://vu.muxihuayi.cn

[R55] 压缩与解压
来源：http://my.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nf.gzmigu.cn

[R56] 远程拷贝
来源：http://ko.gzmigu.cn

scp file user@host:/path/
来源：http://hy.shxzukj.cn

[R57] 远程执行命令
来源：http://er.bjjhwx.cn

ssh user@host 'uptime'
来源：http://kt.jctech888.com.cn

[R58] 下载文件
来源：http://jf.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xu.shxzukj.cn

[R59] 发 POST JSON
来源：http://yj.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://be.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://bx.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cp.asd995.cn

[R61] 磁盘占用
来源：http://ba.chemitech.net.cn

df -h;  du -sh *
来源：http://pi.nicolike.cn

[R62] 找最占空间的文件
来源：http://is.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://es.jianghongdianzi.cn

[R63] 内存与进程
来源：http://bb.521024.cn

free -h;  ps aux | grep nginx
来源：http://no.colortex.cn

[R64] 结束进程
来源：http://uc.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://zn.gzmigu.cn

[R65] 查看端口占用
来源：http://gm.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oy.muxihuayi.cn

[R66] 定时任务
来源：http://jc.shxzukj.cn

crontab -e;  crontab -l
来源：http://ie.nicolike.cn

[R67] 生成随机十六进制串
来源：http://ft.jianghongdianzi.cn

openssl rand -hex 16
来源：http://ou.9csxet.cn

[R68] 计算文件校验值
来源：http://gq.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cw.shxzukj.cn

[R69] 生成随机密码
来源：http://ae.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://ir.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://ka.newstarts.cn

date +%s;  date -d @1700000000
来源：http://jx.shtwfgs.cn

[R71] 日期格式化
来源：http://uj.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zn.hahajie.cn

[R72] 等待端口就绪
来源：http://so.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yo.lnxyls.cn

[R73] 分割大日志
来源：http://yd.yuexingan06.cn

split -l 1000 big.log part_
来源：http://sf.yuntaijiaju.cn

[R74] 批量重命名
来源：http://tv.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://np.jctech888.com.cn

[R75] 导出环境变量
来源：http://bt.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://hv.jctech888.com.cn

[R76] 使用临时文件
来源：http://js.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ck.colortex.cn

[R77] 读取用户输入
来源：http://uu.yuexingan06.cn

read -rp "请输入: " ans
来源：http://mq.chemitech.net.cn

[R78] 交互式菜单
来源：http://am.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mw.shxzskj.cn

[R79] 解析命令行选项
来源：http://jf.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dj.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://je.szxytkj.cn

time ./run.sh
来源：http://za.asd995.cn

================================================================================
来源：http://up.asd995.cn

S. C / C++ 专题
来源：http://wm.yuexingan06.cn

================================================================================
来源：http://no.huixinmuqiang.cn

[S01] C：Hello World
来源：http://ev.hahajie.cn

#include <stdio.h>
来源：http://lh.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xj.nicolike.cn

[S02] C：变量与格式化输出
来源：http://yd.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://mj.colortex.cn

[S03] C：读入整数
来源：http://ui.lnxyls.cn

int x; scanf("%d", &x);
来源：http://nu.huanxung.cn

[S04] C：字符串复制
来源：http://ok.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vb.szsharing.cn

[S05] C：字符串长度
来源：http://xg.hnjuh.cn


<!-- 参考信息 -->