代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ge.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://ua.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kl.huixiangedu.cn

[Q57] 行号
来源：http://va.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ae.jianghongdianzi.cn

[Q58] 累计求和
来源：http://kc.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rm.gzmigu.cn

[Q59] 分组内累计
来源：http://bz.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uk.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://ij.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://va.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ml.9csxet.cn

[Q61] 移动平均
来源：http://wd.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oo.asd995.cn

[Q62] 分组占比
来源：http://jh.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rg.haigaiapp.cn

[Q63] 开启事务
来源：http://xs.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fe.asd995.cn

[Q64] 提交事务
来源：http://vr.huixiangedu.cn

COMMIT;
来源：http://ne.asd995.cn

[Q65] 回滚事务
来源：http://va.huanxung.cn

ROLLBACK;
来源：http://rs.shxzskj.cn

[Q66] 行锁查询
来源：http://yi.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xr.szxytkj.cn

[Q67] 设置隔离级别
来源：http://yt.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://az.9csxet.cn

[Q68] 保存点
来源：http://ic.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://wp.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://pu.wgjwhj.cn

[Q69] 查看执行计划
来源：http://ko.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ua.colortex.cn

[Q70] 更新统计信息
来源：http://ou.shxzukj.cn

ANALYZE TABLE users;
来源：http://mq.yuexingan06.cn

[Q71] 查看建表语句
来源：http://su.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zl.colortex.cn

[Q72] 查看索引
来源：http://gh.newstarts.cn

SHOW INDEX FROM users;
来源：http://gt.shxzukj.cn

[Q73] 查看表状态
来源：http://qg.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xk.colortex.cn

[Q74] 强制使用索引
来源：http://mv.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nd.521024.cn

[Q75] 日期格式化
来源：http://xx.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fi.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bz.asd995.cn

[Q76] 按天统计
来源：http://jx.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ok.huixiangedu.cn

[Q77] 时间加减
来源：http://oi.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kp.huixiangedu.cn

[Q78] 当前时间
来源：http://nh.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wv.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://rm.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qf.muxihuayi.cn

[Q80] 字符串截取
来源：http://fd.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fe.panjiajie.cn

[Q81] 字符串替换
来源：http://ak.yuexingan06.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://be.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://lc.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lb.shxzskj.cn

[Q83] 大小写转换
来源：http://bv.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lt.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://zb.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://rq.gzmigu.cn

[Q85] 数值取整
来源：http://sr.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yb.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://ys.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jd.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://mt.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nk.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://ta.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pl.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://je.asd995.cn

[Q89] 判断表是否存在
来源：http://nv.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zw.lnxyls.cn

[Q90] 生成序号列
来源：http://lg.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://is.huanxung.cn

================================================================================
来源：http://ih.bookmarksfly.cn

R. Bash 专题
来源：http://on.nszjky.cn

================================================================================
来源：http://sj.lnxyls.cn

[R01] shebang 与严格模式
来源：http://sp.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://vt.hnjuh.cn

set -euo pipefail
来源：http://nt.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://ke.nszjky.cn

name="Tom"; echo "$name"
来源：http://rr.shxzukj.cn

[R03] 只读变量
来源：http://hz.huixinmuqiang.cn

readonly PI=3.14
来源：http://sy.szsharing.cn

[R04] 位置参数
来源：http://dw.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nj.haigaiapp.cn

[R05] 参数默认值
来源：http://ya.shtwfgs.cn

name="${1:-default}"
来源：http://ty.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://ir.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hy.asd995.cn

[R07] if 判断文件
来源：http://hj.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xq.chemitech.net.cn

[R08] 数值比较
来源：http://jh.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dm.huixiangedu.cn

[R09] 字符串比较
来源：http://gz.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lc.huanxung.cn

[R10] 正则匹配
来源：http://uk.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ta.bjjhwx.cn

[R11] case 多分支
来源：http://vi.hahajie.cn

case "$1" in
来源：http://dy.shxzukj.cn

start) echo "启动" ;;
来源：http://du.colortex.cn

stop)  echo "停止" ;;
来源：http://fa.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://cu.bookmarksfly.cn

esac
来源：http://bo.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://qj.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://uz.nicolike.cn

[R13] for 计数循环
来源：http://oy.asd995.cn

for i in {1..10}; do echo "$i"; done
来源：http://av.nicolike.cn

