代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ib.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vl.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jy.colortex.cn

[Q41] 多表连接
来源：http://cp.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ub.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://yb.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://aw.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://id.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://ao.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fh.szxytkj.cn

[Q43] 标量子查询
来源：http://nz.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lz.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://jj.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mt.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://je.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nq.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vs.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tv.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://fd.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ns.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://ga.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ce.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://iz.gzmigu.cn

[Q49] 更新单行
来源：http://tj.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ve.huixinmuqiang.cn

[Q50] 批量更新
来源：http://jv.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://el.521024.cn

[Q51] 用子查询更新
来源：http://vg.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ci.colortex.cn

[Q52] 删除指定行
来源：http://qm.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://ax.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://av.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rd.jianghongdianzi.cn

[Q54] 清空表
来源：http://as.huanxung.cn

TRUNCATE TABLE logs;
来源：http://cw.asd995.cn

[Q55] 排名（并列占位）
来源：http://ta.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dl.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://uq.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qr.hnjuh.cn

[Q57] 行号
来源：http://uk.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hk.jianghongdianzi.cn

[Q58] 累计求和
来源：http://be.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jf.asd995.cn

[Q59] 分组内累计
来源：http://xu.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yv.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://im.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yv.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://et.9csxet.cn

[Q61] 移动平均
来源：http://gy.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dw.haigaiapp.cn

[Q62] 分组占比
来源：http://ql.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://by.muxihuayi.cn

[Q63] 开启事务
来源：http://gf.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yj.bookmarksfly.cn

[Q64] 提交事务
来源：http://zt.nszjky.cn

COMMIT;
来源：http://wv.colortex.cn

[Q65] 回滚事务
来源：http://wc.bjjhwx.cn

ROLLBACK;
来源：http://to.gzmigu.cn

[Q66] 行锁查询
来源：http://fa.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uf.nicolike.cn

[Q67] 设置隔离级别
来源：http://qm.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rd.nszjky.cn

[Q68] 保存点
来源：http://nv.jianghongdianzi.cn

SAVEPOINT sp1;
来源：http://li.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://np.shtwfgs.cn

[Q69] 查看执行计划
来源：http://ng.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bo.newstarts.cn

[Q70] 更新统计信息
来源：http://fs.haigaiapp.cn

ANALYZE TABLE users;
来源：http://um.chemitech.net.cn

[Q71] 查看建表语句
来源：http://by.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kd.9csxet.cn

[Q72] 查看索引
来源：http://az.521024.cn

SHOW INDEX FROM users;
来源：http://sf.szxytkj.cn

[Q73] 查看表状态
来源：http://hy.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lg.jctech888.com.cn

[Q74] 强制使用索引
来源：http://om.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ki.hahajie.cn

[Q75] 日期格式化
来源：http://ur.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kc.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vh.gzmigu.cn

[Q76] 按天统计
来源：http://oz.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pa.huixiangedu.cn

[Q77] 时间加减
来源：http://fy.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ke.huixiangedu.cn

[Q78] 当前时间
来源：http://xx.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ar.hahajie.cn

[Q79] 字符串拼接
来源：http://zp.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yv.bookmarksfly.cn

[Q80] 字符串截取
来源：http://mv.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zy.nicolike.cn

[Q81] 字符串替换
来源：http://ao.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gk.asd995.cn

[Q82] 字符长度与字节长度
来源：http://gt.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jr.yuexingan06.cn

[Q83] 大小写转换
来源：http://oo.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vn.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://sz.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://ar.haigaiapp.cn

[Q85] 数值取整
来源：http://um.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ev.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://pg.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bz.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://zn.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hf.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://rh.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vh.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ej.szsharing.cn

[Q89] 判断表是否存在
来源：http://tv.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hp.haigaiapp.cn

[Q90] 生成序号列
来源：http://bx.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hm.jctech888.com.cn

================================================================================
来源：http://tg.newstarts.cn

R. Bash 专题
来源：http://ng.lnxyls.cn

================================================================================
来源：http://cv.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://tz.gzmigu.cn

