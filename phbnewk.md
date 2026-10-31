代发 wailian999

SHOW INDEX FROM users;
来源：http://se.colortex.cn

[Q73] 查看表状态
来源：http://wl.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://um.muxihuayi.cn

[Q74] 强制使用索引
来源：http://ua.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sj.shtwfgs.cn

[Q75] 日期格式化
来源：http://xs.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ep.huanxung.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yk.muxihuayi.cn

[Q76] 按天统计
来源：http://gd.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://co.huanxung.cn

[Q77] 时间加减
来源：http://eh.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vu.yuntaijiaju.cn

[Q78] 当前时间
来源：http://kj.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tg.hnjuh.cn

[Q79] 字符串拼接
来源：http://iq.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ht.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://qh.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kk.bjjhwx.cn

[Q81] 字符串替换
来源：http://pm.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bg.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://fc.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lf.9csxet.cn

[Q83] 大小写转换
来源：http://xi.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cm.lnxyls.cn

[Q84] 去除首尾空格
来源：http://yn.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://dk.shxzskj.cn

[Q85] 数值取整
来源：http://pt.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qp.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://ef.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fh.hahajie.cn

[Q87] JSON 字段做条件
来源：http://tj.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dm.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://hk.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gc.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ct.lnxyls.cn

[Q89] 判断表是否存在
来源：http://cy.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zp.muxihuayi.cn

[Q90] 生成序号列
来源：http://sd.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uq.jianghongdianzi.cn

================================================================================
来源：http://di.nicolike.cn

R. Bash 专题
来源：http://db.panjiajie.cn

================================================================================
来源：http://yw.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://yr.lnxyls.cn

#!/usr/bin/env bash
来源：http://hp.wgjwhj.cn

set -euo pipefail
来源：http://ig.newstarts.cn

[R02] 变量赋值与使用
来源：http://bw.shxzskj.cn

name="Tom"; echo "$name"
来源：http://ks.shtwfgs.cn

[R03] 只读变量
来源：http://sb.haigaiapp.cn

readonly PI=3.14
来源：http://sm.521024.cn

[R04] 位置参数
来源：http://oc.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rw.muxihuayi.cn

[R05] 参数默认值
来源：http://xt.muxihuayi.cn

name="${1:-default}"
来源：http://xs.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://oc.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tr.haigaiapp.cn

[R07] if 判断文件
来源：http://an.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hp.huixiangedu.cn

[R08] 数值比较
来源：http://qz.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://et.lnxyls.cn

[R09] 字符串比较
来源：http://bb.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cy.wgjwhj.cn

[R10] 正则匹配
来源：http://ki.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vb.shtwfgs.cn

[R11] case 多分支
来源：http://kp.huixinmuqiang.cn

case "$1" in
来源：http://zo.jctech888.com.cn

start) echo "启动" ;;
来源：http://eu.szsharing.cn

stop)  echo "停止" ;;
来源：http://mr.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://ji.huanxung.cn

esac
来源：http://oo.shtwfgs.cn

[R12] for 遍历文件
来源：http://bt.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://jd.colortex.cn

[R13] for 计数循环
来源：http://zf.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://un.shxzskj.cn

[R14] C 风格 for
来源：http://gf.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zj.colortex.cn

[R15] while 逐行读文件
来源：http://bu.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zf.szsharing.cn

[R16] until 等待条件
来源：http://wt.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vn.asd995.cn

[R17] 数组定义与取值
来源：http://pf.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rl.gzmigu.cn

[R18] 遍历数组
来源：http://cs.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vc.wgjwhj.cn

[R19] 数组长度
来源：http://ic.asd995.cn

echo "${#arr[@]}"
来源：http://mo.hahajie.cn

[R20] 关联数组（字典）
来源：http://cw.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jq.huixiangedu.cn

[R21] 字符串长度
来源：http://hd.jctech888.com.cn

echo "${#s}"
来源：http://jo.hnjuh.cn

[R22] 截取子串
来源：http://da.shtwfgs.cn

echo "${s:0:5}"
来源：http://hb.bjjhwx.cn

[R23] 字符串替换
来源：http://tf.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xt.szsharing.cn

[R24] 大小写转换
来源：http://gz.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tf.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://wv.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gr.521024.cn

[R26] 命令替换
来源：http://jp.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://cj.chemitech.net.cn

[R27] 算术展开
来源：http://wz.521024.cn

echo $((1 + 2 * 3))
来源：http://cc.nicolike.cn

