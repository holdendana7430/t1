代发 wailian999

ANALYZE TABLE users;
来源：http://ci.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://wm.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ka.shtwfgs.cn

[Q72] 查看索引
来源：http://wa.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://sg.hahajie.cn

[Q73] 查看表状态
来源：http://ac.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fa.wgjwhj.cn

[Q74] 强制使用索引
来源：http://or.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://no.huixiangedu.cn

[Q75] 日期格式化
来源：http://dp.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kd.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eu.muxihuayi.cn

[Q76] 按天统计
来源：http://yj.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bu.asd995.cn

[Q77] 时间加减
来源：http://iz.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bw.bjjhwx.cn

[Q78] 当前时间
来源：http://zh.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lj.hnjuh.cn

[Q79] 字符串拼接
来源：http://nx.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bp.bookmarksfly.cn

[Q80] 字符串截取
来源：http://hb.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lm.huanxung.cn

[Q81] 字符串替换
来源：http://ct.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ha.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://cl.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ns.521024.cn

[Q83] 大小写转换
来源：http://ti.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jh.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://dm.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://af.chemitech.net.cn

[Q85] 数值取整
来源：http://el.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mw.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://mg.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://to.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://re.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vn.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://jc.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qo.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ym.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://wc.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lb.shxzskj.cn

[Q90] 生成序号列
来源：http://ki.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iu.9csxet.cn

================================================================================
来源：http://va.521024.cn

R. Bash 专题
来源：http://fx.szxytkj.cn

================================================================================
来源：http://pp.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://nf.gzmigu.cn

#!/usr/bin/env bash
来源：http://rn.huanxung.cn

set -euo pipefail
来源：http://qt.colortex.cn

[R02] 变量赋值与使用
来源：http://ld.nicolike.cn

name="Tom"; echo "$name"
来源：http://zl.chemitech.net.cn

[R03] 只读变量
来源：http://ql.haigaiapp.cn

readonly PI=3.14
来源：http://lh.huixinmuqiang.cn

[R04] 位置参数
来源：http://ks.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kv.gzmigu.cn

[R05] 参数默认值
来源：http://at.newstarts.cn

name="${1:-default}"
来源：http://ix.szxytkj.cn

[R06] 判断命令是否存在
来源：http://tr.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fd.jianghongdianzi.cn

[R07] if 判断文件
来源：http://rk.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lr.bjjhwx.cn

[R08] 数值比较
来源：http://eo.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vt.shtwfgs.cn

[R09] 字符串比较
来源：http://up.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bl.nszjky.cn

[R10] 正则匹配
来源：http://ff.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mj.huixiangedu.cn

[R11] case 多分支
来源：http://zt.huixinmuqiang.cn

case "$1" in
来源：http://so.gzmigu.cn

start) echo "启动" ;;
来源：http://pu.521024.cn

stop)  echo "停止" ;;
来源：http://fz.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://an.huixinmuqiang.cn

esac
来源：http://kh.huixiangedu.cn

[R12] for 遍历文件
来源：http://va.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://yp.colortex.cn

[R13] for 计数循环
来源：http://ha.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://nr.haigaiapp.cn

[R14] C 风格 for
来源：http://ba.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zo.lnxyls.cn

[R15] while 逐行读文件
来源：http://ql.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sj.nicolike.cn

[R16] until 等待条件
来源：http://ap.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bx.huixiangedu.cn

[R17] 数组定义与取值
来源：http://yh.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ou.hnjuh.cn

[R18] 遍历数组
来源：http://fi.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sk.haigaiapp.cn

[R19] 数组长度
来源：http://kr.shtwfgs.cn

echo "${#arr[@]}"
来源：http://fq.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://ba.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fz.lnxyls.cn

[R21] 字符串长度
来源：http://sf.wgjwhj.cn

echo "${#s}"
来源：http://ud.nicolike.cn

[R22] 截取子串
来源：http://uc.chemitech.net.cn

echo "${s:0:5}"
来源：http://zh.szxytkj.cn

[R23] 字符串替换
来源：http://mt.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rn.gzmigu.cn

[R24] 大小写转换
来源：http://xr.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fr.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://hr.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qq.9csxet.cn

[R26] 命令替换
来源：http://cy.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://oe.huixiangedu.cn

[R27] 算术展开
来源：http://uf.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://sr.bjjhwx.cn

