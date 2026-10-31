代发 wailian999

[Q44] IN 子查询
来源：http://sd.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://po.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://yt.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uh.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ey.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ot.szxytkj.cn

[Q47] 与平均值比较
来源：http://ag.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tf.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://wc.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kk.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://tr.chemitech.net.cn

[Q49] 更新单行
来源：http://zq.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ks.szxytkj.cn

[Q50] 批量更新
来源：http://ve.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tj.521024.cn

[Q51] 用子查询更新
来源：http://id.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wu.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://dg.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://lk.huanxung.cn

[Q53] 按条件删除
来源：http://hp.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bt.9csxet.cn

[Q54] 清空表
来源：http://iq.colortex.cn

TRUNCATE TABLE logs;
来源：http://tr.nicolike.cn

[Q55] 排名（并列占位）
来源：http://pe.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://st.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://cz.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mb.gzmigu.cn

[Q57] 行号
来源：http://sb.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gq.jctech888.com.cn

[Q58] 累计求和
来源：http://zv.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://in.shtwfgs.cn

[Q59] 分组内累计
来源：http://qq.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iz.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://xx.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ll.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ji.huanxung.cn

[Q61] 移动平均
来源：http://ar.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vr.newstarts.cn

[Q62] 分组占比
来源：http://hr.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tf.9csxet.cn

[Q63] 开启事务
来源：http://st.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jv.asd995.cn

[Q64] 提交事务
来源：http://oi.gzmigu.cn

COMMIT;
来源：http://mo.bjjhwx.cn

[Q65] 回滚事务
来源：http://mj.9csxet.cn

ROLLBACK;
来源：http://vd.szxytkj.cn

[Q66] 行锁查询
来源：http://qz.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xw.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://vx.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zu.hahajie.cn

[Q68] 保存点
来源：http://lg.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://ii.hahajie.cn

ROLLBACK TO sp1;
来源：http://at.chemitech.net.cn

[Q69] 查看执行计划
来源：http://kf.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ld.colortex.cn

[Q70] 更新统计信息
来源：http://ru.yuexingan06.cn

ANALYZE TABLE users;
来源：http://so.newstarts.cn

[Q71] 查看建表语句
来源：http://dx.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ti.shxzukj.cn

[Q72] 查看索引
来源：http://gz.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://fn.wgjwhj.cn

[Q73] 查看表状态
来源：http://jn.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tl.521024.cn

[Q74] 强制使用索引
来源：http://md.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ur.shxzukj.cn

[Q75] 日期格式化
来源：http://ls.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ui.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ph.szxytkj.cn

[Q76] 按天统计
来源：http://lt.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vq.gzmigu.cn

[Q77] 时间加减
来源：http://pi.huanxung.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xy.wgjwhj.cn

[Q78] 当前时间
来源：http://ol.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qh.521024.cn

[Q79] 字符串拼接
来源：http://uj.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ni.huixiangedu.cn

[Q80] 字符串截取
来源：http://nl.jianghongdianzi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vz.yuexingan06.cn

[Q81] 字符串替换
来源：http://zg.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ym.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://ld.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wp.hnjuh.cn

[Q83] 大小写转换
来源：http://wd.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tk.9csxet.cn

[Q84] 去除首尾空格
来源：http://mp.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://ua.yuexingan06.cn

[Q85] 数值取整
来源：http://ez.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ti.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://ha.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vc.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://cj.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lh.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://ug.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ck.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://co.newstarts.cn

[Q89] 判断表是否存在
来源：http://cf.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jb.hahajie.cn

[Q90] 生成序号列
来源：http://fq.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dx.nicolike.cn

================================================================================
来源：http://ug.hnjuh.cn

R. Bash 专题
来源：http://qo.huixiangedu.cn

================================================================================
来源：http://ql.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://fq.asd995.cn

#!/usr/bin/env bash
来源：http://bn.colortex.cn

set -euo pipefail
来源：http://hv.newstarts.cn

[R02] 变量赋值与使用
来源：http://fo.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://xw.9csxet.cn

[R03] 只读变量
来源：http://xw.huixinmuqiang.cn

readonly PI=3.14
来源：http://dr.haigaiapp.cn

[R04] 位置参数
来源：http://mv.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ex.colortex.cn

