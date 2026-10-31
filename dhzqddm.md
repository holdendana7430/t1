代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dz.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qv.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bo.nszjky.cn

[Q41] 多表连接
来源：http://en.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yz.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://fc.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://tk.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://zo.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://qs.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pa.huixinmuqiang.cn

[Q43] 标量子查询
来源：http://sq.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hd.hnjuh.cn

[Q44] IN 子查询
来源：http://dg.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ln.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://en.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pn.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uh.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rp.panjiajie.cn

[Q47] 与平均值比较
来源：http://rp.jianghongdianzi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bs.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://cm.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ot.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://lm.shtwfgs.cn

[Q49] 更新单行
来源：http://ks.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://my.panjiajie.cn

[Q50] 批量更新
来源：http://iw.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sk.chemitech.net.cn

[Q51] 用子查询更新
来源：http://wn.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gx.nicolike.cn

[Q52] 删除指定行
来源：http://zj.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://ci.jctech888.com.cn

[Q53] 按条件删除
来源：http://ov.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yz.lnxyls.cn

[Q54] 清空表
来源：http://eg.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://om.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://wp.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ub.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://bm.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iw.chemitech.net.cn

[Q57] 行号
来源：http://xf.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wy.wgjwhj.cn

[Q58] 累计求和
来源：http://jv.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pg.haigaiapp.cn

[Q59] 分组内累计
来源：http://ah.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://un.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://vz.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fe.jianghongdianzi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://so.jctech888.com.cn

[Q61] 移动平均
来源：http://ar.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rn.szsharing.cn

[Q62] 分组占比
来源：http://nj.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ru.panjiajie.cn

[Q63] 开启事务
来源：http://nj.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nt.asd995.cn

[Q64] 提交事务
来源：http://ff.shtwfgs.cn

COMMIT;
来源：http://to.shxzukj.cn

[Q65] 回滚事务
来源：http://wa.shxzukj.cn

ROLLBACK;
来源：http://qc.9csxet.cn

[Q66] 行锁查询
来源：http://yh.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://no.colortex.cn

[Q67] 设置隔离级别
来源：http://pw.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yl.hahajie.cn

[Q68] 保存点
来源：http://fq.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://ba.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://jn.yuexingan06.cn

[Q69] 查看执行计划
来源：http://mb.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qw.panjiajie.cn

[Q70] 更新统计信息
来源：http://tq.shxzukj.cn

ANALYZE TABLE users;
来源：http://wk.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://rt.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hb.nszjky.cn

[Q72] 查看索引
来源：http://qs.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://jq.asd995.cn

[Q73] 查看表状态
来源：http://pz.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nd.shtwfgs.cn

[Q74] 强制使用索引
来源：http://sk.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mk.huixiangedu.cn

[Q75] 日期格式化
来源：http://ex.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vv.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rl.yuexingan06.cn

[Q76] 按天统计
来源：http://tr.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dl.panjiajie.cn

[Q77] 时间加减
来源：http://sq.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rh.bjjhwx.cn

[Q78] 当前时间
来源：http://rh.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://av.bjjhwx.cn

[Q79] 字符串拼接
来源：http://qq.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ve.szxytkj.cn

[Q80] 字符串截取
来源：http://gp.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yw.asd995.cn

[Q81] 字符串替换
来源：http://qe.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zk.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://ah.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ky.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://qb.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bu.521024.cn

[Q84] 去除首尾空格
来源：http://bg.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://mk.nicolike.cn

[Q85] 数值取整
来源：http://ys.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aj.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://jt.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dh.nicolike.cn

[Q87] JSON 字段做条件
来源：http://su.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ia.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://fu.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tx.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dm.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://km.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sl.wgjwhj.cn

[Q90] 生成序号列
来源：http://dp.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mm.shxzskj.cn

================================================================================
来源：http://pd.shxzskj.cn

R. Bash 专题
来源：http://bv.gzmigu.cn

================================================================================
来源：http://nl.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://rk.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://vh.nicolike.cn

set -euo pipefail
来源：http://nx.gzmigu.cn

[R02] 变量赋值与使用
来源：http://oa.nicolike.cn

name="Tom"; echo "$name"
来源：http://yy.yuexingan06.cn