[R14] C 风格 for
来源：http://gi.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ji.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://pc.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wf.shxzskj.cn

[R16] until 等待条件
来源：http://et.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mx.bjjhwx.cn

[R17] 数组定义与取值
来源：http://mc.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fs.shxzskj.cn

[R18] 遍历数组
来源：http://jw.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://if.shxzukj.cn

[R19] 数组长度
来源：http://io.yuexingan06.cn

echo "${#arr[@]}"
来源：http://lj.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://dy.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pq.panjiajie.cn

[R21] 字符串长度
来源：http://ui.nszjky.cn

echo "${#s}"
来源：http://ir.nicolike.cn

[R22] 截取子串
来源：http://ai.chemitech.net.cn

echo "${s:0:5}"
来源：http://wi.jianghongdianzi.cn

[R23] 字符串替换
来源：http://vc.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://du.huixiangedu.cn

[R24] 大小写转换
来源：http://pd.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kl.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://rw.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pg.newstarts.cn

[R26] 命令替换
来源：http://bc.colortex.cn

now=$(date +%F); echo "$now"
来源：http://mh.jianghongdianzi.cn

[R27] 算术展开
来源：http://ev.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://bn.nszjky.cn

[R28] 浮点运算
来源：http://bz.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://wx.jctech888.com.cn

[R29] 定义函数
来源：http://nk.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cc.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://lt.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://bt.hahajie.cn

[R31] 局部变量
来源：http://el.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://nx.bjjhwx.cn

[R32] 参数个数校验
来源：http://lo.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nz.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://cw.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qh.wgjwhj.cn

[R34] 退出时清理
来源：http://pq.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fi.shtwfgs.cn

[R35] 后台执行并等待
来源：http://ag.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dr.huanxung.cn

[R36] 并发执行多个任务
来源：http://mt.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://va.shxzskj.cn

[R37] 把输出赋给变量
来源：http://mk.jctech888.com.cn

files=$(ls -1)
来源：http://mx.panjiajie.cn

[R38] 管道串联
来源：http://xe.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://bb.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://cd.asd995.cn

cmd > out.log 2>&1
来源：http://rj.yuntaijiaju.cn

[R40] 追加写日志
来源：http://wy.muxihuayi.cn

echo "log" >> out.log
来源：http://ox.szsharing.cn

[R41] 丢弃输出
来源：http://jp.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://sq.hahajie.cn

[R42] 输入重定向
来源：http://dv.chemitech.net.cn

wc -l < a.txt
来源：http://zv.9csxet.cn

[R43] 按名字查找文件
来源：http://my.nicolike.cn

find . -name "*.log" -type f
来源：http://gh.chemitech.net.cn

[R44] 按修改时间查找
来源：http://dc.shtwfgs.cn

find . -mtime -7 -type f
来源：http://oo.muxihuayi.cn

[R45] 批量删除
来源：http://ui.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://xy.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://nj.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kf.huanxung.cn

[R47] sed 单行替换
来源：http://ok.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ei.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://ot.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://ms.huixiangedu.cn

[R49] awk 带条件
来源：http://vw.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://my.panjiajie.cn

[R50] awk 求和
来源：http://zx.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bz.gzmigu.cn

[R51] 排序去重取前几
来源：http://oa.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vd.9csxet.cn

[R52] 统计行数
来源：http://lo.jctech888.com.cn

wc -l a.txt
来源：http://rm.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://qz.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qr.haigaiapp.cn

[R54] 比较两个文件
来源：http://ce.hnjuh.cn

diff a.txt b.txt
来源：http://qg.panjiajie.cn

[R55] 压缩与解压
来源：http://ia.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rv.yuexingan06.cn

[R56] 远程拷贝
来源：http://qr.gzmigu.cn

scp file user@host:/path/
来源：http://gm.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://rl.szxytkj.cn

ssh user@host 'uptime'
来源：http://rr.9csxet.cn

[R58] 下载文件
来源：http://mr.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tx.hahajie.cn

[R59] 发 POST JSON
来源：http://fv.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ej.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://ai.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ni.hnjuh.cn

[R61] 磁盘占用
来源：http://ci.huixinmuqiang.cn

df -h;  du -sh *
来源：http://lw.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://je.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://gd.shxzukj.cn

[R63] 内存与进程
来源：http://xb.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://sh.yuexingan06.cn

