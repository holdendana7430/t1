代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gi.hahajie.cn

[Q75] 日期格式化
来源：http://qf.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://if.jianghongdianzi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rn.szsharing.cn

[Q76] 按天统计
来源：http://cs.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xw.chemitech.net.cn

[Q77] 时间加减
来源：http://de.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://az.bjjhwx.cn

[Q78] 当前时间
来源：http://oa.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lp.wgjwhj.cn

[Q79] 字符串拼接
来源：http://wr.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ss.shxzukj.cn

[Q80] 字符串截取
来源：http://vo.jianghongdianzi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aj.jctech888.com.cn

[Q81] 字符串替换
来源：http://ty.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kg.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://ue.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://me.muxihuayi.cn

[Q83] 大小写转换
来源：http://hd.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zj.shxzukj.cn

[Q84] 去除首尾空格
来源：http://se.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://ns.shtwfgs.cn

[Q85] 数值取整
来源：http://au.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rs.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://nz.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ku.9csxet.cn

[Q87] JSON 字段做条件
来源：http://sn.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xw.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://ia.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mk.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ip.asd995.cn

[Q89] 判断表是否存在
来源：http://xd.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ce.yuexingan06.cn

[Q90] 生成序号列
来源：http://ag.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ml.huanxung.cn

================================================================================
来源：http://ty.huixiangedu.cn

R. Bash 专题
来源：http://fo.hahajie.cn

================================================================================
来源：http://fk.nicolike.cn

[R01] shebang 与严格模式
来源：http://vh.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://gl.hnjuh.cn

set -euo pipefail
来源：http://ph.colortex.cn

[R02] 变量赋值与使用
来源：http://ay.nicolike.cn

name="Tom"; echo "$name"
来源：http://vp.bjjhwx.cn

[R03] 只读变量
来源：http://zb.huixinmuqiang.cn

readonly PI=3.14
来源：http://hb.chemitech.net.cn

[R04] 位置参数
来源：http://sa.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bw.haigaiapp.cn

[R05] 参数默认值
来源：http://lt.haigaiapp.cn

name="${1:-default}"
来源：http://fx.gzmigu.cn

[R06] 判断命令是否存在
来源：http://ro.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ee.panjiajie.cn

[R07] if 判断文件
来源：http://rc.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pp.huanxung.cn

[R08] 数值比较
来源：http://tg.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ww.muxihuayi.cn

[R09] 字符串比较
来源：http://tz.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://om.jianghongdianzi.cn

[R10] 正则匹配
来源：http://ny.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mr.shxzskj.cn

[R11] case 多分支
来源：http://cu.shxzskj.cn

case "$1" in
来源：http://md.szsharing.cn

start) echo "启动" ;;
来源：http://mv.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://hg.huanxung.cn

*)     echo "未知命令" ;;
来源：http://hw.nszjky.cn

esac
来源：http://ib.yuexingan06.cn

[R12] for 遍历文件
来源：http://zd.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://vb.wgjwhj.cn

[R13] for 计数循环
来源：http://tv.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://oc.yuntaijiaju.cn

[R14] C 风格 for
来源：http://wp.9csxet.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pr.asd995.cn

[R15] while 逐行读文件
来源：http://sq.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xq.lnxyls.cn

[R16] until 等待条件
来源：http://uz.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vx.colortex.cn

[R17] 数组定义与取值
来源：http://xe.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wh.lnxyls.cn

[R18] 遍历数组
来源：http://uz.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ah.shxzskj.cn

[R19] 数组长度
来源：http://st.newstarts.cn

echo "${#arr[@]}"
来源：http://rj.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://dg.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://px.huixiangedu.cn

[R21] 字符串长度
来源：http://bn.gzmigu.cn

echo "${#s}"
来源：http://vi.huanxung.cn

[R22] 截取子串
来源：http://ik.gzmigu.cn

echo "${s:0:5}"
来源：http://ii.yuntaijiaju.cn

[R23] 字符串替换
来源：http://nh.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bz.nicolike.cn

[R24] 大小写转换
来源：http://bb.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pi.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://wq.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vl.bjjhwx.cn

[R26] 命令替换
来源：http://nn.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://op.hnjuh.cn

[R27] 算术展开
来源：http://zu.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://xf.muxihuayi.cn

[R28] 浮点运算
来源：http://oe.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://hn.521024.cn

[R29] 定义函数
来源：http://pq.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jv.nszjky.cn

