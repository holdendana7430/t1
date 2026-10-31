代发 wailian999

SHOW INDEX FROM users;
来源：http://lu.hnjuh.cn

[Q73] 查看表状态
来源：http://vx.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nm.jctech888.com.cn

[Q74] 强制使用索引
来源：http://ng.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ef.yuexingan06.cn

[Q75] 日期格式化
来源：http://iu.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ue.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nb.asd995.cn

[Q76] 按天统计
来源：http://ox.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kf.szxytkj.cn

[Q77] 时间加减
来源：http://rg.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gd.huixiangedu.cn

[Q78] 当前时间
来源：http://dq.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tp.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://pc.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kc.521024.cn

[Q80] 字符串截取
来源：http://sk.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xh.hahajie.cn

[Q81] 字符串替换
来源：http://tu.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vc.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://ul.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jk.shxzskj.cn

[Q83] 大小写转换
来源：http://dd.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sk.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://cq.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://mi.yuexingan06.cn

[Q85] 数值取整
来源：http://ru.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jl.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://op.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mv.nszjky.cn

[Q87] JSON 字段做条件
来源：http://oa.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wa.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://xn.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://am.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bt.asd995.cn

[Q89] 判断表是否存在
来源：http://fc.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nr.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://tr.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zl.shtwfgs.cn

================================================================================
来源：http://vy.yuntaijiaju.cn

R. Bash 专题
来源：http://rn.shtwfgs.cn

================================================================================
来源：http://py.nicolike.cn

[R01] shebang 与严格模式
来源：http://we.chemitech.net.cn

#!/usr/bin/env bash
来源：http://hh.asd995.cn

set -euo pipefail
来源：http://xd.szsharing.cn

[R02] 变量赋值与使用
来源：http://ow.huanxung.cn

name="Tom"; echo "$name"
来源：http://wt.haigaiapp.cn

[R03] 只读变量
来源：http://jv.yuexingan06.cn

readonly PI=3.14
来源：http://ad.yuntaijiaju.cn

[R04] 位置参数
来源：http://wd.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rg.newstarts.cn

[R05] 参数默认值
来源：http://ut.yuexingan06.cn

name="${1:-default}"
来源：http://us.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://lo.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yk.jianghongdianzi.cn

[R07] if 判断文件
来源：http://uq.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tt.shxzskj.cn

[R08] 数值比较
来源：http://qk.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nj.huanxung.cn

[R09] 字符串比较
来源：http://uj.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bm.lnxyls.cn

[R10] 正则匹配
来源：http://pd.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://so.asd995.cn

[R11] case 多分支
来源：http://xx.wgjwhj.cn

case "$1" in
来源：http://wp.wgjwhj.cn

start) echo "启动" ;;
来源：http://wc.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://he.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://iq.huanxung.cn

esac
来源：http://rd.bjjhwx.cn

[R12] for 遍历文件
来源：http://he.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://me.shxzskj.cn

[R13] for 计数循环
来源：http://op.asd995.cn

for i in {1..10}; do echo "$i"; done
来源：http://dt.colortex.cn

[R14] C 风格 for
来源：http://xr.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fy.panjiajie.cn

[R15] while 逐行读文件
来源：http://bt.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://px.nicolike.cn

[R16] until 等待条件
来源：http://hj.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aa.hahajie.cn

[R17] 数组定义与取值
来源：http://wx.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ih.yuntaijiaju.cn

[R18] 遍历数组
来源：http://pz.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://od.shxzskj.cn

[R19] 数组长度
来源：http://hy.9csxet.cn

echo "${#arr[@]}"
来源：http://kk.gzmigu.cn

[R20] 关联数组（字典）
来源：http://zi.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ps.chemitech.net.cn

[R21] 字符串长度
来源：http://xe.asd995.cn

echo "${#s}"
来源：http://zv.jianghongdianzi.cn

[R22] 截取子串
来源：http://jw.jctech888.com.cn

echo "${s:0:5}"
来源：http://ri.yuexingan06.cn

[R23] 字符串替换
来源：http://cb.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://si.haigaiapp.cn

[R24] 大小写转换
来源：http://oe.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wp.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://tq.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://av.9csxet.cn

[R26] 命令替换
来源：http://tx.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://hh.521024.cn

