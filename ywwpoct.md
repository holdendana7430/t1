代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yn.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://cl.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ew.hnjuh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bs.huixinmuqiang.cn

[Q61] 移动平均
来源：http://zu.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oc.gzmigu.cn

[Q62] 分组占比
来源：http://sc.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jf.521024.cn

[Q63] 开启事务
来源：http://rh.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wv.huixiangedu.cn

[Q64] 提交事务
来源：http://em.shxzskj.cn

COMMIT;
来源：http://wa.521024.cn

[Q65] 回滚事务
来源：http://oa.yuexingan06.cn

ROLLBACK;
来源：http://bn.shxzskj.cn

[Q66] 行锁查询
来源：http://lg.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://py.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://uw.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hl.yuexingan06.cn

[Q68] 保存点
来源：http://uc.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://nw.asd995.cn

ROLLBACK TO sp1;
来源：http://ds.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://cw.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pd.9csxet.cn

[Q70] 更新统计信息
来源：http://sd.szsharing.cn

ANALYZE TABLE users;
来源：http://xu.lnxyls.cn

[Q71] 查看建表语句
来源：http://ui.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bu.nicolike.cn

[Q72] 查看索引
来源：http://vs.shxzukj.cn

SHOW INDEX FROM users;
来源：http://jo.newstarts.cn

[Q73] 查看表状态
来源：http://co.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bf.newstarts.cn

[Q74] 强制使用索引
来源：http://kx.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cf.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://wt.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qz.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bg.nicolike.cn

[Q76] 按天统计
来源：http://em.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wl.gzmigu.cn

[Q77] 时间加减
来源：http://ho.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://br.huixinmuqiang.cn

[Q78] 当前时间
来源：http://nw.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ce.shxzskj.cn

[Q79] 字符串拼接
来源：http://wh.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qo.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://ak.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mp.bookmarksfly.cn

[Q81] 字符串替换
来源：http://wh.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zp.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://ay.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jw.wgjwhj.cn

[Q83] 大小写转换
来源：http://gt.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ml.panjiajie.cn

[Q84] 去除首尾空格
来源：http://bo.521024.cn

SELECT TRIM(name) FROM users;
来源：http://fs.shxzskj.cn

[Q85] 数值取整
来源：http://ii.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yg.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://jc.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pp.9csxet.cn

[Q87] JSON 字段做条件
来源：http://eq.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ow.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://vh.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://be.huixinmuqiang.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wd.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://te.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ra.lnxyls.cn

[Q90] 生成序号列
来源：http://dp.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mq.chemitech.net.cn

================================================================================
来源：http://dm.asd995.cn

R. Bash 专题
来源：http://og.shxzukj.cn

================================================================================
来源：http://or.huanxung.cn

[R01] shebang 与严格模式
来源：http://mi.newstarts.cn

#!/usr/bin/env bash
来源：http://zd.yuexingan06.cn

set -euo pipefail
来源：http://ku.huanxung.cn

[R02] 变量赋值与使用
来源：http://vm.asd995.cn

name="Tom"; echo "$name"
来源：http://pu.nicolike.cn

[R03] 只读变量
来源：http://tz.huixiangedu.cn

readonly PI=3.14
来源：http://ys.yuntaijiaju.cn

[R04] 位置参数
来源：http://tw.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oc.colortex.cn

[R05] 参数默认值
来源：http://wi.lnxyls.cn

name="${1:-default}"
来源：http://jk.9csxet.cn

[R06] 判断命令是否存在
来源：http://ro.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mj.hahajie.cn

[R07] if 判断文件
来源：http://ih.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cs.jianghongdianzi.cn

[R08] 数值比较
来源：http://kv.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ov.shtwfgs.cn

[R09] 字符串比较
来源：http://qq.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mj.huixinmuqiang.cn

[R10] 正则匹配
来源：http://kc.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rh.lnxyls.cn

[R11] case 多分支
来源：http://gs.yuntaijiaju.cn

case "$1" in
来源：http://pd.9csxet.cn

start) echo "启动" ;;
来源：http://ed.panjiajie.cn

stop)  echo "停止" ;;
来源：http://nc.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://vu.asd995.cn

esac
来源：http://dp.wgjwhj.cn

[R12] for 遍历文件
来源：http://wj.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://gs.huixinmuqiang.cn

[R13] for 计数循环
来源：http://iu.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://sd.shxzukj.cn

[R14] C 风格 for
来源：http://md.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ho.521024.cn

