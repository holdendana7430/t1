代发 wailian999

[Q63] 开启事务
来源：http://dt.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pd.nszjky.cn

[Q64] 提交事务
来源：http://qe.szxytkj.cn

COMMIT;
来源：http://hq.szsharing.cn

[Q65] 回滚事务
来源：http://gt.shxzskj.cn

ROLLBACK;
来源：http://re.huixiangedu.cn

[Q66] 行锁查询
来源：http://ch.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cx.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://om.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hw.szsharing.cn

[Q68] 保存点
来源：http://ho.hnjuh.cn

SAVEPOINT sp1;
来源：http://hr.hnjuh.cn

ROLLBACK TO sp1;
来源：http://ys.huanxung.cn

[Q69] 查看执行计划
来源：http://bf.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lb.shtwfgs.cn

[Q70] 更新统计信息
来源：http://lh.wgjwhj.cn

ANALYZE TABLE users;
来源：http://te.shxzukj.cn

[Q71] 查看建表语句
来源：http://xa.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pw.521024.cn

[Q72] 查看索引
来源：http://ui.panjiajie.cn

SHOW INDEX FROM users;
来源：http://vp.9csxet.cn

[Q73] 查看表状态
来源：http://bi.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://va.521024.cn

[Q74] 强制使用索引
来源：http://nc.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ek.haigaiapp.cn

[Q75] 日期格式化
来源：http://co.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://id.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wv.wgjwhj.cn

[Q76] 按天统计
来源：http://if.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oj.colortex.cn

[Q77] 时间加减
来源：http://vp.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bx.nicolike.cn

[Q78] 当前时间
来源：http://vv.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://di.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://kl.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ox.szsharing.cn

[Q80] 字符串截取
来源：http://ls.9csxet.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vf.jctech888.com.cn

[Q81] 字符串替换
来源：http://qy.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ao.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://ub.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hi.lnxyls.cn

[Q83] 大小写转换
来源：http://am.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tt.shxzskj.cn

[Q84] 去除首尾空格
来源：http://hv.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://oh.haigaiapp.cn

[Q85] 数值取整
来源：http://yk.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lb.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://im.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ab.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://tx.panjiajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sk.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://mf.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nc.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uf.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://tn.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ta.9csxet.cn

[Q90] 生成序号列
来源：http://pz.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hq.asd995.cn

================================================================================
来源：http://xi.bookmarksfly.cn

R. Bash 专题
来源：http://qh.jctech888.com.cn

================================================================================
来源：http://xd.gzmigu.cn

[R01] shebang 与严格模式
来源：http://cf.colortex.cn

#!/usr/bin/env bash
来源：http://ad.jctech888.com.cn

set -euo pipefail
来源：http://xs.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://ta.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://sz.colortex.cn

[R03] 只读变量
来源：http://am.szxytkj.cn

readonly PI=3.14
来源：http://em.hahajie.cn

[R04] 位置参数
来源：http://ie.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cs.muxihuayi.cn

[R05] 参数默认值
来源：http://zo.szsharing.cn

name="${1:-default}"
来源：http://gl.nszjky.cn

[R06] 判断命令是否存在
来源：http://es.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://we.huixiangedu.cn

[R07] if 判断文件
来源：http://mf.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ii.lnxyls.cn

[R08] 数值比较
来源：http://tl.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://an.panjiajie.cn

[R09] 字符串比较
来源：http://yf.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cm.9csxet.cn

[R10] 正则匹配
来源：http://ln.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fx.lnxyls.cn

[R11] case 多分支
来源：http://xc.szxytkj.cn

case "$1" in
来源：http://lf.asd995.cn

start) echo "启动" ;;
来源：http://zv.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://hg.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://cl.panjiajie.cn

esac
来源：http://nh.panjiajie.cn

[R12] for 遍历文件
来源：http://yr.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://ak.shxzskj.cn

[R13] for 计数循环
来源：http://my.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://aw.muxihuayi.cn

[R14] C 风格 for
来源：http://nn.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tf.hnjuh.cn

[R15] while 逐行读文件
来源：http://wf.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vi.haigaiapp.cn

[R16] until 等待条件
来源：http://df.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cc.shxzskj.cn

[R17] 数组定义与取值
来源：http://fi.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ch.huanxung.cn

[R18] 遍历数组
来源：http://hv.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nk.szsharing.cn

[R19] 数组长度
来源：http://ts.colortex.cn

