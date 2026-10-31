代发 wailian999

[Q48] CTE 公用表表达式
来源：http://ol.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nr.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://cy.szsharing.cn

[Q49] 更新单行
来源：http://jo.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dm.gzmigu.cn

[Q50] 批量更新
来源：http://tv.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vk.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://yx.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zo.shxzukj.cn

[Q52] 删除指定行
来源：http://rj.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://xw.yuexingan06.cn

[Q53] 按条件删除
来源：http://ys.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bo.nszjky.cn

[Q54] 清空表
来源：http://rw.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://hs.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://ru.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wl.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://vk.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oo.yuexingan06.cn

[Q57] 行号
来源：http://db.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ir.shtwfgs.cn

[Q58] 累计求和
来源：http://ho.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://br.nszjky.cn

[Q59] 分组内累计
来源：http://jw.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ix.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://ki.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jt.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pn.9csxet.cn

[Q61] 移动平均
来源：http://fn.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fs.huanxung.cn

[Q62] 分组占比
来源：http://vj.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wz.nicolike.cn

[Q63] 开启事务
来源：http://hj.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xp.jianghongdianzi.cn

[Q64] 提交事务
来源：http://ik.hahajie.cn

COMMIT;
来源：http://px.gzmigu.cn

[Q65] 回滚事务
来源：http://as.yuntaijiaju.cn

ROLLBACK;
来源：http://wp.bookmarksfly.cn

[Q66] 行锁查询
来源：http://zp.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ar.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://oz.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rh.bjjhwx.cn

[Q68] 保存点
来源：http://ib.haigaiapp.cn

SAVEPOINT sp1;
来源：http://iz.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://jj.hahajie.cn

[Q69] 查看执行计划
来源：http://sx.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tt.chemitech.net.cn

[Q70] 更新统计信息
来源：http://gk.huanxung.cn

ANALYZE TABLE users;
来源：http://id.asd995.cn

[Q71] 查看建表语句
来源：http://me.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xt.panjiajie.cn

[Q72] 查看索引
来源：http://qr.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://gj.newstarts.cn

[Q73] 查看表状态
来源：http://po.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://df.yuntaijiaju.cn

[Q74] 强制使用索引
来源：http://qa.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sh.chemitech.net.cn

[Q75] 日期格式化
来源：http://af.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://va.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tv.panjiajie.cn

[Q76] 按天统计
来源：http://dh.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rl.panjiajie.cn

[Q77] 时间加减
来源：http://vt.hahajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yb.yuexingan06.cn

[Q78] 当前时间
来源：http://ot.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ux.hnjuh.cn

[Q79] 字符串拼接
来源：http://qd.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zs.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://sa.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kf.shxzskj.cn

[Q81] 字符串替换
来源：http://mw.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sm.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://mr.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eu.521024.cn

[Q83] 大小写转换
来源：http://yv.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://do.nszjky.cn

[Q84] 去除首尾空格
来源：http://ri.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://rq.gzmigu.cn

[Q85] 数值取整
来源：http://ah.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sm.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://en.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nj.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://cz.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://al.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://dr.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dp.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jg.yuntaijiaju.cn

[Q89] 判断表是否存在
来源：http://mk.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gw.shxzukj.cn

[Q90] 生成序号列
来源：http://co.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jk.shxzukj.cn

================================================================================
来源：http://lv.gzmigu.cn

R. Bash 专题
来源：http://nj.521024.cn

================================================================================
来源：http://xb.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://dm.szxytkj.cn

#!/usr/bin/env bash
来源：http://tk.wgjwhj.cn

set -euo pipefail
来源：http://vd.szxytkj.cn

[R02] 变量赋值与使用
来源：http://ji.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://un.shtwfgs.cn

[R03] 只读变量
来源：http://fn.szxytkj.cn

readonly PI=3.14
来源：http://yk.shtwfgs.cn

[R04] 位置参数
来源：http://wz.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hk.shtwfgs.cn

[R05] 参数默认值
来源：http://vr.521024.cn

name="${1:-default}"
来源：http://vt.colortex.cn

[R06] 判断命令是否存在
来源：http://rf.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ng.colortex.cn

[R07] if 判断文件
来源：http://jk.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ns.hahajie.cn

