代发 wailian999

SHOW INDEX FROM users;
来源：http://pc.huixiangedu.cn

[Q73] 查看表状态
来源：http://yq.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gv.chemitech.net.cn

[Q74] 强制使用索引
来源：http://ky.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yk.colortex.cn

[Q75] 日期格式化
来源：http://sx.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xa.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eg.bjjhwx.cn

[Q76] 按天统计
来源：http://jo.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oh.wgjwhj.cn

[Q77] 时间加减
来源：http://ud.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kg.bookmarksfly.cn

[Q78] 当前时间
来源：http://lf.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gp.szxytkj.cn

[Q79] 字符串拼接
来源：http://nh.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dg.jianghongdianzi.cn

[Q80] 字符串截取
来源：http://vz.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ej.asd995.cn

[Q81] 字符串替换
来源：http://ss.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bp.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://km.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kv.bjjhwx.cn

[Q83] 大小写转换
来源：http://yb.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rc.gzmigu.cn

[Q84] 去除首尾空格
来源：http://gf.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://xm.yuntaijiaju.cn

[Q85] 数值取整
来源：http://ug.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tt.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://kr.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vt.colortex.cn

[Q87] JSON 字段做条件
来源：http://iq.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://by.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://ab.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jy.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yt.9csxet.cn

[Q89] 判断表是否存在
来源：http://uk.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lt.muxihuayi.cn

[Q90] 生成序号列
来源：http://gu.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gc.yuexingan06.cn

================================================================================
来源：http://qj.yuexingan06.cn

R. Bash 专题
来源：http://ie.muxihuayi.cn

================================================================================
来源：http://qz.nszjky.cn

[R01] shebang 与严格模式
来源：http://oo.huixiangedu.cn

#!/usr/bin/env bash
来源：http://pa.lnxyls.cn

set -euo pipefail
来源：http://fo.9csxet.cn

[R02] 变量赋值与使用
来源：http://cv.hnjuh.cn

name="Tom"; echo "$name"
来源：http://id.colortex.cn

[R03] 只读变量
来源：http://ux.asd995.cn

readonly PI=3.14
来源：http://ff.newstarts.cn

[R04] 位置参数
来源：http://wy.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jo.521024.cn

[R05] 参数默认值
来源：http://kf.yuexingan06.cn

name="${1:-default}"
来源：http://bo.shxzukj.cn

[R06] 判断命令是否存在
来源：http://pw.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bb.nicolike.cn

[R07] if 判断文件
来源：http://zz.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fg.panjiajie.cn

[R08] 数值比较
来源：http://vq.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cp.9csxet.cn

[R09] 字符串比较
来源：http://se.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qb.huixiangedu.cn

[R10] 正则匹配
来源：http://cn.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vf.lnxyls.cn

[R11] case 多分支
来源：http://bz.yuexingan06.cn

case "$1" in
来源：http://si.szxytkj.cn

start) echo "启动" ;;
来源：http://rk.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://gi.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://lb.newstarts.cn

esac
来源：http://nr.newstarts.cn

[R12] for 遍历文件
来源：http://iu.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://to.nicolike.cn

[R13] for 计数循环
来源：http://sa.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://qi.nicolike.cn

[R14] C 风格 for
来源：http://is.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dl.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://md.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ik.colortex.cn

[R16] until 等待条件
来源：http://jz.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://an.9csxet.cn

[R17] 数组定义与取值
来源：http://eh.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rm.hnjuh.cn

[R18] 遍历数组
来源：http://km.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://of.muxihuayi.cn

[R19] 数组长度
来源：http://un.lnxyls.cn

echo "${#arr[@]}"
来源：http://ye.gzmigu.cn

[R20] 关联数组（字典）
来源：http://mh.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dj.521024.cn

[R21] 字符串长度
来源：http://jg.jctech888.com.cn

echo "${#s}"
来源：http://oh.szsharing.cn

[R22] 截取子串
来源：http://ww.huixiangedu.cn

echo "${s:0:5}"
来源：http://nn.szxytkj.cn

[R23] 字符串替换
来源：http://bi.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ls.panjiajie.cn

[R24] 大小写转换
来源：http://ms.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ie.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://ii.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uo.nszjky.cn

[R26] 命令替换
来源：http://dq.colortex.cn

now=$(date +%F); echo "$now"
来源：http://os.huixinmuqiang.cn

[R27] 算术展开
来源：http://ho.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://xl.shtwfgs.cn

[R28] 浮点运算
来源：http://un.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://kz.hnjuh.cn

