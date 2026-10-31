代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rw.521024.cn

[Q75] 日期格式化
来源：http://jh.szsharing.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://se.jianghongdianzi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zg.bookmarksfly.cn

[Q76] 按天统计
来源：http://ng.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pl.yuexingan06.cn

[Q77] 时间加减
来源：http://wp.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vi.asd995.cn

[Q78] 当前时间
来源：http://rx.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://al.szsharing.cn

[Q79] 字符串拼接
来源：http://gh.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nj.shxzukj.cn

[Q80] 字符串截取
来源：http://jy.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iz.panjiajie.cn

[Q81] 字符串替换
来源：http://zc.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yu.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://zk.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wv.hahajie.cn

[Q83] 大小写转换
来源：http://vi.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://va.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://zv.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://pa.gzmigu.cn

[Q85] 数值取整
来源：http://bb.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tz.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://an.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ft.9csxet.cn

[Q87] JSON 字段做条件
来源：http://sv.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qd.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://gp.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zy.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jw.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://pu.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zx.9csxet.cn

[Q90] 生成序号列
来源：http://da.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pl.shxzukj.cn

================================================================================
来源：http://fw.szxytkj.cn

R. Bash 专题
来源：http://bd.colortex.cn

================================================================================
来源：http://rd.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://du.panjiajie.cn

#!/usr/bin/env bash
来源：http://zf.jianghongdianzi.cn

set -euo pipefail
来源：http://gg.szsharing.cn

[R02] 变量赋值与使用
来源：http://ji.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://fc.nszjky.cn

[R03] 只读变量
来源：http://pi.shxzukj.cn

readonly PI=3.14
来源：http://nm.yuexingan06.cn

[R04] 位置参数
来源：http://mm.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qf.gzmigu.cn

[R05] 参数默认值
来源：http://rq.hnjuh.cn

name="${1:-default}"
来源：http://bg.nicolike.cn

[R06] 判断命令是否存在
来源：http://uq.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ql.jctech888.com.cn

[R07] if 判断文件
来源：http://pl.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://la.jctech888.com.cn

[R08] 数值比较
来源：http://ah.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sg.haigaiapp.cn

[R09] 字符串比较
来源：http://ix.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qo.bookmarksfly.cn

[R10] 正则匹配
来源：http://yc.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zt.panjiajie.cn

[R11] case 多分支
来源：http://br.muxihuayi.cn

case "$1" in
来源：http://dc.bjjhwx.cn

start) echo "启动" ;;
来源：http://jz.hnjuh.cn

stop)  echo "停止" ;;
来源：http://xa.colortex.cn

*)     echo "未知命令" ;;
来源：http://lo.hahajie.cn

esac
来源：http://gm.hnjuh.cn

[R12] for 遍历文件
来源：http://hk.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://si.jctech888.com.cn

[R13] for 计数循环
来源：http://ta.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://sa.jianghongdianzi.cn

[R14] C 风格 for
来源：http://fn.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iv.shxzskj.cn

[R15] while 逐行读文件
来源：http://sq.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kc.nicolike.cn

[R16] until 等待条件
来源：http://tp.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ir.muxihuayi.cn

[R17] 数组定义与取值
来源：http://my.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oq.asd995.cn

[R18] 遍历数组
来源：http://gu.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uj.colortex.cn

[R19] 数组长度
来源：http://yj.shtwfgs.cn

echo "${#arr[@]}"
来源：http://cp.hahajie.cn

[R20] 关联数组（字典）
来源：http://va.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cc.yuntaijiaju.cn

[R21] 字符串长度
来源：http://cy.muxihuayi.cn

echo "${#s}"
来源：http://zt.hnjuh.cn

[R22] 截取子串
来源：http://ob.shxzskj.cn

echo "${s:0:5}"
来源：http://wj.szsharing.cn

[R23] 字符串替换
来源：http://wo.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ij.lnxyls.cn

[R24] 大小写转换
来源：http://io.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fz.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://va.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pg.gzmigu.cn

[R26] 命令替换
来源：http://rl.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://it.yuexingan06.cn

[R27] 算术展开
来源：http://vl.521024.cn

echo $((1 + 2 * 3))
来源：http://ny.shtwfgs.cn

[R28] 浮点运算
来源：http://kz.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://nx.jianghongdianzi.cn

[R29] 定义函数
来源：http://qp.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://se.hnjuh.cn

