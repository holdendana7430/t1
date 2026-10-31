代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hv.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://mk.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ks.wgjwhj.cn

[Q57] 行号
来源：http://jg.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dp.9csxet.cn

[Q58] 累计求和
来源：http://sh.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gb.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://ry.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ul.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://sh.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rp.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ru.muxihuayi.cn

[Q61] 移动平均
来源：http://gh.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qo.yuexingan06.cn

[Q62] 分组占比
来源：http://vn.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sk.szxytkj.cn

[Q63] 开启事务
来源：http://yl.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lh.muxihuayi.cn

[Q64] 提交事务
来源：http://yo.haigaiapp.cn

COMMIT;
来源：http://ix.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://tw.wgjwhj.cn

ROLLBACK;
来源：http://mo.huanxung.cn

[Q66] 行锁查询
来源：http://yp.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://in.lnxyls.cn

[Q67] 设置隔离级别
来源：http://zv.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mz.newstarts.cn

[Q68] 保存点
来源：http://js.panjiajie.cn

SAVEPOINT sp1;
来源：http://em.nszjky.cn

ROLLBACK TO sp1;
来源：http://il.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://yd.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wg.haigaiapp.cn

[Q70] 更新统计信息
来源：http://sb.lnxyls.cn

ANALYZE TABLE users;
来源：http://hk.panjiajie.cn

[Q71] 查看建表语句
来源：http://mm.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://so.bookmarksfly.cn

[Q72] 查看索引
来源：http://xn.huanxung.cn

SHOW INDEX FROM users;
来源：http://kk.jctech888.com.cn

[Q73] 查看表状态
来源：http://dm.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://of.shxzukj.cn

[Q74] 强制使用索引
来源：http://ib.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ct.newstarts.cn

[Q75] 日期格式化
来源：http://bc.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bl.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oz.wgjwhj.cn

[Q76] 按天统计
来源：http://ok.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mc.chemitech.net.cn

[Q77] 时间加减
来源：http://gf.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ow.huanxung.cn

[Q78] 当前时间
来源：http://yj.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vl.jctech888.com.cn

[Q79] 字符串拼接
来源：http://uu.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://if.nszjky.cn

[Q80] 字符串截取
来源：http://tz.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oj.shxzskj.cn

[Q81] 字符串替换
来源：http://is.bjjhwx.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://la.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://ec.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mm.huanxung.cn

[Q83] 大小写转换
来源：http://dp.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ss.hahajie.cn

[Q84] 去除首尾空格
来源：http://xk.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://pc.nszjky.cn

[Q85] 数值取整
来源：http://tl.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zp.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://na.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://td.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://kb.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ko.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://yj.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oy.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://em.shxzukj.cn

[Q89] 判断表是否存在
来源：http://yj.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xh.nicolike.cn

[Q90] 生成序号列
来源：http://yd.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ou.nicolike.cn

================================================================================
来源：http://vm.jctech888.com.cn

R. Bash 专题
来源：http://sg.hnjuh.cn

================================================================================
来源：http://ce.lnxyls.cn

[R01] shebang 与严格模式
来源：http://vz.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://tr.shxzskj.cn

set -euo pipefail
来源：http://fw.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://vu.gzmigu.cn

name="Tom"; echo "$name"
来源：http://kw.huixiangedu.cn

[R03] 只读变量
来源：http://st.szsharing.cn

readonly PI=3.14
来源：http://ul.wgjwhj.cn

[R04] 位置参数
来源：http://rw.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ge.shxzskj.cn

[R05] 参数默认值
来源：http://rw.muxihuayi.cn

name="${1:-default}"
来源：http://go.hahajie.cn

[R06] 判断命令是否存在
来源：http://ll.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mp.asd995.cn

[R07] if 判断文件
来源：http://wb.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ud.gzmigu.cn

[R08] 数值比较
来源：http://dv.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rf.wgjwhj.cn

[R09] 字符串比较
来源：http://vz.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gk.bookmarksfly.cn

[R10] 正则匹配
来源：http://js.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fh.huanxung.cn

[R11] case 多分支
来源：http://te.chemitech.net.cn

case "$1" in
来源：http://ms.lnxyls.cn

start) echo "启动" ;;
来源：http://ln.nicolike.cn

stop)  echo "停止" ;;
来源：http://lz.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://sl.huanxung.cn

esac
来源：http://rk.yuexingan06.cn

[R12] for 遍历文件
来源：http://sn.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://yh.huixiangedu.cn