[R30] 函数返回状态码
来源：http://kh.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://ph.colortex.cn

[R31] 局部变量
来源：http://om.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://le.szsharing.cn

[R32] 参数个数校验
来源：http://kf.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rf.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://ec.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zd.lnxyls.cn

[R34] 退出时清理
来源：http://ai.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zx.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://wj.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ng.hnjuh.cn

[R36] 并发执行多个任务
来源：http://ie.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oy.szxytkj.cn

[R37] 把输出赋给变量
来源：http://si.jctech888.com.cn

files=$(ls -1)
来源：http://et.gzmigu.cn

[R38] 管道串联
来源：http://ph.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://ue.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://et.wgjwhj.cn

cmd > out.log 2>&1
来源：http://us.yuntaijiaju.cn

[R40] 追加写日志
来源：http://fj.szxytkj.cn

echo "log" >> out.log
来源：http://km.yuexingan06.cn

[R41] 丢弃输出
来源：http://ju.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://tt.lnxyls.cn

[R42] 输入重定向
来源：http://jk.lnxyls.cn

wc -l < a.txt
来源：http://ly.nicolike.cn

[R43] 按名字查找文件
来源：http://dm.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://nz.9csxet.cn

[R44] 按修改时间查找
来源：http://mw.asd995.cn

find . -mtime -7 -type f
来源：http://iu.szxytkj.cn

[R45] 批量删除
来源：http://gl.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://xe.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://gg.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dk.bookmarksfly.cn

[R47] sed 单行替换
来源：http://ug.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uk.nicolike.cn

[R48] awk 取指定列
来源：http://ub.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://ez.nicolike.cn

[R49] awk 带条件
来源：http://ry.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lc.yuexingan06.cn

[R50] awk 求和
来源：http://ny.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mo.huanxung.cn

[R51] 排序去重取前几
来源：http://vn.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kl.szsharing.cn

[R52] 统计行数
来源：http://if.hahajie.cn

wc -l a.txt
来源：http://lz.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://gk.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cb.gzmigu.cn

[R54] 比较两个文件
来源：http://yw.huanxung.cn

diff a.txt b.txt
来源：http://ge.gzmigu.cn

[R55] 压缩与解压
来源：http://ya.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ch.panjiajie.cn

[R56] 远程拷贝
来源：http://qj.lnxyls.cn

scp file user@host:/path/
来源：http://we.jctech888.com.cn

[R57] 远程执行命令
来源：http://jf.shtwfgs.cn

ssh user@host 'uptime'
来源：http://gj.newstarts.cn

[R58] 下载文件
来源：http://jj.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ou.9csxet.cn

[R59] 发 POST JSON
来源：http://qd.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gc.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://eh.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://li.gzmigu.cn

[R61] 磁盘占用
来源：http://qi.shxzskj.cn

df -h;  du -sh *
来源：http://yz.hnjuh.cn

[R62] 找最占空间的文件
来源：http://bk.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://un.9csxet.cn

[R63] 内存与进程
来源：http://xs.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://pa.hnjuh.cn

[R64] 结束进程
来源：http://wt.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://ht.haigaiapp.cn

[R65] 查看端口占用
来源：http://fi.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ai.bookmarksfly.cn

[R66] 定时任务
来源：http://fq.shtwfgs.cn

crontab -e;  crontab -l
来源：http://ky.521024.cn

[R67] 生成随机十六进制串
来源：http://ik.asd995.cn

openssl rand -hex 16
来源：http://zv.colortex.cn

[R68] 计算文件校验值
来源：http://km.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yr.asd995.cn

[R69] 生成随机密码
来源：http://pf.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://hi.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://td.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://jk.9csxet.cn

[R71] 日期格式化
来源：http://yv.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nz.huixiangedu.cn

[R72] 等待端口就绪
来源：http://nd.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mi.jctech888.com.cn

[R73] 分割大日志
来源：http://nm.shxzskj.cn

split -l 1000 big.log part_
来源：http://nl.hnjuh.cn

[R74] 批量重命名
来源：http://jj.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qv.huixiangedu.cn

[R75] 导出环境变量
来源：http://vr.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://uv.lnxyls.cn

[R76] 使用临时文件
来源：http://no.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hk.huanxung.cn

[R77] 读取用户输入
来源：http://gi.jctech888.com.cn

read -rp "请输入: " ans
来源：http://cr.szxytkj.cn

