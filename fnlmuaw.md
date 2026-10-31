代发 wailian999

[Q61] 移动平均
来源：http://tc.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nf.521024.cn

[Q62] 分组占比
来源：http://jy.shtwfgs.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mw.shxzukj.cn

[Q63] 开启事务
来源：http://ag.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tb.shxzukj.cn

[Q64] 提交事务
来源：http://jt.yuntaijiaju.cn

COMMIT;
来源：http://vu.hnjuh.cn

[Q65] 回滚事务
来源：http://an.shxzukj.cn

ROLLBACK;
来源：http://qh.yuexingan06.cn

[Q66] 行锁查询
来源：http://qz.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ws.nszjky.cn

[Q67] 设置隔离级别
来源：http://ye.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fe.jianghongdianzi.cn

[Q68] 保存点
来源：http://dc.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://th.lnxyls.cn

ROLLBACK TO sp1;
来源：http://zv.chemitech.net.cn

[Q69] 查看执行计划
来源：http://li.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qn.gzmigu.cn

[Q70] 更新统计信息
来源：http://uc.shxzukj.cn

ANALYZE TABLE users;
来源：http://py.shtwfgs.cn

[Q71] 查看建表语句
来源：http://gh.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qw.newstarts.cn

[Q72] 查看索引
来源：http://hm.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://mm.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://ys.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://el.huixiangedu.cn

[Q74] 强制使用索引
来源：http://ec.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://av.panjiajie.cn

[Q75] 日期格式化
来源：http://fw.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xi.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tw.shtwfgs.cn

[Q76] 按天统计
来源：http://kr.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fd.yuntaijiaju.cn

[Q77] 时间加减
来源：http://vr.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oa.yuntaijiaju.cn

[Q78] 当前时间
来源：http://qb.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zl.shxzukj.cn

[Q79] 字符串拼接
来源：http://nk.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bb.haigaiapp.cn

[Q80] 字符串截取
来源：http://mg.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://or.jctech888.com.cn

[Q81] 字符串替换
来源：http://rc.bookmarksfly.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ra.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://nx.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vo.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://gh.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vp.hnjuh.cn

[Q84] 去除首尾空格
来源：http://js.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://cc.huixinmuqiang.cn

[Q85] 数值取整
来源：http://ez.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bo.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://iv.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hj.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://kb.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kp.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://bh.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jn.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eg.colortex.cn

[Q89] 判断表是否存在
来源：http://go.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://he.colortex.cn

[Q90] 生成序号列
来源：http://bn.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ay.jctech888.com.cn

================================================================================
来源：http://mz.shxzskj.cn

R. Bash 专题
来源：http://ch.panjiajie.cn

================================================================================
来源：http://uh.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://ar.colortex.cn

#!/usr/bin/env bash
来源：http://gp.chemitech.net.cn

set -euo pipefail
来源：http://eb.huanxung.cn

[R02] 变量赋值与使用
来源：http://co.9csxet.cn

name="Tom"; echo "$name"
来源：http://nb.521024.cn

[R03] 只读变量
来源：http://rp.haigaiapp.cn

readonly PI=3.14
来源：http://dm.lnxyls.cn

[R04] 位置参数
来源：http://ya.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://li.muxihuayi.cn

[R05] 参数默认值
来源：http://jb.muxihuayi.cn

name="${1:-default}"
来源：http://cu.nicolike.cn

[R06] 判断命令是否存在
来源：http://om.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gv.huixiangedu.cn

[R07] if 判断文件
来源：http://wo.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xi.szsharing.cn

[R08] 数值比较
来源：http://bp.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fp.shxzukj.cn

[R09] 字符串比较
来源：http://jq.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wj.yuntaijiaju.cn

[R10] 正则匹配
来源：http://qo.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ov.jianghongdianzi.cn

[R11] case 多分支
来源：http://yf.yuntaijiaju.cn

case "$1" in
来源：http://px.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://uc.521024.cn

stop)  echo "停止" ;;
来源：http://pm.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://zw.gzmigu.cn

esac
来源：http://kl.hnjuh.cn

[R12] for 遍历文件
来源：http://su.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://kc.bjjhwx.cn

[R13] for 计数循环
来源：http://yl.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://ci.colortex.cn

[R14] C 风格 for
来源：http://fb.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qn.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://nh.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://as.jctech888.com.cn

[R16] until 等待条件
来源：http://cy.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pk.gzmigu.cn

[R17] 数组定义与取值
来源：http://au.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xk.muxihuayi.cn

[R18] 遍历数组
来源：http://br.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dh.9csxet.cn

