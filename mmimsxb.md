代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://ui.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pd.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://pb.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://eb.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ug.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qv.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jw.nszjky.cn

[Q41] 多表连接
来源：http://wh.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dw.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://cx.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://qv.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://ui.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://hb.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xd.asd995.cn

[Q43] 标量子查询
来源：http://at.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mu.chemitech.net.cn

[Q44] IN 子查询
来源：http://ob.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qn.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://io.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bd.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kg.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dv.huanxung.cn

[Q47] 与平均值比较
来源：http://ea.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vs.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://kz.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bc.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://xu.9csxet.cn

[Q49] 更新单行
来源：http://sz.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dg.bjjhwx.cn

[Q50] 批量更新
来源：http://eh.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vs.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://zb.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ip.9csxet.cn

[Q52] 删除指定行
来源：http://uv.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://hc.huanxung.cn

[Q53] 按条件删除
来源：http://lw.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kc.hnjuh.cn

[Q54] 清空表
来源：http://eo.newstarts.cn

TRUNCATE TABLE logs;
来源：http://rh.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://pg.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://po.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://mv.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ux.hnjuh.cn

[Q57] 行号
来源：http://ys.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nm.shxzskj.cn

[Q58] 累计求和
来源：http://ie.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://or.huixiangedu.cn

[Q59] 分组内累计
来源：http://ts.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jq.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://ep.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bt.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ur.bjjhwx.cn

[Q61] 移动平均
来源：http://dl.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sj.shxzskj.cn

[Q62] 分组占比
来源：http://hy.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zn.hnjuh.cn

[Q63] 开启事务
来源：http://dy.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ej.521024.cn

[Q64] 提交事务
来源：http://zh.shtwfgs.cn

COMMIT;
来源：http://fz.huanxung.cn

[Q65] 回滚事务
来源：http://ro.chemitech.net.cn

ROLLBACK;
来源：http://ba.shxzukj.cn

[Q66] 行锁查询
来源：http://kt.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jd.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://aj.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mr.lnxyls.cn

[Q68] 保存点
来源：http://um.huanxung.cn

SAVEPOINT sp1;
来源：http://dw.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://ie.huixiangedu.cn

[Q69] 查看执行计划
来源：http://pt.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xj.shxzukj.cn

[Q70] 更新统计信息
来源：http://xq.jctech888.com.cn

ANALYZE TABLE users;
来源：http://qu.newstarts.cn

[Q71] 查看建表语句
来源：http://jm.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zt.colortex.cn

[Q72] 查看索引
来源：http://ji.panjiajie.cn

SHOW INDEX FROM users;
来源：http://qf.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://us.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qc.jctech888.com.cn

[Q74] 强制使用索引
来源：http://wz.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aq.nszjky.cn

[Q75] 日期格式化
来源：http://qi.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mz.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vl.asd995.cn

[Q76] 按天统计
来源：http://el.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hs.asd995.cn

[Q77] 时间加减
来源：http://xg.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eu.asd995.cn

[Q78] 当前时间
来源：http://sd.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pt.hnjuh.cn

[Q79] 字符串拼接
来源：http://rn.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ma.lnxyls.cn

[Q80] 字符串截取
来源：http://mk.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wm.panjiajie.cn

[Q81] 字符串替换
来源：http://xg.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wi.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://dd.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://og.hnjuh.cn

[Q83] 大小写转换
来源：http://di.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jn.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://jt.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://ya.gzmigu.cn

[Q85] 数值取整
来源：http://kl.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lz.colortex.cn

[Q86] 读取 JSON 字段
来源：http://xj.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ma.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://tb.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://us.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://hi.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bd.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://od.shxzukj.cn

[Q89] 判断表是否存在
来源：http://ch.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://la.shtwfgs.cn

[Q90] 生成序号列
来源：http://fk.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vj.521024.cn

================================================================================
来源：http://ir.jctech888.com.cn

R. Bash 专题
来源：http://wm.nszjky.cn

================================================================================
来源：http://gd.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://mj.colortex.cn

#!/usr/bin/env bash
来源：http://tq.521024.cn

set -euo pipefail
来源：http://id.colortex.cn

