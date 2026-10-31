代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xp.haigaiapp.cn

[Q56] 密集排名（并列不占位）
来源：http://fb.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zp.jctech888.com.cn

[Q57] 行号
来源：http://fu.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://re.bjjhwx.cn

[Q58] 累计求和
来源：http://ft.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nw.szxytkj.cn

[Q59] 分组内累计
来源：http://ik.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cr.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://bz.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ao.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gd.huanxung.cn

[Q61] 移动平均
来源：http://ll.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://we.shxzskj.cn

[Q62] 分组占比
来源：http://eq.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qg.haigaiapp.cn

[Q63] 开启事务
来源：http://wr.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hr.chemitech.net.cn

[Q64] 提交事务
来源：http://st.newstarts.cn

COMMIT;
来源：http://ui.521024.cn

[Q65] 回滚事务
来源：http://nz.hahajie.cn

ROLLBACK;
来源：http://qf.asd995.cn

[Q66] 行锁查询
来源：http://rx.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xv.colortex.cn

[Q67] 设置隔离级别
来源：http://bt.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kz.szxytkj.cn

[Q68] 保存点
来源：http://ud.shxzskj.cn

SAVEPOINT sp1;
来源：http://xr.shxzukj.cn

ROLLBACK TO sp1;
来源：http://br.newstarts.cn

[Q69] 查看执行计划
来源：http://rt.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hm.hahajie.cn

[Q70] 更新统计信息
来源：http://gn.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://nh.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://we.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://np.jianghongdianzi.cn

[Q72] 查看索引
来源：http://ji.9csxet.cn

SHOW INDEX FROM users;
来源：http://yc.bjjhwx.cn

[Q73] 查看表状态
来源：http://xv.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tv.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://gq.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cp.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://ja.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ze.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xz.lnxyls.cn

[Q76] 按天统计
来源：http://yy.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ap.huixiangedu.cn

[Q77] 时间加减
来源：http://ju.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qi.huixinmuqiang.cn

[Q78] 当前时间
来源：http://ux.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rb.muxihuayi.cn

[Q79] 字符串拼接
来源：http://pf.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nw.521024.cn

[Q80] 字符串截取
来源：http://jc.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cg.asd995.cn

[Q81] 字符串替换
来源：http://to.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mj.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://dk.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sy.huanxung.cn

[Q83] 大小写转换
来源：http://te.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kg.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://cv.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://gj.huixiangedu.cn

[Q85] 数值取整
来源：http://bh.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://to.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://hq.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cm.szsharing.cn

[Q87] JSON 字段做条件
来源：http://ef.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://df.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://el.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dw.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xq.521024.cn

[Q89] 判断表是否存在
来源：http://au.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bl.wgjwhj.cn

[Q90] 生成序号列
来源：http://qv.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xz.jctech888.com.cn

================================================================================
来源：http://xi.chemitech.net.cn

R. Bash 专题
来源：http://te.huanxung.cn

================================================================================
来源：http://ac.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://ux.colortex.cn

#!/usr/bin/env bash
来源：http://ew.yuntaijiaju.cn

set -euo pipefail
来源：http://og.szxytkj.cn

[R02] 变量赋值与使用
来源：http://fc.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://an.shtwfgs.cn

[R03] 只读变量
来源：http://yq.shtwfgs.cn

readonly PI=3.14
来源：http://vr.shtwfgs.cn

[R04] 位置参数
来源：http://qj.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xi.wgjwhj.cn

[R05] 参数默认值
来源：http://wx.521024.cn

name="${1:-default}"
来源：http://xu.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://st.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lq.hnjuh.cn

[R07] if 判断文件
来源：http://qn.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ie.bjjhwx.cn

[R08] 数值比较
来源：http://sv.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bw.hnjuh.cn

[R09] 字符串比较
来源：http://ft.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://st.colortex.cn

[R10] 正则匹配
来源：http://fv.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hc.gzmigu.cn

[R11] case 多分支
来源：http://ek.newstarts.cn

case "$1" in
来源：http://fy.wgjwhj.cn

start) echo "启动" ;;
来源：http://hb.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://ff.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://ri.szxytkj.cn

esac
来源：http://ag.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://zn.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://mu.lnxyls.cn

[R13] for 计数循环
来源：http://xs.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://hb.huixinmuqiang.cn

[R14] C 风格 for
来源：http://sl.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fz.colortex.cn

