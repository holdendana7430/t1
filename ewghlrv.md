代发 wailian999

[Q76] 按天统计
来源：http://hw.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ur.szxytkj.cn

[Q77] 时间加减
来源：http://yx.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zh.huanxung.cn

[Q78] 当前时间
来源：http://re.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lu.bjjhwx.cn

[Q79] 字符串拼接
来源：http://gg.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uj.shxzukj.cn

[Q80] 字符串截取
来源：http://jw.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uh.shxzukj.cn

[Q81] 字符串替换
来源：http://gu.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hc.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://za.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tk.nicolike.cn

[Q83] 大小写转换
来源：http://qu.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qo.shxzskj.cn

[Q84] 去除首尾空格
来源：http://cd.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://sm.jctech888.com.cn

[Q85] 数值取整
来源：http://et.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hp.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://ms.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zn.521024.cn

[Q87] JSON 字段做条件
来源：http://ee.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sa.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://ik.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ir.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ha.yuntaijiaju.cn

[Q89] 判断表是否存在
来源：http://wv.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bd.hnjuh.cn

[Q90] 生成序号列
来源：http://ih.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mk.huanxung.cn

================================================================================
来源：http://sr.yuntaijiaju.cn

R. Bash 专题
来源：http://nf.huixiangedu.cn

================================================================================
来源：http://mk.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://mg.shtwfgs.cn

#!/usr/bin/env bash
来源：http://gh.gzmigu.cn

set -euo pipefail
来源：http://lq.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://tf.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://pi.bjjhwx.cn

[R03] 只读变量
来源：http://fr.yuexingan06.cn

readonly PI=3.14
来源：http://vk.gzmigu.cn

[R04] 位置参数
来源：http://ft.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ou.szxytkj.cn

[R05] 参数默认值
来源：http://ex.nicolike.cn

name="${1:-default}"
来源：http://gb.521024.cn

[R06] 判断命令是否存在
来源：http://yw.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nf.jianghongdianzi.cn

[R07] if 判断文件
来源：http://gw.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uv.huixiangedu.cn

[R08] 数值比较
来源：http://nt.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qd.bjjhwx.cn

[R09] 字符串比较
来源：http://lb.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pd.bookmarksfly.cn

[R10] 正则匹配
来源：http://ia.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://li.yuntaijiaju.cn

[R11] case 多分支
来源：http://cc.asd995.cn

case "$1" in
来源：http://dy.szxytkj.cn

start) echo "启动" ;;
来源：http://kx.nicolike.cn

stop)  echo "停止" ;;
来源：http://ec.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://ju.shxzukj.cn

esac
来源：http://oo.hahajie.cn

[R12] for 遍历文件
来源：http://na.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://dw.szsharing.cn

[R13] for 计数循环
来源：http://uc.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://si.shtwfgs.cn

[R14] C 风格 for
来源：http://xs.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uv.colortex.cn

[R15] while 逐行读文件
来源：http://sd.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eo.chemitech.net.cn

[R16] until 等待条件
来源：http://wr.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://os.huixiangedu.cn

[R17] 数组定义与取值
来源：http://sj.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uy.yuntaijiaju.cn

[R18] 遍历数组
来源：http://ap.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vz.szxytkj.cn

[R19] 数组长度
来源：http://iq.szsharing.cn

echo "${#arr[@]}"
来源：http://bb.newstarts.cn

[R20] 关联数组（字典）
来源：http://xv.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nl.shxzskj.cn

[R21] 字符串长度
来源：http://of.bjjhwx.cn

echo "${#s}"
来源：http://de.hnjuh.cn

[R22] 截取子串
来源：http://gh.hnjuh.cn

echo "${s:0:5}"
来源：http://al.nszjky.cn

[R23] 字符串替换
来源：http://er.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ns.521024.cn

[R24] 大小写转换
来源：http://zb.colortex.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cx.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://cm.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zb.shxzskj.cn

[R26] 命令替换
来源：http://mn.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://id.yuexingan06.cn

[R27] 算术展开
来源：http://zs.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://ix.chemitech.net.cn

[R28] 浮点运算
来源：http://hs.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://lt.huanxung.cn

[R29] 定义函数
来源：http://bq.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ck.shxzukj.cn

[R30] 函数返回状态码
来源：http://qy.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://vz.huixinmuqiang.cn

[R31] 局部变量
来源：http://fl.nszjky.cn

f() { local x=1; echo "$x"; }
来源：http://tl.bjjhwx.cn