[R27] 算术展开
来源：http://yy.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://va.huixinmuqiang.cn

[R28] 浮点运算
来源：http://kg.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://pb.szxytkj.cn

[R29] 定义函数
来源：http://nn.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ft.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://wi.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://go.jctech888.com.cn

[R31] 局部变量
来源：http://fo.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://oe.panjiajie.cn

[R32] 参数个数校验
来源：http://hj.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qe.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://bu.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lb.jctech888.com.cn

[R34] 退出时清理
来源：http://oc.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://om.huixiangedu.cn

[R35] 后台执行并等待
来源：http://qb.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vv.nszjky.cn

[R36] 并发执行多个任务
来源：http://jr.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zy.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://be.muxihuayi.cn

files=$(ls -1)
来源：http://hv.hnjuh.cn

[R38] 管道串联
来源：http://gl.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://ze.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://ko.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://jn.hahajie.cn

[R40] 追加写日志
来源：http://yi.shxzukj.cn

echo "log" >> out.log
来源：http://tn.jctech888.com.cn

[R41] 丢弃输出
来源：http://nu.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://th.nszjky.cn

[R42] 输入重定向
来源：http://rc.lnxyls.cn

wc -l < a.txt
来源：http://wh.szxytkj.cn

[R43] 按名字查找文件
来源：http://sg.shxzskj.cn

find . -name "*.log" -type f
来源：http://rj.huanxung.cn

[R44] 按修改时间查找
来源：http://ew.nicolike.cn

find . -mtime -7 -type f
来源：http://dr.lnxyls.cn

[R45] 批量删除
来源：http://vk.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://gw.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://wa.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dl.nicolike.cn

[R47] sed 单行替换
来源：http://ma.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ay.haigaiapp.cn

[R48] awk 取指定列
来源：http://dj.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://xw.gzmigu.cn

[R49] awk 带条件
来源：http://oc.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ox.bookmarksfly.cn

[R50] awk 求和
来源：http://rs.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wg.huixiangedu.cn

[R51] 排序去重取前几
来源：http://wp.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dv.huanxung.cn

[R52] 统计行数
来源：http://uh.muxihuayi.cn

wc -l a.txt
来源：http://cu.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://wc.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://my.szsharing.cn

[R54] 比较两个文件
来源：http://im.muxihuayi.cn

diff a.txt b.txt
来源：http://vp.huanxung.cn

[R55] 压缩与解压
来源：http://yt.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vp.muxihuayi.cn

[R56] 远程拷贝
来源：http://do.huanxung.cn

scp file user@host:/path/
来源：http://yk.newstarts.cn

[R57] 远程执行命令
来源：http://dw.asd995.cn

ssh user@host 'uptime'
来源：http://xg.jianghongdianzi.cn

[R58] 下载文件
来源：http://pv.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://em.haigaiapp.cn

[R59] 发 POST JSON
来源：http://ov.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://na.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://cu.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ey.szsharing.cn

[R61] 磁盘占用
来源：http://ly.hahajie.cn

df -h;  du -sh *
来源：http://ci.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://dd.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://gc.9csxet.cn

[R63] 内存与进程
来源：http://aa.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://os.jianghongdianzi.cn

[R64] 结束进程
来源：http://jl.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://mb.nszjky.cn

[R65] 查看端口占用
来源：http://et.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hh.huixinmuqiang.cn

[R66] 定时任务
来源：http://bd.shtwfgs.cn

crontab -e;  crontab -l
来源：http://bf.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://tu.wgjwhj.cn

openssl rand -hex 16
来源：http://bf.newstarts.cn

[R68] 计算文件校验值
来源：http://yw.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qs.bjjhwx.cn

[R69] 生成随机密码
来源：http://eb.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://tq.nszjky.cn

[R70] 时间戳与互转
来源：http://qo.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://kf.yuexingan06.cn

[R71] 日期格式化
来源：http://fs.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qz.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://qw.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dj.muxihuayi.cn

[R73] 分割大日志
来源：http://zs.panjiajie.cn

split -l 1000 big.log part_
来源：http://ql.chemitech.net.cn

[R74] 批量重命名
来源：http://co.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xo.shxzskj.cn

[R75] 导出环境变量
来源：http://mx.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://hv.haigaiapp.cn

[R76] 使用临时文件
来源：http://bh.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vv.szxytkj.cn