[R30] 函数返回状态码
来源：http://mc.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://fi.yuexingan06.cn

[R31] 局部变量
来源：http://oh.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://uo.nszjky.cn

[R32] 参数个数校验
来源：http://ha.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dc.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://fm.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cm.nicolike.cn

[R34] 退出时清理
来源：http://dd.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wi.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://lr.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dx.shxzukj.cn

[R36] 并发执行多个任务
来源：http://fu.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wb.521024.cn

[R37] 把输出赋给变量
来源：http://zm.huixiangedu.cn

files=$(ls -1)
来源：http://hc.nszjky.cn

[R38] 管道串联
来源：http://jg.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://jd.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://cn.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://hv.yuexingan06.cn

[R40] 追加写日志
来源：http://eo.muxihuayi.cn

echo "log" >> out.log
来源：http://mj.bookmarksfly.cn

[R41] 丢弃输出
来源：http://rm.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://tv.yuexingan06.cn

[R42] 输入重定向
来源：http://gd.yuntaijiaju.cn

wc -l < a.txt
来源：http://cg.gzmigu.cn

[R43] 按名字查找文件
来源：http://kp.shxzukj.cn

find . -name "*.log" -type f
来源：http://yv.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://jo.shxzskj.cn

find . -mtime -7 -type f
来源：http://eh.bookmarksfly.cn

[R45] 批量删除
来源：http://ks.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://hx.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://ac.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xx.jctech888.com.cn

[R47] sed 单行替换
来源：http://lb.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ix.szxytkj.cn

[R48] awk 取指定列
来源：http://jv.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://fy.huanxung.cn

[R49] awk 带条件
来源：http://pv.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jm.haigaiapp.cn

[R50] awk 求和
来源：http://po.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qf.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://ot.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://px.panjiajie.cn

[R52] 统计行数
来源：http://vd.yuntaijiaju.cn

wc -l a.txt
来源：http://qt.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://yo.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mx.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://my.newstarts.cn

diff a.txt b.txt
来源：http://fv.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://jb.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://of.lnxyls.cn

[R56] 远程拷贝
来源：http://oy.chemitech.net.cn

scp file user@host:/path/
来源：http://kh.lnxyls.cn

[R57] 远程执行命令
来源：http://my.shtwfgs.cn

ssh user@host 'uptime'
来源：http://gg.hahajie.cn

[R58] 下载文件
来源：http://dm.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xu.panjiajie.cn

[R59] 发 POST JSON
来源：http://xm.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tr.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://rm.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fw.szsharing.cn

[R61] 磁盘占用
来源：http://jw.shxzskj.cn

df -h;  du -sh *
来源：http://ri.colortex.cn

[R62] 找最占空间的文件
来源：http://vp.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://fd.huanxung.cn

[R63] 内存与进程
来源：http://lu.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://ct.shxzskj.cn

[R64] 结束进程
来源：http://hl.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://bx.huanxung.cn

[R65] 查看端口占用
来源：http://dx.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gi.nszjky.cn

[R66] 定时任务
来源：http://hp.jctech888.com.cn

crontab -e;  crontab -l
来源：http://yo.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://eq.huanxung.cn

openssl rand -hex 16
来源：http://zi.panjiajie.cn

[R68] 计算文件校验值
来源：http://fs.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rq.szxytkj.cn

[R69] 生成随机密码
来源：http://qz.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://wp.nszjky.cn

[R70] 时间戳与互转
来源：http://tw.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://xm.chemitech.net.cn

[R71] 日期格式化
来源：http://zt.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://iu.gzmigu.cn

[R72] 等待端口就绪
来源：http://rp.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lh.szxytkj.cn

[R73] 分割大日志
来源：http://ow.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://de.chemitech.net.cn

[R74] 批量重命名
来源：http://xo.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://og.9csxet.cn

[R75] 导出环境变量
来源：http://wv.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://ql.hnjuh.cn

[R76] 使用临时文件
来源：http://qr.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qb.bookmarksfly.cn

[R77] 读取用户输入
来源：http://ob.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://tk.muxihuayi.cn

[R78] 交互式菜单
来源：http://mv.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xl.haigaiapp.cn

[R79] 解析命令行选项
来源：http://pv.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wb.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://ra.szxytkj.cn

time ./run.sh
来源：http://ct.shtwfgs.cn

