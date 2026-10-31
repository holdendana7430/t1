代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zd.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://fs.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bo.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://il.szxytkj.cn

[Q76] 按天统计
来源：http://bl.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cf.bookmarksfly.cn

[Q77] 时间加减
来源：http://fy.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rb.huanxung.cn

[Q78] 当前时间
来源：http://do.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fr.nicolike.cn

[Q79] 字符串拼接
来源：http://ge.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cb.521024.cn

[Q80] 字符串截取
来源：http://id.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zz.bjjhwx.cn

[Q81] 字符串替换
来源：http://wt.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rs.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://ko.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pi.szxytkj.cn

[Q83] 大小写转换
来源：http://rh.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zy.hahajie.cn

[Q84] 去除首尾空格
来源：http://vi.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://gq.shxzskj.cn

[Q85] 数值取整
来源：http://zs.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lz.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://bq.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ru.huanxung.cn

[Q87] JSON 字段做条件
来源：http://tw.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sp.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://wv.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://by.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ev.shxzukj.cn

[Q89] 判断表是否存在
来源：http://wt.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wj.panjiajie.cn

[Q90] 生成序号列
来源：http://mh.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rs.shxzukj.cn

================================================================================
来源：http://jd.shxzukj.cn

R. Bash 专题
来源：http://qd.jctech888.com.cn

================================================================================
来源：http://ac.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://wj.chemitech.net.cn

#!/usr/bin/env bash
来源：http://hw.colortex.cn

set -euo pipefail
来源：http://xb.huanxung.cn

[R02] 变量赋值与使用
来源：http://wz.newstarts.cn

name="Tom"; echo "$name"
来源：http://mr.chemitech.net.cn

[R03] 只读变量
来源：http://gu.asd995.cn

readonly PI=3.14
来源：http://lz.jianghongdianzi.cn

[R04] 位置参数
来源：http://or.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kq.hahajie.cn

[R05] 参数默认值
来源：http://ei.bjjhwx.cn

name="${1:-default}"
来源：http://pw.hahajie.cn

[R06] 判断命令是否存在
来源：http://ns.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://za.shtwfgs.cn

[R07] if 判断文件
来源：http://ma.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fb.lnxyls.cn

[R08] 数值比较
来源：http://xf.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://px.nszjky.cn

[R09] 字符串比较
来源：http://bw.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xs.szxytkj.cn

[R10] 正则匹配
来源：http://bz.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sc.newstarts.cn

[R11] case 多分支
来源：http://kx.colortex.cn

case "$1" in
来源：http://ty.9csxet.cn

start) echo "启动" ;;
来源：http://ej.521024.cn

stop)  echo "停止" ;;
来源：http://it.huanxung.cn

*)     echo "未知命令" ;;
来源：http://br.haigaiapp.cn

esac
来源：http://mz.bjjhwx.cn

[R12] for 遍历文件
来源：http://ex.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://rz.lnxyls.cn

[R13] for 计数循环
来源：http://ko.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://lv.szsharing.cn

[R14] C 风格 for
来源：http://gv.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://po.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://kc.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xl.hnjuh.cn

[R16] until 等待条件
来源：http://lm.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bc.bjjhwx.cn

[R17] 数组定义与取值
来源：http://ze.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zq.asd995.cn

[R18] 遍历数组
来源：http://rq.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ls.jianghongdianzi.cn

[R19] 数组长度
来源：http://za.bjjhwx.cn

echo "${#arr[@]}"
来源：http://ce.colortex.cn

[R20] 关联数组（字典）
来源：http://fu.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ux.chemitech.net.cn

[R21] 字符串长度
来源：http://us.yuntaijiaju.cn

echo "${#s}"
来源：http://fj.bjjhwx.cn

[R22] 截取子串
来源：http://ft.asd995.cn

echo "${s:0:5}"
来源：http://bl.huixinmuqiang.cn

[R23] 字符串替换
来源：http://ai.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cl.shxzskj.cn

[R24] 大小写转换
来源：http://uq.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bf.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://po.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oa.nicolike.cn

[R26] 命令替换
来源：http://mm.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://zl.szxytkj.cn

[R27] 算术展开
来源：http://uv.521024.cn

echo $((1 + 2 * 3))
来源：http://lt.hahajie.cn

[R28] 浮点运算
来源：http://ex.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://ue.hahajie.cn

[R29] 定义函数
来源：http://cc.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kg.szxytkj.cn

[R30] 函数返回状态码
来源：http://vu.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://dv.yuntaijiaju.cn

