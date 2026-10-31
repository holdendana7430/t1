代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zo.panjiajie.cn

[Q75] 日期格式化
来源：http://ch.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mc.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bd.bjjhwx.cn

[Q76] 按天统计
来源：http://bj.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zv.bookmarksfly.cn

[Q77] 时间加减
来源：http://sd.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qa.huanxung.cn

[Q78] 当前时间
来源：http://dz.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nv.9csxet.cn

[Q79] 字符串拼接
来源：http://kl.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tc.newstarts.cn

[Q80] 字符串截取
来源：http://bq.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bu.hnjuh.cn

[Q81] 字符串替换
来源：http://wo.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tq.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://tx.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ad.szsharing.cn

[Q83] 大小写转换
来源：http://nz.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lq.panjiajie.cn

[Q84] 去除首尾空格
来源：http://cu.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://iu.jctech888.com.cn

[Q85] 数值取整
来源：http://bz.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sl.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://eh.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ei.huanxung.cn

[Q87] JSON 字段做条件
来源：http://td.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zi.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://eg.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ce.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mi.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://fw.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://po.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://ip.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aw.yuexingan06.cn

================================================================================
来源：http://qn.jianghongdianzi.cn

R. Bash 专题
来源：http://zo.colortex.cn

================================================================================
来源：http://eb.9csxet.cn

[R01] shebang 与严格模式
来源：http://gf.chemitech.net.cn

#!/usr/bin/env bash
来源：http://hs.hahajie.cn

set -euo pipefail
来源：http://jg.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://fk.gzmigu.cn

name="Tom"; echo "$name"
来源：http://xp.yuexingan06.cn

[R03] 只读变量
来源：http://xb.521024.cn

readonly PI=3.14
来源：http://nm.lnxyls.cn

[R04] 位置参数
来源：http://yx.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ri.wgjwhj.cn

[R05] 参数默认值
来源：http://og.muxihuayi.cn

name="${1:-default}"
来源：http://dp.shxzskj.cn

[R06] 判断命令是否存在
来源：http://qv.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oc.huanxung.cn

[R07] if 判断文件
来源：http://yk.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ly.9csxet.cn

[R08] 数值比较
来源：http://wc.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ej.lnxyls.cn

[R09] 字符串比较
来源：http://vm.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ce.gzmigu.cn

[R10] 正则匹配
来源：http://xz.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qn.szxytkj.cn

[R11] case 多分支
来源：http://or.hnjuh.cn

case "$1" in
来源：http://wh.yuexingan06.cn

start) echo "启动" ;;
来源：http://wl.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://jr.huanxung.cn

*)     echo "未知命令" ;;
来源：http://su.hnjuh.cn

esac
来源：http://ob.szsharing.cn

[R12] for 遍历文件
来源：http://dt.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://hc.nszjky.cn

[R13] for 计数循环
来源：http://re.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://mo.shxzskj.cn

[R14] C 风格 for
来源：http://td.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xl.shtwfgs.cn

[R15] while 逐行读文件
来源：http://ur.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bt.nicolike.cn

[R16] until 等待条件
来源：http://nq.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vh.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://ax.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://if.huanxung.cn

[R18] 遍历数组
来源：http://lu.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xa.gzmigu.cn

[R19] 数组长度
来源：http://li.hahajie.cn

echo "${#arr[@]}"
来源：http://nz.bookmarksfly.cn

[R20] 关联数组（字典）
来源：http://hc.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ge.colortex.cn

[R21] 字符串长度
来源：http://tq.yuntaijiaju.cn

echo "${#s}"
来源：http://zk.muxihuayi.cn

[R22] 截取子串
来源：http://xe.521024.cn

echo "${s:0:5}"
来源：http://dj.jianghongdianzi.cn

[R23] 字符串替换
来源：http://af.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rk.shxzukj.cn

[R24] 大小写转换
来源：http://xr.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gz.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://in.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zi.lnxyls.cn

[R26] 命令替换
来源：http://tl.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://xo.yuntaijiaju.cn

[R27] 算术展开
来源：http://pg.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://ct.huixiangedu.cn

[R28] 浮点运算
来源：http://gn.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://ve.nszjky.cn

[R29] 定义函数
来源：http://dp.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kt.nicolike.cn

[R30] 函数返回状态码
来源：http://qu.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://xa.chemitech.net.cn

[R31] 局部变量
来源：http://bl.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://ac.huixiangedu.cn

