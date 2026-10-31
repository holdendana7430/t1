代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qw.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://rp.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wj.jianghongdianzi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ve.gzmigu.cn

[Q61] 移动平均
来源：http://je.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lt.yuntaijiaju.cn

[Q62] 分组占比
来源：http://qn.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ao.chemitech.net.cn

[Q63] 开启事务
来源：http://vx.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fx.jianghongdianzi.cn

[Q64] 提交事务
来源：http://hy.nszjky.cn

COMMIT;
来源：http://jo.lnxyls.cn

[Q65] 回滚事务
来源：http://yl.muxihuayi.cn

ROLLBACK;
来源：http://lx.muxihuayi.cn

[Q66] 行锁查询
来源：http://nw.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gi.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://zj.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dq.hahajie.cn

[Q68] 保存点
来源：http://fe.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://zl.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://cx.bjjhwx.cn

[Q69] 查看执行计划
来源：http://hz.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wy.haigaiapp.cn

[Q70] 更新统计信息
来源：http://yz.chemitech.net.cn

ANALYZE TABLE users;
来源：http://nu.huixiangedu.cn

[Q71] 查看建表语句
来源：http://fx.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zg.asd995.cn

[Q72] 查看索引
来源：http://jc.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://rs.bookmarksfly.cn

[Q73] 查看表状态
来源：http://ea.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xb.huixiangedu.cn

[Q74] 强制使用索引
来源：http://zx.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ne.hahajie.cn

[Q75] 日期格式化
来源：http://xl.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ep.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iw.jctech888.com.cn

[Q76] 按天统计
来源：http://hi.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zf.colortex.cn

[Q77] 时间加减
来源：http://fz.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bn.muxihuayi.cn

[Q78] 当前时间
来源：http://om.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lv.yuexingan06.cn

[Q79] 字符串拼接
来源：http://hg.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://md.jianghongdianzi.cn

[Q80] 字符串截取
来源：http://au.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zs.bookmarksfly.cn

[Q81] 字符串替换
来源：http://tm.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ty.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://pd.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mf.chemitech.net.cn

[Q83] 大小写转换
来源：http://sc.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yk.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://gh.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://oi.hnjuh.cn

[Q85] 数值取整
来源：http://qe.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rp.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://su.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nv.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://jy.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bj.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://rz.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wi.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dr.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://pb.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nd.chemitech.net.cn

[Q90] 生成序号列
来源：http://qk.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vt.panjiajie.cn

================================================================================
来源：http://zs.haigaiapp.cn

R. Bash 专题
来源：http://hl.lnxyls.cn

================================================================================
来源：http://nn.colortex.cn

[R01] shebang 与严格模式
来源：http://pp.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://cp.jianghongdianzi.cn

set -euo pipefail
来源：http://pt.asd995.cn

[R02] 变量赋值与使用
来源：http://sj.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://xo.panjiajie.cn

[R03] 只读变量
来源：http://uh.lnxyls.cn

readonly PI=3.14
来源：http://mn.nszjky.cn

[R04] 位置参数
来源：http://yw.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uu.jianghongdianzi.cn

[R05] 参数默认值
来源：http://en.nszjky.cn

name="${1:-default}"
来源：http://oh.panjiajie.cn

[R06] 判断命令是否存在
来源：http://qm.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uk.chemitech.net.cn

[R07] if 判断文件
来源：http://et.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rg.huanxung.cn

[R08] 数值比较
来源：http://cf.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qx.lnxyls.cn

[R09] 字符串比较
来源：http://sb.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jl.9csxet.cn

[R10] 正则匹配
来源：http://zr.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rz.lnxyls.cn

[R11] case 多分支
来源：http://qq.huixinmuqiang.cn

case "$1" in
来源：http://oa.nszjky.cn

start) echo "启动" ;;
来源：http://qr.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://my.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://uc.nszjky.cn

esac
来源：http://kx.jctech888.com.cn

[R12] for 遍历文件
来源：http://lx.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://jt.nszjky.cn

[R13] for 计数循环
来源：http://yr.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://yn.shtwfgs.cn

[R14] C 风格 for
来源：http://az.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sg.szxytkj.cn

[R15] while 逐行读文件
来源：http://py.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eu.jianghongdianzi.cn

[R16] until 等待条件
来源：http://do.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ra.nicolike.cn

[R17] 数组定义与取值
来源：http://ok.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ac.newstarts.cn

