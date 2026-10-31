代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qw.asd995.cn

[Q52] 删除指定行
来源：http://ub.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://rb.gzmigu.cn

[Q53] 按条件删除
来源：http://pa.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tn.hahajie.cn

[Q54] 清空表
来源：http://cs.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://fj.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://dc.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oe.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://oh.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tz.muxihuayi.cn

[Q57] 行号
来源：http://hi.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://am.521024.cn

[Q58] 累计求和
来源：http://pq.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tl.nszjky.cn

[Q59] 分组内累计
来源：http://gw.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hn.jianghongdianzi.cn

[Q60] 取上一行 / 下一行
来源：http://wq.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ea.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sj.gzmigu.cn

[Q61] 移动平均
来源：http://cz.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zf.521024.cn

[Q62] 分组占比
来源：http://vq.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ys.shxzukj.cn

[Q63] 开启事务
来源：http://xv.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rf.panjiajie.cn

[Q64] 提交事务
来源：http://ix.huanxung.cn

COMMIT;
来源：http://jw.shxzukj.cn

[Q65] 回滚事务
来源：http://td.haigaiapp.cn

ROLLBACK;
来源：http://vj.nicolike.cn

[Q66] 行锁查询
来源：http://rr.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cg.colortex.cn

[Q67] 设置隔离级别
来源：http://hy.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jk.panjiajie.cn

[Q68] 保存点
来源：http://yr.lnxyls.cn

SAVEPOINT sp1;
来源：http://iz.szxytkj.cn

ROLLBACK TO sp1;
来源：http://jq.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://ba.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gy.colortex.cn

[Q70] 更新统计信息
来源：http://te.gzmigu.cn

ANALYZE TABLE users;
来源：http://ir.gzmigu.cn

[Q71] 查看建表语句
来源：http://nj.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zi.hnjuh.cn

[Q72] 查看索引
来源：http://lb.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://xx.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://hf.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ms.colortex.cn

[Q74] 强制使用索引
来源：http://du.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bj.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://hh.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://im.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ap.yuntaijiaju.cn

[Q76] 按天统计
来源：http://lp.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wp.haigaiapp.cn

[Q77] 时间加减
来源：http://rr.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yu.jctech888.com.cn

[Q78] 当前时间
来源：http://dk.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lr.huixiangedu.cn

[Q79] 字符串拼接
来源：http://oa.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xe.bjjhwx.cn

[Q80] 字符串截取
来源：http://py.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kn.bjjhwx.cn

[Q81] 字符串替换
来源：http://gu.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://es.asd995.cn

[Q82] 字符长度与字节长度
来源：http://qb.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nm.muxihuayi.cn

[Q83] 大小写转换
来源：http://rk.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wb.panjiajie.cn

[Q84] 去除首尾空格
来源：http://gl.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://zr.shtwfgs.cn

[Q85] 数值取整
来源：http://hx.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tk.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://hv.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ti.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://ge.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://et.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://iv.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rw.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kq.szxytkj.cn

[Q89] 判断表是否存在
来源：http://lz.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pm.chemitech.net.cn

[Q90] 生成序号列
来源：http://eq.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ob.szxytkj.cn

================================================================================
来源：http://or.gzmigu.cn

R. Bash 专题
来源：http://bq.bookmarksfly.cn

================================================================================
来源：http://ye.521024.cn

[R01] shebang 与严格模式
来源：http://tr.shxzukj.cn

#!/usr/bin/env bash
来源：http://wm.gzmigu.cn

set -euo pipefail
来源：http://cc.colortex.cn

[R02] 变量赋值与使用
来源：http://hq.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://nv.chemitech.net.cn

[R03] 只读变量
来源：http://bb.shtwfgs.cn

readonly PI=3.14
来源：http://cm.shxzukj.cn

[R04] 位置参数
来源：http://jh.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ft.521024.cn

[R05] 参数默认值
来源：http://zq.huixinmuqiang.cn

name="${1:-default}"
来源：http://yi.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://wg.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ti.newstarts.cn

[R07] if 判断文件
来源：http://bb.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hv.521024.cn

[R08] 数值比较
来源：http://ml.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tm.colortex.cn

[R09] 字符串比较
来源：http://qz.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ah.muxihuayi.cn

[R10] 正则匹配
来源：http://qa.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://la.yuntaijiaju.cn

[R11] case 多分支
来源：http://zf.hnjuh.cn

case "$1" in
来源：http://cy.newstarts.cn