[R32] 参数个数校验
来源：http://iz.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oz.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://mn.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uv.huanxung.cn

[R34] 退出时清理
来源：http://pd.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gu.hahajie.cn

[R35] 后台执行并等待
来源：http://sv.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vg.521024.cn

[R36] 并发执行多个任务
来源：http://mf.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wn.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://ou.szsharing.cn

files=$(ls -1)
来源：http://hr.newstarts.cn

[R38] 管道串联
来源：http://cs.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://gu.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://wj.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://qq.hahajie.cn

[R40] 追加写日志
来源：http://ff.nszjky.cn

echo "log" >> out.log
来源：http://lh.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://jk.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://kz.huanxung.cn

[R42] 输入重定向
来源：http://dg.newstarts.cn

wc -l < a.txt
来源：http://qn.chemitech.net.cn

[R43] 按名字查找文件
来源：http://wn.nicolike.cn

find . -name "*.log" -type f
来源：http://jt.muxihuayi.cn

[R44] 按修改时间查找
来源：http://kc.521024.cn

find . -mtime -7 -type f
来源：http://qi.hahajie.cn

[R45] 批量删除
来源：http://ic.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://ad.lnxyls.cn

[R46] 递归替换文件内容
来源：http://kl.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yr.huanxung.cn

[R47] sed 单行替换
来源：http://nm.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sl.jctech888.com.cn

[R48] awk 取指定列
来源：http://qe.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://sc.muxihuayi.cn

[R49] awk 带条件
来源：http://wr.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ol.bjjhwx.cn

[R50] awk 求和
来源：http://lw.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yh.hnjuh.cn

[R51] 排序去重取前几
来源：http://dl.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yf.huanxung.cn

[R52] 统计行数
来源：http://zt.nszjky.cn

wc -l a.txt
来源：http://sc.asd995.cn

[R53] 查看文件头与实时尾
来源：http://xl.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gg.gzmigu.cn

[R54] 比较两个文件
来源：http://ye.bjjhwx.cn

diff a.txt b.txt
来源：http://le.wgjwhj.cn

[R55] 压缩与解压
来源：http://ke.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jb.wgjwhj.cn

[R56] 远程拷贝
来源：http://gk.yuexingan06.cn

scp file user@host:/path/
来源：http://fs.shxzukj.cn

[R57] 远程执行命令
来源：http://jp.newstarts.cn

ssh user@host 'uptime'
来源：http://ws.yuntaijiaju.cn

[R58] 下载文件
来源：http://fu.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://th.nszjky.cn

[R59] 发 POST JSON
来源：http://da.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vd.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://fr.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dq.521024.cn

[R61] 磁盘占用
来源：http://tt.bookmarksfly.cn

df -h;  du -sh *
来源：http://ug.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://vv.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://vg.shtwfgs.cn

[R63] 内存与进程
来源：http://pq.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://lb.shtwfgs.cn

[R64] 结束进程
来源：http://lw.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://cm.asd995.cn

[R65] 查看端口占用
来源：http://ey.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oh.nszjky.cn

[R66] 定时任务
来源：http://gy.lnxyls.cn

crontab -e;  crontab -l
来源：http://bu.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://tx.hahajie.cn

openssl rand -hex 16
来源：http://gi.huixiangedu.cn

[R68] 计算文件校验值
来源：http://tz.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pk.colortex.cn

[R69] 生成随机密码
来源：http://if.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://wn.huanxung.cn

[R70] 时间戳与互转
来源：http://ku.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://xq.gzmigu.cn

[R71] 日期格式化
来源：http://yu.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ly.wgjwhj.cn

[R72] 等待端口就绪
来源：http://bf.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hr.yuexingan06.cn

[R73] 分割大日志
来源：http://up.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://lq.hahajie.cn

[R74] 批量重命名
来源：http://fo.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ud.huanxung.cn

[R75] 导出环境变量
来源：http://mf.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://jk.nicolike.cn

[R76] 使用临时文件
来源：http://wo.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://os.lnxyls.cn

[R77] 读取用户输入
来源：http://kz.huanxung.cn

read -rp "请输入: " ans
来源：http://pv.szsharing.cn

[R78] 交互式菜单
来源：http://as.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ck.colortex.cn

[R79] 解析命令行选项
来源：http://td.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jp.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://ir.panjiajie.cn

time ./run.sh
来源：http://dm.wgjwhj.cn

