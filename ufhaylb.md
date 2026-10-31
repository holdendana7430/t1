代发 wailian999

SHOW INDEX FROM users;
来源：http://gi.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://jq.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ql.bjjhwx.cn

[Q74] 强制使用索引
来源：http://sb.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iq.shxzukj.cn

[Q75] 日期格式化
来源：http://mv.szsharing.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qe.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hd.szsharing.cn

[Q76] 按天统计
来源：http://ts.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zj.nszjky.cn

[Q77] 时间加减
来源：http://gz.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jh.521024.cn

[Q78] 当前时间
来源：http://cf.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qh.hnjuh.cn

[Q79] 字符串拼接
来源：http://qy.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://be.wgjwhj.cn

[Q80] 字符串截取
来源：http://zs.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tu.nicolike.cn

[Q81] 字符串替换
来源：http://mp.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jm.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://ok.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qc.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://ge.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pq.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://sn.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://tx.hahajie.cn

[Q85] 数值取整
来源：http://pn.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://er.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://lt.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ua.asd995.cn

[Q87] JSON 字段做条件
来源：http://pq.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nw.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://lw.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kp.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xg.szsharing.cn

[Q89] 判断表是否存在
来源：http://fp.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yi.nszjky.cn

[Q90] 生成序号列
来源：http://mg.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rr.chemitech.net.cn

================================================================================
来源：http://by.chemitech.net.cn

R. Bash 专题
来源：http://mj.9csxet.cn

================================================================================
来源：http://hq.9csxet.cn

[R01] shebang 与严格模式
来源：http://vc.panjiajie.cn

#!/usr/bin/env bash
来源：http://hv.szxytkj.cn

set -euo pipefail
来源：http://mz.gzmigu.cn

[R02] 变量赋值与使用
来源：http://ke.hahajie.cn

name="Tom"; echo "$name"
来源：http://eg.nszjky.cn

[R03] 只读变量
来源：http://nw.nszjky.cn

readonly PI=3.14
来源：http://zl.chemitech.net.cn

[R04] 位置参数
来源：http://fh.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kz.chemitech.net.cn

[R05] 参数默认值
来源：http://ni.haigaiapp.cn

name="${1:-default}"
来源：http://hh.shxzskj.cn

[R06] 判断命令是否存在
来源：http://dg.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uo.shxzskj.cn

[R07] if 判断文件
来源：http://cr.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mc.lnxyls.cn

[R08] 数值比较
来源：http://hx.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zq.9csxet.cn

[R09] 字符串比较
来源：http://ef.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ka.colortex.cn

[R10] 正则匹配
来源：http://tz.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uc.chemitech.net.cn

[R11] case 多分支
来源：http://wd.huixiangedu.cn

case "$1" in
来源：http://fq.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://pe.huanxung.cn

stop)  echo "停止" ;;
来源：http://zc.colortex.cn

*)     echo "未知命令" ;;
来源：http://tc.nicolike.cn

esac
来源：http://rn.asd995.cn

[R12] for 遍历文件
来源：http://pb.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://iq.chemitech.net.cn

[R13] for 计数循环
来源：http://pc.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://lf.haigaiapp.cn

[R14] C 风格 for
来源：http://qi.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ew.wgjwhj.cn

[R15] while 逐行读文件
来源：http://dd.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qb.gzmigu.cn

[R16] until 等待条件
来源：http://ms.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xe.hnjuh.cn

[R17] 数组定义与取值
来源：http://uu.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ng.bookmarksfly.cn

[R18] 遍历数组
来源：http://fv.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ig.lnxyls.cn

[R19] 数组长度
来源：http://st.colortex.cn

echo "${#arr[@]}"
来源：http://sv.newstarts.cn

[R20] 关联数组（字典）
来源：http://nu.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ol.hahajie.cn

[R21] 字符串长度
来源：http://bb.yuntaijiaju.cn

echo "${#s}"
来源：http://jz.shxzskj.cn

[R22] 截取子串
来源：http://sx.shtwfgs.cn

echo "${s:0:5}"
来源：http://bu.panjiajie.cn

[R23] 字符串替换
来源：http://gq.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xi.shxzskj.cn

[R24] 大小写转换
来源：http://ct.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ab.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://ys.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ik.shxzukj.cn

[R26] 命令替换
来源：http://th.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://nm.yuntaijiaju.cn

