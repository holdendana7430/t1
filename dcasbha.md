代发 wailian999

ANALYZE TABLE users;
来源：http://ub.huanxung.cn

[Q71] 查看建表语句
来源：http://gw.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xp.huanxung.cn

[Q72] 查看索引
来源：http://kb.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://rd.newstarts.cn

[Q73] 查看表状态
来源：http://hi.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://st.huanxung.cn

[Q74] 强制使用索引
来源：http://ds.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nm.huixiangedu.cn

[Q75] 日期格式化
来源：http://ib.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aj.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pq.szsharing.cn

[Q76] 按天统计
来源：http://gf.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bf.shxzskj.cn

[Q77] 时间加减
来源：http://ff.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cj.shxzskj.cn

[Q78] 当前时间
来源：http://ha.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cj.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://ck.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dn.shxzskj.cn

[Q80] 字符串截取
来源：http://ma.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vw.shxzskj.cn

[Q81] 字符串替换
来源：http://rt.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ed.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://ih.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vy.shtwfgs.cn

[Q83] 大小写转换
来源：http://ne.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lg.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://rh.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://rh.shtwfgs.cn

[Q85] 数值取整
来源：http://ly.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wk.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://tn.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zo.nicolike.cn

[Q87] JSON 字段做条件
来源：http://aj.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ha.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://qy.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://km.huixinmuqiang.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wd.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://mh.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qn.nszjky.cn

[Q90] 生成序号列
来源：http://er.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ot.szsharing.cn

================================================================================
来源：http://ub.bookmarksfly.cn

R. Bash 专题
来源：http://ji.jctech888.com.cn

================================================================================
来源：http://gg.asd995.cn

[R01] shebang 与严格模式
来源：http://az.shxzukj.cn

#!/usr/bin/env bash
来源：http://mb.huixinmuqiang.cn

set -euo pipefail
来源：http://tw.nicolike.cn

[R02] 变量赋值与使用
来源：http://mz.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://vk.lnxyls.cn

[R03] 只读变量
来源：http://kr.huanxung.cn

readonly PI=3.14
来源：http://iw.nicolike.cn

[R04] 位置参数
来源：http://oa.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ok.panjiajie.cn

[R05] 参数默认值
来源：http://za.huixiangedu.cn

name="${1:-default}"
来源：http://rd.szsharing.cn

[R06] 判断命令是否存在
来源：http://tj.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ry.jianghongdianzi.cn

[R07] if 判断文件
来源：http://lu.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nb.gzmigu.cn

[R08] 数值比较
来源：http://td.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bo.jianghongdianzi.cn

[R09] 字符串比较
来源：http://js.nszjky.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://je.newstarts.cn

[R10] 正则匹配
来源：http://rz.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cx.jianghongdianzi.cn

[R11] case 多分支
来源：http://nb.asd995.cn

case "$1" in
来源：http://eb.jctech888.com.cn

start) echo "启动" ;;
来源：http://ft.shxzukj.cn

stop)  echo "停止" ;;
来源：http://ko.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://zc.huixinmuqiang.cn

esac
来源：http://ep.yuexingan06.cn

[R12] for 遍历文件
来源：http://ly.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://fo.9csxet.cn

[R13] for 计数循环
来源：http://an.asd995.cn

for i in {1..10}; do echo "$i"; done
来源：http://jc.wgjwhj.cn

[R14] C 风格 for
来源：http://rh.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gc.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://nz.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://le.yuntaijiaju.cn

[R16] until 等待条件
来源：http://hy.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://la.szsharing.cn

[R17] 数组定义与取值
来源：http://wt.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://us.521024.cn

[R18] 遍历数组
来源：http://pe.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fo.nszjky.cn

[R19] 数组长度
来源：http://fa.colortex.cn

echo "${#arr[@]}"
来源：http://cm.szxytkj.cn

[R20] 关联数组（字典）
来源：http://uc.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qx.gzmigu.cn

[R21] 字符串长度
来源：http://ct.chemitech.net.cn

echo "${#s}"
来源：http://hw.bjjhwx.cn

[R22] 截取子串
来源：http://jb.shtwfgs.cn

echo "${s:0:5}"
来源：http://yj.panjiajie.cn

[R23] 字符串替换
来源：http://nz.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qi.shtwfgs.cn

[R24] 大小写转换
来源：http://en.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://od.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://dx.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ek.hnjuh.cn

