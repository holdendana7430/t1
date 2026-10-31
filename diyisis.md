代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ip.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ud.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tb.huixinmuqiang.cn

[Q41] 多表连接
来源：http://bh.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xp.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://dx.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://nl.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://ov.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://sk.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yf.panjiajie.cn

[Q43] 标量子查询
来源：http://nf.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dx.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://ai.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ik.521024.cn

[Q45] EXISTS 判断存在
来源：http://jv.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hr.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mc.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://on.nszjky.cn

[Q47] 与平均值比较
来源：http://ld.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jm.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://gw.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ji.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://uh.lnxyls.cn

[Q49] 更新单行
来源：http://kk.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iu.panjiajie.cn

[Q50] 批量更新
来源：http://ol.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://md.huixiangedu.cn

[Q51] 用子查询更新
来源：http://tn.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qa.bjjhwx.cn

[Q52] 删除指定行
来源：http://go.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://lp.jctech888.com.cn

[Q53] 按条件删除
来源：http://at.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://si.asd995.cn

[Q54] 清空表
来源：http://kk.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://qs.colortex.cn

[Q55] 排名（并列占位）
来源：http://zt.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yn.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://vs.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uc.huixinmuqiang.cn

[Q57] 行号
来源：http://cw.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qz.521024.cn

[Q58] 累计求和
来源：http://sl.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rj.muxihuayi.cn

[Q59] 分组内累计
来源：http://yb.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qr.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://nd.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dx.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lr.muxihuayi.cn

[Q61] 移动平均
来源：http://sr.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hu.huanxung.cn

[Q62] 分组占比
来源：http://ui.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ti.yuexingan06.cn

[Q63] 开启事务
来源：http://ii.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tp.shtwfgs.cn

[Q64] 提交事务
来源：http://un.gzmigu.cn

COMMIT;
来源：http://cd.gzmigu.cn

[Q65] 回滚事务
来源：http://rx.gzmigu.cn

ROLLBACK;
来源：http://mb.bjjhwx.cn

[Q66] 行锁查询
来源：http://cb.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ef.9csxet.cn

[Q67] 设置隔离级别
来源：http://dv.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qg.shxzskj.cn

[Q68] 保存点
来源：http://ku.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://aq.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://yv.colortex.cn

[Q69] 查看执行计划
来源：http://zc.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ho.9csxet.cn

[Q70] 更新统计信息
来源：http://hh.szsharing.cn

ANALYZE TABLE users;
来源：http://gj.nicolike.cn

[Q71] 查看建表语句
来源：http://zg.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://br.panjiajie.cn

[Q72] 查看索引
来源：http://jb.nicolike.cn

SHOW INDEX FROM users;
来源：http://kl.shxzskj.cn

[Q73] 查看表状态
来源：http://ki.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gw.lnxyls.cn

[Q74] 强制使用索引
来源：http://ii.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mv.asd995.cn

[Q75] 日期格式化
来源：http://sc.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pa.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://os.panjiajie.cn

[Q76] 按天统计
来源：http://pf.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zz.asd995.cn

[Q77] 时间加减
来源：http://uo.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://my.szsharing.cn

[Q78] 当前时间
来源：http://sz.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rn.huanxung.cn

[Q79] 字符串拼接
来源：http://wu.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fh.nszjky.cn

[Q80] 字符串截取
来源：http://lo.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sy.huixiangedu.cn

[Q81] 字符串替换
来源：http://gv.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://az.colortex.cn

[Q82] 字符长度与字节长度
来源：http://wa.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ws.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://yj.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dv.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://qs.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://va.lnxyls.cn

[Q85] 数值取整
来源：http://rr.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ts.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://ze.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ns.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://wv.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tg.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://zz.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gl.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mv.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://ew.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zz.521024.cn

[Q90] 生成序号列
来源：http://eg.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jo.colortex.cn

================================================================================
来源：http://vd.asd995.cn

R. Bash 专题
来源：http://hc.bookmarksfly.cn

================================================================================
来源：http://hj.shxzukj.cn

[R01] shebang 与严格模式
来源：http://ya.lnxyls.cn

#!/usr/bin/env bash
来源：http://ee.bookmarksfly.cn

