代发 wailian999

[Q48] CTE 公用表表达式
来源：http://vk.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cl.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://qg.bookmarksfly.cn

[Q49] 更新单行
来源：http://yd.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oq.szxytkj.cn

[Q50] 批量更新
来源：http://mu.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://we.bjjhwx.cn

[Q51] 用子查询更新
来源：http://co.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fp.huanxung.cn

[Q52] 删除指定行
来源：http://us.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://yv.bookmarksfly.cn

[Q53] 按条件删除
来源：http://xd.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ol.nszjky.cn

[Q54] 清空表
来源：http://oo.521024.cn

TRUNCATE TABLE logs;
来源：http://oc.gzmigu.cn

[Q55] 排名（并列占位）
来源：http://eq.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jw.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://va.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ch.shtwfgs.cn

[Q57] 行号
来源：http://bo.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ky.muxihuayi.cn

[Q58] 累计求和
来源：http://sp.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ux.521024.cn

[Q59] 分组内累计
来源：http://sb.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wm.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://si.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pa.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nz.colortex.cn

[Q61] 移动平均
来源：http://ki.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nt.newstarts.cn

[Q62] 分组占比
来源：http://qk.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://br.nicolike.cn

[Q63] 开启事务
来源：http://ib.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vr.huixiangedu.cn

[Q64] 提交事务
来源：http://gz.huixiangedu.cn

COMMIT;
来源：http://uo.521024.cn

[Q65] 回滚事务
来源：http://hx.nszjky.cn

ROLLBACK;
来源：http://hv.szsharing.cn

[Q66] 行锁查询
来源：http://va.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uc.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://ce.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lc.colortex.cn

[Q68] 保存点
来源：http://yv.521024.cn

SAVEPOINT sp1;
来源：http://ac.shxzskj.cn

ROLLBACK TO sp1;
来源：http://ic.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://xz.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rg.9csxet.cn

[Q70] 更新统计信息
来源：http://bg.nicolike.cn

ANALYZE TABLE users;
来源：http://ly.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://pr.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ww.hahajie.cn

[Q72] 查看索引
来源：http://jm.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://dd.nicolike.cn

[Q73] 查看表状态
来源：http://iz.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vq.yuntaijiaju.cn

[Q74] 强制使用索引
来源：http://fm.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tv.huanxung.cn

[Q75] 日期格式化
来源：http://mq.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rq.9csxet.cn

[Q76] 按天统计
来源：http://hf.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hr.yuntaijiaju.cn

[Q77] 时间加减
来源：http://uf.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gb.haigaiapp.cn

[Q78] 当前时间
来源：http://zl.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xj.jctech888.com.cn

[Q79] 字符串拼接
来源：http://cr.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ul.wgjwhj.cn

[Q80] 字符串截取
来源：http://wx.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hh.hahajie.cn

[Q81] 字符串替换
来源：http://ab.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://eh.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://ta.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vo.hahajie.cn

[Q83] 大小写转换
来源：http://mj.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rw.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://uu.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://mk.shxzskj.cn

[Q85] 数值取整
来源：http://sj.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vl.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://el.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vr.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://xx.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vd.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://nt.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xb.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ye.newstarts.cn

[Q89] 判断表是否存在
来源：http://ew.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xb.gzmigu.cn

[Q90] 生成序号列
来源：http://cq.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jm.panjiajie.cn

================================================================================
来源：http://wf.shtwfgs.cn

R. Bash 专题
来源：http://ty.shxzskj.cn

================================================================================
来源：http://qe.panjiajie.cn

[R01] shebang 与严格模式
来源：http://rm.bjjhwx.cn

#!/usr/bin/env bash
来源：http://er.hnjuh.cn

set -euo pipefail
来源：http://ub.nszjky.cn

[R02] 变量赋值与使用
来源：http://kd.nszjky.cn

name="Tom"; echo "$name"
来源：http://pa.jianghongdianzi.cn

[R03] 只读变量
来源：http://yu.nszjky.cn

readonly PI=3.14
来源：http://ba.newstarts.cn

[R04] 位置参数
来源：http://fe.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://np.wgjwhj.cn

[R05] 参数默认值
来源：http://lk.szxytkj.cn

name="${1:-default}"
来源：http://rf.asd995.cn

[R06] 判断命令是否存在
来源：http://hg.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wh.bookmarksfly.cn

