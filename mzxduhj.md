代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pe.shtwfgs.cn

[Q75] 日期格式化
来源：http://xp.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jl.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kh.yuexingan06.cn

[Q76] 按天统计
来源：http://wc.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cz.jianghongdianzi.cn

[Q77] 时间加减
来源：http://ra.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hn.nicolike.cn

[Q78] 当前时间
来源：http://al.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dq.nszjky.cn

[Q79] 字符串拼接
来源：http://dl.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xz.9csxet.cn

[Q80] 字符串截取
来源：http://ks.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cm.haigaiapp.cn

[Q81] 字符串替换
来源：http://dz.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sb.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://cb.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sh.wgjwhj.cn

[Q83] 大小写转换
来源：http://sb.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pd.panjiajie.cn

[Q84] 去除首尾空格
来源：http://in.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://sx.huixiangedu.cn

[Q85] 数值取整
来源：http://xl.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jl.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://zk.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nk.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://kt.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bd.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://tz.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bu.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dl.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://fs.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ey.shxzskj.cn

[Q90] 生成序号列
来源：http://bt.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fm.hahajie.cn

================================================================================
来源：http://cc.bookmarksfly.cn

R. Bash 专题
来源：http://wd.wgjwhj.cn

================================================================================
来源：http://qc.9csxet.cn

[R01] shebang 与严格模式
来源：http://ed.colortex.cn

#!/usr/bin/env bash
来源：http://dn.shxzskj.cn

set -euo pipefail
来源：http://xe.szxytkj.cn

[R02] 变量赋值与使用
来源：http://fs.shxzukj.cn

name="Tom"; echo "$name"
来源：http://vt.bookmarksfly.cn

[R03] 只读变量
来源：http://hc.muxihuayi.cn

readonly PI=3.14
来源：http://yx.panjiajie.cn

[R04] 位置参数
来源：http://vh.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ad.wgjwhj.cn

[R05] 参数默认值
来源：http://do.nicolike.cn

name="${1:-default}"
来源：http://aj.lnxyls.cn

[R06] 判断命令是否存在
来源：http://dd.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://az.521024.cn

[R07] if 判断文件
来源：http://gx.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ng.haigaiapp.cn

[R08] 数值比较
来源：http://wf.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rw.colortex.cn

[R09] 字符串比较
来源：http://bk.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oa.shxzskj.cn

[R10] 正则匹配
来源：http://gh.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bi.shxzskj.cn

[R11] case 多分支
来源：http://ga.gzmigu.cn

case "$1" in
来源：http://no.gzmigu.cn

start) echo "启动" ;;
来源：http://il.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://oj.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://ry.haigaiapp.cn

esac
来源：http://xv.shxzukj.cn

[R12] for 遍历文件
来源：http://nl.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://rk.bookmarksfly.cn

[R13] for 计数循环
来源：http://jl.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://sz.gzmigu.cn

[R14] C 风格 for
来源：http://qe.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lf.9csxet.cn

[R15] while 逐行读文件
来源：http://xz.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://br.hahajie.cn

[R16] until 等待条件
来源：http://jl.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ar.muxihuayi.cn

[R17] 数组定义与取值
来源：http://bd.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hy.newstarts.cn

[R18] 遍历数组
来源：http://mt.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oj.chemitech.net.cn

[R19] 数组长度
来源：http://jn.yuexingan06.cn

echo "${#arr[@]}"
来源：http://mo.colortex.cn

[R20] 关联数组（字典）
来源：http://li.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ww.szxytkj.cn

[R21] 字符串长度
来源：http://dg.huixiangedu.cn

echo "${#s}"
来源：http://hu.szxytkj.cn

[R22] 截取子串
来源：http://yo.nicolike.cn

echo "${s:0:5}"
来源：http://qs.szxytkj.cn

[R23] 字符串替换
来源：http://do.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ju.bjjhwx.cn

[R24] 大小写转换
来源：http://dq.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jj.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://bc.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://et.szxytkj.cn

[R26] 命令替换
来源：http://rq.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://qi.szsharing.cn

[R27] 算术展开
来源：http://ly.521024.cn

echo $((1 + 2 * 3))
来源：http://yv.9csxet.cn

[R28] 浮点运算
来源：http://ri.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://sc.chemitech.net.cn

[R29] 定义函数
来源：http://un.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nv.szxytkj.cn

[R30] 函数返回状态码
来源：http://wg.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://ps.jctech888.com.cn

[R31] 局部变量
来源：http://zx.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://nm.lnxyls.cn

