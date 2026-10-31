代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://qg.nicolike.cn

[Q30] 分组统计
来源：http://by.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sl.hahajie.cn

[Q31] 分组后过滤
来源：http://vg.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lg.9csxet.cn

[Q32] 分组拼接字符串
来源：http://ky.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rm.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wl.colortex.cn

[Q33] 多列分组
来源：http://kr.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kk.hnjuh.cn

[Q34] 每组取第一条
来源：http://mj.521024.cn

SELECT * FROM (
来源：http://we.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nb.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://wt.yuexingan06.cn

[Q35] 内连接
来源：http://wu.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pu.newstarts.cn

[Q36] 左连接
来源：http://yz.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ou.hahajie.cn

[Q37] 右连接
来源：http://jq.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zq.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qj.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ub.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://no.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qg.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ps.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://oj.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oh.huixiangedu.cn

[Q41] 多表连接
来源：http://nc.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ky.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://cw.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://rr.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://kh.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://dq.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bs.asd995.cn

[Q43] 标量子查询
来源：http://gv.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sn.szxytkj.cn

[Q44] IN 子查询
来源：http://bp.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jo.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://pa.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://th.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lg.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bz.wgjwhj.cn

[Q47] 与平均值比较
来源：http://br.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oa.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://em.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hp.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://ly.shxzukj.cn

[Q49] 更新单行
来源：http://ly.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eq.hahajie.cn

[Q50] 批量更新
来源：http://rl.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gj.szxytkj.cn

[Q51] 用子查询更新
来源：http://mh.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oq.panjiajie.cn

[Q52] 删除指定行
来源：http://jd.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://tt.panjiajie.cn

[Q53] 按条件删除
来源：http://bd.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vw.bjjhwx.cn

[Q54] 清空表
来源：http://dn.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://xb.nicolike.cn

[Q55] 排名（并列占位）
来源：http://ud.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ju.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://cu.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qq.shxzskj.cn

[Q57] 行号
来源：http://hz.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sb.szxytkj.cn

[Q58] 累计求和
来源：http://xu.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iu.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://wz.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://np.huixiangedu.cn

[Q60] 取上一行 / 下一行
来源：http://cw.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kt.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lt.nszjky.cn

[Q61] 移动平均
来源：http://ww.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vg.szxytkj.cn

[Q62] 分组占比
来源：http://uq.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ws.lnxyls.cn

[Q63] 开启事务
来源：http://cx.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qx.muxihuayi.cn

[Q64] 提交事务
来源：http://cn.wgjwhj.cn

COMMIT;
来源：http://qz.shxzskj.cn

[Q65] 回滚事务
来源：http://qr.wgjwhj.cn

ROLLBACK;
来源：http://us.muxihuayi.cn

[Q66] 行锁查询
来源：http://kc.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ef.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://dg.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://js.newstarts.cn

[Q68] 保存点
来源：http://vq.hahajie.cn

SAVEPOINT sp1;
来源：http://yk.lnxyls.cn

ROLLBACK TO sp1;
来源：http://fo.521024.cn

[Q69] 查看执行计划
来源：http://vj.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zp.panjiajie.cn

[Q70] 更新统计信息
来源：http://bg.lnxyls.cn

ANALYZE TABLE users;
来源：http://ua.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://vu.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yf.bjjhwx.cn

[Q72] 查看索引
来源：http://su.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://dg.newstarts.cn

[Q73] 查看表状态
来源：http://di.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lm.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://up.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qp.nicolike.cn

[Q75] 日期格式化
来源：http://ge.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uo.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kv.szxytkj.cn

[Q76] 按天统计
来源：http://wj.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jz.muxihuayi.cn

[Q77] 时间加减
来源：http://od.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jb.shtwfgs.cn

[Q78] 当前时间
来源：http://ir.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ch.muxihuayi.cn

[Q79] 字符串拼接
来源：http://dv.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://si.jianghongdianzi.cn

[Q80] 字符串截取
来源：http://yc.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rw.jianghongdianzi.cn

[Q81] 字符串替换
来源：http://xu.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nq.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://vr.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gd.muxihuayi.cn

[Q83] 大小写转换
来源：http://gm.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://id.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://cp.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://wk.chemitech.net.cn

[Q85] 数值取整
来源：http://ef.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cv.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://he.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hj.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://qh.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oo.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://yb.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ux.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pd.panjiajie.cn

[Q89] 判断表是否存在
来源：http://hm.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ks.haigaiapp.cn

[Q90] 生成序号列
来源：http://ug.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xm.szxytkj.cn

================================================================================
来源：http://ji.hnjuh.cn

R. Bash 专题
来源：http://lc.bookmarksfly.cn

================================================================================
来源：http://jr.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://td.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://jp.muxihuayi.cn

set -euo pipefail
来源：http://ij.nicolike.cn

[R02] 变量赋值与使用
来源：http://ef.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://yr.gzmigu.cn

[R03] 只读变量
来源：http://by.nicolike.cn

readonly PI=3.14
来源：http://ci.shxzukj.cn

[R04] 位置参数
来源：http://rb.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dm.bjjhwx.cn

[R05] 参数默认值
来源：http://sk.haigaiapp.cn

name="${1:-default}"
来源：http://xi.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://wd.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lz.colortex.cn

[R07] if 判断文件
来源：http://sn.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ux.bookmarksfly.cn

[R08] 数值比较
来源：http://eq.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ws.newstarts.cn

[R09] 字符串比较
来源：http://bl.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tg.muxihuayi.cn

[R10] 正则匹配
来源：http://ub.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://os.9csxet.cn

[R11] case 多分支
来源：http://up.bookmarksfly.cn

case "$1" in
来源：http://vh.huanxung.cn

start) echo "启动" ;;
来源：http://yb.521024.cn