[R29] 定义函数
来源：http://as.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bi.huixiangedu.cn

[R30] 函数返回状态码
来源：http://gz.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://ef.wgjwhj.cn

[R31] 局部变量
来源：http://rj.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://uw.bjjhwx.cn

[R32] 参数个数校验
来源：http://wy.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cx.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://zx.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ww.jctech888.com.cn

[R34] 退出时清理
来源：http://ah.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bp.521024.cn

[R35] 后台执行并等待
来源：http://dr.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gb.nszjky.cn

[R36] 并发执行多个任务
来源：http://ss.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cm.gzmigu.cn

[R37] 把输出赋给变量
来源：http://df.lnxyls.cn

files=$(ls -1)
来源：http://zl.wgjwhj.cn

[R38] 管道串联
来源：http://ua.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://fu.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://br.colortex.cn

cmd > out.log 2>&1
来源：http://hz.shxzukj.cn

[R40] 追加写日志
来源：http://oo.hahajie.cn

echo "log" >> out.log
来源：http://ai.panjiajie.cn

[R41] 丢弃输出
来源：http://mw.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://pn.yuntaijiaju.cn

[R42] 输入重定向
来源：http://yi.jianghongdianzi.cn

wc -l < a.txt
来源：http://lw.521024.cn

[R43] 按名字查找文件
来源：http://ee.jctech888.com.cn

find . -name "*.log" -type f
来源：http://jq.shxzskj.cn

[R44] 按修改时间查找
来源：http://li.huixiangedu.cn

find . -mtime -7 -type f
来源：http://md.shxzukj.cn

[R45] 批量删除
来源：http://iu.szsharing.cn

find . -name "*.tmp" -delete
来源：http://ka.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://cp.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ut.521024.cn

[R47] sed 单行替换
来源：http://ry.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rn.bookmarksfly.cn

[R48] awk 取指定列
来源：http://js.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://za.szsharing.cn

[R49] awk 带条件
来源：http://yf.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xq.lnxyls.cn

[R50] awk 求和
来源：http://pd.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://af.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://ke.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ah.wgjwhj.cn

[R52] 统计行数
来源：http://pj.521024.cn

wc -l a.txt
来源：http://eh.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://vr.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://su.newstarts.cn

[R54] 比较两个文件
来源：http://mh.shtwfgs.cn

diff a.txt b.txt
来源：http://er.jctech888.com.cn

[R55] 压缩与解压
来源：http://yd.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ap.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://bp.bookmarksfly.cn

scp file user@host:/path/
来源：http://kv.shtwfgs.cn

[R57] 远程执行命令
来源：http://sr.asd995.cn

ssh user@host 'uptime'
来源：http://jr.bjjhwx.cn

[R58] 下载文件
来源：http://el.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lh.asd995.cn

[R59] 发 POST JSON
来源：http://tx.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fw.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://sw.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sx.colortex.cn

[R61] 磁盘占用
来源：http://kj.shxzukj.cn

df -h;  du -sh *
来源：http://se.shxzskj.cn

[R62] 找最占空间的文件
来源：http://tn.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://ts.muxihuayi.cn

[R63] 内存与进程
来源：http://ta.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://cc.nszjky.cn

[R64] 结束进程
来源：http://mr.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://yp.nicolike.cn

[R65] 查看端口占用
来源：http://ev.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ba.huixinmuqiang.cn

[R66] 定时任务
来源：http://ng.shxzskj.cn

crontab -e;  crontab -l
来源：http://mp.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://ok.huixinmuqiang.cn

openssl rand -hex 16
来源：http://uf.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://yg.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xi.hahajie.cn

[R69] 生成随机密码
来源：http://kk.521024.cn

head -c 16 /dev/urandom | base64
来源：http://tt.szxytkj.cn

[R70] 时间戳与互转
来源：http://la.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://wy.521024.cn

[R71] 日期格式化
来源：http://un.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ri.asd995.cn

[R72] 等待端口就绪
来源：http://cb.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ug.szxytkj.cn

[R73] 分割大日志
来源：http://ky.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://qs.gzmigu.cn

[R74] 批量重命名
来源：http://cs.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qx.hnjuh.cn

[R75] 导出环境变量
来源：http://un.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://lm.521024.cn

[R76] 使用临时文件
来源：http://ax.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lg.huanxung.cn

[R77] 读取用户输入
来源：http://dw.gzmigu.cn

read -rp "请输入: " ans
来源：http://yw.panjiajie.cn

[R78] 交互式菜单
来源：http://ek.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mr.haigaiapp.cn