echo "${#arr[@]}"
来源：http://vg.lnxyls.cn

[R20] 关联数组（字典）
来源：http://lw.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://es.newstarts.cn

[R21] 字符串长度
来源：http://et.huanxung.cn

echo "${#s}"
来源：http://mw.shxzukj.cn

[R22] 截取子串
来源：http://zt.szsharing.cn

echo "${s:0:5}"
来源：http://ry.muxihuayi.cn

[R23] 字符串替换
来源：http://aa.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://th.yuexingan06.cn

[R24] 大小写转换
来源：http://pu.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tj.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://pa.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vv.huanxung.cn

[R26] 命令替换
来源：http://pk.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://af.wgjwhj.cn

[R27] 算术展开
来源：http://gy.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://oo.gzmigu.cn

[R28] 浮点运算
来源：http://fz.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://uq.shxzskj.cn

[R29] 定义函数
来源：http://ky.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xu.9csxet.cn

[R30] 函数返回状态码
来源：http://sj.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://gh.shtwfgs.cn

[R31] 局部变量
来源：http://rc.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://dr.hnjuh.cn

[R32] 参数个数校验
来源：http://lb.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ib.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://vr.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jc.huixinmuqiang.cn

[R34] 退出时清理
来源：http://mm.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xh.szxytkj.cn

[R35] 后台执行并等待
来源：http://ve.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jq.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://iz.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rj.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://vi.521024.cn

files=$(ls -1)
来源：http://sw.shxzskj.cn

[R38] 管道串联
来源：http://go.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://sx.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://rz.lnxyls.cn

cmd > out.log 2>&1
来源：http://kn.jctech888.com.cn

[R40] 追加写日志
来源：http://su.shxzukj.cn

echo "log" >> out.log
来源：http://lj.hnjuh.cn

[R41] 丢弃输出
来源：http://mz.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://vp.wgjwhj.cn

[R42] 输入重定向
来源：http://oo.huanxung.cn

wc -l < a.txt
来源：http://vw.shxzskj.cn

[R43] 按名字查找文件
来源：http://rf.colortex.cn

find . -name "*.log" -type f
来源：http://lc.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://ue.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://et.szsharing.cn

[R45] 批量删除
来源：http://dy.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://vn.gzmigu.cn

[R46] 递归替换文件内容
来源：http://kn.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qm.wgjwhj.cn

[R47] sed 单行替换
来源：http://ix.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ed.jctech888.com.cn

[R48] awk 取指定列
来源：http://hn.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://gj.yuexingan06.cn

[R49] awk 带条件
来源：http://yw.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yb.lnxyls.cn

[R50] awk 求和
来源：http://sp.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zl.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://gx.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://st.colortex.cn

[R52] 统计行数
来源：http://ji.asd995.cn

wc -l a.txt
来源：http://pm.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://od.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dv.wgjwhj.cn

[R54] 比较两个文件
来源：http://qd.nicolike.cn

diff a.txt b.txt
来源：http://um.szsharing.cn

[R55] 压缩与解压
来源：http://ga.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wy.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://uv.huixinmuqiang.cn

scp file user@host:/path/
来源：http://tk.jctech888.com.cn

[R57] 远程执行命令
来源：http://bb.shtwfgs.cn

ssh user@host 'uptime'
来源：http://hw.huanxung.cn

[R58] 下载文件
来源：http://ys.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sx.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://ay.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sl.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://nk.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cy.nicolike.cn

[R61] 磁盘占用
来源：http://cq.jctech888.com.cn

df -h;  du -sh *
来源：http://vd.521024.cn

[R62] 找最占空间的文件
来源：http://gg.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://vt.jianghongdianzi.cn

[R63] 内存与进程
来源：http://pn.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://yp.huixinmuqiang.cn

[R64] 结束进程
来源：http://cy.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://mp.shxzukj.cn

[R65] 查看端口占用
来源：http://ld.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tn.nszjky.cn

[R66] 定时任务
来源：http://vn.nicolike.cn

crontab -e;  crontab -l
来源：http://bn.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://fb.hahajie.cn

openssl rand -hex 16
来源：http://zt.szxytkj.cn

[R68] 计算文件校验值
来源：http://le.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wf.9csxet.cn

[R69] 生成随机密码
来源：http://le.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://wj.asd995.cn

[R70] 时间戳与互转
来源：http://ki.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://ah.haigaiapp.cn