[R02] 变量赋值与使用
来源：http://zf.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://xk.bookmarksfly.cn

[R03] 只读变量
来源：http://yv.lnxyls.cn

readonly PI=3.14
来源：http://zs.shxzskj.cn

[R04] 位置参数
来源：http://pt.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://id.jctech888.com.cn

[R05] 参数默认值
来源：http://ao.yuntaijiaju.cn

name="${1:-default}"
来源：http://xq.szxytkj.cn

[R06] 判断命令是否存在
来源：http://vb.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uu.nszjky.cn

[R07] if 判断文件
来源：http://dk.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fe.521024.cn

[R08] 数值比较
来源：http://kb.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pl.huixinmuqiang.cn

[R09] 字符串比较
来源：http://ib.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fu.szxytkj.cn

[R10] 正则匹配
来源：http://wu.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ht.newstarts.cn

[R11] case 多分支
来源：http://uv.huanxung.cn

case "$1" in
来源：http://uf.colortex.cn

start) echo "启动" ;;
来源：http://jb.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://kc.nicolike.cn

*)     echo "未知命令" ;;
来源：http://ri.wgjwhj.cn

esac
来源：http://xk.hahajie.cn

[R12] for 遍历文件
来源：http://ka.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://ji.gzmigu.cn

[R13] for 计数循环
来源：http://vt.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://fe.yuntaijiaju.cn

[R14] C 风格 for
来源：http://ey.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ih.9csxet.cn

[R15] while 逐行读文件
来源：http://su.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pu.yuntaijiaju.cn

[R16] until 等待条件
来源：http://hw.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mu.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://tq.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fv.huixinmuqiang.cn

[R18] 遍历数组
来源：http://pn.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wf.jianghongdianzi.cn

[R19] 数组长度
来源：http://zi.newstarts.cn

echo "${#arr[@]}"
来源：http://mb.hnjuh.cn

[R20] 关联数组（字典）
来源：http://jv.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ah.bookmarksfly.cn

[R21] 字符串长度
来源：http://ia.yuexingan06.cn

echo "${#s}"
来源：http://vi.hnjuh.cn

[R22] 截取子串
来源：http://gz.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://su.asd995.cn

[R23] 字符串替换
来源：http://vz.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dr.hnjuh.cn

[R24] 大小写转换
来源：http://hr.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fr.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://vx.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vy.shtwfgs.cn

[R26] 命令替换
来源：http://yo.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://bi.haigaiapp.cn

[R27] 算术展开
来源：http://mi.521024.cn

echo $((1 + 2 * 3))
来源：http://cb.newstarts.cn

[R28] 浮点运算
来源：http://jw.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://il.huanxung.cn

[R29] 定义函数
来源：http://sb.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rw.szsharing.cn

[R30] 函数返回状态码
来源：http://gy.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://no.yuexingan06.cn

[R31] 局部变量
来源：http://pr.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://uq.9csxet.cn

[R32] 参数个数校验
来源：http://lx.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://in.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://uj.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xh.muxihuayi.cn

[R34] 退出时清理
来源：http://er.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://co.bjjhwx.cn

[R35] 后台执行并等待
来源：http://jg.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gz.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://kv.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qo.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://zj.haigaiapp.cn

files=$(ls -1)
来源：http://am.yuexingan06.cn

[R38] 管道串联
来源：http://lb.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://wa.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://cw.nicolike.cn

cmd > out.log 2>&1
来源：http://ai.szxytkj.cn

[R40] 追加写日志
来源：http://hs.muxihuayi.cn

echo "log" >> out.log
来源：http://ow.bjjhwx.cn

[R41] 丢弃输出
来源：http://od.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://so.jianghongdianzi.cn

[R42] 输入重定向
来源：http://ov.lnxyls.cn

wc -l < a.txt
来源：http://hy.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://ak.newstarts.cn

find . -name "*.log" -type f
来源：http://cu.521024.cn

[R44] 按修改时间查找
来源：http://ql.huanxung.cn

find . -mtime -7 -type f
来源：http://kj.lnxyls.cn

[R45] 批量删除
来源：http://fk.nszjky.cn

find . -name "*.tmp" -delete
来源：http://rg.huanxung.cn