#!/usr/bin/env bash
来源：http://bc.asd995.cn

set -euo pipefail
来源：http://nb.szsharing.cn

[R02] 变量赋值与使用
来源：http://gi.szxytkj.cn

name="Tom"; echo "$name"
来源：http://on.szsharing.cn

[R03] 只读变量
来源：http://lx.jctech888.com.cn

readonly PI=3.14
来源：http://cf.panjiajie.cn

[R04] 位置参数
来源：http://gg.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://id.wgjwhj.cn

[R05] 参数默认值
来源：http://rs.521024.cn

name="${1:-default}"
来源：http://ut.szxytkj.cn

[R06] 判断命令是否存在
来源：http://sg.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yf.nicolike.cn

[R07] if 判断文件
来源：http://vo.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ii.nszjky.cn

[R08] 数值比较
来源：http://xy.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ke.bookmarksfly.cn

[R09] 字符串比较
来源：http://ef.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ps.yuexingan06.cn

[R10] 正则匹配
来源：http://uq.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kf.newstarts.cn

[R11] case 多分支
来源：http://ig.521024.cn

case "$1" in
来源：http://au.panjiajie.cn

start) echo "启动" ;;
来源：http://rs.521024.cn

stop)  echo "停止" ;;
来源：http://fc.521024.cn

*)     echo "未知命令" ;;
来源：http://nb.panjiajie.cn

esac
来源：http://ga.jctech888.com.cn

[R12] for 遍历文件
来源：http://fr.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://fi.szsharing.cn

[R13] for 计数循环
来源：http://qd.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://dp.shtwfgs.cn

[R14] C 风格 for
来源：http://uy.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ps.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://gs.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://df.521024.cn

[R16] until 等待条件
来源：http://vy.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vc.muxihuayi.cn

[R17] 数组定义与取值
来源：http://jl.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cv.wgjwhj.cn

[R18] 遍历数组
来源：http://bv.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mb.chemitech.net.cn

[R19] 数组长度
来源：http://gr.newstarts.cn

echo "${#arr[@]}"
来源：http://zp.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://jm.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ye.jianghongdianzi.cn

[R21] 字符串长度
来源：http://mh.nicolike.cn

echo "${#s}"
来源：http://rr.szxytkj.cn

[R22] 截取子串
来源：http://lv.muxihuayi.cn

echo "${s:0:5}"
来源：http://sh.asd995.cn

[R23] 字符串替换
来源：http://zr.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ic.colortex.cn

[R24] 大小写转换
来源：http://rd.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://aa.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://vn.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jj.huanxung.cn

[R26] 命令替换
来源：http://gl.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://ow.huanxung.cn

[R27] 算术展开
来源：http://wf.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://qo.shxzukj.cn

[R28] 浮点运算
来源：http://ol.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://um.yuexingan06.cn

[R29] 定义函数
来源：http://vz.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ck.yuntaijiaju.cn

[R30] 函数返回状态码
来源：http://hg.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://ly.huixiangedu.cn

[R31] 局部变量
来源：http://mm.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://gy.hnjuh.cn

[R32] 参数个数校验
来源：http://xy.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nl.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://uk.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://el.nicolike.cn

[R34] 退出时清理
来源：http://ee.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ly.shxzukj.cn

[R35] 后台执行并等待
来源：http://cb.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ci.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://ee.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kb.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://ep.lnxyls.cn

files=$(ls -1)
来源：http://jm.hnjuh.cn

[R38] 管道串联
来源：http://eq.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://fo.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://kq.yuexingan06.cn

cmd > out.log 2>&1
来源：http://nj.szsharing.cn

[R40] 追加写日志
来源：http://nc.shxzukj.cn

echo "log" >> out.log
来源：http://lp.yuexingan06.cn

[R41] 丢弃输出
来源：http://my.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://nm.szxytkj.cn

[R42] 输入重定向
来源：http://kd.szxytkj.cn

wc -l < a.txt
来源：http://iv.jctech888.com.cn

[R43] 按名字查找文件
来源：http://yo.panjiajie.cn

find . -name "*.log" -type f
来源：http://ed.colortex.cn

