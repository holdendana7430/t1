代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ue.hahajie.cn

[Q50] 批量更新
来源：http://dv.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wq.muxihuayi.cn

[Q51] 用子查询更新
来源：http://qr.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ae.nicolike.cn

[Q52] 删除指定行
来源：http://lv.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://ho.szsharing.cn

[Q53] 按条件删除
来源：http://ci.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eo.huixinmuqiang.cn

[Q54] 清空表
来源：http://ls.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://ft.newstarts.cn

[Q55] 排名（并列占位）
来源：http://qi.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cp.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://ar.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pc.szxytkj.cn

[Q57] 行号
来源：http://sw.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hn.bjjhwx.cn

[Q58] 累计求和
来源：http://pc.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xg.huanxung.cn

[Q59] 分组内累计
来源：http://us.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cc.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://ww.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ro.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rw.gzmigu.cn

[Q61] 移动平均
来源：http://pv.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ep.panjiajie.cn

[Q62] 分组占比
来源：http://lt.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ut.huanxung.cn

[Q63] 开启事务
来源：http://dh.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dw.szsharing.cn

[Q64] 提交事务
来源：http://om.9csxet.cn

COMMIT;
来源：http://ss.colortex.cn

[Q65] 回滚事务
来源：http://iq.panjiajie.cn

ROLLBACK;
来源：http://dr.chemitech.net.cn

[Q66] 行锁查询
来源：http://or.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nm.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://ft.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cu.szsharing.cn

[Q68] 保存点
来源：http://ud.521024.cn

SAVEPOINT sp1;
来源：http://rc.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://kd.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://xl.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vl.yuexingan06.cn

[Q70] 更新统计信息
来源：http://tb.jctech888.com.cn

ANALYZE TABLE users;
来源：http://wr.lnxyls.cn

[Q71] 查看建表语句
来源：http://jj.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ro.nicolike.cn

[Q72] 查看索引
来源：http://pz.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://nk.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://sj.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pa.hahajie.cn

[Q74] 强制使用索引
来源：http://ao.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hj.wgjwhj.cn

[Q75] 日期格式化
来源：http://kj.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tn.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bs.hahajie.cn

[Q76] 按天统计
来源：http://cw.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://np.wgjwhj.cn

[Q77] 时间加减
来源：http://fy.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cn.panjiajie.cn

[Q78] 当前时间
来源：http://ia.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://de.muxihuayi.cn

[Q79] 字符串拼接
来源：http://gt.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hp.nicolike.cn

[Q80] 字符串截取
来源：http://bz.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wa.9csxet.cn

[Q81] 字符串替换
来源：http://nm.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sa.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://sz.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ub.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://rm.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zj.yuntaijiaju.cn

[Q84] 去除首尾空格
来源：http://dl.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://yx.jianghongdianzi.cn

[Q85] 数值取整
来源：http://fj.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ef.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://mv.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cu.9csxet.cn

[Q87] JSON 字段做条件
来源：http://un.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vh.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://gm.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yy.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hn.9csxet.cn

[Q89] 判断表是否存在
来源：http://je.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tt.panjiajie.cn

[Q90] 生成序号列
来源：http://wl.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vd.chemitech.net.cn

================================================================================
来源：http://qv.huixinmuqiang.cn

R. Bash 专题
来源：http://dh.nszjky.cn

================================================================================
来源：http://qb.hnjuh.cn

[R01] shebang 与严格模式
来源：http://qj.szxytkj.cn

#!/usr/bin/env bash
来源：http://au.szsharing.cn

set -euo pipefail
来源：http://qz.szxytkj.cn

[R02] 变量赋值与使用
来源：http://ke.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://fs.jianghongdianzi.cn

[R03] 只读变量
来源：http://bu.shxzukj.cn

readonly PI=3.14
来源：http://iz.muxihuayi.cn

[R04] 位置参数
来源：http://js.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yx.chemitech.net.cn

[R05] 参数默认值
来源：http://dc.bookmarksfly.cn

name="${1:-default}"
来源：http://hk.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://aw.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://st.nicolike.cn

[R07] if 判断文件
来源：http://nn.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ta.asd995.cn

[R08] 数值比较
来源：http://yw.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dl.muxihuayi.cn

[R09] 字符串比较
来源：http://tm.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mt.9csxet.cn

[R10] 正则匹配
来源：http://yx.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jf.panjiajie.cn