[R28] 浮点运算
来源：http://eq.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://wn.huixiangedu.cn

[R29] 定义函数
来源：http://ws.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qj.hnjuh.cn

[R30] 函数返回状态码
来源：http://nm.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://db.hahajie.cn

[R31] 局部变量
来源：http://jk.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://qk.hnjuh.cn

[R32] 参数个数校验
来源：http://vq.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qm.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://sv.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wd.szxytkj.cn

[R34] 退出时清理
来源：http://bx.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qy.bjjhwx.cn

[R35] 后台执行并等待
来源：http://vq.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rx.521024.cn

[R36] 并发执行多个任务
来源：http://nq.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iv.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://bg.shxzukj.cn

files=$(ls -1)
来源：http://dc.hahajie.cn

[R38] 管道串联
来源：http://ik.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://tq.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://ha.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://li.panjiajie.cn

[R40] 追加写日志
来源：http://wg.521024.cn

echo "log" >> out.log
来源：http://sy.jctech888.com.cn

[R41] 丢弃输出
来源：http://po.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://fg.muxihuayi.cn

[R42] 输入重定向
来源：http://pl.9csxet.cn

wc -l < a.txt
来源：http://rx.bjjhwx.cn

[R43] 按名字查找文件
来源：http://zl.wgjwhj.cn

find . -name "*.log" -type f
来源：http://bp.colortex.cn

[R44] 按修改时间查找
来源：http://wi.panjiajie.cn

find . -mtime -7 -type f
来源：http://oo.newstarts.cn

[R45] 批量删除
来源：http://ov.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://mv.shxzukj.cn

[R46] 递归替换文件内容
来源：http://of.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lt.jctech888.com.cn

[R47] sed 单行替换
来源：http://vy.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://iy.huanxung.cn

[R48] awk 取指定列
来源：http://pc.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://wn.jctech888.com.cn

[R49] awk 带条件
来源：http://gw.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ty.hahajie.cn

[R50] awk 求和
来源：http://wn.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lb.hnjuh.cn

[R51] 排序去重取前几
来源：http://nj.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://my.shxzukj.cn

[R52] 统计行数
来源：http://kx.lnxyls.cn

wc -l a.txt
来源：http://kh.521024.cn

[R53] 查看文件头与实时尾
来源：http://ua.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uj.gzmigu.cn

[R54] 比较两个文件
来源：http://fs.lnxyls.cn

diff a.txt b.txt
来源：http://mp.jctech888.com.cn

[R55] 压缩与解压
来源：http://gi.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tn.yuexingan06.cn

[R56] 远程拷贝
来源：http://do.newstarts.cn

scp file user@host:/path/
来源：http://qb.9csxet.cn

[R57] 远程执行命令
来源：http://fi.hnjuh.cn

ssh user@host 'uptime'
来源：http://ff.bjjhwx.cn

[R58] 下载文件
来源：http://nj.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pi.haigaiapp.cn

[R59] 发 POST JSON
来源：http://yb.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jp.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://tq.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zm.shxzukj.cn

[R61] 磁盘占用
来源：http://gz.bookmarksfly.cn

df -h;  du -sh *
来源：http://yv.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://ba.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://bk.lnxyls.cn

[R63] 内存与进程
来源：http://bb.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://sx.chemitech.net.cn

[R64] 结束进程
来源：http://rr.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://oh.huixiangedu.cn

[R65] 查看端口占用
来源：http://cb.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ym.9csxet.cn

[R66] 定时任务
来源：http://zi.9csxet.cn

crontab -e;  crontab -l
来源：http://sh.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://jw.lnxyls.cn

openssl rand -hex 16
来源：http://rf.haigaiapp.cn

[R68] 计算文件校验值
来源：http://wc.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nz.colortex.cn

[R69] 生成随机密码
来源：http://fo.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://hn.lnxyls.cn

[R70] 时间戳与互转
来源：http://fq.szsharing.cn

date +%s;  date -d @1700000000
来源：http://js.panjiajie.cn

[R71] 日期格式化
来源：http://tk.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://li.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://qm.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://id.yuntaijiaju.cn

[R73] 分割大日志
来源：http://ur.chemitech.net.cn

split -l 1000 big.log part_
来源：http://is.chemitech.net.cn

[R74] 批量重命名
来源：http://xd.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cn.asd995.cn

[R75] 导出环境变量
来源：http://ss.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://qb.chemitech.net.cn

[R76] 使用临时文件
来源：http://cp.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rv.gzmigu.cn