================================================================================
来源：http://uy.521024.cn

S. C / C++ 专题
来源：http://sw.shxzskj.cn

================================================================================
来源：http://vn.szxytkj.cn

[S01] C：Hello World
来源：http://pm.jianghongdianzi.cn

#include <stdio.h>
来源：http://lt.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yp.colortex.cn

[S02] C：变量与格式化输出
来源：http://ja.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://pn.hnjuh.cn

[S03] C：读入整数
来源：http://tb.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://eb.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://ra.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ij.newstarts.cn

[S05] C：字符串长度
来源：http://sf.521024.cn

strlen(s)
来源：http://ih.gzmigu.cn

[S06] C：字符串比较
来源：http://xv.asd995.cn

strcmp(a, b) == 0
来源：http://lc.huanxung.cn

[S07] C：数组遍历求和
来源：http://lr.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gz.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://lq.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pb.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://ia.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rd.yuexingan06.cn

[S10] C：指针与解引用
来源：http://tb.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://jo.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://jg.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://sr.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fa.9csxet.cn

fclose(f);
来源：http://zr.asd995.cn

[S12] C：写文件
来源：http://ai.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mo.bookmarksfly.cn

[S13] C：宏定义
来源：http://fl.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://em.haigaiapp.cn

[S14] C：枚举
来源：http://gz.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://pb.gzmigu.cn

[S15] C：类型转换
来源：http://dc.huixinmuqiang.cn

(double) a / b
来源：http://nf.nszjky.cn

[S16] C：位操作置位
来源：http://tk.gzmigu.cn

x |= (1 << 3);
来源：http://kk.colortex.cn

[S17] C：安全拼接字符串
来源：http://kc.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ni.9csxet.cn

[S18] C：命令行参数
来源：http://ax.hnjuh.cn

int main(int argc, char **argv)
来源：http://gx.hnjuh.cn

[S19] C：快速排序
来源：http://zg.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ct.wgjwhj.cn

[S20] C：二分查找
来源：http://vc.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gw.shxzukj.cn

[S21] C：字符类别判断
来源：http://hd.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ks.nszjky.cn

[S22] C：字符串转数字
来源：http://ty.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nz.lnxyls.cn

[S23] C：随机数
来源：http://to.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nw.9csxet.cn

[S24] C：获取本地时间
来源：http://pz.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mc.asd995.cn

[S25] C：内存拷贝
来源：http://sa.szxytkj.cn

memcpy(dst, src, n);
来源：http://hm.asd995.cn

[S26] C：内存清零
来源：http://ez.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://nd.huanxung.cn

[S27] C：定义常量
来源：http://kg.wgjwhj.cn

const double PI = 3.14159;
来源：http://kf.huixiangedu.cn

[S28] C：静态变量
来源：http://jn.bookmarksfly.cn

static int counter = 0;
来源：http://gc.jianghongdianzi.cn

[S29] C：变参函数
来源：http://vt.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://me.shxzskj.cn

[S30] C：头文件保护
来源：http://ap.muxihuayi.cn

#ifndef X_H
来源：http://rl.huanxung.cn

#define X_H
来源：http://yo.yuntaijiaju.cn

#endif
来源：http://ap.lnxyls.cn

[S31] C++：Hello World
来源：http://ax.9csxet.cn

#include <iostream>
来源：http://gw.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://dn.szxytkj.cn

[S32] C++：字符串
来源：http://jf.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://oz.hahajie.cn

[S33] C++：vector 增删
来源：http://cr.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yr.panjiajie.cn

[S34] C++：遍历 vector
来源：http://ai.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://mo.huixinmuqiang.cn

[S35] C++：map
来源：http://vj.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mi.9csxet.cn

[S36] C++：unordered_map
来源：http://li.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fo.haigaiapp.cn

[S37] C++：set
来源：http://tt.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vs.jctech888.com.cn

[S38] C++：排序
来源：http://yx.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://qc.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://rd.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yp.521024.cn

[S40] C++：查找元素
来源：http://ll.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kh.szxytkj.cn

[S41] C++：类与构造函数
来源：http://xc.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pc.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://xw.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://lo.yuexingan06.cn

[S43] C++：智能指针
来源：http://hv.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://mi.huanxung.cn

[S44] C++：引用传参
来源：http://oo.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://wk.yuexingan06.cn


<!-- 参考信息 -->