[R26] 命令替换
来源：http://ms.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://oj.9csxet.cn

[R27] 算术展开
来源：http://ka.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://ym.szxytkj.cn

[R28] 浮点运算
来源：http://kb.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://hu.9csxet.cn

[R29] 定义函数
来源：http://xb.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cc.wgjwhj.cn

[R30] 函数返回状态码
来源：http://uv.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://yg.shxzukj.cn

[R31] 局部变量
来源：http://lw.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://hn.hahajie.cn

[R32] 参数个数校验
来源：http://pq.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yq.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://jb.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bl.panjiajie.cn

[R34] 退出时清理
来源：http://ha.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qf.hnjuh.cn

[R35] 后台执行并等待
来源：http://yj.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gw.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://lv.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jc.colortex.cn

[R37] 把输出赋给变量
来源：http://pd.jianghongdianzi.cn

files=$(ls -1)
来源：http://pi.huixinmuqiang.cn

[R38] 管道串联
来源：http://vw.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://uh.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://gg.hnjuh.cn

cmd > out.log 2>&1
来源：http://te.haigaiapp.cn

[R40] 追加写日志
来源：http://aw.panjiajie.cn

echo "log" >> out.log
来源：http://vl.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://wg.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://mg.yuntaijiaju.cn

[R42] 输入重定向
来源：http://wx.chemitech.net.cn

wc -l < a.txt
来源：http://ua.lnxyls.cn

[R43] 按名字查找文件
来源：http://mx.521024.cn

find . -name "*.log" -type f
来源：http://ul.shxzukj.cn

[R44] 按修改时间查找
来源：http://yz.chemitech.net.cn

find . -mtime -7 -type f
来源：http://qe.huixiangedu.cn

[R45] 批量删除
来源：http://la.hahajie.cn

find . -name "*.tmp" -delete
来源：http://ce.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://ex.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jn.hnjuh.cn

[R47] sed 单行替换
来源：http://lc.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sq.nicolike.cn

[R48] awk 取指定列
来源：http://qk.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://on.wgjwhj.cn

[R49] awk 带条件
来源：http://cq.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jk.bjjhwx.cn

[R50] awk 求和
来源：http://xj.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jc.szsharing.cn

[R51] 排序去重取前几
来源：http://dn.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rz.jctech888.com.cn

[R52] 统计行数
来源：http://sx.shtwfgs.cn

wc -l a.txt
来源：http://og.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://gr.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xc.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://rg.newstarts.cn

diff a.txt b.txt
来源：http://jg.yuexingan06.cn

[R55] 压缩与解压
来源：http://bh.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cw.shxzukj.cn

[R56] 远程拷贝
来源：http://ly.wgjwhj.cn

scp file user@host:/path/
来源：http://rq.hnjuh.cn

[R57] 远程执行命令
来源：http://ez.hahajie.cn

ssh user@host 'uptime'
来源：http://pz.hahajie.cn

[R58] 下载文件
来源：http://on.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lk.lnxyls.cn

[R59] 发 POST JSON
来源：http://pu.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gt.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://oj.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wx.huixiangedu.cn

[R61] 磁盘占用
来源：http://dh.521024.cn

df -h;  du -sh *
来源：http://ga.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://yx.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://zp.yuexingan06.cn

[R63] 内存与进程
来源：http://uz.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://ee.hnjuh.cn

[R64] 结束进程
来源：http://ch.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://gb.hnjuh.cn

[R65] 查看端口占用
来源：http://dx.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ik.nicolike.cn

[R66] 定时任务
来源：http://eg.huanxung.cn

crontab -e;  crontab -l
来源：http://az.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://rl.shxzukj.cn

openssl rand -hex 16
来源：http://xv.nszjky.cn

[R68] 计算文件校验值
来源：http://yb.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rc.haigaiapp.cn

[R69] 生成随机密码
来源：http://mv.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://po.huanxung.cn

[R70] 时间戳与互转
来源：http://uf.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://gj.9csxet.cn

[R71] 日期格式化
来源：http://fd.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lp.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://jf.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vk.huixinmuqiang.cn

[R73] 分割大日志
来源：http://fa.gzmigu.cn

split -l 1000 big.log part_
来源：http://kv.shxzukj.cn

[R74] 批量重命名
来源：http://zl.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lw.asd995.cn

[R75] 导出环境变量
来源：http://zj.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://ah.521024.cn

[R76] 使用临时文件
来源：http://vb.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eo.lnxyls.cn