start) echo "启动" ;;
来源：http://rg.hnjuh.cn

stop)  echo "停止" ;;
来源：http://lm.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://rq.yuntaijiaju.cn

esac
来源：http://to.huixiangedu.cn

[R12] for 遍历文件
来源：http://bb.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://pc.yuexingan06.cn

[R13] for 计数循环
来源：http://ib.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://ww.huixinmuqiang.cn

[R14] C 风格 for
来源：http://ri.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ev.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://kp.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gf.colortex.cn

[R16] until 等待条件
来源：http://xb.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://da.lnxyls.cn

[R17] 数组定义与取值
来源：http://ok.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vt.jianghongdianzi.cn

[R18] 遍历数组
来源：http://sd.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ma.szsharing.cn

[R19] 数组长度
来源：http://nz.nszjky.cn

echo "${#arr[@]}"
来源：http://tx.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://il.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hq.nszjky.cn

[R21] 字符串长度
来源：http://dp.wgjwhj.cn

echo "${#s}"
来源：http://am.bjjhwx.cn

[R22] 截取子串
来源：http://nv.shxzukj.cn

echo "${s:0:5}"
来源：http://gj.huanxung.cn

[R23] 字符串替换
来源：http://og.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sr.szxytkj.cn

[R24] 大小写转换
来源：http://ek.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jg.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://vq.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sc.jctech888.com.cn

[R26] 命令替换
来源：http://id.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://xz.huixiangedu.cn

[R27] 算术展开
来源：http://aa.9csxet.cn

echo $((1 + 2 * 3))
来源：http://si.jctech888.com.cn

[R28] 浮点运算
来源：http://ql.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://ow.huixiangedu.cn

[R29] 定义函数
来源：http://pe.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zw.yuexingan06.cn

[R30] 函数返回状态码
来源：http://wz.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://as.muxihuayi.cn

[R31] 局部变量
来源：http://pp.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://pr.chemitech.net.cn

[R32] 参数个数校验
来源：http://qv.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kw.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://du.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ky.gzmigu.cn

[R34] 退出时清理
来源：http://ez.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gx.panjiajie.cn

[R35] 后台执行并等待
来源：http://tt.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jm.shxzskj.cn

[R36] 并发执行多个任务
来源：http://fj.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ni.gzmigu.cn

[R37] 把输出赋给变量
来源：http://xn.colortex.cn

files=$(ls -1)
来源：http://as.chemitech.net.cn

[R38] 管道串联
来源：http://dm.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://xz.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://fz.newstarts.cn

cmd > out.log 2>&1
来源：http://ix.huixinmuqiang.cn

[R40] 追加写日志
来源：http://rc.9csxet.cn

echo "log" >> out.log
来源：http://ig.hahajie.cn

[R41] 丢弃输出
来源：http://wt.nszjky.cn

cmd >/dev/null 2>&1
来源：http://lm.muxihuayi.cn

[R42] 输入重定向
来源：http://yv.shxzukj.cn

wc -l < a.txt
来源：http://wi.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://ym.wgjwhj.cn

find . -name "*.log" -type f
来源：http://hq.shxzukj.cn

[R44] 按修改时间查找
来源：http://mr.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://vt.jctech888.com.cn

[R45] 批量删除
来源：http://fj.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://dr.newstarts.cn

[R46] 递归替换文件内容
来源：http://yr.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ab.gzmigu.cn

[R47] sed 单行替换
来源：http://xj.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hu.colortex.cn

[R48] awk 取指定列
来源：http://qy.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://wu.huixinmuqiang.cn

[R49] awk 带条件
来源：http://pt.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ut.newstarts.cn

[R50] awk 求和
来源：http://sc.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cm.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://wp.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nx.nszjky.cn

[R52] 统计行数
来源：http://lp.newstarts.cn

wc -l a.txt
来源：http://bj.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://qv.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pj.bjjhwx.cn

[R54] 比较两个文件
来源：http://eu.hahajie.cn

diff a.txt b.txt
来源：http://iv.nszjky.cn

[R55] 压缩与解压
来源：http://bt.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://th.nszjky.cn

[R56] 远程拷贝
来源：http://lb.jianghongdianzi.cn

scp file user@host:/path/
来源：http://om.shxzukj.cn

[R57] 远程执行命令
来源：http://zq.shxzskj.cn

ssh user@host 'uptime'
来源：http://wf.muxihuayi.cn

[R58] 下载文件
来源：http://nw.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ps.9csxet.cn

