代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ic.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://ey.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zr.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nc.jianghongdianzi.cn

[Q76] 按天统计
来源：http://gl.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lo.nicolike.cn

[Q77] 时间加减
来源：http://xs.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oq.szxytkj.cn

[Q78] 当前时间
来源：http://pp.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ds.nszjky.cn

[Q79] 字符串拼接
来源：http://sr.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nt.asd995.cn

[Q80] 字符串截取
来源：http://ka.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qv.shxzskj.cn

[Q81] 字符串替换
来源：http://ce.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wx.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://df.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gd.shxzskj.cn

[Q83] 大小写转换
来源：http://gy.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lm.szsharing.cn

[Q84] 去除首尾空格
来源：http://yq.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://hi.bjjhwx.cn

[Q85] 数值取整
来源：http://yg.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jf.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://he.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lf.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://qu.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wu.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://kd.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eh.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aq.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://pp.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bn.shtwfgs.cn

[Q90] 生成序号列
来源：http://jk.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oh.muxihuayi.cn

================================================================================
来源：http://xk.nicolike.cn

R. Bash 专题
来源：http://ur.huanxung.cn

================================================================================
来源：http://fb.nicolike.cn

[R01] shebang 与严格模式
来源：http://nt.nicolike.cn

#!/usr/bin/env bash
来源：http://qp.gzmigu.cn

set -euo pipefail
来源：http://se.hahajie.cn

[R02] 变量赋值与使用
来源：http://rr.szxytkj.cn

name="Tom"; echo "$name"
来源：http://na.szsharing.cn

[R03] 只读变量
来源：http://fk.huixiangedu.cn

readonly PI=3.14
来源：http://fb.521024.cn

[R04] 位置参数
来源：http://en.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://is.yuntaijiaju.cn

[R05] 参数默认值
来源：http://hw.chemitech.net.cn

name="${1:-default}"
来源：http://kx.521024.cn

[R06] 判断命令是否存在
来源：http://ic.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sj.yuntaijiaju.cn

[R07] if 判断文件
来源：http://or.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vg.szxytkj.cn

[R08] 数值比较
来源：http://mi.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lf.shxzukj.cn

[R09] 字符串比较
来源：http://yp.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hj.yuexingan06.cn

[R10] 正则匹配
来源：http://fz.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gq.bjjhwx.cn

[R11] case 多分支
来源：http://nw.chemitech.net.cn

case "$1" in
来源：http://kv.nicolike.cn

start) echo "启动" ;;
来源：http://tm.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://uv.huanxung.cn

*)     echo "未知命令" ;;
来源：http://ht.shxzukj.cn

esac
来源：http://wh.521024.cn

[R12] for 遍历文件
来源：http://xg.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://qr.shxzukj.cn

[R13] for 计数循环
来源：http://ao.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://ps.nicolike.cn

[R14] C 风格 for
来源：http://kb.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vw.haigaiapp.cn

[R15] while 逐行读文件
来源：http://ly.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kc.hahajie.cn

[R16] until 等待条件
来源：http://zz.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ew.panjiajie.cn

[R17] 数组定义与取值
来源：http://hm.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oz.gzmigu.cn

[R18] 遍历数组
来源：http://sf.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qp.bookmarksfly.cn

[R19] 数组长度
来源：http://tz.shtwfgs.cn

echo "${#arr[@]}"
来源：http://lz.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://kv.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wi.muxihuayi.cn

[R21] 字符串长度
来源：http://he.haigaiapp.cn

echo "${#s}"
来源：http://gb.lnxyls.cn

[R22] 截取子串
来源：http://yl.521024.cn

echo "${s:0:5}"
来源：http://cu.asd995.cn

[R23] 字符串替换
来源：http://yg.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bj.szsharing.cn

[R24] 大小写转换
来源：http://dt.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kr.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://oc.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zi.huanxung.cn

[R26] 命令替换
来源：http://db.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://yz.shxzukj.cn

[R27] 算术展开
来源：http://pl.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://dj.muxihuayi.cn

[R28] 浮点运算
来源：http://us.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://qn.gzmigu.cn

[R29] 定义函数
来源：http://lt.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://em.colortex.cn

[R30] 函数返回状态码
来源：http://jp.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://ts.newstarts.cn

[R31] 局部变量
来源：http://bc.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://vv.nszjky.cn

