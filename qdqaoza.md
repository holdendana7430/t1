代发 wailian999

[Q61] 移动平均
来源：http://xj.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vs.bookmarksfly.cn

[Q62] 分组占比
来源：http://tv.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xb.szsharing.cn

[Q63] 开启事务
来源：http://hv.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zb.panjiajie.cn

[Q64] 提交事务
来源：http://ri.szxytkj.cn

COMMIT;
来源：http://kr.panjiajie.cn

[Q65] 回滚事务
来源：http://cz.haigaiapp.cn

ROLLBACK;
来源：http://mb.yuexingan06.cn

[Q66] 行锁查询
来源：http://ny.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qa.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://pt.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ea.9csxet.cn

[Q68] 保存点
来源：http://zu.asd995.cn

SAVEPOINT sp1;
来源：http://zn.szxytkj.cn

ROLLBACK TO sp1;
来源：http://qs.yuexingan06.cn

[Q69] 查看执行计划
来源：http://gf.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nk.gzmigu.cn

[Q70] 更新统计信息
来源：http://bq.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://re.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://ov.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qt.huixiangedu.cn

[Q72] 查看索引
来源：http://os.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://sr.bjjhwx.cn

[Q73] 查看表状态
来源：http://ey.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yc.bjjhwx.cn

[Q74] 强制使用索引
来源：http://zz.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yg.shtwfgs.cn

[Q75] 日期格式化
来源：http://bp.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ss.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://de.9csxet.cn

[Q76] 按天统计
来源：http://li.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cv.nicolike.cn

[Q77] 时间加减
来源：http://pw.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dp.521024.cn

[Q78] 当前时间
来源：http://md.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hk.hnjuh.cn

[Q79] 字符串拼接
来源：http://mo.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xb.gzmigu.cn

[Q80] 字符串截取
来源：http://vb.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://am.bjjhwx.cn

[Q81] 字符串替换
来源：http://pe.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qg.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://ab.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://il.bookmarksfly.cn

[Q83] 大小写转换
来源：http://xb.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://px.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://ey.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://ue.jianghongdianzi.cn

[Q85] 数值取整
来源：http://nn.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mo.asd995.cn

[Q86] 读取 JSON 字段
来源：http://sg.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fs.nicolike.cn

[Q87] JSON 字段做条件
来源：http://bt.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xk.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://la.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oh.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jx.newstarts.cn

[Q89] 判断表是否存在
来源：http://rt.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qj.hahajie.cn

[Q90] 生成序号列
来源：http://au.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sm.newstarts.cn

================================================================================
来源：http://ee.asd995.cn

R. Bash 专题
来源：http://zt.haigaiapp.cn

================================================================================
来源：http://mo.colortex.cn

[R01] shebang 与严格模式
来源：http://ql.colortex.cn

#!/usr/bin/env bash
来源：http://ci.521024.cn

set -euo pipefail
来源：http://vo.asd995.cn

[R02] 变量赋值与使用
来源：http://rn.521024.cn

name="Tom"; echo "$name"
来源：http://oq.bjjhwx.cn

[R03] 只读变量
来源：http://zy.hahajie.cn

readonly PI=3.14
来源：http://nh.521024.cn

[R04] 位置参数
来源：http://wo.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kp.newstarts.cn

[R05] 参数默认值
来源：http://jj.szxytkj.cn

name="${1:-default}"
来源：http://dz.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://ai.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zp.shxzukj.cn

[R07] if 判断文件
来源：http://xg.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://it.9csxet.cn

[R08] 数值比较
来源：http://jl.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ey.gzmigu.cn

[R09] 字符串比较
来源：http://nj.nszjky.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cw.shxzskj.cn

[R10] 正则匹配
来源：http://kh.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mu.colortex.cn

[R11] case 多分支
来源：http://ci.shtwfgs.cn

case "$1" in
来源：http://vc.chemitech.net.cn

start) echo "启动" ;;
来源：http://ic.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://db.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://ls.lnxyls.cn

esac
来源：http://fx.shxzukj.cn

[R12] for 遍历文件
来源：http://rk.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://bx.lnxyls.cn

[R13] for 计数循环
来源：http://hk.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://il.szxytkj.cn

[R14] C 风格 for
来源：http://vl.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gh.asd995.cn

[R15] while 逐行读文件
来源：http://lh.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pt.szxytkj.cn

[R16] until 等待条件
来源：http://xj.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wn.shxzskj.cn

[R17] 数组定义与取值
来源：http://rg.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tc.gzmigu.cn

[R18] 遍历数组
来源：http://xz.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gh.hnjuh.cn