[R64] 结束进程
来源：http://pv.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://bz.shxzskj.cn

[R65] 查看端口占用
来源：http://er.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ea.bjjhwx.cn

[R66] 定时任务
来源：http://pk.haigaiapp.cn

crontab -e;  crontab -l
来源：http://tq.asd995.cn

[R67] 生成随机十六进制串
来源：http://uv.asd995.cn

openssl rand -hex 16
来源：http://ng.muxihuayi.cn

[R68] 计算文件校验值
来源：http://ti.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pg.asd995.cn

[R69] 生成随机密码
来源：http://va.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://yd.shtwfgs.cn

[R70] 时间戳与互转
来源：http://ur.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://sq.9csxet.cn

[R71] 日期格式化
来源：http://iu.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ps.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://nc.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mx.asd995.cn

[R73] 分割大日志
来源：http://xk.asd995.cn

split -l 1000 big.log part_
来源：http://wx.shxzukj.cn

[R74] 批量重命名
来源：http://ik.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oi.muxihuayi.cn

[R75] 导出环境变量
来源：http://ya.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://vn.bjjhwx.cn

[R76] 使用临时文件
来源：http://ea.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yb.gzmigu.cn

[R77] 读取用户输入
来源：http://vk.panjiajie.cn

read -rp "请输入: " ans
来源：http://cn.muxihuayi.cn

[R78] 交互式菜单
来源：http://om.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bz.9csxet.cn

[R79] 解析命令行选项
来源：http://uo.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qx.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://am.muxihuayi.cn

time ./run.sh
来源：http://vb.muxihuayi.cn

================================================================================
来源：http://ee.yuexingan06.cn

S. C / C++ 专题
来源：http://qm.colortex.cn

================================================================================
来源：http://hx.bookmarksfly.cn

[S01] C：Hello World
来源：http://mu.9csxet.cn

#include <stdio.h>
来源：http://jv.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nq.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://am.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://sb.bookmarksfly.cn

[S03] C：读入整数
来源：http://ym.panjiajie.cn

int x; scanf("%d", &x);
来源：http://ud.panjiajie.cn

[S04] C：字符串复制
来源：http://pc.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yi.colortex.cn

[S05] C：字符串长度
来源：http://za.huanxung.cn

strlen(s)
来源：http://sl.nicolike.cn

[S06] C：字符串比较
来源：http://pk.hnjuh.cn

strcmp(a, b) == 0
来源：http://uc.newstarts.cn

[S07] C：数组遍历求和
来源：http://mh.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gy.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://or.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nq.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://vm.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yi.521024.cn

[S10] C：指针与解引用
来源：http://bv.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://qc.shxzskj.cn

[S11] C：逐行读文件
来源：http://jl.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://ta.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hu.muxihuayi.cn

fclose(f);
来源：http://lb.newstarts.cn

[S12] C：写文件
来源：http://nu.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://br.hnjuh.cn

[S13] C：宏定义
来源：http://qr.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rq.shtwfgs.cn

[S14] C：枚举
来源：http://ty.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://ss.jctech888.com.cn

[S15] C：类型转换
来源：http://lu.bookmarksfly.cn

(double) a / b
来源：http://yw.muxihuayi.cn

[S16] C：位操作置位
来源：http://bt.shxzukj.cn

x |= (1 << 3);
来源：http://nz.nszjky.cn

[S17] C：安全拼接字符串
来源：http://vn.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mf.huanxung.cn

[S18] C：命令行参数
来源：http://vt.lnxyls.cn

int main(int argc, char **argv)
来源：http://oz.hahajie.cn

[S19] C：快速排序
来源：http://ie.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tc.asd995.cn

[S20] C：二分查找
来源：http://ye.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nn.shxzukj.cn

[S21] C：字符类别判断
来源：http://or.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ze.521024.cn

[S22] C：字符串转数字
来源：http://bp.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fm.huixiangedu.cn

[S23] C：随机数
来源：http://dd.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bb.hahajie.cn

[S24] C：获取本地时间
来源：http://tf.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://li.huixiangedu.cn

[S25] C：内存拷贝
来源：http://vi.nicolike.cn

memcpy(dst, src, n);
来源：http://oy.jctech888.com.cn

[S26] C：内存清零
来源：http://yb.colortex.cn


<!-- 参考信息 -->