[R32] 参数个数校验
来源：http://nu.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fr.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://vp.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rm.haigaiapp.cn

[R34] 退出时清理
来源：http://ln.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ef.shxzukj.cn

[R35] 后台执行并等待
来源：http://fs.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gq.shxzskj.cn

[R36] 并发执行多个任务
来源：http://wk.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eu.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://aw.nicolike.cn

files=$(ls -1)
来源：http://ko.szsharing.cn

[R38] 管道串联
来源：http://uj.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://gf.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://cz.wgjwhj.cn

cmd > out.log 2>&1
来源：http://uf.jctech888.com.cn

[R40] 追加写日志
来源：http://zh.lnxyls.cn

echo "log" >> out.log
来源：http://if.gzmigu.cn

[R41] 丢弃输出
来源：http://zl.9csxet.cn

cmd >/dev/null 2>&1
来源：http://si.hnjuh.cn

[R42] 输入重定向
来源：http://et.bookmarksfly.cn

wc -l < a.txt
来源：http://cv.9csxet.cn

[R43] 按名字查找文件
来源：http://qu.jctech888.com.cn

find . -name "*.log" -type f
来源：http://zo.bjjhwx.cn

[R44] 按修改时间查找
来源：http://cp.lnxyls.cn

find . -mtime -7 -type f
来源：http://lo.jctech888.com.cn

[R45] 批量删除
来源：http://nu.9csxet.cn

find . -name "*.tmp" -delete
来源：http://to.newstarts.cn

[R46] 递归替换文件内容
来源：http://lt.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iv.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://so.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mg.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://ny.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://pg.shtwfgs.cn

[R49] awk 带条件
来源：http://oj.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eb.bjjhwx.cn

[R50] awk 求和
来源：http://vm.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vd.lnxyls.cn

[R51] 排序去重取前几
来源：http://va.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rs.9csxet.cn

[R52] 统计行数
来源：http://gs.bjjhwx.cn

wc -l a.txt
来源：http://si.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://rd.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jz.huanxung.cn

[R54] 比较两个文件
来源：http://cy.hahajie.cn

diff a.txt b.txt
来源：http://zo.jctech888.com.cn

[R55] 压缩与解压
来源：http://sb.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ee.szxytkj.cn

[R56] 远程拷贝
来源：http://kw.yuntaijiaju.cn

scp file user@host:/path/
来源：http://xu.nicolike.cn

[R57] 远程执行命令
来源：http://go.521024.cn

ssh user@host 'uptime'
来源：http://ff.nicolike.cn

[R58] 下载文件
来源：http://sx.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kg.nicolike.cn

[R59] 发 POST JSON
来源：http://te.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yb.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://bv.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cm.bookmarksfly.cn

[R61] 磁盘占用
来源：http://xu.szxytkj.cn

df -h;  du -sh *
来源：http://rt.colortex.cn

[R62] 找最占空间的文件
来源：http://gn.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://yz.asd995.cn

[R63] 内存与进程
来源：http://lu.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://ux.hahajie.cn

[R64] 结束进程
来源：http://lw.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://uk.yuexingan06.cn

[R65] 查看端口占用
来源：http://pk.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dq.9csxet.cn

[R66] 定时任务
来源：http://qg.hahajie.cn

crontab -e;  crontab -l
来源：http://zu.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://jo.panjiajie.cn

openssl rand -hex 16
来源：http://zb.nicolike.cn

[R68] 计算文件校验值
来源：http://di.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://em.huixiangedu.cn

[R69] 生成随机密码
来源：http://xe.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://li.asd995.cn

[R70] 时间戳与互转
来源：http://pd.521024.cn

date +%s;  date -d @1700000000
来源：http://fd.huixiangedu.cn

[R71] 日期格式化
来源：http://vv.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ie.haigaiapp.cn

[R72] 等待端口就绪
来源：http://pw.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rl.shxzskj.cn

[R73] 分割大日志
来源：http://am.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://hu.9csxet.cn

[R74] 批量重命名
来源：http://mg.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nz.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://vi.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://jv.huixiangedu.cn

[R76] 使用临时文件
来源：http://gw.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oq.huixiangedu.cn

[R77] 读取用户输入
来源：http://ka.haigaiapp.cn

read -rp "请输入: " ans
来源：http://ys.shtwfgs.cn

[R78] 交互式菜单
来源：http://zd.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yf.521024.cn

[R79] 解析命令行选项
来源：http://aa.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dc.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://ry.yuntaijiaju.cn