[R08] 数值比较
来源：http://vu.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qe.hnjuh.cn

[R09] 字符串比较
来源：http://yg.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hy.huixinmuqiang.cn

[R10] 正则匹配
来源：http://hl.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xs.gzmigu.cn

[R11] case 多分支
来源：http://jl.shtwfgs.cn

case "$1" in
来源：http://mb.panjiajie.cn

start) echo "启动" ;;
来源：http://eo.asd995.cn

stop)  echo "停止" ;;
来源：http://kw.newstarts.cn

*)     echo "未知命令" ;;
来源：http://wx.wgjwhj.cn

esac
来源：http://af.nicolike.cn

[R12] for 遍历文件
来源：http://jh.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://pu.panjiajie.cn

[R13] for 计数循环
来源：http://ot.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://dw.bookmarksfly.cn

[R14] C 风格 for
来源：http://tp.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mc.szxytkj.cn

[R15] while 逐行读文件
来源：http://xg.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zl.bjjhwx.cn

[R16] until 等待条件
来源：http://lh.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dv.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://gv.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://go.huanxung.cn

[R18] 遍历数组
来源：http://kp.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kl.wgjwhj.cn

[R19] 数组长度
来源：http://ra.lnxyls.cn

echo "${#arr[@]}"
来源：http://sl.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://jy.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://te.nicolike.cn

[R21] 字符串长度
来源：http://fy.chemitech.net.cn

echo "${#s}"
来源：http://nt.colortex.cn

[R22] 截取子串
来源：http://uf.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://jh.wgjwhj.cn

[R23] 字符串替换
来源：http://ux.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hn.newstarts.cn

[R24] 大小写转换
来源：http://yv.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dx.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://ww.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ny.huanxung.cn

[R26] 命令替换
来源：http://il.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://mg.shxzskj.cn

[R27] 算术展开
来源：http://kz.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://al.newstarts.cn

[R28] 浮点运算
来源：http://sl.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://yq.szxytkj.cn

[R29] 定义函数
来源：http://gj.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jf.szxytkj.cn

[R30] 函数返回状态码
来源：http://at.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://dc.huanxung.cn

[R31] 局部变量
来源：http://pw.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://em.shxzskj.cn

[R32] 参数个数校验
来源：http://hd.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vs.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://ij.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ik.shxzskj.cn

[R34] 退出时清理
来源：http://yk.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kr.muxihuayi.cn

[R35] 后台执行并等待
来源：http://fa.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fd.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://sj.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ec.hnjuh.cn

[R37] 把输出赋给变量
来源：http://ly.gzmigu.cn

files=$(ls -1)
来源：http://xy.jctech888.com.cn

[R38] 管道串联
来源：http://rz.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://pf.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://gx.huixiangedu.cn

cmd > out.log 2>&1
来源：http://cj.wgjwhj.cn

[R40] 追加写日志
来源：http://fz.lnxyls.cn

echo "log" >> out.log
来源：http://ly.nicolike.cn

[R41] 丢弃输出
来源：http://my.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://yy.szsharing.cn

[R42] 输入重定向
来源：http://ub.hahajie.cn

wc -l < a.txt
来源：http://so.newstarts.cn

[R43] 按名字查找文件
来源：http://ah.huanxung.cn

find . -name "*.log" -type f
来源：http://qg.newstarts.cn

[R44] 按修改时间查找
来源：http://yl.lnxyls.cn

find . -mtime -7 -type f
来源：http://xg.huixiangedu.cn

[R45] 批量删除
来源：http://xf.nicolike.cn

find . -name "*.tmp" -delete
来源：http://wo.hnjuh.cn

[R46] 递归替换文件内容
来源：http://ai.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jn.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://bl.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bp.shxzskj.cn

[R48] awk 取指定列
来源：http://fg.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://hi.yuexingan06.cn

[R49] awk 带条件
来源：http://qa.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://da.haigaiapp.cn

[R50] awk 求和
来源：http://gz.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mj.shtwfgs.cn

[R51] 排序去重取前几
来源：http://yu.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ws.colortex.cn

[R52] 统计行数
来源：http://oz.asd995.cn

wc -l a.txt
来源：http://jj.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://er.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fr.huanxung.cn

[R54] 比较两个文件
来源：http://ck.jianghongdianzi.cn