[R07] if 判断文件
来源：http://pe.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nl.hahajie.cn

[R08] 数值比较
来源：http://iv.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qi.shtwfgs.cn

[R09] 字符串比较
来源：http://yq.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ug.panjiajie.cn

[R10] 正则匹配
来源：http://zw.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://is.haigaiapp.cn

[R11] case 多分支
来源：http://hr.chemitech.net.cn

case "$1" in
来源：http://bf.asd995.cn

start) echo "启动" ;;
来源：http://qb.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://uz.huanxung.cn

*)     echo "未知命令" ;;
来源：http://hl.yuexingan06.cn

esac
来源：http://jk.wgjwhj.cn

[R12] for 遍历文件
来源：http://wh.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://hp.haigaiapp.cn

[R13] for 计数循环
来源：http://pf.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://ik.lnxyls.cn

[R14] C 风格 for
来源：http://uh.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sv.gzmigu.cn

[R15] while 逐行读文件
来源：http://nn.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ol.nszjky.cn

[R16] until 等待条件
来源：http://ef.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lg.panjiajie.cn

[R17] 数组定义与取值
来源：http://ei.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hl.gzmigu.cn

[R18] 遍历数组
来源：http://ci.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tl.9csxet.cn

[R19] 数组长度
来源：http://oo.chemitech.net.cn

echo "${#arr[@]}"
来源：http://zb.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://kz.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zl.nszjky.cn

[R21] 字符串长度
来源：http://id.jctech888.com.cn

echo "${#s}"
来源：http://lp.9csxet.cn

[R22] 截取子串
来源：http://ej.bjjhwx.cn

echo "${s:0:5}"
来源：http://vm.newstarts.cn

[R23] 字符串替换
来源：http://oz.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iw.9csxet.cn

[R24] 大小写转换
来源：http://ap.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kn.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://kh.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://al.521024.cn

[R26] 命令替换
来源：http://pi.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://nz.szsharing.cn

[R27] 算术展开
来源：http://tm.colortex.cn

echo $((1 + 2 * 3))
来源：http://kv.shxzukj.cn

[R28] 浮点运算
来源：http://he.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://nh.huanxung.cn

[R29] 定义函数
来源：http://jc.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uw.shtwfgs.cn

[R30] 函数返回状态码
来源：http://rk.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://gj.shxzskj.cn

[R31] 局部变量
来源：http://ok.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://km.shxzukj.cn

[R32] 参数个数校验
来源：http://fy.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hl.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://ei.bookmarksfly.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ud.lnxyls.cn

[R34] 退出时清理
来源：http://kl.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ub.bjjhwx.cn

[R35] 后台执行并等待
来源：http://we.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cm.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://kb.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ln.asd995.cn

[R37] 把输出赋给变量
来源：http://cm.chemitech.net.cn

files=$(ls -1)
来源：http://vw.shtwfgs.cn

[R38] 管道串联
来源：http://kk.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://ek.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://pr.yuexingan06.cn

cmd > out.log 2>&1
来源：http://cj.hnjuh.cn

[R40] 追加写日志
来源：http://vq.shtwfgs.cn

echo "log" >> out.log
来源：http://tk.chemitech.net.cn

[R41] 丢弃输出
来源：http://jy.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://zy.huanxung.cn

[R42] 输入重定向
来源：http://ye.asd995.cn

wc -l < a.txt
来源：http://mb.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://ms.nszjky.cn

find . -name "*.log" -type f
来源：http://dr.huanxung.cn

[R44] 按修改时间查找
来源：http://rf.gzmigu.cn

find . -mtime -7 -type f
来源：http://ub.haigaiapp.cn

[R45] 批量删除
来源：http://vr.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://wm.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://gh.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nl.9csxet.cn

[R47] sed 单行替换
来源：http://xy.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://om.9csxet.cn

[R48] awk 取指定列
来源：http://ad.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://cf.muxihuayi.cn

[R49] awk 带条件
来源：http://tv.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jt.shtwfgs.cn

[R50] awk 求和
来源：http://vq.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dr.szsharing.cn

[R51] 排序去重取前几
来源：http://pl.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bc.asd995.cn

[R52] 统计行数
来源：http://dp.nszjky.cn

wc -l a.txt
来源：http://kc.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://ag.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://op.haigaiapp.cn