[R05] 参数默认值
来源：http://ju.jctech888.com.cn

name="${1:-default}"
来源：http://an.colortex.cn

[R06] 判断命令是否存在
来源：http://zc.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vv.521024.cn

[R07] if 判断文件
来源：http://yu.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vm.nszjky.cn

[R08] 数值比较
来源：http://xy.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cr.szxytkj.cn

[R09] 字符串比较
来源：http://hk.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qi.huixinmuqiang.cn

[R10] 正则匹配
来源：http://ph.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aq.yuexingan06.cn

[R11] case 多分支
来源：http://yh.shxzukj.cn

case "$1" in
来源：http://rr.huanxung.cn

start) echo "启动" ;;
来源：http://xj.szsharing.cn

stop)  echo "停止" ;;
来源：http://gc.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://hm.huanxung.cn

esac
来源：http://qj.asd995.cn

[R12] for 遍历文件
来源：http://xi.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://qf.panjiajie.cn

[R13] for 计数循环
来源：http://mr.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://al.colortex.cn

[R14] C 风格 for
来源：http://ys.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yu.hnjuh.cn

[R15] while 逐行读文件
来源：http://cy.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sg.huixiangedu.cn

[R16] until 等待条件
来源：http://mx.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://du.panjiajie.cn

[R17] 数组定义与取值
来源：http://po.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://km.huanxung.cn

[R18] 遍历数组
来源：http://sc.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gl.yuntaijiaju.cn

[R19] 数组长度
来源：http://le.shtwfgs.cn

echo "${#arr[@]}"
来源：http://hj.shxzskj.cn

[R20] 关联数组（字典）
来源：http://bx.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aj.asd995.cn

[R21] 字符串长度
来源：http://ob.haigaiapp.cn

echo "${#s}"
来源：http://aj.nszjky.cn

[R22] 截取子串
来源：http://bx.yuexingan06.cn

echo "${s:0:5}"
来源：http://qz.szxytkj.cn

[R23] 字符串替换
来源：http://bq.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://up.huixiangedu.cn

[R24] 大小写转换
来源：http://ei.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yl.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://ts.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bi.yuntaijiaju.cn

[R26] 命令替换
来源：http://le.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://oz.hnjuh.cn

[R27] 算术展开
来源：http://kk.hahajie.cn

echo $((1 + 2 * 3))
来源：http://po.9csxet.cn

[R28] 浮点运算
来源：http://ja.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://lu.panjiajie.cn

[R29] 定义函数
来源：http://gn.jctech888.com.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wj.nicolike.cn

[R30] 函数返回状态码
来源：http://on.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://tf.newstarts.cn

[R31] 局部变量
来源：http://pz.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://kx.asd995.cn

[R32] 参数个数校验
来源：http://mi.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hy.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://vx.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xk.hnjuh.cn

[R34] 退出时清理
来源：http://ob.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nk.haigaiapp.cn

[R35] 后台执行并等待
来源：http://ok.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tw.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://lr.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qc.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://qp.bookmarksfly.cn

files=$(ls -1)
来源：http://fl.521024.cn

[R38] 管道串联
来源：http://jx.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://ze.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://cl.nszjky.cn

cmd > out.log 2>&1
来源：http://cm.asd995.cn

[R40] 追加写日志
来源：http://vo.szxytkj.cn

echo "log" >> out.log
来源：http://ym.gzmigu.cn

[R41] 丢弃输出
来源：http://vr.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://ey.lnxyls.cn

[R42] 输入重定向
来源：http://vs.panjiajie.cn

wc -l < a.txt
来源：http://tf.hahajie.cn

[R43] 按名字查找文件
来源：http://fx.asd995.cn

find . -name "*.log" -type f
来源：http://ak.huixiangedu.cn

[R44] 按修改时间查找
来源：http://gx.newstarts.cn

find . -mtime -7 -type f
来源：http://yk.muxihuayi.cn

[R45] 批量删除
来源：http://df.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://nr.nszjky.cn

[R46] 递归替换文件内容
来源：http://vd.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://od.hnjuh.cn

[R47] sed 单行替换
来源：http://pu.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oe.shtwfgs.cn

[R48] awk 取指定列
来源：http://np.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://bh.yuntaijiaju.cn

[R49] awk 带条件
来源：http://sg.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rx.hahajie.cn