[R11] case 多分支
来源：http://vz.bookmarksfly.cn

case "$1" in
来源：http://mq.panjiajie.cn

start) echo "启动" ;;
来源：http://ot.newstarts.cn

stop)  echo "停止" ;;
来源：http://jb.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://bc.panjiajie.cn

esac
来源：http://ec.haigaiapp.cn

[R12] for 遍历文件
来源：http://nj.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://de.huixinmuqiang.cn

[R13] for 计数循环
来源：http://gj.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://yo.bjjhwx.cn

[R14] C 风格 for
来源：http://rk.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yk.nicolike.cn

[R15] while 逐行读文件
来源：http://ue.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jd.huixiangedu.cn

[R16] until 等待条件
来源：http://ae.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zl.huixiangedu.cn

[R17] 数组定义与取值
来源：http://fw.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lu.szxytkj.cn

[R18] 遍历数组
来源：http://rj.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qr.asd995.cn

[R19] 数组长度
来源：http://oh.szsharing.cn

echo "${#arr[@]}"
来源：http://lg.huanxung.cn

[R20] 关联数组（字典）
来源：http://io.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nx.lnxyls.cn

[R21] 字符串长度
来源：http://kr.hahajie.cn

echo "${#s}"
来源：http://vu.yuexingan06.cn

[R22] 截取子串
来源：http://go.chemitech.net.cn

echo "${s:0:5}"
来源：http://wy.asd995.cn

[R23] 字符串替换
来源：http://tf.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qn.nszjky.cn

[R24] 大小写转换
来源：http://qw.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://py.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://oo.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mm.huanxung.cn

[R26] 命令替换
来源：http://or.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://eb.haigaiapp.cn

[R27] 算术展开
来源：http://eo.9csxet.cn

echo $((1 + 2 * 3))
来源：http://xm.yuntaijiaju.cn

[R28] 浮点运算
来源：http://ww.521024.cn

echo "scale=2; 10/3" | bc
来源：http://gk.gzmigu.cn

[R29] 定义函数
来源：http://gc.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aj.haigaiapp.cn

[R30] 函数返回状态码
来源：http://po.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://rz.wgjwhj.cn

[R31] 局部变量
来源：http://tn.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://vn.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://ev.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bi.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://ra.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lo.jctech888.com.cn

[R34] 退出时清理
来源：http://nw.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lx.nicolike.cn

[R35] 后台执行并等待
来源：http://yk.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dv.nicolike.cn

[R36] 并发执行多个任务
来源：http://xs.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://la.szsharing.cn

[R37] 把输出赋给变量
来源：http://xl.huixinmuqiang.cn

files=$(ls -1)
来源：http://jk.szxytkj.cn

[R38] 管道串联
来源：http://rd.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://lb.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://bs.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://xo.haigaiapp.cn

[R40] 追加写日志
来源：http://xa.haigaiapp.cn

echo "log" >> out.log
来源：http://fg.haigaiapp.cn

[R41] 丢弃输出
来源：http://wi.nicolike.cn

cmd >/dev/null 2>&1
来源：http://da.yuntaijiaju.cn

[R42] 输入重定向
来源：http://jl.shxzukj.cn

wc -l < a.txt
来源：http://sj.newstarts.cn

[R43] 按名字查找文件
来源：http://gp.shxzskj.cn

find . -name "*.log" -type f
来源：http://eb.huixiangedu.cn

[R44] 按修改时间查找
来源：http://st.9csxet.cn

find . -mtime -7 -type f
来源：http://ul.asd995.cn

[R45] 批量删除
来源：http://ip.521024.cn

find . -name "*.tmp" -delete
来源：http://np.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://in.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xu.asd995.cn

[R47] sed 单行替换
来源：http://uj.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mr.bookmarksfly.cn

[R48] awk 取指定列
来源：http://bx.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://nf.9csxet.cn

[R49] awk 带条件
来源：http://wm.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sf.szsharing.cn

[R50] awk 求和
来源：http://bw.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fl.szsharing.cn

[R51] 排序去重取前几
来源：http://xq.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ud.huanxung.cn

[R52] 统计行数
来源：http://si.newstarts.cn

wc -l a.txt
来源：http://fm.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://pd.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rk.nszjky.cn

[R54] 比较两个文件
来源：http://oh.9csxet.cn

diff a.txt b.txt
来源：http://ga.panjiajie.cn

[R55] 压缩与解压
来源：http://vg.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oo.bjjhwx.cn