[R28] 浮点运算
来源：http://jq.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://sc.muxihuayi.cn

[R29] 定义函数
来源：http://bq.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mf.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://ky.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://xe.bjjhwx.cn

[R31] 局部变量
来源：http://vr.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://ja.wgjwhj.cn

[R32] 参数个数校验
来源：http://xa.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eu.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://zh.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pa.nicolike.cn

[R34] 退出时清理
来源：http://ei.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xp.muxihuayi.cn

[R35] 后台执行并等待
来源：http://cd.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://as.9csxet.cn

[R36] 并发执行多个任务
来源：http://rk.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ik.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://ba.shxzukj.cn

files=$(ls -1)
来源：http://gg.nszjky.cn

[R38] 管道串联
来源：http://vg.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://wv.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://cq.haigaiapp.cn

cmd > out.log 2>&1
来源：http://dy.panjiajie.cn

[R40] 追加写日志
来源：http://nr.nicolike.cn

echo "log" >> out.log
来源：http://lf.bookmarksfly.cn

[R41] 丢弃输出
来源：http://uh.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://va.gzmigu.cn

[R42] 输入重定向
来源：http://ch.lnxyls.cn

wc -l < a.txt
来源：http://bc.521024.cn

[R43] 按名字查找文件
来源：http://nr.gzmigu.cn

find . -name "*.log" -type f
来源：http://lp.muxihuayi.cn

[R44] 按修改时间查找
来源：http://qz.panjiajie.cn

find . -mtime -7 -type f
来源：http://pb.lnxyls.cn

[R45] 批量删除
来源：http://pv.nszjky.cn

find . -name "*.tmp" -delete
来源：http://er.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://fd.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tn.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://di.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tn.hnjuh.cn

[R48] awk 取指定列
来源：http://do.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://po.colortex.cn

[R49] awk 带条件
来源：http://at.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kf.colortex.cn

[R50] awk 求和
来源：http://se.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zn.chemitech.net.cn

[R51] 排序去重取前几
来源：http://kj.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://us.huixinmuqiang.cn

[R52] 统计行数
来源：http://lw.huixinmuqiang.cn

wc -l a.txt
来源：http://rm.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://nu.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fq.jctech888.com.cn

[R54] 比较两个文件
来源：http://sm.nicolike.cn

diff a.txt b.txt
来源：http://gw.colortex.cn

[R55] 压缩与解压
来源：http://zs.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yw.shtwfgs.cn

[R56] 远程拷贝
来源：http://xp.lnxyls.cn

scp file user@host:/path/
来源：http://ma.colortex.cn

[R57] 远程执行命令
来源：http://yg.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://eh.hahajie.cn

[R58] 下载文件
来源：http://ky.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oa.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://xg.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sc.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://ek.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nb.wgjwhj.cn

[R61] 磁盘占用
来源：http://ix.nicolike.cn

df -h;  du -sh *
来源：http://yf.hahajie.cn

[R62] 找最占空间的文件
来源：http://fd.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://rr.asd995.cn

[R63] 内存与进程
来源：http://en.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://zl.shxzukj.cn

[R64] 结束进程
来源：http://js.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://yw.bjjhwx.cn

[R65] 查看端口占用
来源：http://yh.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ik.yuntaijiaju.cn

[R66] 定时任务
来源：http://mf.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://dq.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://iz.huixiangedu.cn

openssl rand -hex 16
来源：http://uu.hahajie.cn

[R68] 计算文件校验值
来源：http://oe.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fd.521024.cn

[R69] 生成随机密码
来源：http://or.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://zs.lnxyls.cn

[R70] 时间戳与互转
来源：http://rm.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://kj.bookmarksfly.cn

[R71] 日期格式化
来源：http://tr.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bp.521024.cn

[R72] 等待端口就绪
来源：http://gt.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://df.shxzskj.cn

[R73] 分割大日志
来源：http://td.newstarts.cn

split -l 1000 big.log part_
来源：http://ff.jctech888.com.cn

[R74] 批量重命名
来源：http://go.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://he.shxzukj.cn

[R75] 导出环境变量
来源：http://ms.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://jg.chemitech.net.cn

[R76] 使用临时文件
来源：http://yy.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uc.hahajie.cn

[R77] 读取用户输入
来源：http://co.9csxet.cn

