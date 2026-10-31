代发 wailian999

[Q33] 多列分组
来源：http://pw.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wt.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://ii.521024.cn

SELECT * FROM (
来源：http://iz.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://la.lnxyls.cn

) t WHERE rn = 1;
来源：http://tf.bookmarksfly.cn

[Q35] 内连接
来源：http://ni.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sq.shxzukj.cn

[Q36] 左连接
来源：http://pv.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://av.muxihuayi.cn

[Q37] 右连接
来源：http://hd.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qx.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sy.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tj.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://yv.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dw.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://md.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vr.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://od.szsharing.cn

[Q41] 多表连接
来源：http://cl.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://am.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://mf.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://ut.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://ma.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://nz.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://al.nszjky.cn

[Q43] 标量子查询
来源：http://iy.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ol.huixiangedu.cn

[Q44] IN 子查询
来源：http://po.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://od.asd995.cn

[Q45] EXISTS 判断存在
来源：http://pq.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dd.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gd.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ma.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://lc.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mp.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://et.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pq.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://bv.szxytkj.cn

[Q49] 更新单行
来源：http://gb.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fi.shxzskj.cn

[Q50] 批量更新
来源：http://cz.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xw.colortex.cn

[Q51] 用子查询更新
来源：http://yy.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yo.bjjhwx.cn

[Q52] 删除指定行
来源：http://fs.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://kp.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://em.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ce.shtwfgs.cn

[Q54] 清空表
来源：http://kn.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://uq.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://az.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ps.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://mb.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gn.shtwfgs.cn

[Q57] 行号
来源：http://ch.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tc.muxihuayi.cn

[Q58] 累计求和
来源：http://xi.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pw.huixiangedu.cn

[Q59] 分组内累计
来源：http://kb.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vx.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://me.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://om.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rm.yuntaijiaju.cn

[Q61] 移动平均
来源：http://eb.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oh.szsharing.cn

[Q62] 分组占比
来源：http://ym.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dm.nicolike.cn

[Q63] 开启事务
来源：http://ax.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rv.bjjhwx.cn

[Q64] 提交事务
来源：http://ba.hahajie.cn

COMMIT;
来源：http://za.nicolike.cn

[Q65] 回滚事务
来源：http://mj.521024.cn

ROLLBACK;
来源：http://zw.shxzukj.cn

[Q66] 行锁查询
来源：http://ky.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ie.nicolike.cn

[Q67] 设置隔离级别
来源：http://hz.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xw.asd995.cn

[Q68] 保存点
来源：http://cs.521024.cn

SAVEPOINT sp1;
来源：http://df.521024.cn

ROLLBACK TO sp1;
来源：http://hw.nszjky.cn

[Q69] 查看执行计划
来源：http://pn.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hd.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://cs.muxihuayi.cn

ANALYZE TABLE users;
来源：http://xa.bjjhwx.cn

[Q71] 查看建表语句
来源：http://id.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pd.nszjky.cn

[Q72] 查看索引
来源：http://yc.nszjky.cn

SHOW INDEX FROM users;
来源：http://hc.panjiajie.cn

[Q73] 查看表状态
来源：http://mk.521024.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ci.9csxet.cn

[Q74] 强制使用索引
来源：http://dw.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://or.nszjky.cn

[Q75] 日期格式化
来源：http://ip.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kh.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vl.nicolike.cn

[Q76] 按天统计
来源：http://du.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ew.shxzskj.cn

[Q77] 时间加减
来源：http://wp.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mc.jianghongdianzi.cn

[Q78] 当前时间
来源：http://yp.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jh.jctech888.com.cn

[Q79] 字符串拼接
来源：http://zy.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mi.nicolike.cn

[Q80] 字符串截取
来源：http://cn.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jk.wgjwhj.cn

[Q81] 字符串替换
来源：http://wx.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vf.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://cn.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gn.bookmarksfly.cn

[Q83] 大小写转换
来源：http://qo.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cf.gzmigu.cn

[Q84] 去除首尾空格
来源：http://vi.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://wz.muxihuayi.cn

[Q85] 数值取整
来源：http://vv.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bc.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://vx.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nm.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://wy.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rf.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://gd.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lp.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tg.lnxyls.cn

[Q89] 判断表是否存在
来源：http://in.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ax.yuexingan06.cn

