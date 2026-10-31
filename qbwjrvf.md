代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://xx.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://pg.chemitech.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://al.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://jl.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://is.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://my.gzmigu.cn

[Q43] 标量子查询
来源：http://ye.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pi.shxzskj.cn

[Q44] IN 子查询
来源：http://wn.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ke.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://vi.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ak.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qh.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gh.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://jp.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bx.colortex.cn

[Q48] CTE 公用表表达式
来源：http://sw.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mb.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://ql.nicolike.cn

[Q49] 更新单行
来源：http://sm.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tm.hahajie.cn

[Q50] 批量更新
来源：http://fw.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ml.colortex.cn

[Q51] 用子查询更新
来源：http://wi.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ef.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://cz.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://jw.newstarts.cn

[Q53] 按条件删除
来源：http://xq.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bh.jianghongdianzi.cn

[Q54] 清空表
来源：http://dh.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://em.521024.cn

[Q55] 排名（并列占位）
来源：http://ei.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fn.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://ez.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ef.szsharing.cn

[Q57] 行号
来源：http://ww.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tr.yuexingan06.cn

[Q58] 累计求和
来源：http://qk.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rd.bjjhwx.cn

[Q59] 分组内累计
来源：http://ui.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dp.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://rs.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qf.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zh.shxzukj.cn

[Q61] 移动平均
来源：http://yy.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bs.chemitech.net.cn

[Q62] 分组占比
来源：http://cf.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://er.panjiajie.cn

[Q63] 开启事务
来源：http://rs.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qk.shtwfgs.cn

[Q64] 提交事务
来源：http://es.9csxet.cn

COMMIT;
来源：http://yo.muxihuayi.cn

[Q65] 回滚事务
来源：http://vc.shxzukj.cn

ROLLBACK;
来源：http://cj.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://ir.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nc.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://dk.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lq.lnxyls.cn

[Q68] 保存点
来源：http://cs.asd995.cn

SAVEPOINT sp1;
来源：http://lk.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://tr.9csxet.cn

[Q69] 查看执行计划
来源：http://nb.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wi.newstarts.cn

[Q70] 更新统计信息
来源：http://mq.nicolike.cn

ANALYZE TABLE users;
来源：http://we.jctech888.com.cn

[Q71] 查看建表语句
来源：http://aw.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iw.lnxyls.cn

[Q72] 查看索引
来源：http://lu.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://nv.huixiangedu.cn

[Q73] 查看表状态
来源：http://ik.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://we.colortex.cn

[Q74] 强制使用索引
来源：http://zj.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vg.panjiajie.cn

[Q75] 日期格式化
来源：http://jq.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ij.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vr.521024.cn

[Q76] 按天统计
来源：http://fd.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://or.chemitech.net.cn

[Q77] 时间加减
来源：http://sr.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://np.bookmarksfly.cn

[Q78] 当前时间
来源：http://za.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bs.nicolike.cn

[Q79] 字符串拼接
来源：http://sp.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zt.9csxet.cn

[Q80] 字符串截取
来源：http://ma.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oa.bookmarksfly.cn

[Q81] 字符串替换
来源：http://xv.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ef.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://qi.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yt.colortex.cn

[Q83] 大小写转换
来源：http://th.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://em.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://mq.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://lp.haigaiapp.cn

[Q85] 数值取整
来源：http://bc.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pu.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://fa.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kf.9csxet.cn

[Q87] JSON 字段做条件
来源：http://la.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ys.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://xs.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mi.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yq.nszjky.cn

[Q89] 判断表是否存在
来源：http://wu.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iu.lnxyls.cn

[Q90] 生成序号列
来源：http://lf.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ey.shtwfgs.cn

================================================================================
来源：http://ut.lnxyls.cn

R. Bash 专题
来源：http://ge.nicolike.cn

================================================================================
来源：http://xa.hnjuh.cn

[R01] shebang 与严格模式
来源：http://ay.asd995.cn

#!/usr/bin/env bash
来源：http://mq.asd995.cn

set -euo pipefail
来源：http://yt.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://ko.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://qr.haigaiapp.cn

[R03] 只读变量
来源：http://wu.szsharing.cn

readonly PI=3.14
来源：http://yz.huixiangedu.cn

[R04] 位置参数
来源：http://gl.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dm.shxzskj.cn