[R19] 数组长度
来源：http://sy.shxzukj.cn

echo "${#arr[@]}"
来源：http://cr.newstarts.cn

[R20] 关联数组（字典）
来源：http://xb.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ry.colortex.cn

[R21] 字符串长度
来源：http://ea.shtwfgs.cn

echo "${#s}"
来源：http://cs.wgjwhj.cn

[R22] 截取子串
来源：http://up.jctech888.com.cn

echo "${s:0:5}"
来源：http://kl.shxzukj.cn

[R23] 字符串替换
来源：http://ml.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iv.jctech888.com.cn

[R24] 大小写转换
来源：http://tn.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rb.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://hr.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cm.yuntaijiaju.cn

[R26] 命令替换
来源：http://ce.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://gq.huixiangedu.cn

[R27] 算术展开
来源：http://uq.nszjky.cn

echo $((1 + 2 * 3))
来源：http://vo.haigaiapp.cn

[R28] 浮点运算
来源：http://fi.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://ad.haigaiapp.cn

[R29] 定义函数
来源：http://xc.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fi.huixiangedu.cn

[R30] 函数返回状态码
来源：http://ft.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://ev.hahajie.cn

[R31] 局部变量
来源：http://tw.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://uk.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://eo.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://go.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://kz.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jp.szsharing.cn

[R34] 退出时清理
来源：http://gj.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xv.bjjhwx.cn

[R35] 后台执行并等待
来源：http://jy.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vv.szsharing.cn

[R36] 并发执行多个任务
来源：http://xd.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lw.nszjky.cn

[R37] 把输出赋给变量
来源：http://sa.muxihuayi.cn

files=$(ls -1)
来源：http://rf.shxzukj.cn

[R38] 管道串联
来源：http://rt.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://ll.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://os.yuexingan06.cn

cmd > out.log 2>&1
来源：http://ox.chemitech.net.cn

[R40] 追加写日志
来源：http://lt.asd995.cn

echo "log" >> out.log
来源：http://bp.asd995.cn

[R41] 丢弃输出
来源：http://hw.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://rp.521024.cn

[R42] 输入重定向
来源：http://tf.bjjhwx.cn

wc -l < a.txt
来源：http://vi.haigaiapp.cn

[R43] 按名字查找文件
来源：http://cy.haigaiapp.cn

find . -name "*.log" -type f
来源：http://uv.gzmigu.cn

[R44] 按修改时间查找
来源：http://ut.shxzskj.cn

find . -mtime -7 -type f
来源：http://ft.hnjuh.cn

[R45] 批量删除
来源：http://nc.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://bs.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://oi.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bw.chemitech.net.cn

[R47] sed 单行替换
来源：http://zr.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bb.haigaiapp.cn

[R48] awk 取指定列
来源：http://go.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://ej.521024.cn

[R49] awk 带条件
来源：http://lt.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ps.shxzskj.cn

[R50] awk 求和
来源：http://zv.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://js.huanxung.cn

[R51] 排序去重取前几
来源：http://po.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sa.wgjwhj.cn

[R52] 统计行数
来源：http://fb.bjjhwx.cn

wc -l a.txt
来源：http://cj.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://ix.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ot.yuexingan06.cn

[R54] 比较两个文件
来源：http://si.shxzskj.cn

diff a.txt b.txt
来源：http://ex.muxihuayi.cn

[R55] 压缩与解压
来源：http://ea.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pk.lnxyls.cn

[R56] 远程拷贝
来源：http://kx.521024.cn

scp file user@host:/path/
来源：http://eo.szxytkj.cn

[R57] 远程执行命令
来源：http://pl.muxihuayi.cn

ssh user@host 'uptime'
来源：http://ni.szsharing.cn

[R58] 下载文件
来源：http://bn.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://np.asd995.cn

[R59] 发 POST JSON
来源：http://fs.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cg.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://nh.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hl.szsharing.cn

[R61] 磁盘占用
来源：http://qv.9csxet.cn

df -h;  du -sh *
来源：http://nk.nszjky.cn

[R62] 找最占空间的文件
来源：http://we.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://lu.wgjwhj.cn

[R63] 内存与进程
来源：http://vf.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://wn.huixinmuqiang.cn

[R64] 结束进程
来源：http://hj.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://by.nszjky.cn

[R65] 查看端口占用
来源：http://hh.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fa.jianghongdianzi.cn

[R66] 定时任务
来源：http://dd.shxzskj.cn

crontab -e;  crontab -l
来源：http://bb.szsharing.cn

[R67] 生成随机十六进制串
来源：http://rn.szxytkj.cn