[R44] 按修改时间查找
来源：http://km.shxzukj.cn

find . -mtime -7 -type f
来源：http://jj.huanxung.cn

[R45] 批量删除
来源：http://ey.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://hx.shxzukj.cn

[R46] 递归替换文件内容
来源：http://sv.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oo.bjjhwx.cn

[R47] sed 单行替换
来源：http://dk.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zr.nicolike.cn

[R48] awk 取指定列
来源：http://be.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://rf.muxihuayi.cn

[R49] awk 带条件
来源：http://en.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hb.nicolike.cn

[R50] awk 求和
来源：http://nz.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mh.szsharing.cn

[R51] 排序去重取前几
来源：http://bk.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vk.szxytkj.cn

[R52] 统计行数
来源：http://dq.jianghongdianzi.cn

wc -l a.txt
来源：http://cl.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://pa.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wt.nszjky.cn

[R54] 比较两个文件
来源：http://sg.jianghongdianzi.cn

diff a.txt b.txt
来源：http://wt.shxzskj.cn

[R55] 压缩与解压
来源：http://ss.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jy.jctech888.com.cn

[R56] 远程拷贝
来源：http://ns.jctech888.com.cn

scp file user@host:/path/
来源：http://tc.asd995.cn

[R57] 远程执行命令
来源：http://ew.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://lc.lnxyls.cn

[R58] 下载文件
来源：http://ti.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ym.colortex.cn

[R59] 发 POST JSON
来源：http://qg.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://np.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://zj.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pj.asd995.cn

[R61] 磁盘占用
来源：http://oe.yuntaijiaju.cn

df -h;  du -sh *
来源：http://nb.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://ev.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://mm.shtwfgs.cn

[R63] 内存与进程
来源：http://mf.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://rf.9csxet.cn

[R64] 结束进程
来源：http://np.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://yd.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://hh.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://se.nicolike.cn

[R66] 定时任务
来源：http://oj.yuexingan06.cn

crontab -e;  crontab -l
来源：http://zi.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://vq.huanxung.cn

openssl rand -hex 16
来源：http://rr.hnjuh.cn

[R68] 计算文件校验值
来源：http://dr.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ux.szxytkj.cn

[R69] 生成随机密码
来源：http://df.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://bf.szsharing.cn

[R70] 时间戳与互转
来源：http://av.hahajie.cn

date +%s;  date -d @1700000000
来源：http://ao.jctech888.com.cn

[R71] 日期格式化
来源：http://cx.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qg.chemitech.net.cn

[R72] 等待端口就绪
来源：http://jk.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://el.bjjhwx.cn

[R73] 分割大日志
来源：http://fy.9csxet.cn

split -l 1000 big.log part_
来源：http://pe.yuexingan06.cn

[R74] 批量重命名
来源：http://qc.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kl.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://zr.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://tv.shtwfgs.cn

[R76] 使用临时文件
来源：http://oq.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ma.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://dd.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://ak.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://lh.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ut.chemitech.net.cn

[R79] 解析命令行选项
来源：http://ml.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ve.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://gl.jianghongdianzi.cn

time ./run.sh
来源：http://hz.gzmigu.cn

================================================================================
来源：http://rm.jctech888.com.cn

S. C / C++ 专题
来源：http://qd.haigaiapp.cn

================================================================================
来源：http://vw.panjiajie.cn

[S01] C：Hello World
来源：http://pa.asd995.cn

#include <stdio.h>
来源：http://pb.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tn.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://wi.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://ls.lnxyls.cn

[S03] C：读入整数
来源：http://yv.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://ib.hahajie.cn

[S04] C：字符串复制
来源：http://ty.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://af.lnxyls.cn

[S05] C：字符串长度
来源：http://wj.jianghongdianzi.cn

strlen(s)
来源：http://ko.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://pq.huixiangedu.cn

strcmp(a, b) == 0
来源：http://ou.newstarts.cn

[S07] C：数组遍历求和
来源：http://fl.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ur.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://yu.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uu.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://fk.shxzskj.cn


<!-- 参考信息 -->