[R13] for 计数循环
来源：http://wb.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://ja.chemitech.net.cn

[R14] C 风格 for
来源：http://sk.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qi.9csxet.cn

[R15] while 逐行读文件
来源：http://wm.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lu.shtwfgs.cn

[R16] until 等待条件
来源：http://yz.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://om.lnxyls.cn

[R17] 数组定义与取值
来源：http://ai.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://aa.shxzukj.cn

[R18] 遍历数组
来源：http://jp.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fh.9csxet.cn

[R19] 数组长度
来源：http://nh.muxihuayi.cn

echo "${#arr[@]}"
来源：http://hc.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://cg.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gu.jianghongdianzi.cn

[R21] 字符串长度
来源：http://in.muxihuayi.cn

echo "${#s}"
来源：http://nf.gzmigu.cn

[R22] 截取子串
来源：http://ru.szsharing.cn

echo "${s:0:5}"
来源：http://sr.gzmigu.cn

[R23] 字符串替换
来源：http://aa.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://we.jctech888.com.cn

[R24] 大小写转换
来源：http://ef.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uu.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://fr.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wc.yuntaijiaju.cn

[R26] 命令替换
来源：http://ld.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://br.gzmigu.cn

[R27] 算术展开
来源：http://wt.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://qn.nszjky.cn

[R28] 浮点运算
来源：http://cu.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://hw.jianghongdianzi.cn

[R29] 定义函数
来源：http://id.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eq.lnxyls.cn

[R30] 函数返回状态码
来源：http://pn.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://hh.haigaiapp.cn

[R31] 局部变量
来源：http://mn.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://nw.panjiajie.cn

[R32] 参数个数校验
来源：http://lf.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sw.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://oh.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nx.nicolike.cn

[R34] 退出时清理
来源：http://ca.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ur.jctech888.com.cn

[R35] 后台执行并等待
来源：http://pi.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ax.hnjuh.cn

[R36] 并发执行多个任务
来源：http://hy.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sx.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://nn.gzmigu.cn

files=$(ls -1)
来源：http://ks.gzmigu.cn

[R38] 管道串联
来源：http://mb.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://md.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://ce.panjiajie.cn

cmd > out.log 2>&1
来源：http://bx.huixinmuqiang.cn

[R40] 追加写日志
来源：http://sp.jianghongdianzi.cn

echo "log" >> out.log
来源：http://ls.shxzskj.cn

[R41] 丢弃输出
来源：http://qv.hahajie.cn

cmd >/dev/null 2>&1
来源：http://go.huixiangedu.cn

[R42] 输入重定向
来源：http://fr.yuexingan06.cn

wc -l < a.txt
来源：http://wq.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://pz.panjiajie.cn

find . -name "*.log" -type f
来源：http://if.colortex.cn

[R44] 按修改时间查找
来源：http://ja.jctech888.com.cn

find . -mtime -7 -type f
来源：http://ym.newstarts.cn

[R45] 批量删除
来源：http://sd.521024.cn

find . -name "*.tmp" -delete
来源：http://db.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://uj.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wj.hahajie.cn

[R47] sed 单行替换
来源：http://yz.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mf.yuexingan06.cn

[R48] awk 取指定列
来源：http://ti.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://rb.colortex.cn

[R49] awk 带条件
来源：http://al.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fl.yuntaijiaju.cn

[R50] awk 求和
来源：http://og.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qh.wgjwhj.cn

[R51] 排序去重取前几
来源：http://rp.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ie.shtwfgs.cn

[R52] 统计行数
来源：http://bb.panjiajie.cn

wc -l a.txt
来源：http://kx.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://dx.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zz.lnxyls.cn

[R54] 比较两个文件
来源：http://sq.shxzukj.cn

diff a.txt b.txt
来源：http://zu.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://qx.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rs.9csxet.cn

[R56] 远程拷贝
来源：http://hs.chemitech.net.cn

scp file user@host:/path/
来源：http://yb.colortex.cn

[R57] 远程执行命令
来源：http://jl.szxytkj.cn

ssh user@host 'uptime'
来源：http://ir.huixiangedu.cn

[R58] 下载文件
来源：http://zc.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dg.haigaiapp.cn

[R59] 发 POST JSON
来源：http://oc.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ij.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://mj.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kx.muxihuayi.cn

[R61] 磁盘占用
来源：http://fq.9csxet.cn

df -h;  du -sh *
来源：http://ts.9csxet.cn

[R62] 找最占空间的文件
来源：http://zz.asd995.cn