openssl rand -hex 16
来源：http://pf.wgjwhj.cn

[R68] 计算文件校验值
来源：http://ss.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yr.colortex.cn

[R69] 生成随机密码
来源：http://lx.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://qv.hnjuh.cn

[R70] 时间戳与互转
来源：http://st.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://si.chemitech.net.cn

[R71] 日期格式化
来源：http://rf.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rj.szsharing.cn

[R72] 等待端口就绪
来源：http://hi.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ec.shxzskj.cn

[R73] 分割大日志
来源：http://gz.panjiajie.cn

split -l 1000 big.log part_
来源：http://pz.panjiajie.cn

[R74] 批量重命名
来源：http://gr.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zb.gzmigu.cn

[R75] 导出环境变量
来源：http://ca.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ux.huanxung.cn

[R76] 使用临时文件
来源：http://wc.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qn.colortex.cn

[R77] 读取用户输入
来源：http://nb.jctech888.com.cn

read -rp "请输入: " ans
来源：http://zj.shxzukj.cn

[R78] 交互式菜单
来源：http://uu.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://un.hnjuh.cn

[R79] 解析命令行选项
来源：http://qz.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://do.colortex.cn

[R80] 查看脚本执行耗时
来源：http://qa.huanxung.cn

time ./run.sh
来源：http://eq.muxihuayi.cn

================================================================================
来源：http://qr.szxytkj.cn

S. C / C++ 专题
来源：http://aq.asd995.cn

================================================================================
来源：http://yz.chemitech.net.cn

[S01] C：Hello World
来源：http://rt.hahajie.cn

#include <stdio.h>
来源：http://vz.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pe.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://gj.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://jf.panjiajie.cn

[S03] C：读入整数
来源：http://dg.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://vd.muxihuayi.cn

[S04] C：字符串复制
来源：http://gp.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wr.colortex.cn

[S05] C：字符串长度
来源：http://tv.huixiangedu.cn

strlen(s)
来源：http://gk.lnxyls.cn

[S06] C：字符串比较
来源：http://hp.nicolike.cn

strcmp(a, b) == 0
来源：http://od.gzmigu.cn

[S07] C：数组遍历求和
来源：http://sn.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bk.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://dn.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hc.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://pb.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pf.newstarts.cn

[S10] C：指针与解引用
来源：http://cw.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://ni.szxytkj.cn

[S11] C：逐行读文件
来源：http://rg.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://aw.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fj.521024.cn

fclose(f);
来源：http://lv.jianghongdianzi.cn

[S12] C：写文件
来源：http://ea.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dq.shtwfgs.cn

[S13] C：宏定义
来源：http://hr.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cg.hahajie.cn

[S14] C：枚举
来源：http://lu.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://uo.szxytkj.cn

[S15] C：类型转换
来源：http://zu.huixinmuqiang.cn

(double) a / b
来源：http://zo.chemitech.net.cn

[S16] C：位操作置位
来源：http://ta.newstarts.cn

x |= (1 << 3);
来源：http://sc.huanxung.cn

[S17] C：安全拼接字符串
来源：http://fk.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bb.shxzukj.cn

[S18] C：命令行参数
来源：http://bt.huanxung.cn

int main(int argc, char **argv)
来源：http://eg.szxytkj.cn

[S19] C：快速排序
来源：http://rb.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cn.hahajie.cn

[S20] C：二分查找
来源：http://tv.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jk.lnxyls.cn

[S21] C：字符类别判断
来源：http://ei.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ua.hnjuh.cn

[S22] C：字符串转数字
来源：http://vs.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lb.gzmigu.cn

[S23] C：随机数
来源：http://bc.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wy.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://np.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gc.szsharing.cn

[S25] C：内存拷贝
来源：http://an.jctech888.com.cn

memcpy(dst, src, n);
来源：http://xg.bookmarksfly.cn

[S26] C：内存清零
来源：http://te.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://qq.jianghongdianzi.cn

[S27] C：定义常量
来源：http://jm.newstarts.cn

const double PI = 3.14159;
来源：http://pi.hahajie.cn

[S28] C：静态变量
来源：http://ac.newstarts.cn

static int counter = 0;
来源：http://gx.panjiajie.cn

[S29] C：变参函数
来源：http://ga.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lf.bjjhwx.cn

[S30] C：头文件保护
来源：http://ns.nszjky.cn

#ifndef X_H
来源：http://ke.9csxet.cn

#define X_H
来源：http://lp.bookmarksfly.cn

#endif
来源：http://ax.nszjky.cn

[S31] C++：Hello World
来源：http://ug.lnxyls.cn


<!-- 参考信息 -->