[R77] 读取用户输入
来源：http://xl.muxihuayi.cn

read -rp "请输入: " ans
来源：http://ch.bookmarksfly.cn

[R78] 交互式菜单
来源：http://wd.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cg.wgjwhj.cn

[R79] 解析命令行选项
来源：http://cn.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mo.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://jr.panjiajie.cn

time ./run.sh
来源：http://tv.colortex.cn

================================================================================
来源：http://dt.szsharing.cn

S. C / C++ 专题
来源：http://vx.gzmigu.cn

================================================================================
来源：http://bv.nicolike.cn

[S01] C：Hello World
来源：http://ca.shtwfgs.cn

#include <stdio.h>
来源：http://lo.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fa.colortex.cn

[S02] C：变量与格式化输出
来源：http://on.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://vg.huixiangedu.cn

[S03] C：读入整数
来源：http://hp.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://cq.wgjwhj.cn

[S04] C：字符串复制
来源：http://ji.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uz.szsharing.cn

[S05] C：字符串长度
来源：http://pv.szsharing.cn

strlen(s)
来源：http://xc.wgjwhj.cn

[S06] C：字符串比较
来源：http://td.muxihuayi.cn

strcmp(a, b) == 0
来源：http://nv.lnxyls.cn

[S07] C：数组遍历求和
来源：http://sj.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vh.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://do.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eb.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://lw.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lh.colortex.cn

[S10] C：指针与解引用
来源：http://jr.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://ut.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://ef.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://hl.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bt.huixinmuqiang.cn

fclose(f);
来源：http://ug.nszjky.cn

[S12] C：写文件
来源：http://xy.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lp.jianghongdianzi.cn

[S13] C：宏定义
来源：http://ku.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oz.huanxung.cn

[S14] C：枚举
来源：http://qg.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://ge.colortex.cn

[S15] C：类型转换
来源：http://ir.szsharing.cn

(double) a / b
来源：http://zb.szsharing.cn

[S16] C：位操作置位
来源：http://gl.lnxyls.cn

x |= (1 << 3);
来源：http://cb.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://hj.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hr.521024.cn

[S18] C：命令行参数
来源：http://dy.shtwfgs.cn

int main(int argc, char **argv)
来源：http://be.shtwfgs.cn

[S19] C：快速排序
来源：http://ny.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ee.nszjky.cn

[S20] C：二分查找
来源：http://qb.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zm.szsharing.cn

[S21] C：字符类别判断
来源：http://rx.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zf.521024.cn

[S22] C：字符串转数字
来源：http://ai.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xi.nszjky.cn

[S23] C：随机数
来源：http://iv.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zi.nszjky.cn

[S24] C：获取本地时间
来源：http://ug.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mv.muxihuayi.cn

[S25] C：内存拷贝
来源：http://xz.panjiajie.cn

memcpy(dst, src, n);
来源：http://gl.asd995.cn

[S26] C：内存清零
来源：http://os.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://wk.chemitech.net.cn

[S27] C：定义常量
来源：http://ym.huanxung.cn

const double PI = 3.14159;
来源：http://hv.bookmarksfly.cn

[S28] C：静态变量
来源：http://pb.panjiajie.cn

static int counter = 0;
来源：http://zy.hnjuh.cn

[S29] C：变参函数
来源：http://ur.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ld.muxihuayi.cn

[S30] C：头文件保护
来源：http://dt.shxzukj.cn

#ifndef X_H
来源：http://fv.chemitech.net.cn

#define X_H
来源：http://dg.yuexingan06.cn

#endif
来源：http://fl.nszjky.cn

[S31] C++：Hello World
来源：http://mb.huixinmuqiang.cn

#include <iostream>
来源：http://wz.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://hx.lnxyls.cn

[S32] C++：字符串
来源：http://tb.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://dn.szxytkj.cn

[S33] C++：vector 增删
来源：http://os.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ik.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://qy.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://vr.szsharing.cn

[S35] C++：map
来源：http://me.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cn.wgjwhj.cn

[S36] C++：unordered_map
来源：http://vu.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rk.huanxung.cn

[S37] C++：set
来源：http://zf.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jq.521024.cn

[S38] C++：排序
来源：http://qb.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://xv.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://su.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gi.bjjhwx.cn

[S40] C++：查找元素
来源：http://jr.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ke.jianghongdianzi.cn


<!-- 参考信息 -->