stop)  echo "停止" ;;
来源：http://wb.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://pa.jctech888.com.cn

esac
来源：http://da.huixiangedu.cn

[R12] for 遍历文件
来源：http://es.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://bb.huixinmuqiang.cn

[R13] for 计数循环
来源：http://qp.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://ho.yuntaijiaju.cn

[R14] C 风格 for
来源：http://wt.9csxet.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qz.muxihuayi.cn

[R15] while 逐行读文件
来源：http://vy.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xd.szsharing.cn

[R16] until 等待条件
来源：http://kd.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dx.hnjuh.cn

[R17] 数组定义与取值
来源：http://on.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ki.wgjwhj.cn

[R18] 遍历数组
来源：http://pp.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tp.yuntaijiaju.cn

[R19] 数组长度
来源：http://fg.521024.cn

echo "${#arr[@]}"
来源：http://to.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://lh.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wo.huanxung.cn

[R21] 字符串长度
来源：http://hx.muxihuayi.cn

echo "${#s}"
来源：http://ak.asd995.cn

[R22] 截取子串
来源：http://ur.jctech888.com.cn

echo "${s:0:5}"
来源：http://ce.yuexingan06.cn

[R23] 字符串替换
来源：http://uj.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bt.yuntaijiaju.cn

[R24] 大小写转换
来源：http://ob.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://by.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://km.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://da.panjiajie.cn

[R26] 命令替换
来源：http://fg.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://ly.panjiajie.cn

[R27] 算术展开
来源：http://bc.521024.cn

echo $((1 + 2 * 3))
来源：http://wb.huixinmuqiang.cn

[R28] 浮点运算
来源：http://kq.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://xj.yuntaijiaju.cn

[R29] 定义函数
来源：http://mf.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bj.colortex.cn

[R30] 函数返回状态码
来源：http://vi.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://dj.newstarts.cn

[R31] 局部变量
来源：http://gd.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://sy.szxytkj.cn

[R32] 参数个数校验
来源：http://te.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://le.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://kt.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tm.colortex.cn

[R34] 退出时清理
来源：http://pz.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sm.huanxung.cn

[R35] 后台执行并等待
来源：http://cz.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lk.huanxung.cn