[R27] 算术展开
来源：http://hj.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://dj.jianghongdianzi.cn

[R28] 浮点运算
来源：http://mr.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://vp.huanxung.cn

[R29] 定义函数
来源：http://fp.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bw.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://fi.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://ct.nszjky.cn

[R31] 局部变量
来源：http://px.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://bg.muxihuayi.cn

[R32] 参数个数校验
来源：http://qy.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rv.asd995.cn

[R33] 捕获错误并提示行号
来源：http://pb.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mu.wgjwhj.cn

[R34] 退出时清理
来源：http://hd.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wo.shxzskj.cn

[R35] 后台执行并等待
来源：http://gu.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yg.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://tp.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hm.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://dc.wgjwhj.cn

files=$(ls -1)
来源：http://cp.yuexingan06.cn

[R38] 管道串联
来源：http://oq.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://jj.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://fy.wgjwhj.cn

cmd > out.log 2>&1
来源：http://fs.lnxyls.cn

[R40] 追加写日志
来源：http://ra.chemitech.net.cn

echo "log" >> out.log
来源：http://ld.wgjwhj.cn

[R41] 丢弃输出
来源：http://ee.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://bw.muxihuayi.cn

[R42] 输入重定向
来源：http://wv.shxzukj.cn

wc -l < a.txt
来源：http://td.szxytkj.cn

[R43] 按名字查找文件
来源：http://vl.chemitech.net.cn

find . -name "*.log" -type f
来源：http://fa.hnjuh.cn

[R44] 按修改时间查找
来源：http://up.wgjwhj.cn

find . -mtime -7 -type f
来源：http://il.shxzukj.cn

[R45] 批量删除
来源：http://rp.colortex.cn

find . -name "*.tmp" -delete
来源：http://ol.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://cm.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hb.shxzskj.cn

[R47] sed 单行替换
来源：http://nt.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://iv.bookmarksfly.cn

[R48] awk 取指定列
来源：http://em.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://up.521024.cn

[R49] awk 带条件
来源：http://ki.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rv.jctech888.com.cn

[R50] awk 求和
来源：http://be.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zg.szsharing.cn

[R51] 排序去重取前几
来源：http://qw.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xv.jianghongdianzi.cn

[R52] 统计行数
来源：http://jq.chemitech.net.cn

wc -l a.txt
来源：http://xr.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://cc.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lb.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://op.bookmarksfly.cn

diff a.txt b.txt
来源：http://cv.gzmigu.cn

[R55] 压缩与解压
来源：http://no.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jd.bjjhwx.cn

[R56] 远程拷贝
来源：http://si.chemitech.net.cn

scp file user@host:/path/
来源：http://dy.shtwfgs.cn

[R57] 远程执行命令
来源：http://ib.shxzskj.cn

ssh user@host 'uptime'
来源：http://ii.shxzskj.cn

[R58] 下载文件
来源：http://ei.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ih.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://gf.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gc.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://an.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cz.bjjhwx.cn

[R61] 磁盘占用
来源：http://mc.muxihuayi.cn

df -h;  du -sh *
来源：http://ka.nicolike.cn

[R62] 找最占空间的文件
来源：http://fs.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://zd.bookmarksfly.cn

[R63] 内存与进程
来源：http://ku.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://yw.huanxung.cn

[R64] 结束进程
来源：http://kq.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://ki.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://rk.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ta.hnjuh.cn

[R66] 定时任务
来源：http://wc.panjiajie.cn

crontab -e;  crontab -l
来源：http://vb.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://iv.hnjuh.cn

openssl rand -hex 16
来源：http://eo.shxzukj.cn

[R68] 计算文件校验值
来源：http://de.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vg.asd995.cn

[R69] 生成随机密码
来源：http://cq.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://lr.shxzukj.cn

[R70] 时间戳与互转
来源：http://hu.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://ew.panjiajie.cn

[R71] 日期格式化
来源：http://at.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lk.521024.cn

[R72] 等待端口就绪
来源：http://zv.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tp.panjiajie.cn

[R73] 分割大日志
来源：http://hs.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://as.muxihuayi.cn

[R74] 批量重命名
来源：http://zi.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ko.shxzukj.cn

[R75] 导出环境变量
来源：http://ec.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://yn.hahajie.cn

[R76] 使用临时文件
来源：http://bc.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://os.szxytkj.cn

[R77] 读取用户输入
来源：http://kn.colortex.cn