[R32] 参数个数校验
来源：http://ck.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uo.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://jc.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uc.nszjky.cn

[R34] 退出时清理
来源：http://ze.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uk.muxihuayi.cn

[R35] 后台执行并等待
来源：http://rk.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ca.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://mx.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wn.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://xs.jctech888.com.cn

files=$(ls -1)
来源：http://bs.wgjwhj.cn

[R38] 管道串联
来源：http://uo.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://kt.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://tt.huixiangedu.cn

cmd > out.log 2>&1
来源：http://kd.haigaiapp.cn

[R40] 追加写日志
来源：http://ll.nicolike.cn

echo "log" >> out.log
来源：http://sz.nszjky.cn

[R41] 丢弃输出
来源：http://wq.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://ix.521024.cn

[R42] 输入重定向
来源：http://oa.shtwfgs.cn

wc -l < a.txt
来源：http://ny.521024.cn

[R43] 按名字查找文件
来源：http://pg.newstarts.cn

find . -name "*.log" -type f
来源：http://ka.haigaiapp.cn

[R44] 按修改时间查找
来源：http://jl.hnjuh.cn

find . -mtime -7 -type f
来源：http://iy.panjiajie.cn

[R45] 批量删除
来源：http://kn.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://vd.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://jy.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bm.jctech888.com.cn

[R47] sed 单行替换
来源：http://wd.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yd.hnjuh.cn

[R48] awk 取指定列
来源：http://sb.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://hp.jctech888.com.cn

[R49] awk 带条件
来源：http://sz.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lu.huixinmuqiang.cn

[R50] awk 求和
来源：http://gt.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wg.huixiangedu.cn

[R51] 排序去重取前几
来源：http://db.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zr.szsharing.cn

[R52] 统计行数
来源：http://by.lnxyls.cn

wc -l a.txt
来源：http://zr.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://om.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iz.panjiajie.cn

[R54] 比较两个文件
来源：http://uq.newstarts.cn

diff a.txt b.txt
来源：http://vp.yuexingan06.cn

[R55] 压缩与解压
来源：http://vd.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ai.521024.cn

[R56] 远程拷贝
来源：http://uw.colortex.cn

scp file user@host:/path/
来源：http://tf.hahajie.cn

[R57] 远程执行命令
来源：http://ul.bjjhwx.cn

ssh user@host 'uptime'
来源：http://eo.shxzukj.cn

[R58] 下载文件
来源：http://vj.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dc.wgjwhj.cn

[R59] 发 POST JSON
来源：http://mb.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oq.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://vj.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ue.521024.cn

[R61] 磁盘占用
来源：http://nx.huixiangedu.cn

df -h;  du -sh *
来源：http://ac.asd995.cn

[R62] 找最占空间的文件
来源：http://kq.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://lp.haigaiapp.cn

[R63] 内存与进程
来源：http://yy.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://de.hahajie.cn

[R64] 结束进程
来源：http://kr.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://pj.wgjwhj.cn

[R65] 查看端口占用
来源：http://fa.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ue.bookmarksfly.cn

[R66] 定时任务
来源：http://lf.nicolike.cn

crontab -e;  crontab -l
来源：http://ee.asd995.cn

[R67] 生成随机十六进制串
来源：http://so.hahajie.cn

openssl rand -hex 16
来源：http://ks.shxzskj.cn

[R68] 计算文件校验值
来源：http://xm.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tr.bjjhwx.cn

[R69] 生成随机密码
来源：http://et.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://pq.521024.cn

[R70] 时间戳与互转
来源：http://xs.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://zw.huixiangedu.cn

[R71] 日期格式化
来源：http://wi.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ru.haigaiapp.cn

[R72] 等待端口就绪
来源：http://in.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eu.muxihuayi.cn

[R73] 分割大日志
来源：http://gr.haigaiapp.cn

split -l 1000 big.log part_
来源：http://sx.huixiangedu.cn

[R74] 批量重命名
来源：http://lp.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qq.hnjuh.cn

[R75] 导出环境变量
来源：http://lu.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://uy.asd995.cn

[R76] 使用临时文件
来源：http://hh.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ep.gzmigu.cn

[R77] 读取用户输入
来源：http://ot.hahajie.cn

read -rp "请输入: " ans
来源：http://hd.asd995.cn

[R78] 交互式菜单
来源：http://fu.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bk.newstarts.cn

[R79] 解析命令行选项
来源：http://rx.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ou.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://ue.colortex.cn