[R78] 交互式菜单
来源：http://kq.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lv.gzmigu.cn

[R79] 解析命令行选项
来源：http://zi.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ys.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://lg.haigaiapp.cn

time ./run.sh
来源：http://le.nicolike.cn

================================================================================
来源：http://ay.asd995.cn

S. C / C++ 专题
来源：http://ya.colortex.cn

================================================================================
来源：http://db.yuntaijiaju.cn

[S01] C：Hello World
来源：http://kt.huixiangedu.cn

#include <stdio.h>
来源：http://pv.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ir.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://rb.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://dt.szxytkj.cn

[S03] C：读入整数
来源：http://ud.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://qr.lnxyls.cn

[S04] C：字符串复制
来源：http://pb.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ub.asd995.cn

[S05] C：字符串长度
来源：http://dj.shtwfgs.cn

strlen(s)
来源：http://vx.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://kh.newstarts.cn

strcmp(a, b) == 0
来源：http://ht.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://wj.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://es.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://ad.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://co.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://ki.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fr.newstarts.cn

[S10] C：指针与解引用
来源：http://cy.szsharing.cn

int *p = &a;  *p = 5;
来源：http://hm.yuexingan06.cn

[S11] C：逐行读文件
来源：http://zz.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://pr.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qv.yuexingan06.cn

fclose(f);
来源：http://jw.shxzukj.cn

[S12] C：写文件
来源：http://zd.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jd.nicolike.cn

[S13] C：宏定义
来源：http://pw.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pu.muxihuayi.cn

[S14] C：枚举
来源：http://im.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://hr.nszjky.cn

[S15] C：类型转换
来源：http://lw.szxytkj.cn

(double) a / b
来源：http://dk.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://ln.huixiangedu.cn

x |= (1 << 3);
来源：http://xr.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://fa.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://os.nszjky.cn

[S18] C：命令行参数
来源：http://xd.huixiangedu.cn

int main(int argc, char **argv)
来源：http://qh.bookmarksfly.cn

[S19] C：快速排序
来源：http://ws.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ux.chemitech.net.cn

[S20] C：二分查找
来源：http://ni.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qh.muxihuayi.cn

[S21] C：字符类别判断
来源：http://wi.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://al.chemitech.net.cn

[S22] C：字符串转数字
来源：http://bk.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ac.hahajie.cn

[S23] C：随机数
来源：http://kl.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kq.haigaiapp.cn

[S24] C：获取本地时间
来源：http://vc.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xj.colortex.cn

[S25] C：内存拷贝
来源：http://vv.szsharing.cn

memcpy(dst, src, n);
来源：http://gu.hahajie.cn

[S26] C：内存清零
来源：http://nh.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://rx.hahajie.cn

[S27] C：定义常量
来源：http://tc.bookmarksfly.cn

const double PI = 3.14159;
来源：http://jn.muxihuayi.cn

[S28] C：静态变量
来源：http://in.szsharing.cn

static int counter = 0;
来源：http://qo.nszjky.cn

[S29] C：变参函数
来源：http://rw.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kk.hnjuh.cn

[S30] C：头文件保护
来源：http://nl.shtwfgs.cn

#ifndef X_H
来源：http://mj.szxytkj.cn

#define X_H
来源：http://fv.wgjwhj.cn

#endif
来源：http://sx.nszjky.cn

[S31] C++：Hello World
来源：http://er.nicolike.cn

#include <iostream>
来源：http://jc.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://mw.huanxung.cn

[S32] C++：字符串
来源：http://iq.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://hc.muxihuayi.cn

[S33] C++：vector 增删
来源：http://pq.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://je.nszjky.cn

[S34] C++：遍历 vector
来源：http://gq.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://vo.szsharing.cn

[S35] C++：map
来源：http://we.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uq.nszjky.cn

[S36] C++：unordered_map
来源：http://au.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qc.huanxung.cn

[S37] C++：set
来源：http://rz.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pf.bookmarksfly.cn

[S38] C++：排序
来源：http://ep.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://pv.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://mg.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fi.wgjwhj.cn

[S40] C++：查找元素
来源：http://be.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fg.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://ya.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lx.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://on.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://ty.yuexingan06.cn

[S43] C++：智能指针
来源：http://jd.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://rt.panjiajie.cn

[S44] C++：引用传参
来源：http://iv.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://lb.hnjuh.cn


<!-- 参考信息 -->