[R59] 发 POST JSON
来源：http://kz.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mo.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://bl.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zs.521024.cn

[R61] 磁盘占用
来源：http://di.muxihuayi.cn

df -h;  du -sh *
来源：http://ua.hnjuh.cn

[R62] 找最占空间的文件
来源：http://bm.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://hg.huixinmuqiang.cn

[R63] 内存与进程
来源：http://sr.asd995.cn

free -h;  ps aux | grep nginx
来源：http://ec.huanxung.cn

[R64] 结束进程
来源：http://ix.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://lu.chemitech.net.cn

[R65] 查看端口占用
来源：http://im.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lz.521024.cn

[R66] 定时任务
来源：http://sv.shxzukj.cn

crontab -e;  crontab -l
来源：http://uk.colortex.cn

[R67] 生成随机十六进制串
来源：http://eg.huixiangedu.cn

openssl rand -hex 16
来源：http://zh.shxzskj.cn

[R68] 计算文件校验值
来源：http://bs.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ak.asd995.cn

[R69] 生成随机密码
来源：http://em.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://jx.shxzskj.cn

[R70] 时间戳与互转
来源：http://pu.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://sh.panjiajie.cn

[R71] 日期格式化
来源：http://on.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rm.jctech888.com.cn

[R72] 等待端口就绪
来源：http://zs.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qe.yuexingan06.cn

[R73] 分割大日志
来源：http://kh.asd995.cn

split -l 1000 big.log part_
来源：http://sa.hnjuh.cn

[R74] 批量重命名
来源：http://gh.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ik.haigaiapp.cn

[R75] 导出环境变量
来源：http://gj.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://st.huanxung.cn

[R76] 使用临时文件
来源：http://ow.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qc.muxihuayi.cn

[R77] 读取用户输入
来源：http://gy.nicolike.cn

read -rp "请输入: " ans
来源：http://ta.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://xx.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pm.szsharing.cn

[R79] 解析命令行选项
来源：http://xu.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://id.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://bm.jctech888.com.cn

time ./run.sh
来源：http://ai.nszjky.cn

================================================================================
来源：http://jo.shxzukj.cn

S. C / C++ 专题
来源：http://yo.haigaiapp.cn

================================================================================
来源：http://tl.wgjwhj.cn

[S01] C：Hello World
来源：http://ja.jianghongdianzi.cn

#include <stdio.h>
来源：http://jx.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pz.huanxung.cn

[S02] C：变量与格式化输出
来源：http://gs.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://zl.chemitech.net.cn

[S03] C：读入整数
来源：http://ua.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://nn.szxytkj.cn

[S04] C：字符串复制
来源：http://uf.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jc.szsharing.cn

[S05] C：字符串长度
来源：http://cp.521024.cn

strlen(s)
来源：http://gh.nicolike.cn

[S06] C：字符串比较
来源：http://rp.panjiajie.cn

strcmp(a, b) == 0
来源：http://ae.9csxet.cn

[S07] C：数组遍历求和
来源：http://xc.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wj.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://rk.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://in.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://lo.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ow.newstarts.cn

[S10] C：指针与解引用
来源：http://re.nicolike.cn

int *p = &a;  *p = 5;
来源：http://va.9csxet.cn

[S11] C：逐行读文件
来源：http://lm.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://xo.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ki.bookmarksfly.cn

fclose(f);
来源：http://zj.asd995.cn

[S12] C：写文件
来源：http://gn.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gw.shxzukj.cn

[S13] C：宏定义
来源：http://lv.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tq.chemitech.net.cn

[S14] C：枚举
来源：http://pa.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ky.bjjhwx.cn

[S15] C：类型转换
来源：http://sm.huixiangedu.cn

(double) a / b
来源：http://le.nszjky.cn

[S16] C：位操作置位
来源：http://td.asd995.cn

x |= (1 << 3);
来源：http://ci.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://ti.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nx.muxihuayi.cn

[S18] C：命令行参数
来源：http://il.asd995.cn

int main(int argc, char **argv)
来源：http://cy.hnjuh.cn

[S19] C：快速排序
来源：http://tl.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hv.yuntaijiaju.cn

[S20] C：二分查找
来源：http://ua.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dt.nszjky.cn

[S21] C：字符类别判断
来源：http://fd.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wl.wgjwhj.cn

[S22] C：字符串转数字
来源：http://wz.panjiajie.cn


<!-- 参考信息 -->