================================================================================
来源：http://cp.huanxung.cn

S. C / C++ 专题
来源：http://tw.szsharing.cn

================================================================================
来源：http://tf.jctech888.com.cn

[S01] C：Hello World
来源：http://bj.shxzskj.cn

#include <stdio.h>
来源：http://hh.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qo.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://le.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://sg.521024.cn

[S03] C：读入整数
来源：http://ks.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://nh.bookmarksfly.cn

[S04] C：字符串复制
来源：http://pn.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://or.nicolike.cn

[S05] C：字符串长度
来源：http://aw.bjjhwx.cn

strlen(s)
来源：http://dr.newstarts.cn

[S06] C：字符串比较
来源：http://nb.haigaiapp.cn

strcmp(a, b) == 0
来源：http://zt.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://pt.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kx.colortex.cn

[S08] C：动态内存分配与释放
来源：http://hd.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ew.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://le.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ui.wgjwhj.cn

[S10] C：指针与解引用
来源：http://os.newstarts.cn

int *p = &a;  *p = 5;
来源：http://lw.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://lq.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://ze.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gh.hahajie.cn

fclose(f);
来源：http://ma.jctech888.com.cn

[S12] C：写文件
来源：http://nc.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://op.shxzskj.cn

[S13] C：宏定义
来源：http://qp.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eo.yuntaijiaju.cn

[S14] C：枚举
来源：http://oc.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://ot.shtwfgs.cn

[S15] C：类型转换
来源：http://wz.wgjwhj.cn

(double) a / b
来源：http://fc.huanxung.cn

[S16] C：位操作置位
来源：http://tt.9csxet.cn

x |= (1 << 3);
来源：http://wp.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://dw.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ja.bookmarksfly.cn

[S18] C：命令行参数
来源：http://rx.hnjuh.cn

int main(int argc, char **argv)
来源：http://id.yuntaijiaju.cn

[S19] C：快速排序
来源：http://is.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ih.asd995.cn

[S20] C：二分查找
来源：http://zz.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yo.huixiangedu.cn

[S21] C：字符类别判断
来源：http://iv.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vv.shtwfgs.cn

[S22] C：字符串转数字
来源：http://gf.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hb.nicolike.cn

[S23] C：随机数
来源：http://df.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nx.hnjuh.cn

[S24] C：获取本地时间
来源：http://nf.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sp.nszjky.cn

[S25] C：内存拷贝
来源：http://lt.asd995.cn

memcpy(dst, src, n);
来源：http://aa.yuexingan06.cn

[S26] C：内存清零
来源：http://rx.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://ry.nszjky.cn

[S27] C：定义常量
来源：http://hd.521024.cn

const double PI = 3.14159;
来源：http://nb.panjiajie.cn

[S28] C：静态变量
来源：http://dw.huanxung.cn

static int counter = 0;
来源：http://io.hnjuh.cn

[S29] C：变参函数
来源：http://au.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tk.newstarts.cn

[S30] C：头文件保护
来源：http://bq.szxytkj.cn

#ifndef X_H
来源：http://fc.gzmigu.cn

#define X_H
来源：http://ym.szsharing.cn

#endif
来源：http://jt.nicolike.cn

[S31] C++：Hello World
来源：http://hf.yuexingan06.cn

#include <iostream>
来源：http://ku.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://ca.bjjhwx.cn

[S32] C++：字符串
来源：http://id.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://ip.shtwfgs.cn

[S33] C++：vector 增删
来源：http://wy.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xh.9csxet.cn

[S34] C++：遍历 vector
来源：http://zj.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://og.jctech888.com.cn

[S35] C++：map
来源：http://qh.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kd.muxihuayi.cn

[S36] C++：unordered_map
来源：http://cu.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bi.hnjuh.cn

[S37] C++：set
来源：http://lg.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sh.nszjky.cn

[S38] C++：排序
来源：http://zz.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://sd.colortex.cn

[S39] C++：自定义比较器排序
来源：http://og.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sl.newstarts.cn

[S40] C++：查找元素
来源：http://qz.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fz.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://vd.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pg.nicolike.cn

[S42] C++：继承与虚函数
来源：http://en.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://as.wgjwhj.cn

[S43] C++：智能指针
来源：http://ln.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://np.haigaiapp.cn

[S44] C++：引用传参
来源：http://yx.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://hr.panjiajie.cn


<!-- 参考信息 -->