du -ah . | sort -rh | head -10
来源：http://nh.wgjwhj.cn

[R63] 内存与进程
来源：http://mq.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://yu.shxzskj.cn

[R64] 结束进程
来源：http://ey.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://da.jctech888.com.cn

[R65] 查看端口占用
来源：http://yh.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xy.shxzukj.cn

[R66] 定时任务
来源：http://ju.nicolike.cn

crontab -e;  crontab -l
来源：http://rp.szsharing.cn

[R67] 生成随机十六进制串
来源：http://nb.colortex.cn

openssl rand -hex 16
来源：http://iw.jctech888.com.cn

[R68] 计算文件校验值
来源：http://ti.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gu.muxihuayi.cn

[R69] 生成随机密码
来源：http://tw.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://hk.hahajie.cn

[R70] 时间戳与互转
来源：http://ho.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://pr.yuexingan06.cn

[R71] 日期格式化
来源：http://ud.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ba.shtwfgs.cn

[R72] 等待端口就绪
来源：http://ys.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qp.shxzukj.cn

[R73] 分割大日志
来源：http://oe.gzmigu.cn

split -l 1000 big.log part_
来源：http://ra.hnjuh.cn

[R74] 批量重命名
来源：http://xb.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iy.asd995.cn

[R75] 导出环境变量
来源：http://rd.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://tb.gzmigu.cn

[R76] 使用临时文件
来源：http://lv.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fe.bjjhwx.cn

[R77] 读取用户输入
来源：http://iy.panjiajie.cn

read -rp "请输入: " ans
来源：http://km.chemitech.net.cn

[R78] 交互式菜单
来源：http://up.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sz.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://tl.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lw.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://zk.jianghongdianzi.cn

time ./run.sh
来源：http://ac.huanxung.cn

================================================================================
来源：http://lf.9csxet.cn

S. C / C++ 专题
来源：http://zz.szxytkj.cn

================================================================================
来源：http://yl.hnjuh.cn

[S01] C：Hello World
来源：http://ph.9csxet.cn

#include <stdio.h>
来源：http://kg.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://va.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://jc.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://or.bookmarksfly.cn

[S03] C：读入整数
来源：http://ej.colortex.cn

int x; scanf("%d", &x);
来源：http://hi.jctech888.com.cn

[S04] C：字符串复制
来源：http://ha.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nb.huixiangedu.cn

[S05] C：字符串长度
来源：http://du.hnjuh.cn

strlen(s)
来源：http://yn.hahajie.cn

[S06] C：字符串比较
来源：http://qc.hnjuh.cn

strcmp(a, b) == 0
来源：http://ie.nszjky.cn

[S07] C：数组遍历求和
来源：http://xj.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lz.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://xu.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ik.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://cg.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yq.colortex.cn

[S10] C：指针与解引用
来源：http://vo.nicolike.cn

int *p = &a;  *p = 5;
来源：http://qa.gzmigu.cn

[S11] C：逐行读文件
来源：http://br.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://rv.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rk.wgjwhj.cn

fclose(f);
来源：http://cy.yuexingan06.cn

[S12] C：写文件
来源：http://ab.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vz.gzmigu.cn

[S13] C：宏定义
来源：http://zr.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rp.9csxet.cn

[S14] C：枚举
来源：http://cg.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://jo.szsharing.cn

[S15] C：类型转换
来源：http://cz.nszjky.cn

(double) a / b
来源：http://qh.hahajie.cn

[S16] C：位操作置位
来源：http://ra.hahajie.cn

x |= (1 << 3);
来源：http://hw.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://wj.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nk.szxytkj.cn

[S18] C：命令行参数
来源：http://mn.muxihuayi.cn

int main(int argc, char **argv)
来源：http://in.huixinmuqiang.cn

[S19] C：快速排序
来源：http://mh.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dj.jianghongdianzi.cn

[S20] C：二分查找
来源：http://ln.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mc.hnjuh.cn

[S21] C：字符类别判断
来源：http://yq.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mk.521024.cn

[S22] C：字符串转数字
来源：http://uw.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eh.jctech888.com.cn

[S23] C：随机数
来源：http://sk.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yq.szsharing.cn

[S24] C：获取本地时间
来源：http://rw.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pt.shtwfgs.cn

[S25] C：内存拷贝
来源：http://ys.newstarts.cn

memcpy(dst, src, n);
来源：http://rl.bookmarksfly.cn

[S26] C：内存清零
来源：http://la.huixiangedu.cn


<!-- 参考信息 -->