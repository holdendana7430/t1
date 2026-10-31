代发 wailian999

SHOW INDEX FROM users;
来源：http://fb.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://iv.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fe.shtwfgs.cn

[Q74] 强制使用索引
来源：http://bv.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gg.wgjwhj.cn

[Q75] 日期格式化
来源：http://is.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ly.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cb.haigaiapp.cn

[Q76] 按天统计
来源：http://qr.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sz.bjjhwx.cn

[Q77] 时间加减
来源：http://wj.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tu.jctech888.com.cn

[Q78] 当前时间
来源：http://oa.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qi.huanxung.cn

[Q79] 字符串拼接
来源：http://ot.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uh.jctech888.com.cn

[Q80] 字符串截取
来源：http://wp.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nn.szsharing.cn

[Q81] 字符串替换
来源：http://lw.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kl.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://ls.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bd.nicolike.cn

[Q83] 大小写转换
来源：http://wm.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ow.nicolike.cn

[Q84] 去除首尾空格
来源：http://jd.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://zm.chemitech.net.cn

[Q85] 数值取整
来源：http://pc.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sq.colortex.cn

[Q86] 读取 JSON 字段
来源：http://nr.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vh.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://ji.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gw.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://ys.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hr.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pn.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://zt.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://me.szxytkj.cn

[Q90] 生成序号列
来源：http://gw.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sg.yuntaijiaju.cn

================================================================================
来源：http://ht.lnxyls.cn

R. Bash 专题
来源：http://bk.shtwfgs.cn

================================================================================
来源：http://mu.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://ji.asd995.cn

#!/usr/bin/env bash
来源：http://es.shxzukj.cn

set -euo pipefail
来源：http://tt.shxzskj.cn

[R02] 变量赋值与使用
来源：http://pe.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://gg.yuntaijiaju.cn

[R03] 只读变量
来源：http://xh.jctech888.com.cn

readonly PI=3.14
来源：http://jt.hahajie.cn

[R04] 位置参数
来源：http://hp.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gx.panjiajie.cn

[R05] 参数默认值
来源：http://vw.huanxung.cn

name="${1:-default}"
来源：http://oz.9csxet.cn

[R06] 判断命令是否存在
来源：http://do.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cq.asd995.cn

[R07] if 判断文件
来源：http://vy.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sr.huixiangedu.cn

[R08] 数值比较
来源：http://yi.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wq.szxytkj.cn

[R09] 字符串比较
来源：http://jf.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hv.bookmarksfly.cn

[R10] 正则匹配
来源：http://ao.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://au.lnxyls.cn

[R11] case 多分支
来源：http://ch.hnjuh.cn

case "$1" in
来源：http://kr.hahajie.cn

start) echo "启动" ;;
来源：http://wy.panjiajie.cn

stop)  echo "停止" ;;
来源：http://ic.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://ql.szsharing.cn

esac
来源：http://sp.panjiajie.cn

[R12] for 遍历文件
来源：http://if.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://fm.jianghongdianzi.cn

[R13] for 计数循环
来源：http://ra.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://er.shxzukj.cn

[R14] C 风格 for
来源：http://oa.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yp.huanxung.cn

[R15] while 逐行读文件
来源：http://qq.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nn.muxihuayi.cn

[R16] until 等待条件
来源：http://ki.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ed.gzmigu.cn

[R17] 数组定义与取值
来源：http://sv.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dh.hnjuh.cn

[R18] 遍历数组
来源：http://fb.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fr.huixinmuqiang.cn

[R19] 数组长度
来源：http://ay.nszjky.cn

echo "${#arr[@]}"
来源：http://ke.shxzukj.cn

[R20] 关联数组（字典）
来源：http://cg.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://st.shxzukj.cn

[R21] 字符串长度
来源：http://xb.gzmigu.cn

echo "${#s}"
来源：http://rs.9csxet.cn

[R22] 截取子串
来源：http://gf.521024.cn

echo "${s:0:5}"
来源：http://qa.nszjky.cn

[R23] 字符串替换
来源：http://as.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sb.szsharing.cn

[R24] 大小写转换
来源：http://qb.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vc.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://ss.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://in.gzmigu.cn

[R26] 命令替换
来源：http://oa.521024.cn

now=$(date +%F); echo "$now"
来源：http://mn.shxzskj.cn

[R27] 算术展开
来源：http://xo.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://gc.jianghongdianzi.cn

[R28] 浮点运算
来源：http://xx.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://og.wgjwhj.cn