[R15] while 逐行读文件
来源：http://hj.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dx.wgjwhj.cn

[R16] until 等待条件
来源：http://ru.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gg.nszjky.cn

[R17] 数组定义与取值
来源：http://zj.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hq.jctech888.com.cn

[R18] 遍历数组
来源：http://yi.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uv.hahajie.cn

[R19] 数组长度
来源：http://zj.wgjwhj.cn

echo "${#arr[@]}"
来源：http://so.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://va.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xx.nszjky.cn

[R21] 字符串长度
来源：http://ns.jianghongdianzi.cn

echo "${#s}"
来源：http://tk.shxzukj.cn

[R22] 截取子串
来源：http://kx.shtwfgs.cn

echo "${s:0:5}"
来源：http://vv.bjjhwx.cn

[R23] 字符串替换
来源：http://xn.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kd.colortex.cn

[R24] 大小写转换
来源：http://rq.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gp.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://ld.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fh.szxytkj.cn

[R26] 命令替换
来源：http://in.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://ut.huixiangedu.cn

[R27] 算术展开
来源：http://ju.9csxet.cn

echo $((1 + 2 * 3))
来源：http://yr.szsharing.cn

[R28] 浮点运算
来源：http://fu.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://sk.gzmigu.cn

[R29] 定义函数
来源：http://wt.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eo.asd995.cn

[R30] 函数返回状态码
来源：http://gz.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://lo.shtwfgs.cn

[R31] 局部变量
来源：http://ct.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://nu.asd995.cn

[R32] 参数个数校验
来源：http://ec.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pt.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://wu.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yi.521024.cn

[R34] 退出时清理
来源：http://ek.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ii.9csxet.cn

[R35] 后台执行并等待
来源：http://mg.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zs.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://gu.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://id.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://hy.nicolike.cn

files=$(ls -1)
来源：http://do.nicolike.cn

[R38] 管道串联
来源：http://py.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://lp.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://kg.huanxung.cn

cmd > out.log 2>&1
来源：http://pe.muxihuayi.cn

[R40] 追加写日志
来源：http://lw.asd995.cn

echo "log" >> out.log
来源：http://tn.nszjky.cn

[R41] 丢弃输出
来源：http://vr.nicolike.cn

cmd >/dev/null 2>&1
来源：http://dd.chemitech.net.cn

[R42] 输入重定向
来源：http://jv.muxihuayi.cn

wc -l < a.txt
来源：http://uc.huixiangedu.cn

[R43] 按名字查找文件
来源：http://ge.shtwfgs.cn

find . -name "*.log" -type f
来源：http://ov.asd995.cn

[R44] 按修改时间查找
来源：http://uq.panjiajie.cn

find . -mtime -7 -type f
来源：http://of.huixiangedu.cn

[R45] 批量删除
来源：http://bw.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://rq.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://fc.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cb.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://lz.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ww.nicolike.cn

[R48] awk 取指定列
来源：http://ox.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://sh.shtwfgs.cn

[R49] awk 带条件
来源：http://ap.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sr.huanxung.cn

[R50] awk 求和
来源：http://bs.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qv.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://jp.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ex.nicolike.cn

[R52] 统计行数
来源：http://ob.newstarts.cn

wc -l a.txt
来源：http://wt.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://pm.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oo.bjjhwx.cn

[R54] 比较两个文件
来源：http://wp.hahajie.cn

diff a.txt b.txt
来源：http://gp.shxzukj.cn

[R55] 压缩与解压
来源：http://bu.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lq.bjjhwx.cn

[R56] 远程拷贝
来源：http://dm.nszjky.cn

scp file user@host:/path/
来源：http://rm.yuexingan06.cn

[R57] 远程执行命令
来源：http://ar.huixiangedu.cn

ssh user@host 'uptime'
来源：http://if.haigaiapp.cn

[R58] 下载文件
来源：http://vj.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://in.lnxyls.cn

[R59] 发 POST JSON
来源：http://jt.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ck.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://xa.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rb.huixiangedu.cn

[R61] 磁盘占用
来源：http://gt.hnjuh.cn

df -h;  du -sh *
来源：http://xm.9csxet.cn

[R62] 找最占空间的文件
来源：http://qb.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://be.szxytkj.cn

[R63] 内存与进程
来源：http://tw.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://wh.huixinmuqiang.cn

[R64] 结束进程
来源：http://pg.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://ga.bjjhwx.cn

[R65] 查看端口占用
来源：http://mk.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uk.shtwfgs.cn