[R46] 递归替换文件内容
来源：http://dk.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zp.colortex.cn

[R47] sed 单行替换
来源：http://hn.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ic.wgjwhj.cn

[R48] awk 取指定列
来源：http://mk.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://fi.colortex.cn

[R49] awk 带条件
来源：http://bj.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ye.jctech888.com.cn

[R50] awk 求和
来源：http://uz.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ro.hnjuh.cn

[R51] 排序去重取前几
来源：http://wz.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fu.hahajie.cn

[R52] 统计行数
来源：http://tn.chemitech.net.cn

wc -l a.txt
来源：http://jl.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://xx.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wg.521024.cn

[R54] 比较两个文件
来源：http://qi.haigaiapp.cn

diff a.txt b.txt
来源：http://ho.chemitech.net.cn

[R55] 压缩与解压
来源：http://hu.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://of.hahajie.cn

[R56] 远程拷贝
来源：http://mb.colortex.cn

scp file user@host:/path/
来源：http://qh.shtwfgs.cn

[R57] 远程执行命令
来源：http://wl.jctech888.com.cn

ssh user@host 'uptime'
来源：http://ra.lnxyls.cn

[R58] 下载文件
来源：http://nw.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ly.9csxet.cn

[R59] 发 POST JSON
来源：http://vd.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ic.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://yr.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nc.hnjuh.cn

[R61] 磁盘占用
来源：http://pt.bjjhwx.cn

df -h;  du -sh *
来源：http://oi.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://fs.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://xw.jianghongdianzi.cn

[R63] 内存与进程
来源：http://an.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://jb.yuexingan06.cn

[R64] 结束进程
来源：http://az.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://ky.szxytkj.cn

[R65] 查看端口占用
来源：http://xt.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rw.muxihuayi.cn

[R66] 定时任务
来源：http://qf.hnjuh.cn

crontab -e;  crontab -l
来源：http://zy.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://un.panjiajie.cn

openssl rand -hex 16
来源：http://yy.muxihuayi.cn

[R68] 计算文件校验值
来源：http://uj.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fd.huanxung.cn

[R69] 生成随机密码
来源：http://fy.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://qm.haigaiapp.cn

[R70] 时间戳与互转
来源：http://mn.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://iw.szxytkj.cn

[R71] 日期格式化
来源：http://od.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dq.szxytkj.cn

[R72] 等待端口就绪
来源：http://pn.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xm.szxytkj.cn

[R73] 分割大日志
来源：http://sq.lnxyls.cn

split -l 1000 big.log part_
来源：http://bd.huixiangedu.cn

[R74] 批量重命名
来源：http://in.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://po.asd995.cn

[R75] 导出环境变量
来源：http://jx.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://gu.colortex.cn

[R76] 使用临时文件
来源：http://uh.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vr.muxihuayi.cn

[R77] 读取用户输入
来源：http://pi.hahajie.cn

read -rp "请输入: " ans
来源：http://tm.muxihuayi.cn

[R78] 交互式菜单
来源：http://vq.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://it.bjjhwx.cn

[R79] 解析命令行选项
来源：http://dq.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nt.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://ek.hnjuh.cn

time ./run.sh
来源：http://wz.haigaiapp.cn

================================================================================
来源：http://ed.huanxung.cn

S. C / C++ 专题
来源：http://fk.jctech888.com.cn

================================================================================
来源：http://cf.huixinmuqiang.cn

[S01] C：Hello World
来源：http://wl.bjjhwx.cn

#include <stdio.h>
来源：http://tp.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ih.hahajie.cn

[S02] C：变量与格式化输出
来源：http://rp.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://ww.nszjky.cn

[S03] C：读入整数
来源：http://mw.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://sx.bjjhwx.cn

[S04] C：字符串复制
来源：http://mz.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jp.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://fg.yuntaijiaju.cn

strlen(s)
来源：http://vo.colortex.cn

[S06] C：字符串比较
来源：http://tw.shxzukj.cn

strcmp(a, b) == 0
来源：http://vc.hnjuh.cn

[S07] C：数组遍历求和
来源：http://dt.shxzukj.cn


<!-- 参考信息 -->