[R05] 参数默认值
来源：http://nf.nicolike.cn

name="${1:-default}"
来源：http://el.nszjky.cn

[R06] 判断命令是否存在
来源：http://qk.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://az.gzmigu.cn

[R07] if 判断文件
来源：http://jz.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rw.huixinmuqiang.cn

[R08] 数值比较
来源：http://ew.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kc.jctech888.com.cn

[R09] 字符串比较
来源：http://da.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dq.jianghongdianzi.cn

[R10] 正则匹配
来源：http://el.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xp.nszjky.cn

[R11] case 多分支
来源：http://hk.9csxet.cn

case "$1" in
来源：http://xa.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://ue.hahajie.cn

stop)  echo "停止" ;;
来源：http://xd.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://py.521024.cn

esac
来源：http://fs.huanxung.cn

[R12] for 遍历文件
来源：http://xk.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://ia.panjiajie.cn

[R13] for 计数循环
来源：http://ga.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://qk.lnxyls.cn

[R14] C 风格 for
来源：http://ki.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rm.haigaiapp.cn

[R15] while 逐行读文件
来源：http://ez.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hj.hnjuh.cn

[R16] until 等待条件
来源：http://ti.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hr.muxihuayi.cn

[R17] 数组定义与取值
来源：http://in.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sl.newstarts.cn

[R18] 遍历数组
来源：http://rk.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ul.nszjky.cn

[R19] 数组长度
来源：http://nv.szxytkj.cn

echo "${#arr[@]}"
来源：http://el.panjiajie.cn

[R20] 关联数组（字典）
来源：http://yr.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bs.szsharing.cn

[R21] 字符串长度
来源：http://ld.huanxung.cn

echo "${#s}"
来源：http://kn.muxihuayi.cn

[R22] 截取子串
来源：http://nw.wgjwhj.cn

echo "${s:0:5}"
来源：http://zv.yuntaijiaju.cn

[R23] 字符串替换
来源：http://mj.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zb.jianghongdianzi.cn

[R24] 大小写转换
来源：http://qb.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hg.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://fc.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://su.hahajie.cn

[R26] 命令替换
来源：http://ts.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://bo.nszjky.cn

[R27] 算术展开
来源：http://dt.nicolike.cn

echo $((1 + 2 * 3))
来源：http://bb.gzmigu.cn

[R28] 浮点运算
来源：http://zd.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://ch.newstarts.cn

[R29] 定义函数
来源：http://fq.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xe.asd995.cn

[R30] 函数返回状态码
来源：http://vb.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://ru.wgjwhj.cn

[R31] 局部变量
来源：http://ng.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://zr.yuexingan06.cn

[R32] 参数个数校验
来源：http://kz.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pn.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://te.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://di.szxytkj.cn

[R34] 退出时清理
来源：http://vm.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uf.newstarts.cn

[R35] 后台执行并等待
来源：http://zc.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sg.colortex.cn

[R36] 并发执行多个任务
来源：http://pv.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pv.asd995.cn

[R37] 把输出赋给变量
来源：http://vk.jianghongdianzi.cn

files=$(ls -1)
来源：http://nm.hnjuh.cn

[R38] 管道串联
来源：http://br.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://df.521024.cn

[R39] 重定向标准输出与错误
来源：http://bx.szxytkj.cn

cmd > out.log 2>&1
来源：http://yd.shxzukj.cn

[R40] 追加写日志
来源：http://fe.haigaiapp.cn

echo "log" >> out.log
来源：http://et.bjjhwx.cn

[R41] 丢弃输出
来源：http://ov.nicolike.cn

cmd >/dev/null 2>&1
来源：http://kk.hahajie.cn

[R42] 输入重定向
来源：http://cv.huixinmuqiang.cn

wc -l < a.txt
来源：http://sx.gzmigu.cn

[R43] 按名字查找文件
来源：http://hp.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://ay.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://dc.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://mk.yuexingan06.cn

[R45] 批量删除
来源：http://mq.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://mx.asd995.cn

[R46] 递归替换文件内容
来源：http://kz.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://if.asd995.cn

[R47] sed 单行替换
来源：http://il.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qg.nicolike.cn

[R48] awk 取指定列
来源：http://cn.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://lg.jianghongdianzi.cn

[R49] awk 带条件
来源：http://yl.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hy.nszjky.cn