[R29] 定义函数
来源：http://gk.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ot.bjjhwx.cn

[R30] 函数返回状态码
来源：http://yt.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://av.nicolike.cn

[R31] 局部变量
来源：http://kc.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://se.haigaiapp.cn

[R32] 参数个数校验
来源：http://wi.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nn.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://po.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cc.521024.cn

[R34] 退出时清理
来源：http://if.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qr.muxihuayi.cn

[R35] 后台执行并等待
来源：http://hd.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rp.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://gf.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ui.521024.cn

[R37] 把输出赋给变量
来源：http://cn.shxzukj.cn

files=$(ls -1)
来源：http://xn.nicolike.cn

[R38] 管道串联
来源：http://wo.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://ap.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://kk.colortex.cn

cmd > out.log 2>&1
来源：http://ht.huixiangedu.cn

[R40] 追加写日志
来源：http://yw.szsharing.cn

echo "log" >> out.log
来源：http://rx.shxzskj.cn

[R41] 丢弃输出
来源：http://cr.nszjky.cn

cmd >/dev/null 2>&1
来源：http://eg.huixinmuqiang.cn

[R42] 输入重定向
来源：http://yq.nicolike.cn

wc -l < a.txt
来源：http://bm.yuexingan06.cn

[R43] 按名字查找文件
来源：http://cj.jctech888.com.cn

find . -name "*.log" -type f
来源：http://aa.huixiangedu.cn

[R44] 按修改时间查找
来源：http://zz.hahajie.cn

find . -mtime -7 -type f
来源：http://ei.huanxung.cn

[R45] 批量删除
来源：http://jl.szsharing.cn

find . -name "*.tmp" -delete
来源：http://lc.colortex.cn

[R46] 递归替换文件内容
来源：http://hp.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fw.shxzskj.cn

[R47] sed 单行替换
来源：http://hs.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bx.yuexingan06.cn

[R48] awk 取指定列
来源：http://xa.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://ey.shxzukj.cn

[R49] awk 带条件
来源：http://xz.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hf.bjjhwx.cn

[R50] awk 求和
来源：http://dh.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cj.nszjky.cn

[R51] 排序去重取前几
来源：http://wj.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tp.muxihuayi.cn

[R52] 统计行数
来源：http://fi.shxzskj.cn

wc -l a.txt
来源：http://jt.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://rs.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sv.huixiangedu.cn

[R54] 比较两个文件
来源：http://oe.haigaiapp.cn

diff a.txt b.txt
来源：http://xl.szsharing.cn

[R55] 压缩与解压
来源：http://og.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ay.szsharing.cn

[R56] 远程拷贝
来源：http://hx.wgjwhj.cn

scp file user@host:/path/
来源：http://yf.colortex.cn

[R57] 远程执行命令
来源：http://bl.shtwfgs.cn

ssh user@host 'uptime'
来源：http://ee.hahajie.cn

[R58] 下载文件
来源：http://gb.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ek.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://ia.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hc.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://bl.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ep.haigaiapp.cn

[R61] 磁盘占用
来源：http://oq.jctech888.com.cn

df -h;  du -sh *
来源：http://tv.gzmigu.cn

[R62] 找最占空间的文件
来源：http://mc.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://ln.shtwfgs.cn

[R63] 内存与进程
来源：http://nr.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://he.muxihuayi.cn

[R64] 结束进程
来源：http://gq.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://kq.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://qn.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gx.nszjky.cn

[R66] 定时任务
来源：http://jp.haigaiapp.cn

crontab -e;  crontab -l
来源：http://gk.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://wx.colortex.cn

openssl rand -hex 16
来源：http://lj.gzmigu.cn

[R68] 计算文件校验值
来源：http://ay.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jl.asd995.cn

[R69] 生成随机密码
来源：http://ms.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://ch.521024.cn

[R70] 时间戳与互转
来源：http://kg.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://fv.hahajie.cn

[R71] 日期格式化
来源：http://nu.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dr.521024.cn

[R72] 等待端口就绪
来源：http://ct.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xf.hahajie.cn

[R73] 分割大日志
来源：http://al.9csxet.cn

split -l 1000 big.log part_
来源：http://xo.yuntaijiaju.cn

[R74] 批量重命名
来源：http://vz.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sv.gzmigu.cn

[R75] 导出环境变量
来源：http://gw.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://ut.muxihuayi.cn

[R76] 使用临时文件
来源：http://dm.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bc.szsharing.cn

[R77] 读取用户输入
来源：http://cy.huixiangedu.cn