[R36] 并发执行多个任务
来源：http://cf.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fi.hnjuh.cn

[R37] 把输出赋给变量
来源：http://mt.wgjwhj.cn

files=$(ls -1)
来源：http://hy.nszjky.cn

[R38] 管道串联
来源：http://hs.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://fb.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://jf.9csxet.cn

cmd > out.log 2>&1
来源：http://tw.jianghongdianzi.cn

[R40] 追加写日志
来源：http://pi.haigaiapp.cn

echo "log" >> out.log
来源：http://ep.colortex.cn

[R41] 丢弃输出
来源：http://ev.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://bm.muxihuayi.cn

[R42] 输入重定向
来源：http://qz.521024.cn

wc -l < a.txt
来源：http://tk.szsharing.cn

[R43] 按名字查找文件
来源：http://ug.newstarts.cn

find . -name "*.log" -type f
来源：http://so.szxytkj.cn

[R44] 按修改时间查找
来源：http://gz.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://qs.haigaiapp.cn

[R45] 批量删除
来源：http://wk.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://qq.asd995.cn

[R46] 递归替换文件内容
来源：http://tp.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zn.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://cn.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kz.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://et.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://mg.bookmarksfly.cn

[R49] awk 带条件
来源：http://bm.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://em.yuntaijiaju.cn

[R50] awk 求和
来源：http://sd.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hd.wgjwhj.cn

[R51] 排序去重取前几
来源：http://cs.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dx.wgjwhj.cn

[R52] 统计行数
来源：http://bn.chemitech.net.cn

wc -l a.txt
来源：http://gt.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://eq.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oz.nicolike.cn

[R54] 比较两个文件
来源：http://ha.lnxyls.cn

diff a.txt b.txt
来源：http://wb.huanxung.cn

[R55] 压缩与解压
来源：http://hl.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://co.shtwfgs.cn

[R56] 远程拷贝
来源：http://tn.nszjky.cn

scp file user@host:/path/
来源：http://ho.nicolike.cn

[R57] 远程执行命令
来源：http://zo.yuexingan06.cn

ssh user@host 'uptime'
来源：http://lc.shxzskj.cn

[R58] 下载文件
来源：http://jb.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hj.521024.cn

[R59] 发 POST JSON
来源：http://cw.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ap.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://zj.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sk.szxytkj.cn

[R61] 磁盘占用
来源：http://my.szsharing.cn

df -h;  du -sh *
来源：http://kg.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://aa.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://rp.521024.cn

[R63] 内存与进程
来源：http://to.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://ig.muxihuayi.cn

[R64] 结束进程
来源：http://qi.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://nb.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://lc.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sj.jctech888.com.cn

[R66] 定时任务
来源：http://do.yuexingan06.cn

crontab -e;  crontab -l
来源：http://vw.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://un.shtwfgs.cn

openssl rand -hex 16
来源：http://bl.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://hf.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lh.panjiajie.cn

[R69] 生成随机密码
来源：http://zy.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://nq.szxytkj.cn

[R70] 时间戳与互转
来源：http://fh.521024.cn

date +%s;  date -d @1700000000
来源：http://id.panjiajie.cn

[R71] 日期格式化
来源：http://fm.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xo.asd995.cn

[R72] 等待端口就绪
来源：http://wr.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fg.shxzukj.cn

[R73] 分割大日志
来源：http://gb.haigaiapp.cn

split -l 1000 big.log part_
来源：http://vf.bookmarksfly.cn

[R74] 批量重命名
来源：http://pl.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ts.szxytkj.cn

[R75] 导出环境变量
来源：http://ug.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://ey.bookmarksfly.cn

[R76] 使用临时文件
来源：http://ka.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kg.hnjuh.cn

[R77] 读取用户输入
来源：http://vt.gzmigu.cn

read -rp "请输入: " ans
来源：http://tq.nszjky.cn

[R78] 交互式菜单
来源：http://kz.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pq.huixiangedu.cn

[R79] 解析命令行选项
来源：http://sn.asd995.cn


<!-- 参考信息 -->