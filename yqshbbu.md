代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://ui.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jj.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://wb.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gh.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://am.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cw.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sb.hahajie.cn

[Q41] 多表连接
来源：http://qh.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wo.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://xt.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://bt.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://fr.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://na.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vf.colortex.cn

[Q43] 标量子查询
来源：http://ks.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tj.nicolike.cn

[Q44] IN 子查询
来源：http://jk.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jz.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://he.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pn.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ju.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tp.hahajie.cn

[Q47] 与平均值比较
来源：http://vw.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vj.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://vh.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ak.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://vv.shxzukj.cn

[Q49] 更新单行
来源：http://fb.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yy.9csxet.cn

[Q50] 批量更新
来源：http://bb.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ft.haigaiapp.cn

[Q51] 用子查询更新
来源：http://az.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ik.szsharing.cn

[Q52] 删除指定行
来源：http://yc.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://rq.huixiangedu.cn

[Q53] 按条件删除
来源：http://ti.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yh.newstarts.cn

[Q54] 清空表
来源：http://qj.szsharing.cn

TRUNCATE TABLE logs;
来源：http://hb.nicolike.cn

[Q55] 排名（并列占位）
来源：http://of.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xy.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://ee.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://on.yuntaijiaju.cn

[Q57] 行号
来源：http://ck.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mk.panjiajie.cn

[Q58] 累计求和
来源：http://cz.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wk.521024.cn

[Q59] 分组内累计
来源：http://rp.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rh.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://gv.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://su.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ma.szsharing.cn

[Q61] 移动平均
来源：http://ec.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tk.nicolike.cn

[Q62] 分组占比
来源：http://mw.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rc.hahajie.cn

[Q63] 开启事务
来源：http://od.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ex.chemitech.net.cn

[Q64] 提交事务
来源：http://oc.szsharing.cn

COMMIT;
来源：http://jk.yuexingan06.cn

[Q65] 回滚事务
来源：http://jw.shxzskj.cn

ROLLBACK;
来源：http://or.shxzskj.cn

[Q66] 行锁查询
来源：http://ld.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ds.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://iv.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ss.gzmigu.cn

[Q68] 保存点
来源：http://dv.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://es.hahajie.cn

ROLLBACK TO sp1;
来源：http://bh.wgjwhj.cn

[Q69] 查看执行计划
来源：http://uy.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pk.chemitech.net.cn

[Q70] 更新统计信息
来源：http://qf.jctech888.com.cn

ANALYZE TABLE users;
来源：http://fh.szxytkj.cn

[Q71] 查看建表语句
来源：http://gw.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fx.szsharing.cn

[Q72] 查看索引
来源：http://dp.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://gs.wgjwhj.cn

[Q73] 查看表状态
来源：http://td.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cc.lnxyls.cn

[Q74] 强制使用索引
来源：http://oq.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vt.9csxet.cn

[Q75] 日期格式化
来源：http://xg.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kh.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zs.jctech888.com.cn

[Q76] 按天统计
来源：http://fz.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gl.chemitech.net.cn

[Q77] 时间加减
来源：http://rt.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yt.521024.cn

[Q78] 当前时间
来源：http://uz.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://br.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://gz.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fr.huanxung.cn

[Q80] 字符串截取
来源：http://ny.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aq.521024.cn

[Q81] 字符串替换
来源：http://ul.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yd.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://ry.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pq.colortex.cn

[Q83] 大小写转换
来源：http://pl.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cn.9csxet.cn

[Q84] 去除首尾空格
来源：http://ua.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://st.yuntaijiaju.cn

[Q85] 数值取整
来源：http://sc.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jk.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://rg.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iq.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://xa.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zf.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://lv.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mo.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zd.szxytkj.cn

[Q89] 判断表是否存在
来源：http://ji.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dp.nszjky.cn

[Q90] 生成序号列
来源：http://gv.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://om.huixinmuqiang.cn

================================================================================
来源：http://vw.gzmigu.cn

R. Bash 专题
来源：http://oj.huixinmuqiang.cn

================================================================================
来源：http://tz.nszjky.cn

[R01] shebang 与严格模式
来源：http://bx.jctech888.com.cn

#!/usr/bin/env bash
来源：http://su.521024.cn

set -euo pipefail
来源：http://nb.hnjuh.cn