[R66] 定时任务
来源：http://ro.9csxet.cn

crontab -e;  crontab -l
来源：http://ac.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://en.hnjuh.cn

openssl rand -hex 16
来源：http://kv.muxihuayi.cn

[R68] 计算文件校验值
来源：http://nb.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oo.colortex.cn

[R69] 生成随机密码
来源：http://gl.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://lh.szsharing.cn

[R70] 时间戳与互转
来源：http://em.9csxet.cn

date +%s;  date -d @1700000000
来源：http://fa.shxzskj.cn

[R71] 日期格式化
来源：http://qh.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ja.hnjuh.cn

[R72] 等待端口就绪
来源：http://ll.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jf.szxytkj.cn

[R73] 分割大日志
来源：http://uz.lnxyls.cn

split -l 1000 big.log part_
来源：http://hn.hnjuh.cn

[R74] 批量重命名
来源：http://vj.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ye.shxzskj.cn

[R75] 导出环境变量
来源：http://oo.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://pv.szsharing.cn

[R76] 使用临时文件
来源：http://nn.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ys.jctech888.com.cn

[R77] 读取用户输入
来源：http://eu.szxytkj.cn

read -rp "请输入: " ans
来源：http://xl.hnjuh.cn

[R78] 交互式菜单
来源：http://ea.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gc.asd995.cn

[R79] 解析命令行选项
来源：http://wf.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rl.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://ua.chemitech.net.cn

time ./run.sh
来源：http://ci.hnjuh.cn

================================================================================
来源：http://lh.jianghongdianzi.cn

S. C / C++ 专题
来源：http://xa.shtwfgs.cn

================================================================================
来源：http://ct.9csxet.cn

[S01] C：Hello World
来源：http://bd.nszjky.cn

#include <stdio.h>
来源：http://hk.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qi.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://zf.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://ki.nicolike.cn

[S03] C：读入整数
来源：http://uh.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://tx.521024.cn

[S04] C：字符串复制
来源：http://wv.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qa.chemitech.net.cn

[S05] C：字符串长度
来源：http://pq.yuntaijiaju.cn

strlen(s)
来源：http://ni.gzmigu.cn

[S06] C：字符串比较
来源：http://ld.gzmigu.cn

strcmp(a, b) == 0
来源：http://wp.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://nc.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rm.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://pw.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://po.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://ts.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vr.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://hk.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://vp.nicolike.cn

[S11] C：逐行读文件
来源：http://em.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://ij.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mv.bookmarksfly.cn

fclose(f);
来源：http://op.huixiangedu.cn

[S12] C：写文件
来源：http://vs.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yt.521024.cn

[S13] C：宏定义
来源：http://bm.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ng.chemitech.net.cn

[S14] C：枚举
来源：http://mt.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://rt.asd995.cn

[S15] C：类型转换
来源：http://sp.huixiangedu.cn

(double) a / b
来源：http://pn.shtwfgs.cn

[S16] C：位操作置位
来源：http://vx.asd995.cn

x |= (1 << 3);
来源：http://mm.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://np.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bv.nszjky.cn

[S18] C：命令行参数
来源：http://oj.nicolike.cn

int main(int argc, char **argv)
来源：http://si.szxytkj.cn

[S19] C：快速排序
来源：http://jz.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yk.chemitech.net.cn

[S20] C：二分查找
来源：http://uf.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kd.newstarts.cn

[S21] C：字符类别判断
来源：http://hy.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yj.shtwfgs.cn

[S22] C：字符串转数字
来源：http://bo.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vw.szxytkj.cn

[S23] C：随机数
来源：http://by.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ws.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://sl.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rd.wgjwhj.cn

[S25] C：内存拷贝
来源：http://zk.shtwfgs.cn

memcpy(dst, src, n);
来源：http://dm.shxzskj.cn

[S26] C：内存清零
来源：http://bg.hahajie.cn

memset(a, 0, sizeof a);
来源：http://vj.szsharing.cn

[S27] C：定义常量
来源：http://eu.colortex.cn

const double PI = 3.14159;
来源：http://pd.nszjky.cn

[S28] C：静态变量
来源：http://dp.huixinmuqiang.cn

static int counter = 0;
来源：http://gm.jctech888.com.cn

[S29] C：变参函数
来源：http://kv.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sp.huixiangedu.cn

[S30] C：头文件保护
来源：http://pq.jianghongdianzi.cn


<!-- 参考信息 -->