[R54] 比较两个文件
来源：http://nf.wgjwhj.cn

diff a.txt b.txt
来源：http://eg.huanxung.cn

[R55] 压缩与解压
来源：http://uw.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jf.panjiajie.cn

[R56] 远程拷贝
来源：http://mw.shxzukj.cn

scp file user@host:/path/
来源：http://ug.9csxet.cn

[R57] 远程执行命令
来源：http://db.lnxyls.cn

ssh user@host 'uptime'
来源：http://gv.hahajie.cn

[R58] 下载文件
来源：http://jb.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dq.gzmigu.cn

[R59] 发 POST JSON
来源：http://ux.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pu.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://yi.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hn.bjjhwx.cn

[R61] 磁盘占用
来源：http://sx.shxzskj.cn

df -h;  du -sh *
来源：http://rt.521024.cn

[R62] 找最占空间的文件
来源：http://lh.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://wp.colortex.cn

[R63] 内存与进程
来源：http://yp.colortex.cn

free -h;  ps aux | grep nginx
来源：http://ek.shxzukj.cn

[R64] 结束进程
来源：http://uj.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://ac.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://zo.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ao.colortex.cn

[R66] 定时任务
来源：http://yw.colortex.cn

crontab -e;  crontab -l
来源：http://yd.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://tt.haigaiapp.cn

openssl rand -hex 16
来源：http://sd.wgjwhj.cn

[R68] 计算文件校验值
来源：http://rt.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ib.yuexingan06.cn

[R69] 生成随机密码
来源：http://sa.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://au.haigaiapp.cn

[R70] 时间戳与互转
来源：http://fr.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://fy.yuexingan06.cn

[R71] 日期格式化
来源：http://os.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hr.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://em.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oy.asd995.cn

[R73] 分割大日志
来源：http://wr.huixiangedu.cn

split -l 1000 big.log part_
来源：http://ew.panjiajie.cn

[R74] 批量重命名
来源：http://fg.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wj.hahajie.cn

[R75] 导出环境变量
来源：http://bm.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://ek.muxihuayi.cn

[R76] 使用临时文件
来源：http://hh.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ea.shxzskj.cn

[R77] 读取用户输入
来源：http://xq.huixiangedu.cn

read -rp "请输入: " ans
来源：http://qz.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://aj.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://st.shtwfgs.cn

[R79] 解析命令行选项
来源：http://jz.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fg.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://qe.newstarts.cn

time ./run.sh
来源：http://ro.yuexingan06.cn

================================================================================
来源：http://kf.colortex.cn

S. C / C++ 专题
来源：http://dp.9csxet.cn

================================================================================
来源：http://tx.colortex.cn

[S01] C：Hello World
来源：http://lc.asd995.cn

#include <stdio.h>
来源：http://rm.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rp.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://dh.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://as.szxytkj.cn

[S03] C：读入整数
来源：http://vw.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://yx.newstarts.cn

[S04] C：字符串复制
来源：http://sa.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dv.hahajie.cn

[S05] C：字符串长度
来源：http://nq.bjjhwx.cn

strlen(s)
来源：http://xq.huanxung.cn

[S06] C：字符串比较
来源：http://of.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://tl.hahajie.cn

[S07] C：数组遍历求和
来源：http://wz.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yi.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://tn.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qo.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://an.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://um.panjiajie.cn

[S10] C：指针与解引用
来源：http://qq.huanxung.cn

int *p = &a;  *p = 5;
来源：http://ll.nicolike.cn

[S11] C：逐行读文件
来源：http://qk.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://ul.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hi.9csxet.cn

fclose(f);
来源：http://ke.bjjhwx.cn

[S12] C：写文件
来源：http://bj.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lu.huixinmuqiang.cn

[S13] C：宏定义
来源：http://ps.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qm.shtwfgs.cn

[S14] C：枚举
来源：http://eo.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://mo.lnxyls.cn

[S15] C：类型转换
来源：http://pm.asd995.cn

(double) a / b
来源：http://zb.asd995.cn

[S16] C：位操作置位
来源：http://of.yuntaijiaju.cn

x |= (1 << 3);
来源：http://ie.9csxet.cn

[S17] C：安全拼接字符串
来源：http://cc.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dc.chemitech.net.cn

[S18] C：命令行参数
来源：http://gw.shtwfgs.cn


<!-- 参考信息 -->