[R50] awk 求和
来源：http://vy.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kk.asd995.cn

[R51] 排序去重取前几
来源：http://ti.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ch.jctech888.com.cn

[R52] 统计行数
来源：http://kf.hnjuh.cn

wc -l a.txt
来源：http://ni.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://qo.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nb.haigaiapp.cn

[R54] 比较两个文件
来源：http://vv.panjiajie.cn

diff a.txt b.txt
来源：http://gf.szsharing.cn

[R55] 压缩与解压
来源：http://zz.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hu.lnxyls.cn

[R56] 远程拷贝
来源：http://bu.wgjwhj.cn

scp file user@host:/path/
来源：http://jw.nicolike.cn

[R57] 远程执行命令
来源：http://hz.9csxet.cn

ssh user@host 'uptime'
来源：http://hc.hnjuh.cn

[R58] 下载文件
来源：http://fj.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xu.lnxyls.cn

[R59] 发 POST JSON
来源：http://os.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://du.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://ou.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uo.bookmarksfly.cn

[R61] 磁盘占用
来源：http://vl.bookmarksfly.cn

df -h;  du -sh *
来源：http://rq.hahajie.cn

[R62] 找最占空间的文件
来源：http://cx.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://kd.jctech888.com.cn

[R63] 内存与进程
来源：http://xr.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://en.chemitech.net.cn

[R64] 结束进程
来源：http://an.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://ff.jctech888.com.cn

[R65] 查看端口占用
来源：http://hw.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ed.gzmigu.cn

[R66] 定时任务
来源：http://yn.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://lz.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://xr.huixiangedu.cn

openssl rand -hex 16
来源：http://yo.panjiajie.cn

[R68] 计算文件校验值
来源：http://us.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ff.hnjuh.cn

[R69] 生成随机密码
来源：http://qk.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://xz.panjiajie.cn

[R70] 时间戳与互转
来源：http://tc.9csxet.cn

date +%s;  date -d @1700000000
来源：http://rm.newstarts.cn

[R71] 日期格式化
来源：http://fv.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oy.huanxung.cn

[R72] 等待端口就绪
来源：http://qk.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vd.newstarts.cn

[R73] 分割大日志
来源：http://wy.wgjwhj.cn

split -l 1000 big.log part_
来源：http://ie.chemitech.net.cn

[R74] 批量重命名
来源：http://wf.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cw.yuexingan06.cn

[R75] 导出环境变量
来源：http://sz.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://yn.shtwfgs.cn

[R76] 使用临时文件
来源：http://ek.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oe.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://ks.hahajie.cn

read -rp "请输入: " ans
来源：http://kc.bjjhwx.cn

[R78] 交互式菜单
来源：http://rl.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yx.gzmigu.cn

[R79] 解析命令行选项
来源：http://sw.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xc.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://ia.521024.cn

time ./run.sh
来源：http://ef.newstarts.cn

================================================================================
来源：http://qs.wgjwhj.cn

S. C / C++ 专题
来源：http://ow.gzmigu.cn

================================================================================
来源：http://jb.hahajie.cn

[S01] C：Hello World
来源：http://wu.shtwfgs.cn

#include <stdio.h>
来源：http://yk.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gb.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://en.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://ys.lnxyls.cn

[S03] C：读入整数
来源：http://ua.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://mm.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://to.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mz.9csxet.cn

[S05] C：字符串长度
来源：http://ir.bookmarksfly.cn

strlen(s)
来源：http://ch.nszjky.cn

[S06] C：字符串比较
来源：http://pc.hnjuh.cn

strcmp(a, b) == 0
来源：http://hp.huanxung.cn

[S07] C：数组遍历求和
来源：http://sb.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uu.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://mb.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wn.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://vs.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nc.shxzukj.cn

[S10] C：指针与解引用
来源：http://nd.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://pj.lnxyls.cn

[S11] C：逐行读文件
来源：http://kh.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://ts.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ib.yuntaijiaju.cn

fclose(f);
来源：http://sv.haigaiapp.cn

[S12] C：写文件
来源：http://wz.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hx.colortex.cn

[S13] C：宏定义
来源：http://jt.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cb.shxzskj.cn

[S14] C：枚举
来源：http://dp.wgjwhj.cn


<!-- 参考信息 -->