[R03] 只读变量
来源：http://ak.jianghongdianzi.cn

readonly PI=3.14
来源：http://um.bjjhwx.cn

[R04] 位置参数
来源：http://ry.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jv.hnjuh.cn

[R05] 参数默认值
来源：http://ht.shxzskj.cn

name="${1:-default}"
来源：http://oq.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://lm.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://db.szxytkj.cn

[R07] if 判断文件
来源：http://ig.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://op.shxzukj.cn

[R08] 数值比较
来源：http://wn.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ml.nszjky.cn

[R09] 字符串比较
来源：http://tl.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nn.muxihuayi.cn

[R10] 正则匹配
来源：http://gu.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vy.hnjuh.cn

[R11] case 多分支
来源：http://om.bjjhwx.cn

case "$1" in
来源：http://jz.nicolike.cn

start) echo "启动" ;;
来源：http://hp.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://zh.hahajie.cn

*)     echo "未知命令" ;;
来源：http://fk.hnjuh.cn

esac
来源：http://wa.gzmigu.cn

[R12] for 遍历文件
来源：http://sc.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://xr.hnjuh.cn

[R13] for 计数循环
来源：http://kl.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://qd.szsharing.cn

[R14] C 风格 for
来源：http://zc.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ew.huixiangedu.cn

[R15] while 逐行读文件
来源：http://nr.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mu.wgjwhj.cn

[R16] until 等待条件
来源：http://qa.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ls.muxihuayi.cn

[R17] 数组定义与取值
来源：http://hk.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lb.wgjwhj.cn

[R18] 遍历数组
来源：http://jm.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wy.jctech888.com.cn

[R19] 数组长度
来源：http://qa.bjjhwx.cn

echo "${#arr[@]}"
来源：http://bz.panjiajie.cn

[R20] 关联数组（字典）
来源：http://ol.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kl.wgjwhj.cn

[R21] 字符串长度
来源：http://ql.muxihuayi.cn

echo "${#s}"
来源：http://xy.huixiangedu.cn

[R22] 截取子串
来源：http://jq.hahajie.cn

echo "${s:0:5}"
来源：http://pl.nicolike.cn

[R23] 字符串替换
来源：http://et.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tu.asd995.cn

[R24] 大小写转换
来源：http://gl.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yw.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://vf.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mt.wgjwhj.cn

[R26] 命令替换
来源：http://ez.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://mn.bjjhwx.cn

[R27] 算术展开
来源：http://ev.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://qr.haigaiapp.cn

[R28] 浮点运算
来源：http://vr.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://nr.nszjky.cn

[R29] 定义函数
来源：http://kv.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hf.haigaiapp.cn

[R30] 函数返回状态码
来源：http://nw.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://if.panjiajie.cn

[R31] 局部变量
来源：http://fn.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://hj.huanxung.cn

[R32] 参数个数校验
来源：http://wh.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yv.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://fv.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yg.bjjhwx.cn

[R34] 退出时清理
来源：http://hx.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ui.gzmigu.cn

[R35] 后台执行并等待
来源：http://cd.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oz.nicolike.cn

[R36] 并发执行多个任务
来源：http://ra.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ig.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://kk.panjiajie.cn

files=$(ls -1)
来源：http://di.nszjky.cn

[R38] 管道串联
来源：http://qt.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://re.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://ct.panjiajie.cn

cmd > out.log 2>&1
来源：http://dd.wgjwhj.cn

[R40] 追加写日志
来源：http://xu.yuexingan06.cn

echo "log" >> out.log
来源：http://cv.szsharing.cn

[R41] 丢弃输出
来源：http://ec.nszjky.cn

cmd >/dev/null 2>&1
来源：http://nx.nicolike.cn

[R42] 输入重定向
来源：http://dy.asd995.cn

wc -l < a.txt
来源：http://wg.jctech888.com.cn

[R43] 按名字查找文件
来源：http://rj.shxzukj.cn

find . -name "*.log" -type f
来源：http://no.panjiajie.cn

[R44] 按修改时间查找
来源：http://td.shtwfgs.cn

find . -mtime -7 -type f
来源：http://jt.yuexingan06.cn