[R50] awk 求和
来源：http://rl.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://in.muxihuayi.cn

[R51] 排序去重取前几
来源：http://lj.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wp.lnxyls.cn

[R52] 统计行数
来源：http://pl.jctech888.com.cn

wc -l a.txt
来源：http://sd.521024.cn

[R53] 查看文件头与实时尾
来源：http://mk.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ex.nicolike.cn

[R54] 比较两个文件
来源：http://kk.jianghongdianzi.cn

diff a.txt b.txt
来源：http://rp.asd995.cn

[R55] 压缩与解压
来源：http://fh.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rd.jctech888.com.cn

[R56] 远程拷贝
来源：http://st.asd995.cn

scp file user@host:/path/
来源：http://xh.yuexingan06.cn

[R57] 远程执行命令
来源：http://ui.huixiangedu.cn

ssh user@host 'uptime'
来源：http://uh.nicolike.cn

[R58] 下载文件
来源：http://sl.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pq.huanxung.cn

[R59] 发 POST JSON
来源：http://br.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sp.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://hz.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gi.panjiajie.cn

[R61] 磁盘占用
来源：http://ia.521024.cn

df -h;  du -sh *
来源：http://mp.asd995.cn

[R62] 找最占空间的文件
来源：http://pn.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://ve.muxihuayi.cn

[R63] 内存与进程
来源：http://lc.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://ih.521024.cn

[R64] 结束进程
来源：http://oe.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://nh.lnxyls.cn

[R65] 查看端口占用
来源：http://dk.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hi.bookmarksfly.cn

[R66] 定时任务
来源：http://tg.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://wj.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://gl.huixinmuqiang.cn

openssl rand -hex 16
来源：http://yx.hnjuh.cn

[R68] 计算文件校验值
来源：http://rm.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tp.nszjky.cn

[R69] 生成随机密码
来源：http://fz.521024.cn

head -c 16 /dev/urandom | base64
来源：http://vy.521024.cn

[R70] 时间戳与互转
来源：http://bw.asd995.cn

date +%s;  date -d @1700000000
来源：http://os.asd995.cn

[R71] 日期格式化
来源：http://tm.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cp.yuexingan06.cn

[R72] 等待端口就绪
来源：http://wc.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dd.nszjky.cn

[R73] 分割大日志
来源：http://zf.521024.cn

split -l 1000 big.log part_
来源：http://un.muxihuayi.cn

[R74] 批量重命名
来源：http://fe.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jk.yuexingan06.cn

[R75] 导出环境变量
来源：http://xl.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://cf.nszjky.cn

[R76] 使用临时文件
来源：http://ud.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ts.haigaiapp.cn

[R77] 读取用户输入
来源：http://cv.huixiangedu.cn

read -rp "请输入: " ans
来源：http://at.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://kt.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vv.gzmigu.cn

[R79] 解析命令行选项
来源：http://nb.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vz.521024.cn

[R80] 查看脚本执行耗时
来源：http://zb.9csxet.cn

time ./run.sh
来源：http://tj.bjjhwx.cn

================================================================================
来源：http://gt.shxzskj.cn

S. C / C++ 专题
来源：http://pr.shtwfgs.cn

================================================================================
来源：http://uq.wgjwhj.cn

[S01] C：Hello World
来源：http://it.huanxung.cn

#include <stdio.h>
来源：http://ur.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cw.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://wc.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://dq.jctech888.com.cn

[S03] C：读入整数
来源：http://nl.huanxung.cn

int x; scanf("%d", &x);
来源：http://eh.szxytkj.cn

[S04] C：字符串复制
来源：http://zb.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oy.lnxyls.cn

[S05] C：字符串长度
来源：http://ul.yuexingan06.cn

strlen(s)
来源：http://jk.huixiangedu.cn

[S06] C：字符串比较
来源：http://yh.shtwfgs.cn

strcmp(a, b) == 0
来源：http://bw.shxzukj.cn

[S07] C：数组遍历求和
来源：http://ve.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qx.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://yx.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hu.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://yz.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yr.9csxet.cn

[S10] C：指针与解引用
来源：http://it.nicolike.cn

int *p = &a;  *p = 5;
来源：http://oz.muxihuayi.cn

[S11] C：逐行读文件
来源：http://qn.lnxyls.cn


<!-- 参考信息 -->