[R31] 局部变量
来源：http://ll.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://pn.haigaiapp.cn

[R32] 参数个数校验
来源：http://vz.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dd.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://fn.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xo.lnxyls.cn

[R34] 退出时清理
来源：http://td.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mz.asd995.cn

[R35] 后台执行并等待
来源：http://tg.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ev.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://jr.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vk.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://zr.9csxet.cn

files=$(ls -1)
来源：http://mu.shxzukj.cn

[R38] 管道串联
来源：http://wj.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://np.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://ss.nszjky.cn

cmd > out.log 2>&1
来源：http://sw.bjjhwx.cn

[R40] 追加写日志
来源：http://wg.huixiangedu.cn

echo "log" >> out.log
来源：http://if.bjjhwx.cn

[R41] 丢弃输出
来源：http://bo.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://bv.asd995.cn

[R42] 输入重定向
来源：http://jy.huixiangedu.cn

wc -l < a.txt
来源：http://na.asd995.cn

[R43] 按名字查找文件
来源：http://dy.asd995.cn

find . -name "*.log" -type f
来源：http://zo.shtwfgs.cn

[R44] 按修改时间查找
来源：http://ic.newstarts.cn

find . -mtime -7 -type f
来源：http://ii.huixinmuqiang.cn

[R45] 批量删除
来源：http://za.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://wq.newstarts.cn

[R46] 递归替换文件内容
来源：http://tc.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kh.hahajie.cn

[R47] sed 单行替换
来源：http://mg.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wf.shtwfgs.cn

[R48] awk 取指定列
来源：http://gq.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://dd.huixiangedu.cn

[R49] awk 带条件
来源：http://wq.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bm.yuntaijiaju.cn

[R50] awk 求和
来源：http://gh.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pt.yuexingan06.cn

[R51] 排序去重取前几
来源：http://sh.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eo.hahajie.cn

[R52] 统计行数
来源：http://dr.colortex.cn

wc -l a.txt
来源：http://og.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://kk.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nt.yuexingan06.cn

[R54] 比较两个文件
来源：http://sj.szsharing.cn

diff a.txt b.txt
来源：http://nu.shxzskj.cn

[R55] 压缩与解压
来源：http://ix.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mb.521024.cn

[R56] 远程拷贝
来源：http://zp.wgjwhj.cn

scp file user@host:/path/
来源：http://op.szxytkj.cn

[R57] 远程执行命令
来源：http://pd.haigaiapp.cn

ssh user@host 'uptime'
来源：http://bp.jianghongdianzi.cn

[R58] 下载文件
来源：http://ic.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cs.521024.cn

[R59] 发 POST JSON
来源：http://iw.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://py.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://xe.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yk.gzmigu.cn

[R61] 磁盘占用
来源：http://qt.shxzskj.cn

df -h;  du -sh *
来源：http://js.asd995.cn

[R62] 找最占空间的文件
来源：http://zd.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://ym.jctech888.com.cn

[R63] 内存与进程
来源：http://xo.colortex.cn

free -h;  ps aux | grep nginx
来源：http://mo.szxytkj.cn

[R64] 结束进程
来源：http://gr.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://uf.521024.cn

[R65] 查看端口占用
来源：http://nh.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://et.nicolike.cn

[R66] 定时任务
来源：http://fl.szxytkj.cn

crontab -e;  crontab -l
来源：http://gq.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://vj.jctech888.com.cn

openssl rand -hex 16
来源：http://uo.panjiajie.cn

[R68] 计算文件校验值
来源：http://sb.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rd.newstarts.cn

[R69] 生成随机密码
来源：http://uu.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://qb.yuexingan06.cn

[R70] 时间戳与互转
来源：http://eu.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://um.hnjuh.cn

[R71] 日期格式化
来源：http://im.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://co.nicolike.cn

[R72] 等待端口就绪
来源：http://kb.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gp.bookmarksfly.cn

[R73] 分割大日志
来源：http://xk.lnxyls.cn

split -l 1000 big.log part_
来源：http://ib.yuntaijiaju.cn

[R74] 批量重命名
来源：http://uo.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zh.9csxet.cn

[R75] 导出环境变量
来源：http://at.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://gp.newstarts.cn

[R76] 使用临时文件
来源：http://tu.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bc.chemitech.net.cn

[R77] 读取用户输入
来源：http://ch.bjjhwx.cn

read -rp "请输入: " ans
来源：http://ng.bookmarksfly.cn

[R78] 交互式菜单
来源：http://ju.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dh.szsharing.cn

[R79] 解析命令行选项
来源：http://eq.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ii.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://zy.bjjhwx.cn