[R19] 数组长度
来源：http://rq.9csxet.cn

echo "${#arr[@]}"
来源：http://st.hahajie.cn

[R20] 关联数组（字典）
来源：http://or.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bp.jianghongdianzi.cn

[R21] 字符串长度
来源：http://xz.colortex.cn

echo "${#s}"
来源：http://mc.muxihuayi.cn

[R22] 截取子串
来源：http://rl.hnjuh.cn

echo "${s:0:5}"
来源：http://ik.newstarts.cn

[R23] 字符串替换
来源：http://je.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jx.shxzukj.cn

[R24] 大小写转换
来源：http://tw.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ph.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://ez.lnxyls.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cg.bjjhwx.cn

[R26] 命令替换
来源：http://ah.521024.cn

now=$(date +%F); echo "$now"
来源：http://kn.huixiangedu.cn

[R27] 算术展开
来源：http://tv.nszjky.cn

echo $((1 + 2 * 3))
来源：http://jj.panjiajie.cn

[R28] 浮点运算
来源：http://uy.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://ii.hahajie.cn

[R29] 定义函数
来源：http://fc.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bm.asd995.cn

[R30] 函数返回状态码
来源：http://qi.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://gs.shxzukj.cn

[R31] 局部变量
来源：http://mn.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://vc.newstarts.cn

[R32] 参数个数校验
来源：http://xl.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hk.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://jy.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kq.huixinmuqiang.cn

[R34] 退出时清理
来源：http://kg.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bx.shxzskj.cn

[R35] 后台执行并等待
来源：http://iu.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ey.nszjky.cn

[R36] 并发执行多个任务
来源：http://lz.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rs.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://hi.yuntaijiaju.cn

files=$(ls -1)
来源：http://zt.muxihuayi.cn

[R38] 管道串联
来源：http://sg.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://ae.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://ha.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://eu.huanxung.cn

[R40] 追加写日志
来源：http://cm.nszjky.cn

echo "log" >> out.log
来源：http://vi.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://iz.newstarts.cn

cmd >/dev/null 2>&1
来源：http://cn.jianghongdianzi.cn

[R42] 输入重定向
来源：http://mj.gzmigu.cn

wc -l < a.txt
来源：http://iu.panjiajie.cn

[R43] 按名字查找文件
来源：http://ch.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://kw.shtwfgs.cn

[R44] 按修改时间查找
来源：http://wb.nszjky.cn

find . -mtime -7 -type f
来源：http://fy.newstarts.cn

[R45] 批量删除
来源：http://ug.newstarts.cn

find . -name "*.tmp" -delete
来源：http://iy.shxzskj.cn

[R46] 递归替换文件内容
来源：http://wu.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://he.521024.cn

[R47] sed 单行替换
来源：http://ae.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oz.jctech888.com.cn

[R48] awk 取指定列
来源：http://zs.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://uz.wgjwhj.cn

[R49] awk 带条件
来源：http://va.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mw.szxytkj.cn

[R50] awk 求和
来源：http://jt.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xo.newstarts.cn

[R51] 排序去重取前几
来源：http://zv.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ud.shtwfgs.cn

[R52] 统计行数
来源：http://tg.hahajie.cn

wc -l a.txt
来源：http://mb.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://yk.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://em.521024.cn

[R54] 比较两个文件
来源：http://hu.hahajie.cn

diff a.txt b.txt
来源：http://xn.9csxet.cn

[R55] 压缩与解压
来源：http://pk.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://si.nszjky.cn

[R56] 远程拷贝
来源：http://ox.newstarts.cn

scp file user@host:/path/
来源：http://so.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://dw.9csxet.cn

ssh user@host 'uptime'
来源：http://dr.nicolike.cn

[R58] 下载文件
来源：http://ly.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kt.hahajie.cn

[R59] 发 POST JSON
来源：http://rc.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lj.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://eo.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pw.521024.cn

[R61] 磁盘占用
来源：http://vw.muxihuayi.cn

df -h;  du -sh *
来源：http://xq.colortex.cn

[R62] 找最占空间的文件
来源：http://ak.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://qk.asd995.cn

[R63] 内存与进程
来源：http://sy.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://oe.gzmigu.cn

[R64] 结束进程
来源：http://qo.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://ql.newstarts.cn

[R65] 查看端口占用
来源：http://dz.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dp.huixinmuqiang.cn

[R66] 定时任务
来源：http://yw.gzmigu.cn

crontab -e;  crontab -l
来源：http://gi.asd995.cn

[R67] 生成随机十六进制串
来源：http://fo.shtwfgs.cn

openssl rand -hex 16
来源：http://xm.szsharing.cn