[R18] 遍历数组
来源：http://ok.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kr.panjiajie.cn

[R19] 数组长度
来源：http://ym.szxytkj.cn

echo "${#arr[@]}"
来源：http://nl.hnjuh.cn

[R20] 关联数组（字典）
来源：http://if.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uy.newstarts.cn

[R21] 字符串长度
来源：http://aq.panjiajie.cn

echo "${#s}"
来源：http://kr.nicolike.cn

[R22] 截取子串
来源：http://bh.asd995.cn

echo "${s:0:5}"
来源：http://zn.hnjuh.cn

[R23] 字符串替换
来源：http://wy.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ey.wgjwhj.cn

[R24] 大小写转换
来源：http://zf.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vs.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://vz.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dq.hnjuh.cn

[R26] 命令替换
来源：http://jn.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://fq.shxzukj.cn

[R27] 算术展开
来源：http://ki.newstarts.cn

echo $((1 + 2 * 3))
来源：http://ne.gzmigu.cn

[R28] 浮点运算
来源：http://mw.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://qp.jianghongdianzi.cn

[R29] 定义函数
来源：http://rq.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ze.szsharing.cn

[R30] 函数返回状态码
来源：http://nc.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://pl.colortex.cn

[R31] 局部变量
来源：http://gw.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://ff.huixiangedu.cn

[R32] 参数个数校验
来源：http://uf.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ky.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://os.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jk.shxzukj.cn

[R34] 退出时清理
来源：http://ho.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nd.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://wm.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rd.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://wf.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sr.lnxyls.cn

[R37] 把输出赋给变量
来源：http://xi.bjjhwx.cn

files=$(ls -1)
来源：http://hg.panjiajie.cn

[R38] 管道串联
来源：http://tr.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://za.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://fy.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://br.jctech888.com.cn

[R40] 追加写日志
来源：http://dm.colortex.cn

echo "log" >> out.log
来源：http://iq.szsharing.cn

[R41] 丢弃输出
来源：http://gg.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://hw.521024.cn

[R42] 输入重定向
来源：http://cg.szxytkj.cn

wc -l < a.txt
来源：http://ac.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://vn.jctech888.com.cn

find . -name "*.log" -type f
来源：http://cj.newstarts.cn

[R44] 按修改时间查找
来源：http://hl.bjjhwx.cn

find . -mtime -7 -type f
来源：http://li.haigaiapp.cn

[R45] 批量删除
来源：http://pm.szsharing.cn

find . -name "*.tmp" -delete
来源：http://mn.huanxung.cn

[R46] 递归替换文件内容
来源：http://hr.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uw.szxytkj.cn

[R47] sed 单行替换
来源：http://xl.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ru.muxihuayi.cn

[R48] awk 取指定列
来源：http://da.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://hg.hahajie.cn

[R49] awk 带条件
来源：http://zh.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zl.bjjhwx.cn

[R50] awk 求和
来源：http://jn.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bw.521024.cn

[R51] 排序去重取前几
来源：http://wa.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ms.chemitech.net.cn

[R52] 统计行数
来源：http://ao.huixiangedu.cn

wc -l a.txt
来源：http://eg.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://gc.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ch.newstarts.cn

[R54] 比较两个文件
来源：http://tc.lnxyls.cn

diff a.txt b.txt
来源：http://ju.jctech888.com.cn

[R55] 压缩与解压
来源：http://ia.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://un.huixiangedu.cn

[R56] 远程拷贝
来源：http://jt.bjjhwx.cn

scp file user@host:/path/
来源：http://ld.shtwfgs.cn

[R57] 远程执行命令
来源：http://cj.newstarts.cn

ssh user@host 'uptime'
来源：http://bv.haigaiapp.cn

[R58] 下载文件
来源：http://vh.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pb.colortex.cn

[R59] 发 POST JSON
来源：http://uh.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gm.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://lp.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ql.szxytkj.cn

[R61] 磁盘占用
来源：http://yq.shxzukj.cn

df -h;  du -sh *
来源：http://wy.szxytkj.cn

[R62] 找最占空间的文件
来源：http://fz.asd995.cn

du -ah . | sort -rh | head -10
来源：http://bh.szsharing.cn

[R63] 内存与进程
来源：http://it.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://zs.szsharing.cn

[R64] 结束进程
来源：http://uu.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://kw.asd995.cn