[R71] 日期格式化
来源：http://xj.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://an.jctech888.com.cn

[R72] 等待端口就绪
来源：http://ml.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ty.shxzskj.cn

[R73] 分割大日志
来源：http://tr.nicolike.cn

split -l 1000 big.log part_
来源：http://wh.nicolike.cn

[R74] 批量重命名
来源：http://dl.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jj.jianghongdianzi.cn

[R75] 导出环境变量
来源：http://jr.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://kb.hnjuh.cn

[R76] 使用临时文件
来源：http://mi.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pu.lnxyls.cn

[R77] 读取用户输入
来源：http://rt.huixiangedu.cn

read -rp "请输入: " ans
来源：http://hv.muxihuayi.cn

[R78] 交互式菜单
来源：http://vv.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sb.hahajie.cn

[R79] 解析命令行选项
来源：http://gf.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ce.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://eg.bookmarksfly.cn

time ./run.sh
来源：http://li.panjiajie.cn

================================================================================
来源：http://ac.shxzukj.cn

S. C / C++ 专题
来源：http://lp.yuntaijiaju.cn

================================================================================
来源：http://vs.szsharing.cn

[S01] C：Hello World
来源：http://xm.muxihuayi.cn

#include <stdio.h>
来源：http://kl.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ce.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://ae.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://kz.newstarts.cn

[S03] C：读入整数
来源：http://wg.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://yb.asd995.cn

[S04] C：字符串复制
来源：http://ok.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gh.huixiangedu.cn

[S05] C：字符串长度
来源：http://ku.shxzskj.cn

strlen(s)
来源：http://sy.bjjhwx.cn

[S06] C：字符串比较
来源：http://rj.shtwfgs.cn

strcmp(a, b) == 0
来源：http://af.colortex.cn

[S07] C：数组遍历求和
来源：http://bw.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ii.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://il.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oy.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://te.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mx.9csxet.cn

[S10] C：指针与解引用
来源：http://wv.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://tp.panjiajie.cn

[S11] C：逐行读文件
来源：http://vs.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://fs.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jb.chemitech.net.cn

fclose(f);
来源：http://hr.shtwfgs.cn

[S12] C：写文件
来源：http://yx.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kb.hnjuh.cn

[S13] C：宏定义
来源：http://wi.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nn.hahajie.cn

[S14] C：枚举
来源：http://ok.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://gv.shxzukj.cn

[S15] C：类型转换
来源：http://yp.haigaiapp.cn

(double) a / b
来源：http://oj.hnjuh.cn

[S16] C：位操作置位
来源：http://pc.huixiangedu.cn

x |= (1 << 3);
来源：http://ky.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://ao.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rf.szxytkj.cn

[S18] C：命令行参数
来源：http://rf.gzmigu.cn

int main(int argc, char **argv)
来源：http://pk.shtwfgs.cn

[S19] C：快速排序
来源：http://bg.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zs.yuntaijiaju.cn

[S20] C：二分查找
来源：http://qh.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qq.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://ss.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hm.yuexingan06.cn

[S22] C：字符串转数字
来源：http://yd.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oe.shtwfgs.cn

[S23] C：随机数
来源：http://vr.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://as.gzmigu.cn

[S24] C：获取本地时间
来源：http://ht.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fh.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://ie.szxytkj.cn

memcpy(dst, src, n);
来源：http://ju.huanxung.cn

[S26] C：内存清零
来源：http://cs.huanxung.cn

memset(a, 0, sizeof a);
来源：http://qt.huixiangedu.cn

[S27] C：定义常量
来源：http://uy.gzmigu.cn

const double PI = 3.14159;
来源：http://tj.muxihuayi.cn

[S28] C：静态变量
来源：http://tb.muxihuayi.cn

static int counter = 0;
来源：http://iv.jianghongdianzi.cn

[S29] C：变参函数
来源：http://lx.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wh.bookmarksfly.cn

[S30] C：头文件保护
来源：http://kd.szsharing.cn

#ifndef X_H
来源：http://se.jctech888.com.cn

#define X_H
来源：http://ba.9csxet.cn

#endif
来源：http://aa.panjiajie.cn

[S31] C++：Hello World
来源：http://ef.nicolike.cn

#include <iostream>
来源：http://is.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://vn.jctech888.com.cn

[S32] C++：字符串
来源：http://ui.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://wu.newstarts.cn


<!-- 参考信息 -->