set -euo pipefail
来源：http://bk.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://fv.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://an.hnjuh.cn

[R03] 只读变量
来源：http://tb.yuntaijiaju.cn

readonly PI=3.14
来源：http://da.colortex.cn

[R04] 位置参数
来源：http://fx.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pf.jctech888.com.cn

[R05] 参数默认值
来源：http://gd.bjjhwx.cn

name="${1:-default}"
来源：http://cz.9csxet.cn

[R06] 判断命令是否存在
来源：http://kd.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ou.szsharing.cn

[R07] if 判断文件
来源：http://qp.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://or.panjiajie.cn

[R08] 数值比较
来源：http://tj.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rw.huixiangedu.cn

[R09] 字符串比较
来源：http://sd.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ux.gzmigu.cn

[R10] 正则匹配
来源：http://hy.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://am.huanxung.cn

[R11] case 多分支
来源：http://jg.gzmigu.cn

case "$1" in
来源：http://kc.bookmarksfly.cn

start) echo "启动" ;;
来源：http://mf.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://ao.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://gv.huanxung.cn

esac
来源：http://rl.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://hb.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://uz.muxihuayi.cn

[R13] for 计数循环
来源：http://ma.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://zn.szsharing.cn

[R14] C 风格 for
来源：http://rg.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uf.yuexingan06.cn

[R15] while 逐行读文件
来源：http://sz.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lf.asd995.cn

[R16] until 等待条件
来源：http://vb.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qs.chemitech.net.cn

[R17] 数组定义与取值
来源：http://qq.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pf.chemitech.net.cn

[R18] 遍历数组
来源：http://yq.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bo.chemitech.net.cn

[R19] 数组长度
来源：http://ed.wgjwhj.cn

echo "${#arr[@]}"
来源：http://jd.shxzskj.cn

[R20] 关联数组（字典）
来源：http://sx.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lq.shtwfgs.cn

[R21] 字符串长度
来源：http://lr.colortex.cn

echo "${#s}"
来源：http://np.lnxyls.cn

[R22] 截取子串
来源：http://pj.hnjuh.cn

echo "${s:0:5}"
来源：http://nj.hnjuh.cn

[R23] 字符串替换
来源：http://qt.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xs.bjjhwx.cn

[R24] 大小写转换
来源：http://vk.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sv.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://vl.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qf.hnjuh.cn

[R26] 命令替换
来源：http://tx.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://et.hnjuh.cn

[R27] 算术展开
来源：http://mh.szsharing.cn

echo $((1 + 2 * 3))
来源：http://kr.colortex.cn

[R28] 浮点运算
来源：http://hw.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://ji.colortex.cn

[R29] 定义函数
来源：http://ib.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zr.asd995.cn

[R30] 函数返回状态码
来源：http://ls.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://eo.szxytkj.cn

[R31] 局部变量
来源：http://cc.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://fy.huanxung.cn

[R32] 参数个数校验
来源：http://ji.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gy.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://hc.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dq.muxihuayi.cn

[R34] 退出时清理
来源：http://ic.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qe.newstarts.cn

[R35] 后台执行并等待
来源：http://ex.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jo.szxytkj.cn

[R36] 并发执行多个任务
来源：http://tm.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uz.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://lb.szsharing.cn

files=$(ls -1)
来源：http://lq.9csxet.cn

[R38] 管道串联
来源：http://qn.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://an.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://hb.asd995.cn

cmd > out.log 2>&1
来源：http://uz.szsharing.cn

[R40] 追加写日志
来源：http://yw.yuexingan06.cn

echo "log" >> out.log
来源：http://eo.yuexingan06.cn

[R41] 丢弃输出
来源：http://uy.9csxet.cn

cmd >/dev/null 2>&1
来源：http://ys.hahajie.cn

[R42] 输入重定向
来源：http://bz.shxzskj.cn

wc -l < a.txt
来源：http://ux.newstarts.cn

[R43] 按名字查找文件
来源：http://fq.bjjhwx.cn

find . -name "*.log" -type f
来源：http://mv.lnxyls.cn

[R44] 按修改时间查找
来源：http://zw.szsharing.cn

find . -mtime -7 -type f
来源：http://lr.asd995.cn