[R45] 批量删除
来源：http://pm.nicolike.cn

find . -name "*.tmp" -delete
来源：http://dw.shxzukj.cn

[R46] 递归替换文件内容
来源：http://gy.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qx.panjiajie.cn

[R47] sed 单行替换
来源：http://kr.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lc.huanxung.cn

[R48] awk 取指定列
来源：http://mk.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://we.haigaiapp.cn

[R49] awk 带条件
来源：http://do.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://go.yuntaijiaju.cn

[R50] awk 求和
来源：http://ms.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://id.colortex.cn

[R51] 排序去重取前几
来源：http://mp.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lz.haigaiapp.cn

[R52] 统计行数
来源：http://dc.nicolike.cn

wc -l a.txt
来源：http://zh.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://ua.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ii.chemitech.net.cn

[R54] 比较两个文件
来源：http://tc.shxzukj.cn

diff a.txt b.txt
来源：http://qq.haigaiapp.cn

[R55] 压缩与解压
来源：http://in.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ve.huixiangedu.cn

[R56] 远程拷贝
来源：http://zl.szsharing.cn

scp file user@host:/path/
来源：http://fp.wgjwhj.cn

[R57] 远程执行命令
来源：http://ln.huanxung.cn

ssh user@host 'uptime'
来源：http://mi.shtwfgs.cn

[R58] 下载文件
来源：http://fn.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wq.9csxet.cn

[R59] 发 POST JSON
来源：http://nw.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wp.521024.cn

[R60] 只看 HTTP 状态码
来源：http://xl.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fo.shxzskj.cn

[R61] 磁盘占用
来源：http://cj.bjjhwx.cn

df -h;  du -sh *
来源：http://ev.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://bc.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://pa.nszjky.cn

[R63] 内存与进程
来源：http://we.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://xp.asd995.cn

[R64] 结束进程
来源：http://za.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://tw.bjjhwx.cn

[R65] 查看端口占用
来源：http://qp.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://se.jctech888.com.cn

[R66] 定时任务
来源：http://sz.gzmigu.cn

crontab -e;  crontab -l
来源：http://rd.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://wj.wgjwhj.cn

openssl rand -hex 16
来源：http://gd.yuexingan06.cn

[R68] 计算文件校验值
来源：http://ju.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kx.asd995.cn

[R69] 生成随机密码
来源：http://rz.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://gc.shxzukj.cn

[R70] 时间戳与互转
来源：http://jf.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://ml.huanxung.cn

[R71] 日期格式化
来源：http://ka.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gp.asd995.cn

[R72] 等待端口就绪
来源：http://gr.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ku.haigaiapp.cn

[R73] 分割大日志
来源：http://me.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://vm.521024.cn

[R74] 批量重命名
来源：http://ky.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tx.panjiajie.cn

[R75] 导出环境变量
来源：http://bf.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://fx.haigaiapp.cn

[R76] 使用临时文件
来源：http://us.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qk.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://hw.lnxyls.cn

read -rp "请输入: " ans
来源：http://st.nicolike.cn

[R78] 交互式菜单
来源：http://tu.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ye.shxzskj.cn

[R79] 解析命令行选项
来源：http://yh.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nu.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://fn.hahajie.cn

time ./run.sh
来源：http://fh.nicolike.cn

================================================================================
来源：http://lb.muxihuayi.cn

S. C / C++ 专题
来源：http://sg.shxzskj.cn

================================================================================
来源：http://ru.9csxet.cn

[S01] C：Hello World
来源：http://xy.shtwfgs.cn

#include <stdio.h>
来源：http://or.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ma.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://zk.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://dc.jianghongdianzi.cn

[S03] C：读入整数
来源：http://wa.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://qu.lnxyls.cn

[S04] C：字符串复制
来源：http://jn.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dz.yuexingan06.cn

[S05] C：字符串长度
来源：http://cb.hahajie.cn

strlen(s)
来源：http://bs.huixiangedu.cn

[S06] C：字符串比较
来源：http://en.colortex.cn

strcmp(a, b) == 0
来源：http://qi.nszjky.cn

[S07] C：数组遍历求和
来源：http://ur.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rv.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://du.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xi.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://md.colortex.cn


<!-- 参考信息 -->