[R65] 查看端口占用
来源：http://zw.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jo.hnjuh.cn

[R66] 定时任务
来源：http://mk.9csxet.cn

crontab -e;  crontab -l
来源：http://kn.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://rb.shtwfgs.cn

openssl rand -hex 16
来源：http://yw.shxzskj.cn

[R68] 计算文件校验值
来源：http://mt.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jk.muxihuayi.cn

[R69] 生成随机密码
来源：http://yf.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://nz.chemitech.net.cn

[R70] 时间戳与互转
来源：http://qk.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://ic.huixinmuqiang.cn

[R71] 日期格式化
来源：http://bt.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bo.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://yi.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qz.huanxung.cn

[R73] 分割大日志
来源：http://hn.asd995.cn

split -l 1000 big.log part_
来源：http://tr.gzmigu.cn

[R74] 批量重命名
来源：http://jk.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oj.szxytkj.cn

[R75] 导出环境变量
来源：http://nq.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://sw.huixiangedu.cn

[R76] 使用临时文件
来源：http://ko.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ey.shtwfgs.cn

[R77] 读取用户输入
来源：http://sb.gzmigu.cn

read -rp "请输入: " ans
来源：http://fn.521024.cn

[R78] 交互式菜单
来源：http://rh.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ug.wgjwhj.cn

[R79] 解析命令行选项
来源：http://wv.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ec.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://nl.bookmarksfly.cn

time ./run.sh
来源：http://ot.shtwfgs.cn

================================================================================
来源：http://vu.huanxung.cn

S. C / C++ 专题
来源：http://jd.chemitech.net.cn

================================================================================
来源：http://zo.yuntaijiaju.cn

[S01] C：Hello World
来源：http://wa.huixinmuqiang.cn

#include <stdio.h>
来源：http://hd.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://se.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://fw.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://sn.newstarts.cn

[S03] C：读入整数
来源：http://uo.521024.cn

int x; scanf("%d", &x);
来源：http://pu.jctech888.com.cn

[S04] C：字符串复制
来源：http://gf.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vg.asd995.cn

[S05] C：字符串长度
来源：http://iq.521024.cn

strlen(s)
来源：http://ri.shxzskj.cn

[S06] C：字符串比较
来源：http://hv.huanxung.cn

strcmp(a, b) == 0
来源：http://vm.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://fw.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nb.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://wc.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ob.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://fd.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uy.huixiangedu.cn

[S10] C：指针与解引用
来源：http://rw.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://gk.hahajie.cn

[S11] C：逐行读文件
来源：http://ho.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://wd.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mu.haigaiapp.cn

fclose(f);
来源：http://gx.shxzukj.cn

[S12] C：写文件
来源：http://lo.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://by.shxzukj.cn

[S13] C：宏定义
来源：http://xs.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://by.panjiajie.cn

[S14] C：枚举
来源：http://js.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://vz.wgjwhj.cn

[S15] C：类型转换
来源：http://gp.huanxung.cn

(double) a / b
来源：http://mj.521024.cn

[S16] C：位操作置位
来源：http://ls.muxihuayi.cn

x |= (1 << 3);
来源：http://dg.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://ts.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kv.colortex.cn

[S18] C：命令行参数
来源：http://qd.muxihuayi.cn

int main(int argc, char **argv)
来源：http://xk.shxzskj.cn

[S19] C：快速排序
来源：http://at.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://td.lnxyls.cn

[S20] C：二分查找
来源：http://ns.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yx.bjjhwx.cn

[S21] C：字符类别判断
来源：http://is.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ux.wgjwhj.cn

[S22] C：字符串转数字
来源：http://aa.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://co.shxzskj.cn

[S23] C：随机数
来源：http://cs.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uv.9csxet.cn

[S24] C：获取本地时间
来源：http://lg.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bo.521024.cn

[S25] C：内存拷贝
来源：http://qu.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://vj.bookmarksfly.cn

[S26] C：内存清零
来源：http://gm.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://li.bookmarksfly.cn

[S27] C：定义常量
来源：http://jt.nszjky.cn

const double PI = 3.14159;
来源：http://jb.wgjwhj.cn

[S28] C：静态变量
来源：http://my.shtwfgs.cn

static int counter = 0;
来源：http://bg.shxzukj.cn

[S29] C：变参函数
来源：http://fy.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mt.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://vc.huixiangedu.cn


<!-- 参考信息 -->