diff a.txt b.txt
来源：http://cd.colortex.cn

[R55] 压缩与解压
来源：http://hu.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xs.huanxung.cn

[R56] 远程拷贝
来源：http://st.szsharing.cn

scp file user@host:/path/
来源：http://gz.panjiajie.cn

[R57] 远程执行命令
来源：http://nl.huixiangedu.cn

ssh user@host 'uptime'
来源：http://ge.shxzskj.cn

[R58] 下载文件
来源：http://el.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sq.shtwfgs.cn

[R59] 发 POST JSON
来源：http://zj.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ex.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://ad.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ay.asd995.cn

[R61] 磁盘占用
来源：http://fq.hahajie.cn

df -h;  du -sh *
来源：http://il.nszjky.cn

[R62] 找最占空间的文件
来源：http://it.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://jr.bookmarksfly.cn

[R63] 内存与进程
来源：http://du.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://nr.szsharing.cn

[R64] 结束进程
来源：http://kl.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://ah.bookmarksfly.cn

[R65] 查看端口占用
来源：http://fm.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gy.szxytkj.cn

[R66] 定时任务
来源：http://lg.nszjky.cn

crontab -e;  crontab -l
来源：http://ef.521024.cn

[R67] 生成随机十六进制串
来源：http://tj.colortex.cn

openssl rand -hex 16
来源：http://lh.521024.cn

[R68] 计算文件校验值
来源：http://ua.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cj.9csxet.cn

[R69] 生成随机密码
来源：http://ja.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://ht.newstarts.cn

[R70] 时间戳与互转
来源：http://gn.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://wv.haigaiapp.cn

[R71] 日期格式化
来源：http://qd.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ll.nszjky.cn

[R72] 等待端口就绪
来源：http://ev.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uf.9csxet.cn

[R73] 分割大日志
来源：http://bu.shxzukj.cn

split -l 1000 big.log part_
来源：http://dw.szxytkj.cn

[R74] 批量重命名
来源：http://vo.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ue.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://is.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://ng.chemitech.net.cn

[R76] 使用临时文件
来源：http://ir.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tr.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://ng.yuexingan06.cn

read -rp "请输入: " ans
来源：http://ap.asd995.cn

[R78] 交互式菜单
来源：http://je.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://aw.shtwfgs.cn

[R79] 解析命令行选项
来源：http://ax.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kr.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://cl.hahajie.cn

time ./run.sh
来源：http://ot.szsharing.cn

================================================================================
来源：http://mp.huixiangedu.cn

S. C / C++ 专题
来源：http://mh.panjiajie.cn

================================================================================
来源：http://yu.muxihuayi.cn

[S01] C：Hello World
来源：http://uz.nicolike.cn

#include <stdio.h>
来源：http://ic.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rl.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://zo.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://ai.shtwfgs.cn

[S03] C：读入整数
来源：http://cq.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://ld.hnjuh.cn

[S04] C：字符串复制
来源：http://fl.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mc.newstarts.cn

[S05] C：字符串长度
来源：http://ap.yuntaijiaju.cn

strlen(s)
来源：http://gl.bookmarksfly.cn

[S06] C：字符串比较
来源：http://vx.9csxet.cn

strcmp(a, b) == 0
来源：http://gv.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://ow.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jj.colortex.cn

[S08] C：动态内存分配与释放
来源：http://gu.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://al.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://pt.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://go.hnjuh.cn

[S10] C：指针与解引用
来源：http://dj.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://bl.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://ep.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://as.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sg.wgjwhj.cn

fclose(f);
来源：http://gn.521024.cn

[S12] C：写文件
来源：http://zb.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bu.huixiangedu.cn

[S13] C：宏定义
来源：http://uf.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://al.jianghongdianzi.cn

[S14] C：枚举
来源：http://bh.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://mx.huixiangedu.cn

[S15] C：类型转换
来源：http://bp.yuexingan06.cn

(double) a / b
来源：http://aq.chemitech.net.cn

[S16] C：位操作置位
来源：http://ap.jctech888.com.cn

x |= (1 << 3);
来源：http://ur.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://dg.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uz.shxzskj.cn

[S18] C：命令行参数
来源：http://fz.nicolike.cn


<!-- 参考信息 -->