[R02] 变量赋值与使用
来源：http://kk.521024.cn

name="Tom"; echo "$name"
来源：http://hh.szxytkj.cn

[R03] 只读变量
来源：http://hj.jctech888.com.cn

readonly PI=3.14
来源：http://bw.szxytkj.cn

[R04] 位置参数
来源：http://tn.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cd.jianghongdianzi.cn

[R05] 参数默认值
来源：http://dt.hahajie.cn

name="${1:-default}"
来源：http://qk.521024.cn

[R06] 判断命令是否存在
来源：http://bo.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ls.yuexingan06.cn

[R07] if 判断文件
来源：http://xz.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lm.nicolike.cn

[R08] 数值比较
来源：http://og.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nw.nicolike.cn

[R09] 字符串比较
来源：http://fd.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mk.bookmarksfly.cn

[R10] 正则匹配
来源：http://cv.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kf.shxzskj.cn

[R11] case 多分支
来源：http://aw.nicolike.cn

case "$1" in
来源：http://le.newstarts.cn

start) echo "启动" ;;
来源：http://ia.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://xx.szsharing.cn

*)     echo "未知命令" ;;
来源：http://an.hnjuh.cn

esac
来源：http://uf.muxihuayi.cn

[R12] for 遍历文件
来源：http://zl.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://ce.chemitech.net.cn

[R13] for 计数循环
来源：http://ef.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://io.bookmarksfly.cn

[R14] C 风格 for
来源：http://qv.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://br.9csxet.cn

[R15] while 逐行读文件
来源：http://jn.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oa.shtwfgs.cn

[R16] until 等待条件
来源：http://vm.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://to.yuexingan06.cn

[R17] 数组定义与取值
来源：http://fh.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oc.huixinmuqiang.cn

[R18] 遍历数组
来源：http://bm.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ng.yuntaijiaju.cn

[R19] 数组长度
来源：http://iy.shxzukj.cn

echo "${#arr[@]}"
来源：http://oa.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://mu.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fe.huixinmuqiang.cn

[R21] 字符串长度
来源：http://gu.huixinmuqiang.cn

echo "${#s}"
来源：http://fu.shxzskj.cn

[R22] 截取子串
来源：http://yu.nszjky.cn

echo "${s:0:5}"
来源：http://uc.panjiajie.cn

[R23] 字符串替换
来源：http://qf.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xs.shtwfgs.cn

[R24] 大小写转换
来源：http://qj.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://aa.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://kd.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hu.gzmigu.cn

[R26] 命令替换
来源：http://hv.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://zn.huanxung.cn

[R27] 算术展开
来源：http://gp.newstarts.cn

echo $((1 + 2 * 3))
来源：http://kd.yuexingan06.cn

[R28] 浮点运算
来源：http://wp.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://yx.yuntaijiaju.cn

[R29] 定义函数
来源：http://ei.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ss.huixiangedu.cn

[R30] 函数返回状态码
来源：http://ve.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://ah.nicolike.cn

[R31] 局部变量
来源：http://wn.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://vx.shtwfgs.cn

[R32] 参数个数校验
来源：http://cl.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lx.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://uh.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lq.9csxet.cn

[R34] 退出时清理
来源：http://xl.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://py.haigaiapp.cn

[R35] 后台执行并等待
来源：http://wl.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sd.nicolike.cn

[R36] 并发执行多个任务
来源：http://ww.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oa.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://ll.asd995.cn

files=$(ls -1)
来源：http://yj.nszjky.cn

[R38] 管道串联
来源：http://cs.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://if.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://qc.521024.cn

cmd > out.log 2>&1
来源：http://ki.bookmarksfly.cn

[R40] 追加写日志
来源：http://vo.9csxet.cn

echo "log" >> out.log
来源：http://jc.nicolike.cn

[R41] 丢弃输出
来源：http://sf.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://ti.shtwfgs.cn

[R42] 输入重定向
来源：http://jg.huixinmuqiang.cn

wc -l < a.txt
来源：http://yz.hahajie.cn

[R43] 按名字查找文件
来源：http://wa.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://lz.yuexingan06.cn

[R44] 按修改时间查找
来源：http://cf.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://yn.chemitech.net.cn

[R45] 批量删除
来源：http://np.asd995.cn