read -rp "请输入: " ans
来源：http://mo.nicolike.cn

[R78] 交互式菜单
来源：http://mh.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pz.colortex.cn

[R79] 解析命令行选项
来源：http://sr.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pw.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://ok.bookmarksfly.cn

time ./run.sh
来源：http://dg.huixinmuqiang.cn

================================================================================
来源：http://xr.huixinmuqiang.cn

S. C / C++ 专题
来源：http://ge.chemitech.net.cn

================================================================================
来源：http://mi.colortex.cn

[S01] C：Hello World
来源：http://wq.bjjhwx.cn

#include <stdio.h>
来源：http://cw.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://un.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://ek.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://fj.shxzukj.cn

[S03] C：读入整数
来源：http://ws.nicolike.cn

int x; scanf("%d", &x);
来源：http://eu.chemitech.net.cn

[S04] C：字符串复制
来源：http://tn.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kk.wgjwhj.cn

[S05] C：字符串长度
来源：http://pn.muxihuayi.cn

strlen(s)
来源：http://bq.colortex.cn

[S06] C：字符串比较
来源：http://rg.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://ry.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://mg.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://be.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://tx.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qn.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://rj.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ti.wgjwhj.cn

[S10] C：指针与解引用
来源：http://pw.hahajie.cn

int *p = &a;  *p = 5;
来源：http://at.bjjhwx.cn

[S11] C：逐行读文件
来源：http://qq.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://kq.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hk.szxytkj.cn

fclose(f);
来源：http://uy.shtwfgs.cn

[S12] C：写文件
来源：http://su.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ak.chemitech.net.cn

[S13] C：宏定义
来源：http://jk.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bk.bjjhwx.cn

[S14] C：枚举
来源：http://zb.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://fr.shxzukj.cn

[S15] C：类型转换
来源：http://fd.hahajie.cn

(double) a / b
来源：http://lr.nicolike.cn

[S16] C：位操作置位
来源：http://du.szxytkj.cn

x |= (1 << 3);
来源：http://pm.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://ub.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kt.hnjuh.cn

[S18] C：命令行参数
来源：http://pc.huixiangedu.cn

int main(int argc, char **argv)
来源：http://fe.jianghongdianzi.cn

[S19] C：快速排序
来源：http://mo.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jx.nicolike.cn

[S20] C：二分查找
来源：http://pj.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qi.colortex.cn

[S21] C：字符类别判断
来源：http://aj.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nu.nicolike.cn

[S22] C：字符串转数字
来源：http://yx.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://if.yuntaijiaju.cn

[S23] C：随机数
来源：http://zw.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://db.yuexingan06.cn

[S24] C：获取本地时间
来源：http://ks.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yp.wgjwhj.cn

[S25] C：内存拷贝
来源：http://pr.bjjhwx.cn

memcpy(dst, src, n);
来源：http://uv.szxytkj.cn

[S26] C：内存清零
来源：http://pr.hahajie.cn

memset(a, 0, sizeof a);
来源：http://uy.wgjwhj.cn

[S27] C：定义常量
来源：http://ie.nszjky.cn

const double PI = 3.14159;
来源：http://hm.szxytkj.cn

[S28] C：静态变量
来源：http://ae.wgjwhj.cn

static int counter = 0;
来源：http://qp.chemitech.net.cn

[S29] C：变参函数
来源：http://pf.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fc.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://dr.521024.cn

#ifndef X_H
来源：http://je.huixiangedu.cn

#define X_H
来源：http://uv.521024.cn

#endif
来源：http://qf.bjjhwx.cn

[S31] C++：Hello World
来源：http://bv.szxytkj.cn

#include <iostream>
来源：http://rt.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://nt.huixiangedu.cn

[S32] C++：字符串
来源：http://rp.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://bh.newstarts.cn

[S33] C++：vector 增删
来源：http://at.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yk.asd995.cn

[S34] C++：遍历 vector
来源：http://yq.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://eq.hahajie.cn

[S35] C++：map
来源：http://cg.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oh.gzmigu.cn

[S36] C++：unordered_map
来源：http://cy.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ed.lnxyls.cn

[S37] C++：set
来源：http://eq.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kc.521024.cn

[S38] C++：排序
来源：http://yr.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://ty.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://xj.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://my.9csxet.cn

[S40] C++：查找元素
来源：http://ep.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rh.panjiajie.cn

[S41] C++：类与构造函数
来源：http://tk.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yr.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://sj.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://hv.yuexingan06.cn


<!-- 参考信息 -->