[R56] 远程拷贝
来源：http://yr.chemitech.net.cn

scp file user@host:/path/
来源：http://yo.nszjky.cn

[R57] 远程执行命令
来源：http://em.muxihuayi.cn

ssh user@host 'uptime'
来源：http://zw.wgjwhj.cn

[R58] 下载文件
来源：http://hy.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mc.szsharing.cn

[R59] 发 POST JSON
来源：http://wf.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://em.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://oo.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zj.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://hr.gzmigu.cn

df -h;  du -sh *
来源：http://dc.shxzukj.cn

[R62] 找最占空间的文件
来源：http://py.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://qo.wgjwhj.cn

[R63] 内存与进程
来源：http://mt.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://lq.wgjwhj.cn

[R64] 结束进程
来源：http://ov.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://yw.szsharing.cn

[R65] 查看端口占用
来源：http://pz.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://go.gzmigu.cn

[R66] 定时任务
来源：http://np.bjjhwx.cn

crontab -e;  crontab -l
来源：http://db.521024.cn

[R67] 生成随机十六进制串
来源：http://bh.huixiangedu.cn

openssl rand -hex 16
来源：http://ds.9csxet.cn

[R68] 计算文件校验值
来源：http://qy.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zn.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://nt.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://iw.jctech888.com.cn

[R70] 时间戳与互转
来源：http://qc.nszjky.cn

date +%s;  date -d @1700000000
来源：http://eb.bookmarksfly.cn

[R71] 日期格式化
来源：http://ms.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jr.yuexingan06.cn

[R72] 等待端口就绪
来源：http://qa.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vz.jianghongdianzi.cn

[R73] 分割大日志
来源：http://tx.shxzukj.cn

split -l 1000 big.log part_
来源：http://gb.asd995.cn

[R74] 批量重命名
来源：http://rw.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dn.yuexingan06.cn

[R75] 导出环境变量
来源：http://ee.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://uw.shxzukj.cn

[R76] 使用临时文件
来源：http://xd.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bp.nszjky.cn

[R77] 读取用户输入
来源：http://up.yuexingan06.cn

read -rp "请输入: " ans
来源：http://yz.shxzukj.cn

[R78] 交互式菜单
来源：http://bd.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ki.haigaiapp.cn

[R79] 解析命令行选项
来源：http://uw.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ws.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://vp.huixinmuqiang.cn

time ./run.sh
来源：http://rf.9csxet.cn

================================================================================
来源：http://xe.jianghongdianzi.cn

S. C / C++ 专题
来源：http://tc.colortex.cn

================================================================================
来源：http://bw.hahajie.cn

[S01] C：Hello World
来源：http://ko.9csxet.cn

#include <stdio.h>
来源：http://pu.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ug.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://iw.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://uj.huixinmuqiang.cn

[S03] C：读入整数
来源：http://oy.huanxung.cn

int x; scanf("%d", &x);
来源：http://nk.lnxyls.cn

[S04] C：字符串复制
来源：http://et.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ma.chemitech.net.cn

[S05] C：字符串长度
来源：http://ag.gzmigu.cn

strlen(s)
来源：http://nf.shxzukj.cn

[S06] C：字符串比较
来源：http://xu.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://io.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://xa.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://el.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://jy.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ua.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://dc.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fu.shxzukj.cn

[S10] C：指针与解引用
来源：http://fg.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://hj.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://jd.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://pz.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xw.jianghongdianzi.cn

fclose(f);
来源：http://ne.nicolike.cn

[S12] C：写文件
来源：http://lg.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mg.bookmarksfly.cn

[S13] C：宏定义
来源：http://pw.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bo.shtwfgs.cn

[S14] C：枚举
来源：http://ns.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://yx.jianghongdianzi.cn

[S15] C：类型转换
来源：http://mi.szsharing.cn

(double) a / b
来源：http://ux.huanxung.cn

[S16] C：位操作置位
来源：http://va.muxihuayi.cn

x |= (1 << 3);
来源：http://ve.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://ui.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jr.lnxyls.cn

[S18] C：命令行参数
来源：http://cf.huixiangedu.cn

int main(int argc, char **argv)
来源：http://sd.asd995.cn

[S19] C：快速排序
来源：http://ag.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dz.huixiangedu.cn

[S20] C：二分查找
来源：http://mw.nicolike.cn


<!-- 参考信息 -->