[R32] 参数个数校验
来源：http://st.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zv.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://zh.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xu.asd995.cn

[R34] 退出时清理
来源：http://ag.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ko.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://iu.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tu.521024.cn

[R36] 并发执行多个任务
来源：http://xn.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xs.hahajie.cn

[R37] 把输出赋给变量
来源：http://hq.shxzskj.cn

files=$(ls -1)
来源：http://qh.haigaiapp.cn

[R38] 管道串联
来源：http://uk.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://je.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://an.asd995.cn

cmd > out.log 2>&1
来源：http://jp.haigaiapp.cn

[R40] 追加写日志
来源：http://ia.shxzskj.cn

echo "log" >> out.log
来源：http://cz.gzmigu.cn

[R41] 丢弃输出
来源：http://gg.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://af.bookmarksfly.cn

[R42] 输入重定向
来源：http://ml.colortex.cn

wc -l < a.txt
来源：http://fu.chemitech.net.cn

[R43] 按名字查找文件
来源：http://pb.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://nd.panjiajie.cn

[R44] 按修改时间查找
来源：http://pn.chemitech.net.cn

find . -mtime -7 -type f
来源：http://is.huanxung.cn

[R45] 批量删除
来源：http://so.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://ug.9csxet.cn

[R46] 递归替换文件内容
来源：http://xg.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gp.gzmigu.cn

[R47] sed 单行替换
来源：http://pp.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mo.hnjuh.cn

[R48] awk 取指定列
来源：http://zs.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://ag.521024.cn

[R49] awk 带条件
来源：http://ol.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mo.haigaiapp.cn

[R50] awk 求和
来源：http://ul.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gb.lnxyls.cn

[R51] 排序去重取前几
来源：http://dt.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://et.yuntaijiaju.cn

[R52] 统计行数
来源：http://ej.panjiajie.cn

wc -l a.txt
来源：http://bc.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://pn.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jc.muxihuayi.cn

[R54] 比较两个文件
来源：http://cr.chemitech.net.cn

diff a.txt b.txt
来源：http://yx.bjjhwx.cn

[R55] 压缩与解压
来源：http://dn.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bd.521024.cn

[R56] 远程拷贝
来源：http://uf.asd995.cn

scp file user@host:/path/
来源：http://az.shtwfgs.cn

[R57] 远程执行命令
来源：http://sf.hnjuh.cn

ssh user@host 'uptime'
来源：http://qd.hahajie.cn

[R58] 下载文件
来源：http://ie.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kj.nicolike.cn

[R59] 发 POST JSON
来源：http://mv.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eo.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://qt.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hp.shxzskj.cn

[R61] 磁盘占用
来源：http://ry.jianghongdianzi.cn

df -h;  du -sh *
来源：http://ho.huanxung.cn

[R62] 找最占空间的文件
来源：http://pe.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://ps.newstarts.cn

[R63] 内存与进程
来源：http://da.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://lv.lnxyls.cn

[R64] 结束进程
来源：http://nz.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://hq.panjiajie.cn

[R65] 查看端口占用
来源：http://ot.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gb.nszjky.cn

[R66] 定时任务
来源：http://st.nszjky.cn

crontab -e;  crontab -l
来源：http://fp.szsharing.cn

[R67] 生成随机十六进制串
来源：http://ff.asd995.cn

openssl rand -hex 16
来源：http://rg.muxihuayi.cn

[R68] 计算文件校验值
来源：http://tb.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lr.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://mo.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://ul.9csxet.cn

[R70] 时间戳与互转
来源：http://sz.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://qm.shtwfgs.cn

[R71] 日期格式化
来源：http://it.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zo.szsharing.cn

[R72] 等待端口就绪
来源：http://vk.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oa.huixinmuqiang.cn

[R73] 分割大日志
来源：http://uy.lnxyls.cn

split -l 1000 big.log part_
来源：http://kz.panjiajie.cn

[R74] 批量重命名
来源：http://hw.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pk.gzmigu.cn

[R75] 导出环境变量
来源：http://hy.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://lx.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://vk.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mh.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://vo.hnjuh.cn

read -rp "请输入: " ans
来源：http://ql.wgjwhj.cn

[R78] 交互式菜单
来源：http://fc.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ye.szsharing.cn

[R79] 解析命令行选项
来源：http://dl.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tt.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://ks.szxytkj.cn