[R79] 解析命令行选项
来源：http://gw.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tt.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://mj.hnjuh.cn

time ./run.sh
来源：http://bc.521024.cn

================================================================================
来源：http://ah.wgjwhj.cn

S. C / C++ 专题
来源：http://vd.shxzukj.cn

================================================================================
来源：http://eg.jctech888.com.cn

[S01] C：Hello World
来源：http://qm.szxytkj.cn

#include <stdio.h>
来源：http://yl.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zi.nicolike.cn

[S02] C：变量与格式化输出
来源：http://er.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://zq.hnjuh.cn

[S03] C：读入整数
来源：http://kq.newstarts.cn

int x; scanf("%d", &x);
来源：http://sn.huanxung.cn

[S04] C：字符串复制
来源：http://ze.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lc.521024.cn

[S05] C：字符串长度
来源：http://pd.jctech888.com.cn

strlen(s)
来源：http://ay.panjiajie.cn

[S06] C：字符串比较
来源：http://vx.muxihuayi.cn

strcmp(a, b) == 0
来源：http://vp.shxzukj.cn

[S07] C：数组遍历求和
来源：http://ue.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tz.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://nn.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dr.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://iq.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ux.hnjuh.cn

[S10] C：指针与解引用
来源：http://yb.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://ws.panjiajie.cn

[S11] C：逐行读文件
来源：http://ei.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://nx.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nc.bookmarksfly.cn

fclose(f);
来源：http://wn.nicolike.cn

[S12] C：写文件
来源：http://ow.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vc.asd995.cn

[S13] C：宏定义
来源：http://ya.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xj.shtwfgs.cn

[S14] C：枚举
来源：http://eb.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://ah.bjjhwx.cn

[S15] C：类型转换
来源：http://hi.huixinmuqiang.cn

(double) a / b
来源：http://rd.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://uo.szxytkj.cn

x |= (1 << 3);
来源：http://no.colortex.cn

[S17] C：安全拼接字符串
来源：http://yv.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mh.9csxet.cn

[S18] C：命令行参数
来源：http://vr.hahajie.cn

int main(int argc, char **argv)
来源：http://cu.huanxung.cn

[S19] C：快速排序
来源：http://ad.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hd.bookmarksfly.cn

[S20] C：二分查找
来源：http://jj.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qu.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://pr.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zk.muxihuayi.cn

[S22] C：字符串转数字
来源：http://hp.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yo.nszjky.cn

[S23] C：随机数
来源：http://oc.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fb.newstarts.cn

[S24] C：获取本地时间
来源：http://ku.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wn.hahajie.cn

[S25] C：内存拷贝
来源：http://gv.muxihuayi.cn

memcpy(dst, src, n);
来源：http://bo.bjjhwx.cn

[S26] C：内存清零
来源：http://df.9csxet.cn

memset(a, 0, sizeof a);
来源：http://sq.haigaiapp.cn

[S27] C：定义常量
来源：http://ss.bookmarksfly.cn

const double PI = 3.14159;
来源：http://ln.yuexingan06.cn

[S28] C：静态变量
来源：http://wp.newstarts.cn

static int counter = 0;
来源：http://ur.nszjky.cn

[S29] C：变参函数
来源：http://rx.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xl.chemitech.net.cn

[S30] C：头文件保护
来源：http://ss.huanxung.cn

#ifndef X_H
来源：http://rj.bookmarksfly.cn

#define X_H
来源：http://gu.yuntaijiaju.cn

#endif
来源：http://wh.asd995.cn

[S31] C++：Hello World
来源：http://ua.shxzukj.cn

#include <iostream>
来源：http://kl.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://xr.haigaiapp.cn

[S32] C++：字符串
来源：http://tv.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://sh.shtwfgs.cn

[S33] C++：vector 增删
来源：http://wu.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://na.asd995.cn

[S34] C++：遍历 vector
来源：http://yt.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://gz.jctech888.com.cn

[S35] C++：map
来源：http://fq.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yh.muxihuayi.cn

[S36] C++：unordered_map
来源：http://tk.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mr.asd995.cn

[S37] C++：set
来源：http://nn.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wy.hnjuh.cn

[S38] C++：排序
来源：http://jd.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://gq.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://xb.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ph.gzmigu.cn

[S40] C++：查找元素
来源：http://eo.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://st.gzmigu.cn

[S41] C++：类与构造函数
来源：http://po.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ue.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://pt.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://uu.muxihuayi.cn


<!-- 参考信息 -->