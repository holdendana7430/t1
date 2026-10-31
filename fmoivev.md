代发 wailian999

[Q44] IN 子查询
来源：http://pd.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jl.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://pm.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bn.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ql.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://du.yuexingan06.cn

[Q47] 与平均值比较
来源：http://jh.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zt.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://sl.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ga.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://pe.huixiangedu.cn

[Q49] 更新单行
来源：http://vq.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ez.nicolike.cn

[Q50] 批量更新
来源：http://qq.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nf.chemitech.net.cn

[Q51] 用子查询更新
来源：http://vw.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fh.nszjky.cn

[Q52] 删除指定行
来源：http://yf.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://fr.gzmigu.cn

[Q53] 按条件删除
来源：http://tp.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rj.lnxyls.cn

[Q54] 清空表
来源：http://jj.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://pi.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://za.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ol.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://xy.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wh.yuntaijiaju.cn

[Q57] 行号
来源：http://vc.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xb.wgjwhj.cn

[Q58] 累计求和
来源：http://gc.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wa.huanxung.cn

[Q59] 分组内累计
来源：http://ha.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://id.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://an.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uh.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lj.shtwfgs.cn

[Q61] 移动平均
来源：http://rn.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xe.shxzskj.cn

[Q62] 分组占比
来源：http://zn.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vv.lnxyls.cn

[Q63] 开启事务
来源：http://gy.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qx.haigaiapp.cn

[Q64] 提交事务
来源：http://at.panjiajie.cn

COMMIT;
来源：http://dw.gzmigu.cn

[Q65] 回滚事务
来源：http://ot.yuntaijiaju.cn

ROLLBACK;
来源：http://mw.nszjky.cn

[Q66] 行锁查询
来源：http://ka.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vg.shxzskj.cn

[Q67] 设置隔离级别
来源：http://fu.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eq.shxzukj.cn

[Q68] 保存点
来源：http://ww.colortex.cn

SAVEPOINT sp1;
来源：http://vj.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://ct.hnjuh.cn

[Q69] 查看执行计划
来源：http://ys.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ar.hnjuh.cn

[Q70] 更新统计信息
来源：http://hf.szxytkj.cn

ANALYZE TABLE users;
来源：http://do.asd995.cn

[Q71] 查看建表语句
来源：http://yl.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://le.shxzukj.cn

[Q72] 查看索引
来源：http://rr.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://xq.asd995.cn

[Q73] 查看表状态
来源：http://jt.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xm.szsharing.cn

[Q74] 强制使用索引
来源：http://zu.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xr.panjiajie.cn

[Q75] 日期格式化
来源：http://la.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dj.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wb.yuntaijiaju.cn

[Q76] 按天统计
来源：http://ij.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ze.nicolike.cn

[Q77] 时间加减
来源：http://hn.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fq.yuexingan06.cn

[Q78] 当前时间
来源：http://sw.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fg.szxytkj.cn

[Q79] 字符串拼接
来源：http://go.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nb.9csxet.cn

[Q80] 字符串截取
来源：http://cf.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sa.newstarts.cn

[Q81] 字符串替换
来源：http://ob.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ec.521024.cn

[Q82] 字符长度与字节长度
来源：http://db.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ax.shxzukj.cn

[Q83] 大小写转换
来源：http://tl.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qi.nicolike.cn

[Q84] 去除首尾空格
来源：http://fz.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://xm.shxzskj.cn

[Q85] 数值取整
来源：http://xm.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nu.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://kw.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xj.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://ey.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pa.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://jm.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://we.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fm.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://lk.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fx.hahajie.cn

[Q90] 生成序号列
来源：http://tn.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://om.shtwfgs.cn

================================================================================
来源：http://vz.nicolike.cn

R. Bash 专题
来源：http://na.jctech888.com.cn

================================================================================
来源：http://hl.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://sa.haigaiapp.cn

#!/usr/bin/env bash
来源：http://om.nszjky.cn

set -euo pipefail
来源：http://xg.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://zj.nszjky.cn

name="Tom"; echo "$name"
来源：http://ex.gzmigu.cn

[R03] 只读变量
来源：http://ut.chemitech.net.cn

readonly PI=3.14
来源：http://pw.asd995.cn

[R04] 位置参数
来源：http://kx.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jz.shxzskj.cn

[R05] 参数默认值
来源：http://ui.jianghongdianzi.cn