[R45] 批量删除
来源：http://vw.colortex.cn

find . -name "*.tmp" -delete
来源：http://gj.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://qj.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fz.szxytkj.cn

[R47] sed 单行替换
来源：http://xl.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zq.bjjhwx.cn

[R48] awk 取指定列
来源：http://la.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://au.szsharing.cn

[R49] awk 带条件
来源：http://xe.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://so.shtwfgs.cn

[R50] awk 求和
来源：http://rw.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vi.gzmigu.cn

[R51] 排序去重取前几
来源：http://ml.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://up.chemitech.net.cn

[R52] 统计行数
来源：http://in.haigaiapp.cn

wc -l a.txt
来源：http://pq.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://gf.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rg.shxzukj.cn

[R54] 比较两个文件
来源：http://bo.huanxung.cn

diff a.txt b.txt
来源：http://kg.chemitech.net.cn

[R55] 压缩与解压
来源：http://nx.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bh.jctech888.com.cn

[R56] 远程拷贝
来源：http://yt.wgjwhj.cn

scp file user@host:/path/
来源：http://np.huanxung.cn

[R57] 远程执行命令
来源：http://aj.muxihuayi.cn

ssh user@host 'uptime'
来源：http://sg.szsharing.cn

[R58] 下载文件
来源：http://cr.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gs.shxzskj.cn

[R59] 发 POST JSON
来源：http://vo.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gu.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://zd.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xr.szsharing.cn

[R61] 磁盘占用
来源：http://xn.newstarts.cn

df -h;  du -sh *
来源：http://az.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://ah.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://cx.colortex.cn

[R63] 内存与进程
来源：http://wh.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://pe.muxihuayi.cn

[R64] 结束进程
来源：http://be.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://bl.9csxet.cn

[R65] 查看端口占用
来源：http://ln.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ez.gzmigu.cn

[R66] 定时任务
来源：http://ot.hnjuh.cn

crontab -e;  crontab -l
来源：http://nl.colortex.cn

[R67] 生成随机十六进制串
来源：http://gu.9csxet.cn

openssl rand -hex 16
来源：http://tg.asd995.cn

[R68] 计算文件校验值
来源：http://ne.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zx.nszjky.cn

[R69] 生成随机密码
来源：http://vo.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://wa.jctech888.com.cn

[R70] 时间戳与互转
来源：http://yf.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://et.panjiajie.cn

[R71] 日期格式化
来源：http://vb.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wq.nicolike.cn

[R72] 等待端口就绪
来源：http://me.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lt.nicolike.cn

[R73] 分割大日志
来源：http://vc.panjiajie.cn

split -l 1000 big.log part_
来源：http://ym.bookmarksfly.cn

[R74] 批量重命名
来源：http://mf.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hb.bookmarksfly.cn

[R75] 导出环境变量
来源：http://dd.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://fa.bookmarksfly.cn

[R76] 使用临时文件
来源：http://hb.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sm.panjiajie.cn

[R77] 读取用户输入
来源：http://gy.wgjwhj.cn

read -rp "请输入: " ans
来源：http://tb.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://kc.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ik.szxytkj.cn

[R79] 解析命令行选项
来源：http://ts.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://or.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://yg.szsharing.cn

time ./run.sh
来源：http://km.bookmarksfly.cn

================================================================================
来源：http://ja.panjiajie.cn

S. C / C++ 专题
来源：http://ch.hnjuh.cn

================================================================================
来源：http://vp.huixiangedu.cn

[S01] C：Hello World
来源：http://uz.nicolike.cn

#include <stdio.h>
来源：http://tk.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lw.hahajie.cn

[S02] C：变量与格式化输出
来源：http://fv.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://we.jctech888.com.cn

[S03] C：读入整数
来源：http://to.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://ao.9csxet.cn

[S04] C：字符串复制
来源：http://lu.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://us.bookmarksfly.cn

[S05] C：字符串长度
来源：http://ey.shxzukj.cn

strlen(s)
来源：http://ra.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://ac.gzmigu.cn

strcmp(a, b) == 0
来源：http://qw.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://nh.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yq.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://un.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pe.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://za.huixiangedu.cn


<!-- 参考信息 -->