[Q90] 生成序号列
来源：http://ro.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tq.huixinmuqiang.cn

================================================================================
来源：http://ej.colortex.cn

R. Bash 专题
来源：http://py.shtwfgs.cn

================================================================================
来源：http://bp.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://ym.yuexingan06.cn

#!/usr/bin/env bash
来源：http://vm.shtwfgs.cn

set -euo pipefail
来源：http://fx.hnjuh.cn

[R02] 变量赋值与使用
来源：http://aa.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://cx.wgjwhj.cn

[R03] 只读变量
来源：http://pm.shxzukj.cn

readonly PI=3.14
来源：http://qd.lnxyls.cn

[R04] 位置参数
来源：http://lq.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kw.9csxet.cn

[R05] 参数默认值
来源：http://yt.yuntaijiaju.cn

name="${1:-default}"
来源：http://mb.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://kk.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mt.haigaiapp.cn

[R07] if 判断文件
来源：http://zs.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://we.newstarts.cn

[R08] 数值比较
来源：http://wq.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pz.yuexingan06.cn

[R09] 字符串比较
来源：http://dz.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://od.wgjwhj.cn

[R10] 正则匹配
来源：http://fu.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vy.hahajie.cn

[R11] case 多分支
来源：http://ls.szxytkj.cn

case "$1" in
来源：http://mn.haigaiapp.cn

start) echo "启动" ;;
来源：http://bk.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://uf.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://ow.nszjky.cn

esac
来源：http://iq.bookmarksfly.cn

[R12] for 遍历文件
来源：http://bd.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://an.szsharing.cn

[R13] for 计数循环
来源：http://lg.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://dt.yuexingan06.cn

[R14] C 风格 for
来源：http://ni.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lv.hnjuh.cn

[R15] while 逐行读文件
来源：http://ap.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ag.hahajie.cn

[R16] until 等待条件
来源：http://uf.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dj.gzmigu.cn

[R17] 数组定义与取值
来源：http://xl.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cl.bjjhwx.cn

[R18] 遍历数组
来源：http://oc.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yz.szsharing.cn

[R19] 数组长度
来源：http://gf.jctech888.com.cn

echo "${#arr[@]}"
来源：http://bv.521024.cn

[R20] 关联数组（字典）
来源：http://mm.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hn.yuntaijiaju.cn

[R21] 字符串长度
来源：http://pu.shtwfgs.cn

echo "${#s}"
来源：http://xk.shxzskj.cn

[R22] 截取子串
来源：http://yz.hnjuh.cn

echo "${s:0:5}"
来源：http://nv.huixiangedu.cn

[R23] 字符串替换
来源：http://ly.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gm.gzmigu.cn

[R24] 大小写转换
来源：http://fh.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yg.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://qf.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sy.yuexingan06.cn

[R26] 命令替换
来源：http://cf.haigaiapp.cn

now=$(date +%F); echo "$now"
来源：http://yq.bjjhwx.cn

[R27] 算术展开
来源：http://vn.hahajie.cn

echo $((1 + 2 * 3))
来源：http://yd.szxytkj.cn

[R28] 浮点运算
来源：http://tr.521024.cn

echo "scale=2; 10/3" | bc
来源：http://sr.shxzukj.cn

[R29] 定义函数
来源：http://ge.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jq.nszjky.cn

[R30] 函数返回状态码
来源：http://kq.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://mh.asd995.cn

[R31] 局部变量
来源：http://xp.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://tt.hnjuh.cn

[R32] 参数个数校验
来源：http://eh.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qq.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://un.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vk.panjiajie.cn

[R34] 退出时清理
来源：http://xg.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jg.521024.cn

[R35] 后台执行并等待
来源：http://lt.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vo.gzmigu.cn

[R36] 并发执行多个任务
来源：http://gt.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ag.panjiajie.cn

[R37] 把输出赋给变量
来源：http://oa.lnxyls.cn

files=$(ls -1)
来源：http://oo.9csxet.cn

[R38] 管道串联
来源：http://rh.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://qt.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://im.muxihuayi.cn

cmd > out.log 2>&1
来源：http://xr.bjjhwx.cn

[R40] 追加写日志
来源：http://sk.lnxyls.cn