name="${1:-default}"
来源：http://xl.newstarts.cn

[R06] 判断命令是否存在
来源：http://xo.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kc.jianghongdianzi.cn

[R07] if 判断文件
来源：http://cw.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jk.newstarts.cn

[R08] 数值比较
来源：http://zt.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jb.asd995.cn

[R09] 字符串比较
来源：http://ie.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jq.huanxung.cn

[R10] 正则匹配
来源：http://bm.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tq.lnxyls.cn

[R11] case 多分支
来源：http://tt.muxihuayi.cn

case "$1" in
来源：http://da.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://oi.colortex.cn

stop)  echo "停止" ;;
来源：http://cn.nszjky.cn

*)     echo "未知命令" ;;
来源：http://qv.shxzukj.cn

esac
来源：http://yx.wgjwhj.cn

[R12] for 遍历文件
来源：http://hb.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://oc.wgjwhj.cn

[R13] for 计数循环
来源：http://td.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://oo.muxihuayi.cn

[R14] C 风格 for
来源：http://qk.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ac.wgjwhj.cn

[R15] while 逐行读文件
来源：http://il.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ar.huixinmuqiang.cn

[R16] until 等待条件
来源：http://uw.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fb.colortex.cn

[R17] 数组定义与取值
来源：http://cs.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ha.huixinmuqiang.cn

[R18] 遍历数组
来源：http://so.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tt.panjiajie.cn

[R19] 数组长度
来源：http://mu.521024.cn

echo "${#arr[@]}"
来源：http://fx.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://ao.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bd.shtwfgs.cn

[R21] 字符串长度
来源：http://qz.panjiajie.cn

echo "${#s}"
来源：http://sb.shxzukj.cn

[R22] 截取子串
来源：http://kf.szsharing.cn

echo "${s:0:5}"
来源：http://me.newstarts.cn

[R23] 字符串替换
来源：http://vi.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yc.shxzskj.cn

[R24] 大小写转换
来源：http://is.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://th.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://pq.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ve.chemitech.net.cn

[R26] 命令替换
来源：http://zs.haigaiapp.cn

now=$(date +%F); echo "$now"
来源：http://rn.nicolike.cn

[R27] 算术展开
来源：http://wo.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://db.nicolike.cn

[R28] 浮点运算
来源：http://vg.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://pc.muxihuayi.cn

[R29] 定义函数
来源：http://ab.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hm.bjjhwx.cn

[R30] 函数返回状态码
来源：http://td.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://zj.9csxet.cn

[R31] 局部变量
来源：http://jj.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://tb.colortex.cn

[R32] 参数个数校验
来源：http://fw.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kl.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://pl.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zz.lnxyls.cn

[R34] 退出时清理
来源：http://qy.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zx.gzmigu.cn

[R35] 后台执行并等待
来源：http://ac.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fv.szxytkj.cn

[R36] 并发执行多个任务
来源：http://ey.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eq.szxytkj.cn

[R37] 把输出赋给变量
来源：http://xc.wgjwhj.cn

files=$(ls -1)
来源：http://sk.nszjky.cn

[R38] 管道串联
来源：http://qj.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://ni.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://dr.muxihuayi.cn

cmd > out.log 2>&1
来源：http://os.muxihuayi.cn

[R40] 追加写日志
来源：http://lu.shtwfgs.cn

echo "log" >> out.log
来源：http://ur.521024.cn

[R41] 丢弃输出
来源：http://ax.szsharing.cn

cmd >/dev/null 2>&1
来源：http://eb.shxzskj.cn

[R42] 输入重定向
来源：http://oa.bjjhwx.cn

wc -l < a.txt
来源：http://ae.hahajie.cn

[R43] 按名字查找文件
来源：http://dj.colortex.cn

find . -name "*.log" -type f
来源：http://zi.newstarts.cn

[R44] 按修改时间查找
来源：http://rc.nszjky.cn

find . -mtime -7 -type f
来源：http://vc.newstarts.cn

[R45] 批量删除
来源：http://rr.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://bq.9csxet.cn

[R46] 递归替换文件内容
来源：http://gy.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lj.jctech888.com.cn

[R47] sed 单行替换
来源：http://wj.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jc.newstarts.cn

[R48] awk 取指定列
来源：http://ui.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://bl.newstarts.cn

[R49] awk 带条件
来源：http://kj.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bv.szxytkj.cn

[R50] awk 求和
来源：http://vx.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pe.bjjhwx.cn