read -rp "请输入: " ans
来源：http://vp.bookmarksfly.cn

[R78] 交互式菜单
来源：http://vf.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wo.wgjwhj.cn

[R79] 解析命令行选项
来源：http://cw.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zg.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://yj.haigaiapp.cn

time ./run.sh
来源：http://iw.9csxet.cn

================================================================================
来源：http://ei.shxzukj.cn

S. C / C++ 专题
来源：http://gd.panjiajie.cn

================================================================================
来源：http://ai.panjiajie.cn

[S01] C：Hello World
来源：http://nj.gzmigu.cn

#include <stdio.h>
来源：http://ey.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://na.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://ig.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://uz.521024.cn

[S03] C：读入整数
来源：http://mn.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://gb.huanxung.cn

[S04] C：字符串复制
来源：http://ew.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rk.9csxet.cn

[S05] C：字符串长度
来源：http://bd.huanxung.cn

strlen(s)
来源：http://yu.shxzukj.cn

[S06] C：字符串比较
来源：http://ls.yuexingan06.cn

strcmp(a, b) == 0
来源：http://jk.521024.cn

[S07] C：数组遍历求和
来源：http://fl.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://py.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://zc.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ri.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://hq.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sf.9csxet.cn

[S10] C：指针与解引用
来源：http://hp.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://qd.huixiangedu.cn

[S11] C：逐行读文件
来源：http://ey.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://eb.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vc.hnjuh.cn

fclose(f);
来源：http://ya.shxzskj.cn

[S12] C：写文件
来源：http://rl.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sf.9csxet.cn

[S13] C：宏定义
来源：http://dd.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ax.521024.cn

[S14] C：枚举
来源：http://bd.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://zw.huanxung.cn

[S15] C：类型转换
来源：http://ot.colortex.cn

(double) a / b
来源：http://gt.shxzukj.cn

[S16] C：位操作置位
来源：http://wr.hnjuh.cn

x |= (1 << 3);
来源：http://mm.hahajie.cn

[S17] C：安全拼接字符串
来源：http://od.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ps.panjiajie.cn

[S18] C：命令行参数
来源：http://bu.newstarts.cn

int main(int argc, char **argv)
来源：http://ro.lnxyls.cn

[S19] C：快速排序
来源：http://su.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qt.szxytkj.cn

[S20] C：二分查找
来源：http://rg.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lt.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://hq.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tx.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://lq.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sa.gzmigu.cn

[S23] C：随机数
来源：http://ff.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uk.newstarts.cn

[S24] C：获取本地时间
来源：http://fu.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jy.muxihuayi.cn

[S25] C：内存拷贝
来源：http://ct.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://ye.jctech888.com.cn

[S26] C：内存清零
来源：http://by.nszjky.cn

memset(a, 0, sizeof a);
来源：http://ol.yuexingan06.cn

[S27] C：定义常量
来源：http://xs.nszjky.cn

const double PI = 3.14159;
来源：http://xp.chemitech.net.cn

[S28] C：静态变量
来源：http://cg.shtwfgs.cn

static int counter = 0;
来源：http://uq.9csxet.cn

[S29] C：变参函数
来源：http://ox.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nv.9csxet.cn

[S30] C：头文件保护
来源：http://dp.haigaiapp.cn

#ifndef X_H
来源：http://vt.9csxet.cn

#define X_H
来源：http://id.jctech888.com.cn

#endif
来源：http://eo.huixiangedu.cn

[S31] C++：Hello World
来源：http://ay.shtwfgs.cn

#include <iostream>
来源：http://ha.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://jb.szsharing.cn

[S32] C++：字符串
来源：http://em.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://pq.szxytkj.cn

[S33] C++：vector 增删
来源：http://oj.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ev.gzmigu.cn

[S34] C++：遍历 vector
来源：http://nq.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://ly.huixinmuqiang.cn

[S35] C++：map
来源：http://rb.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lb.huixiangedu.cn

[S36] C++：unordered_map
来源：http://ly.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://er.lnxyls.cn

[S37] C++：set
来源：http://wl.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fb.jctech888.com.cn

[S38] C++：排序
来源：http://gl.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://cu.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://mg.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tk.shtwfgs.cn

[S40] C++：查找元素
来源：http://qw.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://um.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://zm.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dn.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://ov.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://aq.yuntaijiaju.cn


<!-- 参考信息 -->