[R15] while 逐行读文件
来源：http://bk.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rr.szsharing.cn

[R16] until 等待条件
来源：http://ja.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pn.huanxung.cn

[R17] 数组定义与取值
来源：http://yc.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://li.chemitech.net.cn

[R18] 遍历数组
来源：http://mq.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ha.shxzukj.cn

[R19] 数组长度
来源：http://mq.shxzskj.cn

echo "${#arr[@]}"
来源：http://up.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://jc.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sw.huixinmuqiang.cn

[R21] 字符串长度
来源：http://xf.shxzukj.cn

echo "${#s}"
来源：http://fv.bookmarksfly.cn

[R22] 截取子串
来源：http://xl.shxzukj.cn

echo "${s:0:5}"
来源：http://hr.nszjky.cn

[R23] 字符串替换
来源：http://vd.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ay.shtwfgs.cn

[R24] 大小写转换
来源：http://by.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vs.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://wf.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cw.hnjuh.cn

[R26] 命令替换
来源：http://gu.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://pp.shxzukj.cn

[R27] 算术展开
来源：http://ix.huanxung.cn

echo $((1 + 2 * 3))
来源：http://tv.521024.cn

[R28] 浮点运算
来源：http://rc.huixiangedu.cn

echo "scale=2; 10/3" | bc
来源：http://wt.hahajie.cn

[R29] 定义函数
来源：http://jy.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rh.nicolike.cn

[R30] 函数返回状态码
来源：http://nu.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://wp.nszjky.cn

[R31] 局部变量
来源：http://wc.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://sx.521024.cn

[R32] 参数个数校验
来源：http://em.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://on.colortex.cn

[R33] 捕获错误并提示行号
来源：http://ky.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yq.szxytkj.cn

[R34] 退出时清理
来源：http://ke.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rm.lnxyls.cn

[R35] 后台执行并等待
来源：http://cu.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nr.shxzukj.cn

[R36] 并发执行多个任务
来源：http://qt.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://on.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://ep.huanxung.cn

files=$(ls -1)
来源：http://rp.yuntaijiaju.cn

[R38] 管道串联
来源：http://ev.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://mt.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://na.jctech888.com.cn

cmd > out.log 2>&1
来源：http://tf.huanxung.cn

[R40] 追加写日志
来源：http://qr.hnjuh.cn

echo "log" >> out.log
来源：http://ut.panjiajie.cn

[R41] 丢弃输出
来源：http://xd.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://ag.colortex.cn

[R42] 输入重定向
来源：http://wo.lnxyls.cn

wc -l < a.txt
来源：http://ta.muxihuayi.cn

[R43] 按名字查找文件
来源：http://se.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://ny.szsharing.cn

[R44] 按修改时间查找
来源：http://dv.panjiajie.cn

find . -mtime -7 -type f
来源：http://ca.nicolike.cn

[R45] 批量删除
来源：http://ib.colortex.cn

find . -name "*.tmp" -delete
来源：http://jh.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://fj.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ku.shxzskj.cn

[R47] sed 单行替换
来源：http://gh.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dy.bookmarksfly.cn

[R48] awk 取指定列
来源：http://sk.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://yl.shxzukj.cn

[R49] awk 带条件
来源：http://na.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jx.huanxung.cn

[R50] awk 求和
来源：http://pk.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://os.yuexingan06.cn

[R51] 排序去重取前几
来源：http://ic.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ov.panjiajie.cn

[R52] 统计行数
来源：http://pf.hnjuh.cn

wc -l a.txt
来源：http://nv.colortex.cn

[R53] 查看文件头与实时尾
来源：http://ef.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ui.lnxyls.cn

[R54] 比较两个文件
来源：http://gr.newstarts.cn

diff a.txt b.txt
来源：http://zi.shxzskj.cn

[R55] 压缩与解压
来源：http://ev.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dn.gzmigu.cn

[R56] 远程拷贝
来源：http://pn.bjjhwx.cn

scp file user@host:/path/
来源：http://bq.szxytkj.cn

[R57] 远程执行命令
来源：http://ta.colortex.cn

ssh user@host 'uptime'
来源：http://nk.wgjwhj.cn

[R58] 下载文件
来源：http://yy.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fh.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://ro.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mk.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://ba.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uh.wgjwhj.cn

[R61] 磁盘占用
来源：http://wz.yuntaijiaju.cn