[R51] 排序去重取前几
来源：http://qs.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jw.asd995.cn

[R52] 统计行数
来源：http://cb.bjjhwx.cn

wc -l a.txt
来源：http://rp.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://km.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xm.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://te.yuexingan06.cn

diff a.txt b.txt
来源：http://nu.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://ck.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kn.muxihuayi.cn

[R56] 远程拷贝
来源：http://pg.asd995.cn

scp file user@host:/path/
来源：http://qs.hahajie.cn

[R57] 远程执行命令
来源：http://ry.shxzukj.cn

ssh user@host 'uptime'
来源：http://sg.nicolike.cn

[R58] 下载文件
来源：http://tp.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uy.haigaiapp.cn

[R59] 发 POST JSON
来源：http://ok.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kx.521024.cn

[R60] 只看 HTTP 状态码
来源：http://ui.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rt.bjjhwx.cn

[R61] 磁盘占用
来源：http://wy.yuexingan06.cn

df -h;  du -sh *
来源：http://uj.colortex.cn

[R62] 找最占空间的文件
来源：http://cv.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://ph.yuexingan06.cn

[R63] 内存与进程
来源：http://qe.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://ux.colortex.cn

[R64] 结束进程
来源：http://my.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://mm.jctech888.com.cn

[R65] 查看端口占用
来源：http://mq.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ik.yuexingan06.cn

[R66] 定时任务
来源：http://pn.hnjuh.cn

crontab -e;  crontab -l
来源：http://fk.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://gy.huixinmuqiang.cn

openssl rand -hex 16
来源：http://bk.hnjuh.cn

[R68] 计算文件校验值
来源：http://la.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gd.nszjky.cn

[R69] 生成随机密码
来源：http://bd.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://hn.huanxung.cn

[R70] 时间戳与互转
来源：http://rv.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://pk.nicolike.cn

[R71] 日期格式化
来源：http://ns.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bb.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://ja.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://js.szxytkj.cn

[R73] 分割大日志
来源：http://rz.9csxet.cn

split -l 1000 big.log part_
来源：http://nl.shxzskj.cn

[R74] 批量重命名
来源：http://de.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bz.9csxet.cn

[R75] 导出环境变量
来源：http://rv.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://sf.lnxyls.cn

[R76] 使用临时文件
来源：http://ww.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kx.bookmarksfly.cn

[R77] 读取用户输入
来源：http://qz.nszjky.cn

read -rp "请输入: " ans
来源：http://kt.jctech888.com.cn

[R78] 交互式菜单
来源：http://qi.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ub.lnxyls.cn

[R79] 解析命令行选项
来源：http://gm.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mx.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://hy.yuntaijiaju.cn

time ./run.sh
来源：http://jp.szxytkj.cn

================================================================================
来源：http://wu.haigaiapp.cn

S. C / C++ 专题
来源：http://xc.chemitech.net.cn

================================================================================
来源：http://uf.shxzskj.cn

[S01] C：Hello World
来源：http://cf.szxytkj.cn

#include <stdio.h>
来源：http://hh.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sv.nicolike.cn

[S02] C：变量与格式化输出
来源：http://rv.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://md.szxytkj.cn

[S03] C：读入整数
来源：http://du.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://vs.521024.cn

[S04] C：字符串复制
来源：http://xj.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tl.shtwfgs.cn

[S05] C：字符串长度
来源：http://vr.nicolike.cn

strlen(s)
来源：http://xz.nicolike.cn

[S06] C：字符串比较
来源：http://xt.shtwfgs.cn

strcmp(a, b) == 0
来源：http://iw.szsharing.cn

[S07] C：数组遍历求和
来源：http://wg.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ht.asd995.cn

[S08] C：动态内存分配与释放
来源：http://kz.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xm.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://ro.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vj.colortex.cn

[S10] C：指针与解引用
来源：http://ob.9csxet.cn

int *p = &a;  *p = 5;
来源：http://mz.shxzukj.cn

[S11] C：逐行读文件
来源：http://pi.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://ko.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gd.jianghongdianzi.cn

fclose(f);
来源：http://fc.nicolike.cn

[S12] C：写文件
来源：http://xa.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oj.szxytkj.cn

[S13] C：宏定义
来源：http://ca.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://of.huixinmuqiang.cn

[S14] C：枚举
来源：http://dn.gzmigu.cn


<!-- 参考信息 -->