time ./run.sh
来源：http://vn.shxzukj.cn

================================================================================
来源：http://an.nicolike.cn

S. C / C++ 专题
来源：http://xr.nicolike.cn

================================================================================
来源：http://dj.szsharing.cn

[S01] C：Hello World
来源：http://ge.huanxung.cn

#include <stdio.h>
来源：http://zt.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qp.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://qf.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://ad.hahajie.cn

[S03] C：读入整数
来源：http://ml.szsharing.cn

int x; scanf("%d", &x);
来源：http://xd.asd995.cn

[S04] C：字符串复制
来源：http://gh.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://go.bjjhwx.cn

[S05] C：字符串长度
来源：http://cq.huixiangedu.cn

strlen(s)
来源：http://su.jctech888.com.cn

[S06] C：字符串比较
来源：http://vx.colortex.cn

strcmp(a, b) == 0
来源：http://uw.panjiajie.cn

[S07] C：数组遍历求和
来源：http://mp.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cu.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://hz.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://au.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://mz.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sb.gzmigu.cn

[S10] C：指针与解引用
来源：http://uu.asd995.cn

int *p = &a;  *p = 5;
来源：http://cr.chemitech.net.cn

[S11] C：逐行读文件
来源：http://cr.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://is.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ke.hahajie.cn

fclose(f);
来源：http://af.haigaiapp.cn

[S12] C：写文件
来源：http://sr.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ut.nicolike.cn

[S13] C：宏定义
来源：http://mb.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hi.huanxung.cn

[S14] C：枚举
来源：http://hz.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://jq.hnjuh.cn

[S15] C：类型转换
来源：http://by.hahajie.cn

(double) a / b
来源：http://qj.lnxyls.cn

[S16] C：位操作置位
来源：http://hd.jctech888.com.cn

x |= (1 << 3);
来源：http://je.nszjky.cn

[S17] C：安全拼接字符串
来源：http://xj.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cb.hahajie.cn

[S18] C：命令行参数
来源：http://xp.gzmigu.cn

int main(int argc, char **argv)
来源：http://ms.hnjuh.cn

[S19] C：快速排序
来源：http://lx.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ky.huixinmuqiang.cn

[S20] C：二分查找
来源：http://jg.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hc.gzmigu.cn

[S21] C：字符类别判断
来源：http://jm.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cz.nszjky.cn

[S22] C：字符串转数字
来源：http://nh.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://up.muxihuayi.cn

[S23] C：随机数
来源：http://vh.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xe.haigaiapp.cn

[S24] C：获取本地时间
来源：http://ew.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pw.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://ac.wgjwhj.cn

memcpy(dst, src, n);
来源：http://th.yuexingan06.cn

[S26] C：内存清零
来源：http://dm.colortex.cn

memset(a, 0, sizeof a);
来源：http://hh.nszjky.cn

[S27] C：定义常量
来源：http://rr.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://uq.521024.cn

[S28] C：静态变量
来源：http://ug.asd995.cn

static int counter = 0;
来源：http://tf.panjiajie.cn

[S29] C：变参函数
来源：http://pc.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dk.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://ra.bjjhwx.cn

#ifndef X_H
来源：http://up.newstarts.cn

#define X_H
来源：http://fa.9csxet.cn

#endif
来源：http://wn.chemitech.net.cn

[S31] C++：Hello World
来源：http://ob.haigaiapp.cn

#include <iostream>
来源：http://br.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://zo.szsharing.cn

[S32] C++：字符串
来源：http://nh.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://mf.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://jc.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uh.gzmigu.cn

[S34] C++：遍历 vector
来源：http://fu.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://sg.9csxet.cn

[S35] C++：map
来源：http://ij.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ja.bjjhwx.cn

[S36] C++：unordered_map
来源：http://rq.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ey.panjiajie.cn

[S37] C++：set
来源：http://bo.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xl.newstarts.cn

[S38] C++：排序
来源：http://rn.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://gb.521024.cn

[S39] C++：自定义比较器排序
来源：http://es.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fi.hahajie.cn

[S40] C++：查找元素
来源：http://kn.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cv.szxytkj.cn

[S41] C++：类与构造函数
来源：http://tx.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vx.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://ia.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://cm.huixiangedu.cn

[S43] C++：智能指针
来源：http://dx.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://xi.shxzukj.cn

[S44] C++：引用传参
来源：http://do.colortex.cn

void inc(int &x) { ++x; }
来源：http://xx.hnjuh.cn


<!-- 参考信息 -->