time ./run.sh
来源：http://ho.haigaiapp.cn

================================================================================
来源：http://fy.gzmigu.cn

S. C / C++ 专题
来源：http://fb.shtwfgs.cn

================================================================================
来源：http://fo.lnxyls.cn

[S01] C：Hello World
来源：http://vx.shxzskj.cn

#include <stdio.h>
来源：http://el.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xx.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://ow.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://qw.asd995.cn

[S03] C：读入整数
来源：http://ck.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://aa.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://en.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://es.panjiajie.cn

[S05] C：字符串长度
来源：http://is.gzmigu.cn

strlen(s)
来源：http://tn.gzmigu.cn

[S06] C：字符串比较
来源：http://au.wgjwhj.cn

strcmp(a, b) == 0
来源：http://mn.gzmigu.cn

[S07] C：数组遍历求和
来源：http://dy.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jr.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://ql.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zg.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://in.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zh.huixiangedu.cn

[S10] C：指针与解引用
来源：http://ny.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://qk.shxzukj.cn

[S11] C：逐行读文件
来源：http://gg.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://hh.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dz.haigaiapp.cn

fclose(f);
来源：http://wj.hahajie.cn

[S12] C：写文件
来源：http://gu.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xq.szxytkj.cn

[S13] C：宏定义
来源：http://hb.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sz.hnjuh.cn

[S14] C：枚举
来源：http://ad.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://fh.jctech888.com.cn

[S15] C：类型转换
来源：http://ac.nszjky.cn

(double) a / b
来源：http://xm.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://lx.yuexingan06.cn

x |= (1 << 3);
来源：http://yh.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://th.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vj.jctech888.com.cn

[S18] C：命令行参数
来源：http://fy.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://nd.szxytkj.cn

[S19] C：快速排序
来源：http://bf.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nr.9csxet.cn

[S20] C：二分查找
来源：http://py.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xg.newstarts.cn

[S21] C：字符类别判断
来源：http://yg.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hu.szsharing.cn

[S22] C：字符串转数字
来源：http://ni.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ka.shtwfgs.cn

[S23] C：随机数
来源：http://jr.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wf.lnxyls.cn

[S24] C：获取本地时间
来源：http://br.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dh.bjjhwx.cn

[S25] C：内存拷贝
来源：http://wd.hnjuh.cn

memcpy(dst, src, n);
来源：http://ow.nicolike.cn

[S26] C：内存清零
来源：http://gd.colortex.cn

memset(a, 0, sizeof a);
来源：http://cp.jctech888.com.cn

[S27] C：定义常量
来源：http://dk.szsharing.cn

const double PI = 3.14159;
来源：http://zm.jctech888.com.cn

[S28] C：静态变量
来源：http://wi.bookmarksfly.cn

static int counter = 0;
来源：http://dr.9csxet.cn

[S29] C：变参函数
来源：http://re.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nc.newstarts.cn

[S30] C：头文件保护
来源：http://bf.huixiangedu.cn

#ifndef X_H
来源：http://sa.haigaiapp.cn

#define X_H
来源：http://xn.lnxyls.cn

#endif
来源：http://zx.hnjuh.cn

[S31] C++：Hello World
来源：http://df.szxytkj.cn

#include <iostream>
来源：http://pv.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://oi.lnxyls.cn

[S32] C++：字符串
来源：http://cd.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://mn.521024.cn

[S33] C++：vector 增删
来源：http://ib.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zw.panjiajie.cn

[S34] C++：遍历 vector
来源：http://us.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://dz.colortex.cn

[S35] C++：map
来源：http://nx.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hx.muxihuayi.cn

[S36] C++：unordered_map
来源：http://jt.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dj.gzmigu.cn

[S37] C++：set
来源：http://un.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nq.asd995.cn

[S38] C++：排序
来源：http://zr.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://tr.521024.cn

[S39] C++：自定义比较器排序
来源：http://qq.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xn.newstarts.cn

[S40] C++：查找元素
来源：http://ir.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bd.shxzukj.cn

[S41] C++：类与构造函数
来源：http://ds.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sw.asd995.cn

[S42] C++：继承与虚函数
来源：http://zc.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://nf.shxzukj.cn

[S43] C++：智能指针
来源：http://th.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://vw.9csxet.cn

[S44] C++：引用传参
来源：http://ay.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://dc.9csxet.cn

[S45] C++：lambda
来源：http://pg.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vo.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://bg.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yu.jianghongdianzi.cn


<!-- 参考信息 -->