read -rp "请输入: " ans
来源：http://zh.jctech888.com.cn

[R78] 交互式菜单
来源：http://xv.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lb.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://ex.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iz.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://vo.asd995.cn

time ./run.sh
来源：http://yo.shxzukj.cn

================================================================================
来源：http://pr.nicolike.cn

S. C / C++ 专题
来源：http://xq.muxihuayi.cn

================================================================================
来源：http://nt.nszjky.cn

[S01] C：Hello World
来源：http://lw.szsharing.cn

#include <stdio.h>
来源：http://xv.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gi.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://yg.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://bb.bookmarksfly.cn

[S03] C：读入整数
来源：http://rk.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://zr.gzmigu.cn

[S04] C：字符串复制
来源：http://zm.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rb.newstarts.cn

[S05] C：字符串长度
来源：http://fy.shxzukj.cn

strlen(s)
来源：http://ev.newstarts.cn

[S06] C：字符串比较
来源：http://xt.nicolike.cn

strcmp(a, b) == 0
来源：http://nb.521024.cn

[S07] C：数组遍历求和
来源：http://fc.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://es.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://sa.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vo.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://kq.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://by.huanxung.cn

[S10] C：指针与解引用
来源：http://dl.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://de.bjjhwx.cn

[S11] C：逐行读文件
来源：http://pn.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://ti.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gj.wgjwhj.cn

fclose(f);
来源：http://am.szxytkj.cn

[S12] C：写文件
来源：http://ta.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lm.bjjhwx.cn

[S13] C：宏定义
来源：http://eo.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uv.szsharing.cn

[S14] C：枚举
来源：http://wl.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://ab.bookmarksfly.cn

[S15] C：类型转换
来源：http://wk.jianghongdianzi.cn

(double) a / b
来源：http://nt.shxzskj.cn

[S16] C：位操作置位
来源：http://vj.jianghongdianzi.cn

x |= (1 << 3);
来源：http://nf.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://yd.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gf.huixiangedu.cn

[S18] C：命令行参数
来源：http://bv.huixiangedu.cn

int main(int argc, char **argv)
来源：http://dz.nszjky.cn

[S19] C：快速排序
来源：http://zx.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bg.yuntaijiaju.cn

[S20] C：二分查找
来源：http://jh.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fv.hahajie.cn

[S21] C：字符类别判断
来源：http://im.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ac.huixiangedu.cn

[S22] C：字符串转数字
来源：http://fi.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ov.asd995.cn

[S23] C：随机数
来源：http://zg.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://aa.9csxet.cn

[S24] C：获取本地时间
来源：http://oh.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rt.szsharing.cn

[S25] C：内存拷贝
来源：http://nx.szsharing.cn

memcpy(dst, src, n);
来源：http://nx.huanxung.cn

[S26] C：内存清零
来源：http://nh.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://sw.9csxet.cn

[S27] C：定义常量
来源：http://kv.hnjuh.cn

const double PI = 3.14159;
来源：http://iq.lnxyls.cn

[S28] C：静态变量
来源：http://ox.chemitech.net.cn

static int counter = 0;
来源：http://fx.9csxet.cn

[S29] C：变参函数
来源：http://ms.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tg.nicolike.cn

[S30] C：头文件保护
来源：http://ll.9csxet.cn

#ifndef X_H
来源：http://uq.haigaiapp.cn

#define X_H
来源：http://do.hnjuh.cn

#endif
来源：http://rs.wgjwhj.cn

[S31] C++：Hello World
来源：http://th.wgjwhj.cn

#include <iostream>
来源：http://sz.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://gs.newstarts.cn

[S32] C++：字符串
来源：http://nv.521024.cn

std::string s = "hi";  s += "!";
来源：http://kg.panjiajie.cn

[S33] C++：vector 增删
来源：http://xf.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ec.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://fl.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://ax.haigaiapp.cn

[S35] C++：map
来源：http://bo.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sw.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://bc.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yk.9csxet.cn

[S37] C++：set
来源：http://ul.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ym.asd995.cn

[S38] C++：排序
来源：http://av.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://ec.asd995.cn

[S39] C++：自定义比较器排序
来源：http://nh.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pj.shxzukj.cn

[S40] C++：查找元素
来源：http://wl.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vb.szxytkj.cn


<!-- 参考信息 -->