[R77] 读取用户输入
来源：http://yt.yuexingan06.cn

read -rp "请输入: " ans
来源：http://gp.9csxet.cn

[R78] 交互式菜单
来源：http://mb.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rn.shxzukj.cn

[R79] 解析命令行选项
来源：http://gi.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wo.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://lz.jianghongdianzi.cn

time ./run.sh
来源：http://vb.szsharing.cn

================================================================================
来源：http://bp.shtwfgs.cn

S. C / C++ 专题
来源：http://ta.jianghongdianzi.cn

================================================================================
来源：http://up.szxytkj.cn

[S01] C：Hello World
来源：http://vg.panjiajie.cn

#include <stdio.h>
来源：http://el.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cw.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://tv.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://fu.wgjwhj.cn

[S03] C：读入整数
来源：http://ut.nicolike.cn

int x; scanf("%d", &x);
来源：http://yj.asd995.cn

[S04] C：字符串复制
来源：http://pj.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cd.521024.cn

[S05] C：字符串长度
来源：http://ay.szsharing.cn

strlen(s)
来源：http://zn.newstarts.cn

[S06] C：字符串比较
来源：http://cm.521024.cn

strcmp(a, b) == 0
来源：http://jd.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://af.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ds.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://jt.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rb.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://jn.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kq.lnxyls.cn

[S10] C：指针与解引用
来源：http://sz.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://ct.jctech888.com.cn

[S11] C：逐行读文件
来源：http://zh.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://jk.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cc.szxytkj.cn

fclose(f);
来源：http://xz.huixiangedu.cn

[S12] C：写文件
来源：http://fg.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ma.bjjhwx.cn

[S13] C：宏定义
来源：http://zi.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xi.jctech888.com.cn

[S14] C：枚举
来源：http://fn.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ej.bookmarksfly.cn

[S15] C：类型转换
来源：http://kx.huanxung.cn

(double) a / b
来源：http://cj.hahajie.cn

[S16] C：位操作置位
来源：http://fj.yuntaijiaju.cn

x |= (1 << 3);
来源：http://se.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://qv.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jq.shtwfgs.cn

[S18] C：命令行参数
来源：http://wv.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://ls.521024.cn

[S19] C：快速排序
来源：http://df.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qo.shxzukj.cn

[S20] C：二分查找
来源：http://yk.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://di.shxzskj.cn

[S21] C：字符类别判断
来源：http://sp.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://up.asd995.cn

[S22] C：字符串转数字
来源：http://ji.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lb.colortex.cn

[S23] C：随机数
来源：http://wr.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://at.newstarts.cn

[S24] C：获取本地时间
来源：http://jo.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ax.szxytkj.cn

[S25] C：内存拷贝
来源：http://pe.bjjhwx.cn

memcpy(dst, src, n);
来源：http://zy.521024.cn

[S26] C：内存清零
来源：http://ip.asd995.cn

memset(a, 0, sizeof a);
来源：http://uq.huanxung.cn

[S27] C：定义常量
来源：http://bc.colortex.cn

const double PI = 3.14159;
来源：http://lj.521024.cn

[S28] C：静态变量
来源：http://ms.newstarts.cn

static int counter = 0;
来源：http://zl.9csxet.cn

[S29] C：变参函数
来源：http://um.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ko.9csxet.cn

[S30] C：头文件保护
来源：http://ew.9csxet.cn

#ifndef X_H
来源：http://kr.panjiajie.cn

#define X_H
来源：http://af.szsharing.cn

#endif
来源：http://ym.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://yo.nicolike.cn

#include <iostream>
来源：http://jb.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://jz.gzmigu.cn

[S32] C++：字符串
来源：http://te.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://nc.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://yp.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lz.521024.cn

[S34] C++：遍历 vector
来源：http://im.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://kb.shtwfgs.cn

[S35] C++：map
来源：http://cn.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lz.haigaiapp.cn

[S36] C++：unordered_map
来源：http://nc.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mh.yuexingan06.cn

[S37] C++：set
来源：http://ae.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iz.colortex.cn

[S38] C++：排序
来源：http://er.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://id.colortex.cn

[S39] C++：自定义比较器排序
来源：http://vb.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://um.haigaiapp.cn

[S40] C++：查找元素
来源：http://ju.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yp.shxzukj.cn

[S41] C++：类与构造函数
来源：http://au.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://af.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://qa.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://zs.szxytkj.cn


<!-- 参考信息 -->