df -h;  du -sh *
来源：http://jp.asd995.cn

[R62] 找最占空间的文件
来源：http://sf.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://ra.huixinmuqiang.cn

[R63] 内存与进程
来源：http://mk.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://sr.huixiangedu.cn

[R64] 结束进程
来源：http://co.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://tb.hnjuh.cn

[R65] 查看端口占用
来源：http://vo.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dg.panjiajie.cn

[R66] 定时任务
来源：http://ny.wgjwhj.cn

crontab -e;  crontab -l
来源：http://kv.newstarts.cn

[R67] 生成随机十六进制串
来源：http://dd.chemitech.net.cn

openssl rand -hex 16
来源：http://yu.haigaiapp.cn

[R68] 计算文件校验值
来源：http://xn.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gz.shtwfgs.cn

[R69] 生成随机密码
来源：http://fp.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://el.hahajie.cn

[R70] 时间戳与互转
来源：http://xa.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://fu.jctech888.com.cn

[R71] 日期格式化
来源：http://qy.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lg.bjjhwx.cn

[R72] 等待端口就绪
来源：http://hy.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ew.shxzskj.cn

[R73] 分割大日志
来源：http://wq.yuexingan06.cn

split -l 1000 big.log part_
来源：http://cn.huanxung.cn

[R74] 批量重命名
来源：http://sw.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dx.wgjwhj.cn

[R75] 导出环境变量
来源：http://mh.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://lk.asd995.cn

[R76] 使用临时文件
来源：http://kx.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ip.shtwfgs.cn

[R77] 读取用户输入
来源：http://nt.yuexingan06.cn

read -rp "请输入: " ans
来源：http://uy.chemitech.net.cn

[R78] 交互式菜单
来源：http://jc.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bs.huanxung.cn

[R79] 解析命令行选项
来源：http://ti.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ej.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://kt.shxzukj.cn

time ./run.sh
来源：http://jo.newstarts.cn

================================================================================
来源：http://ks.yuntaijiaju.cn

S. C / C++ 专题
来源：http://vd.jianghongdianzi.cn

================================================================================
来源：http://yu.huixiangedu.cn

[S01] C：Hello World
来源：http://vc.9csxet.cn

#include <stdio.h>
来源：http://am.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xx.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://rn.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://fu.bjjhwx.cn

[S03] C：读入整数
来源：http://uf.asd995.cn

int x; scanf("%d", &x);
来源：http://yr.nicolike.cn

[S04] C：字符串复制
来源：http://rd.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ge.colortex.cn

[S05] C：字符串长度
来源：http://po.521024.cn

strlen(s)
来源：http://wv.szsharing.cn

[S06] C：字符串比较
来源：http://bm.chemitech.net.cn

strcmp(a, b) == 0
来源：http://rs.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://sa.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://os.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://sk.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iy.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://qx.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sk.muxihuayi.cn

[S10] C：指针与解引用
来源：http://ij.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://mj.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://wd.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://vu.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nu.521024.cn

fclose(f);
来源：http://hw.yuntaijiaju.cn

[S12] C：写文件
来源：http://yz.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hh.hahajie.cn

[S13] C：宏定义
来源：http://bb.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cl.asd995.cn

[S14] C：枚举
来源：http://bq.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://np.panjiajie.cn

[S15] C：类型转换
来源：http://tj.lnxyls.cn

(double) a / b
来源：http://gh.shtwfgs.cn

[S16] C：位操作置位
来源：http://nx.panjiajie.cn

x |= (1 << 3);
来源：http://gu.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://xy.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yl.shtwfgs.cn

[S18] C：命令行参数
来源：http://jp.huanxung.cn

int main(int argc, char **argv)
来源：http://ez.panjiajie.cn

[S19] C：快速排序
来源：http://xf.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lv.jianghongdianzi.cn

[S20] C：二分查找
来源：http://sd.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vc.huanxung.cn

[S21] C：字符类别判断
来源：http://rr.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zw.szxytkj.cn

[S22] C：字符串转数字
来源：http://bn.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mu.jctech888.com.cn

[S23] C：随机数
来源：http://ip.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bl.nszjky.cn

[S24] C：获取本地时间
来源：http://dx.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://es.9csxet.cn

[S25] C：内存拷贝
来源：http://he.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://xm.521024.cn

[S26] C：内存清零
来源：http://ho.shxzukj.cn


<!-- 参考信息 -->