[R77] 读取用户输入
来源：http://at.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://uq.chemitech.net.cn

[R78] 交互式菜单
来源：http://rl.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tq.9csxet.cn

[R79] 解析命令行选项
来源：http://bh.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dq.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://qg.9csxet.cn

time ./run.sh
来源：http://kz.huanxung.cn

================================================================================
来源：http://bn.521024.cn

S. C / C++ 专题
来源：http://ek.szxytkj.cn

================================================================================
来源：http://bn.muxihuayi.cn

[S01] C：Hello World
来源：http://hd.jctech888.com.cn

#include <stdio.h>
来源：http://ml.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kg.asd995.cn

[S02] C：变量与格式化输出
来源：http://ea.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://cr.shtwfgs.cn

[S03] C：读入整数
来源：http://js.huanxung.cn

int x; scanf("%d", &x);
来源：http://eo.gzmigu.cn

[S04] C：字符串复制
来源：http://uh.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gm.wgjwhj.cn

[S05] C：字符串长度
来源：http://ny.shxzukj.cn

strlen(s)
来源：http://kd.jctech888.com.cn

[S06] C：字符串比较
来源：http://ut.lnxyls.cn

strcmp(a, b) == 0
来源：http://yz.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://de.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xe.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://ll.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ad.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://cy.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mj.newstarts.cn

[S10] C：指针与解引用
来源：http://ep.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://vg.newstarts.cn

[S11] C：逐行读文件
来源：http://bb.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://up.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wp.shxzskj.cn

fclose(f);
来源：http://ye.nszjky.cn

[S12] C：写文件
来源：http://np.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fp.hahajie.cn

[S13] C：宏定义
来源：http://ya.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dc.9csxet.cn

[S14] C：枚举
来源：http://ej.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://bb.haigaiapp.cn

[S15] C：类型转换
来源：http://zk.colortex.cn

(double) a / b
来源：http://qt.bjjhwx.cn

[S16] C：位操作置位
来源：http://kv.panjiajie.cn

x |= (1 << 3);
来源：http://lo.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://nl.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qm.gzmigu.cn

[S18] C：命令行参数
来源：http://qo.newstarts.cn

int main(int argc, char **argv)
来源：http://mg.nszjky.cn

[S19] C：快速排序
来源：http://mc.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rh.haigaiapp.cn

[S20] C：二分查找
来源：http://vv.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lq.shtwfgs.cn

[S21] C：字符类别判断
来源：http://lm.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xn.colortex.cn

[S22] C：字符串转数字
来源：http://ue.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vh.bookmarksfly.cn

[S23] C：随机数
来源：http://qv.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jg.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://xn.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ke.jctech888.com.cn

[S25] C：内存拷贝
来源：http://xc.szxytkj.cn

memcpy(dst, src, n);
来源：http://st.newstarts.cn

[S26] C：内存清零
来源：http://jg.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://dj.nicolike.cn

[S27] C：定义常量
来源：http://jh.521024.cn

const double PI = 3.14159;
来源：http://wf.huixiangedu.cn

[S28] C：静态变量
来源：http://lu.nicolike.cn

static int counter = 0;
来源：http://qn.bookmarksfly.cn

[S29] C：变参函数
来源：http://nn.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wq.huixiangedu.cn

[S30] C：头文件保护
来源：http://zs.hnjuh.cn

#ifndef X_H
来源：http://gw.szsharing.cn

#define X_H
来源：http://pz.muxihuayi.cn

#endif
来源：http://ra.hahajie.cn

[S31] C++：Hello World
来源：http://dg.jianghongdianzi.cn

#include <iostream>
来源：http://zf.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://eo.nszjky.cn

[S32] C++：字符串
来源：http://mi.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://pl.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://tk.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yo.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://fa.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://hv.jianghongdianzi.cn

[S35] C++：map
来源：http://zf.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qc.asd995.cn

[S36] C++：unordered_map
来源：http://mg.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://um.9csxet.cn

[S37] C++：set
来源：http://bg.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yi.szxytkj.cn

[S38] C++：排序
来源：http://lv.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://yw.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://om.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qx.szsharing.cn

[S40] C++：查找元素
来源：http://yt.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ls.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://ye.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rz.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://mp.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://lp.shxzukj.cn


<!-- 参考信息 -->