find . -name "*.tmp" -delete
来源：http://wk.521024.cn

[R46] 递归替换文件内容
来源：http://iv.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cu.haigaiapp.cn

[R47] sed 单行替换
来源：http://vu.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rh.hnjuh.cn

[R48] awk 取指定列
来源：http://pl.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://wi.nszjky.cn

[R49] awk 带条件
来源：http://hv.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fz.muxihuayi.cn

[R50] awk 求和
来源：http://rn.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://du.haigaiapp.cn

[R51] 排序去重取前几
来源：http://xl.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gd.yuexingan06.cn

[R52] 统计行数
来源：http://dq.nicolike.cn

wc -l a.txt
来源：http://rk.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://bn.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gh.haigaiapp.cn

[R54] 比较两个文件
来源：http://cm.bookmarksfly.cn

diff a.txt b.txt
来源：http://gk.wgjwhj.cn

[R55] 压缩与解压
来源：http://li.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://od.gzmigu.cn

[R56] 远程拷贝
来源：http://ia.huixiangedu.cn

scp file user@host:/path/
来源：http://ce.shxzskj.cn

[R57] 远程执行命令
来源：http://ec.panjiajie.cn

ssh user@host 'uptime'
来源：http://co.szxytkj.cn

[R58] 下载文件
来源：http://ad.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ms.gzmigu.cn

[R59] 发 POST JSON
来源：http://il.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kj.521024.cn

[R60] 只看 HTTP 状态码
来源：http://vx.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lg.bookmarksfly.cn

[R61] 磁盘占用
来源：http://hx.9csxet.cn

df -h;  du -sh *
来源：http://pf.lnxyls.cn

[R62] 找最占空间的文件
来源：http://jo.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://xt.haigaiapp.cn

[R63] 内存与进程
来源：http://td.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://qs.muxihuayi.cn

[R64] 结束进程
来源：http://wd.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://jy.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://lf.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ka.huixiangedu.cn

[R66] 定时任务
来源：http://ue.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://ry.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://xp.huixinmuqiang.cn

openssl rand -hex 16
来源：http://lk.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://tx.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qe.colortex.cn

[R69] 生成随机密码
来源：http://nq.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://dl.wgjwhj.cn

[R70] 时间戳与互转
来源：http://yh.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://pj.shxzskj.cn

[R71] 日期格式化
来源：http://ak.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ua.shxzukj.cn

[R72] 等待端口就绪
来源：http://cu.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eh.huixiangedu.cn

[R73] 分割大日志
来源：http://hs.colortex.cn

split -l 1000 big.log part_
来源：http://ev.huixiangedu.cn

[R74] 批量重命名
来源：http://uz.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uu.jctech888.com.cn

[R75] 导出环境变量
来源：http://xn.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://uy.bookmarksfly.cn

[R76] 使用临时文件
来源：http://np.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qj.szxytkj.cn

[R77] 读取用户输入
来源：http://jk.lnxyls.cn

read -rp "请输入: " ans
来源：http://qn.chemitech.net.cn

[R78] 交互式菜单
来源：http://yp.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ul.haigaiapp.cn

[R79] 解析命令行选项
来源：http://cf.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xs.521024.cn

[R80] 查看脚本执行耗时
来源：http://nw.bookmarksfly.cn

time ./run.sh
来源：http://iu.521024.cn

================================================================================
来源：http://sw.jctech888.com.cn

S. C / C++ 专题
来源：http://hq.9csxet.cn

================================================================================
来源：http://db.huixiangedu.cn

[S01] C：Hello World
来源：http://rw.wgjwhj.cn

#include <stdio.h>
来源：http://yh.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gy.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://bu.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://nq.newstarts.cn

[S03] C：读入整数
来源：http://hh.panjiajie.cn

int x; scanf("%d", &x);
来源：http://fu.huixiangedu.cn

[S04] C：字符串复制
来源：http://uf.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kh.colortex.cn

[S05] C：字符串长度
来源：http://eo.hahajie.cn

strlen(s)
来源：http://ww.szxytkj.cn

[S06] C：字符串比较
来源：http://rg.9csxet.cn

strcmp(a, b) == 0
来源：http://kb.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://rb.muxihuayi.cn


<!-- 参考信息 -->