time ./run.sh
来源：http://oi.colortex.cn

================================================================================
来源：http://ew.yuexingan06.cn

S. C / C++ 专题
来源：http://uw.9csxet.cn

================================================================================
来源：http://fd.yuexingan06.cn

[S01] C：Hello World
来源：http://zp.yuntaijiaju.cn

#include <stdio.h>
来源：http://nf.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://so.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://ku.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://kn.huanxung.cn

[S03] C：读入整数
来源：http://si.colortex.cn

int x; scanf("%d", &x);
来源：http://kx.jctech888.com.cn

[S04] C：字符串复制
来源：http://ze.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://py.hnjuh.cn

[S05] C：字符串长度
来源：http://eb.yuntaijiaju.cn

strlen(s)
来源：http://no.asd995.cn

[S06] C：字符串比较
来源：http://be.9csxet.cn

strcmp(a, b) == 0
来源：http://po.hahajie.cn

[S07] C：数组遍历求和
来源：http://bn.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hr.asd995.cn

[S08] C：动态内存分配与释放
来源：http://os.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ok.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://mr.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ot.wgjwhj.cn

[S10] C：指针与解引用
来源：http://lc.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://vy.shxzskj.cn

[S11] C：逐行读文件
来源：http://xg.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://xi.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lx.huanxung.cn

fclose(f);
来源：http://ls.hnjuh.cn

[S12] C：写文件
来源：http://qi.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xk.panjiajie.cn

[S13] C：宏定义
来源：http://we.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ye.hahajie.cn

[S14] C：枚举
来源：http://yj.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://uw.bookmarksfly.cn

[S15] C：类型转换
来源：http://jb.bjjhwx.cn

(double) a / b
来源：http://sg.panjiajie.cn

[S16] C：位操作置位
来源：http://lw.521024.cn

x |= (1 << 3);
来源：http://lo.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://xb.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vv.521024.cn

[S18] C：命令行参数
来源：http://mr.9csxet.cn

int main(int argc, char **argv)
来源：http://ft.hnjuh.cn

[S19] C：快速排序
来源：http://qz.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ho.asd995.cn

[S20] C：二分查找
来源：http://fq.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oh.huanxung.cn

[S21] C：字符类别判断
来源：http://jw.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zl.lnxyls.cn

[S22] C：字符串转数字
来源：http://cj.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ms.lnxyls.cn

[S23] C：随机数
来源：http://jn.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hh.haigaiapp.cn

[S24] C：获取本地时间
来源：http://be.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lb.gzmigu.cn

[S25] C：内存拷贝
来源：http://io.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://dj.wgjwhj.cn

[S26] C：内存清零
来源：http://sx.9csxet.cn

memset(a, 0, sizeof a);
来源：http://mh.shtwfgs.cn

[S27] C：定义常量
来源：http://wf.panjiajie.cn

const double PI = 3.14159;
来源：http://ym.nicolike.cn

[S28] C：静态变量
来源：http://dk.jianghongdianzi.cn

static int counter = 0;
来源：http://eu.chemitech.net.cn

[S29] C：变参函数
来源：http://me.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://am.asd995.cn

[S30] C：头文件保护
来源：http://vz.chemitech.net.cn

#ifndef X_H
来源：http://lf.huixiangedu.cn

#define X_H
来源：http://ii.yuntaijiaju.cn

#endif
来源：http://qf.asd995.cn

[S31] C++：Hello World
来源：http://ou.shtwfgs.cn

#include <iostream>
来源：http://rd.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://lf.9csxet.cn

[S32] C++：字符串
来源：http://ev.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://zl.9csxet.cn

[S33] C++：vector 增删
来源：http://wv.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hy.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://wn.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://wg.bookmarksfly.cn

[S35] C++：map
来源：http://ya.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jg.colortex.cn

[S36] C++：unordered_map
来源：http://hd.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://da.wgjwhj.cn

[S37] C++：set
来源：http://cn.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mr.huanxung.cn

[S38] C++：排序
来源：http://mm.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://zu.colortex.cn

[S39] C++：自定义比较器排序
来源：http://sw.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ek.shxzukj.cn

[S40] C++：查找元素
来源：http://zx.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zo.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://ah.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ny.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://kk.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://pc.szsharing.cn

[S43] C++：智能指针
来源：http://yw.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://nr.huixiangedu.cn

[S44] C++：引用传参
来源：http://ud.9csxet.cn

void inc(int &x) { ++x; }
来源：http://jw.jctech888.com.cn


<!-- 参考信息 -->