time ./run.sh
来源：http://ax.lnxyls.cn

================================================================================
来源：http://ac.szxytkj.cn

S. C / C++ 专题
来源：http://ok.huixinmuqiang.cn

================================================================================
来源：http://iq.bookmarksfly.cn

[S01] C：Hello World
来源：http://al.bjjhwx.cn

#include <stdio.h>
来源：http://td.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lm.newstarts.cn

[S02] C：变量与格式化输出
来源：http://dr.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://yb.shxzskj.cn

[S03] C：读入整数
来源：http://fw.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://xw.bookmarksfly.cn

[S04] C：字符串复制
来源：http://yw.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rv.hnjuh.cn

[S05] C：字符串长度
来源：http://uu.colortex.cn

strlen(s)
来源：http://pi.jctech888.com.cn

[S06] C：字符串比较
来源：http://hx.wgjwhj.cn

strcmp(a, b) == 0
来源：http://xm.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://qp.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lr.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://gw.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ob.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://gb.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nc.panjiajie.cn

[S10] C：指针与解引用
来源：http://sy.huanxung.cn

int *p = &a;  *p = 5;
来源：http://ev.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://gr.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://if.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ke.nicolike.cn

fclose(f);
来源：http://cj.bjjhwx.cn

[S12] C：写文件
来源：http://gy.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lt.yuexingan06.cn

[S13] C：宏定义
来源：http://xr.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ed.szxytkj.cn

[S14] C：枚举
来源：http://zz.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://vj.nszjky.cn

[S15] C：类型转换
来源：http://xs.521024.cn

(double) a / b
来源：http://sa.shxzskj.cn

[S16] C：位操作置位
来源：http://hy.szsharing.cn

x |= (1 << 3);
来源：http://um.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://xf.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xo.lnxyls.cn

[S18] C：命令行参数
来源：http://po.lnxyls.cn

int main(int argc, char **argv)
来源：http://yf.muxihuayi.cn

[S19] C：快速排序
来源：http://dj.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://un.bjjhwx.cn

[S20] C：二分查找
来源：http://ru.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://om.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://co.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yo.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://wx.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eu.bjjhwx.cn

[S23] C：随机数
来源：http://rf.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ku.hahajie.cn

[S24] C：获取本地时间
来源：http://dj.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ba.bjjhwx.cn

[S25] C：内存拷贝
来源：http://yf.nicolike.cn

memcpy(dst, src, n);
来源：http://jj.jctech888.com.cn

[S26] C：内存清零
来源：http://ss.hahajie.cn

memset(a, 0, sizeof a);
来源：http://lw.muxihuayi.cn

[S27] C：定义常量
来源：http://gv.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://dy.hnjuh.cn

[S28] C：静态变量
来源：http://ne.szsharing.cn

static int counter = 0;
来源：http://ku.jianghongdianzi.cn

[S29] C：变参函数
来源：http://mz.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sy.panjiajie.cn

[S30] C：头文件保护
来源：http://oh.gzmigu.cn

#ifndef X_H
来源：http://ct.jctech888.com.cn

#define X_H
来源：http://pz.huixinmuqiang.cn

#endif
来源：http://zb.nszjky.cn

[S31] C++：Hello World
来源：http://sx.shxzskj.cn

#include <iostream>
来源：http://ri.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://rl.gzmigu.cn

[S32] C++：字符串
来源：http://qn.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://qa.wgjwhj.cn

[S33] C++：vector 增删
来源：http://kd.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iq.hahajie.cn

[S34] C++：遍历 vector
来源：http://ar.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://jt.szxytkj.cn

[S35] C++：map
来源：http://cl.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ea.szxytkj.cn

[S36] C++：unordered_map
来源：http://rz.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sv.asd995.cn

[S37] C++：set
来源：http://zd.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tv.huixiangedu.cn

[S38] C++：排序
来源：http://xi.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://ea.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://rd.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://je.colortex.cn

[S40] C++：查找元素
来源：http://eb.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eg.shxzskj.cn

[S41] C++：类与构造函数
来源：http://xy.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ic.9csxet.cn

[S42] C++：继承与虚函数
来源：http://fg.521024.cn

class B : public Base { public: void f() override {} };
来源：http://zw.hnjuh.cn

[S43] C++：智能指针
来源：http://ji.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://wy.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://jc.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://gw.bookmarksfly.cn


<!-- 参考信息 -->