echo "log" >> out.log
来源：http://dc.szxytkj.cn

[R41] 丢弃输出
来源：http://rs.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://gu.nicolike.cn

[R42] 输入重定向
来源：http://yx.asd995.cn

wc -l < a.txt
来源：http://uf.shxzukj.cn

[R43] 按名字查找文件
来源：http://wm.hnjuh.cn

find . -name "*.log" -type f
来源：http://wn.nszjky.cn

[R44] 按修改时间查找
来源：http://zk.bjjhwx.cn

find . -mtime -7 -type f
来源：http://mp.521024.cn

[R45] 批量删除
来源：http://el.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://id.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://lw.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pk.wgjwhj.cn

[R47] sed 单行替换
来源：http://tq.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qa.nicolike.cn

[R48] awk 取指定列
来源：http://ll.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://xi.haigaiapp.cn

[R49] awk 带条件
来源：http://sx.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://by.huixiangedu.cn

[R50] awk 求和
来源：http://nx.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mb.lnxyls.cn

[R51] 排序去重取前几
来源：http://zu.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ma.lnxyls.cn

[R52] 统计行数
来源：http://bq.newstarts.cn

wc -l a.txt
来源：http://px.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://do.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yb.9csxet.cn

[R54] 比较两个文件
来源：http://ty.nszjky.cn

diff a.txt b.txt
来源：http://rb.hnjuh.cn

[R55] 压缩与解压
来源：http://nx.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jc.shtwfgs.cn

[R56] 远程拷贝
来源：http://zv.haigaiapp.cn

scp file user@host:/path/
来源：http://cu.bookmarksfly.cn

[R57] 远程执行命令
来源：http://rx.lnxyls.cn

ssh user@host 'uptime'
来源：http://xt.jctech888.com.cn

[R58] 下载文件
来源：http://lh.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hy.muxihuayi.cn

[R59] 发 POST JSON
来源：http://vy.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ry.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://vi.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vc.nicolike.cn

[R61] 磁盘占用
来源：http://ba.gzmigu.cn

df -h;  du -sh *
来源：http://eg.shxzukj.cn

[R62] 找最占空间的文件
来源：http://oy.521024.cn

du -ah . | sort -rh | head -10
来源：http://qc.hahajie.cn

[R63] 内存与进程
来源：http://mq.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://hd.shxzskj.cn

[R64] 结束进程
来源：http://gc.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://fd.muxihuayi.cn

[R65] 查看端口占用
来源：http://lo.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://if.bjjhwx.cn

[R66] 定时任务
来源：http://wg.wgjwhj.cn

crontab -e;  crontab -l
来源：http://ln.huanxung.cn

[R67] 生成随机十六进制串
来源：http://sk.521024.cn

openssl rand -hex 16
来源：http://uj.chemitech.net.cn

[R68] 计算文件校验值
来源：http://mu.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://up.wgjwhj.cn

[R69] 生成随机密码
来源：http://iy.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://wv.lnxyls.cn

[R70] 时间戳与互转
来源：http://dj.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://rx.asd995.cn

[R71] 日期格式化
来源：http://ft.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ym.9csxet.cn

[R72] 等待端口就绪
来源：http://gh.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ci.wgjwhj.cn

[R73] 分割大日志
来源：http://su.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://ou.szsharing.cn

[R74] 批量重命名
来源：http://qh.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zs.chemitech.net.cn

[R75] 导出环境变量
来源：http://ev.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://ma.nszjky.cn

[R76] 使用临时文件
来源：http://oe.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vo.asd995.cn

[R77] 读取用户输入
来源：http://kk.huixiangedu.cn

read -rp "请输入: " ans
来源：http://rk.shtwfgs.cn

[R78] 交互式菜单
来源：http://sg.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ae.lnxyls.cn

[R79] 解析命令行选项
来源：http://bz.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tu.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://dy.newstarts.cn

time ./run.sh
来源：http://sp.jianghongdianzi.cn

================================================================================
来源：http://op.panjiajie.cn

S. C / C++ 专题
来源：http://et.colortex.cn

================================================================================
来源：http://xo.huanxung.cn

[S01] C：Hello World
来源：http://ka.huixinmuqiang.cn

#include <stdio.h>
来源：http://ml.lnxyls.cn


<!-- 参考信息 -->