[R68] 计算文件校验值
来源：http://tl.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ck.shxzskj.cn

[R69] 生成随机密码
来源：http://si.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://xf.szxytkj.cn

[R70] 时间戳与互转
来源：http://sk.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://kq.yuexingan06.cn

[R71] 日期格式化
来源：http://pg.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ba.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://ja.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wt.bookmarksfly.cn

[R73] 分割大日志
来源：http://in.shxzskj.cn

split -l 1000 big.log part_
来源：http://ku.hnjuh.cn

[R74] 批量重命名
来源：http://nx.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wf.nszjky.cn

[R75] 导出环境变量
来源：http://ax.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://ru.hahajie.cn

[R76] 使用临时文件
来源：http://ix.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mm.shxzskj.cn

[R77] 读取用户输入
来源：http://vz.newstarts.cn

read -rp "请输入: " ans
来源：http://uk.hahajie.cn

[R78] 交互式菜单
来源：http://oc.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vi.lnxyls.cn

[R79] 解析命令行选项
来源：http://wz.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oj.colortex.cn

[R80] 查看脚本执行耗时
来源：http://mi.lnxyls.cn

time ./run.sh
来源：http://rs.chemitech.net.cn

================================================================================
来源：http://vc.nicolike.cn

S. C / C++ 专题
来源：http://xt.asd995.cn

================================================================================
来源：http://px.521024.cn

[S01] C：Hello World
来源：http://mh.huanxung.cn

#include <stdio.h>
来源：http://eu.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fq.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://ue.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://gn.shtwfgs.cn

[S03] C：读入整数
来源：http://rg.nszjky.cn

int x; scanf("%d", &x);
来源：http://gk.lnxyls.cn

[S04] C：字符串复制
来源：http://bj.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fa.hnjuh.cn

[S05] C：字符串长度
来源：http://nh.huixinmuqiang.cn

strlen(s)
来源：http://dg.szsharing.cn

[S06] C：字符串比较
来源：http://uy.bjjhwx.cn

strcmp(a, b) == 0
来源：http://rq.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://wu.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mr.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://tz.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://db.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://ke.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ts.hahajie.cn

[S10] C：指针与解引用
来源：http://wz.hahajie.cn

int *p = &a;  *p = 5;
来源：http://bq.muxihuayi.cn

[S11] C：逐行读文件
来源：http://fb.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://rn.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rd.huixinmuqiang.cn

fclose(f);
来源：http://nj.bookmarksfly.cn

[S12] C：写文件
来源：http://vn.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ag.szxytkj.cn

[S13] C：宏定义
来源：http://tw.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ts.shxzskj.cn

[S14] C：枚举
来源：http://qt.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://dm.panjiajie.cn

[S15] C：类型转换
来源：http://hy.huixiangedu.cn

(double) a / b
来源：http://jl.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://zn.chemitech.net.cn

x |= (1 << 3);
来源：http://nh.szsharing.cn

[S17] C：安全拼接字符串
来源：http://xw.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dr.jctech888.com.cn

[S18] C：命令行参数
来源：http://uj.shxzukj.cn

int main(int argc, char **argv)
来源：http://no.nicolike.cn

[S19] C：快速排序
来源：http://ui.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yu.nszjky.cn

[S20] C：二分查找
来源：http://kw.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aq.nicolike.cn

[S21] C：字符类别判断
来源：http://ft.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ld.wgjwhj.cn

[S22] C：字符串转数字
来源：http://tz.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gq.muxihuayi.cn

[S23] C：随机数
来源：http://io.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://se.asd995.cn

[S24] C：获取本地时间
来源：http://ca.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ps.lnxyls.cn

[S25] C：内存拷贝
来源：http://ib.asd995.cn

memcpy(dst, src, n);
来源：http://bz.gzmigu.cn

[S26] C：内存清零
来源：http://mm.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://vk.9csxet.cn

[S27] C：定义常量
来源：http://nq.chemitech.net.cn

const double PI = 3.14159;
来源：http://rb.haigaiapp.cn

[S28] C：静态变量
来源：http://wz.nszjky.cn

static int counter = 0;
来源：http://dz.chemitech.net.cn

[S29] C：变参函数
来源：http://ca.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mx.huanxung.cn

[S30] C：头文件保护
来源：http://yv.bjjhwx.cn

#ifndef X_H
来源：http://hv.bjjhwx.cn

#define X_H
来源：http://yr.nicolike.cn

#endif
来源：http://tt.shtwfgs.cn

[S31] C++：Hello World
来源：http://bm.colortex.cn


<!-- 参考信息 -->