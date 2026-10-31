代发 wailian999

[Q76] 按天统计
来源：http://fe.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nq.colortex.cn

[Q77] 时间加减
来源：http://ii.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vb.panjiajie.cn

[Q78] 当前时间
来源：http://hp.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tw.521024.cn

[Q79] 字符串拼接
来源：http://zv.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yk.shxzskj.cn

[Q80] 字符串截取
来源：http://mr.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gh.bjjhwx.cn

[Q81] 字符串替换
来源：http://oq.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nj.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://pr.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://au.muxihuayi.cn

[Q83] 大小写转换
来源：http://nc.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zw.newstarts.cn

[Q84] 去除首尾空格
来源：http://ao.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://uu.jianghongdianzi.cn

[Q85] 数值取整
来源：http://yd.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zh.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://ao.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zj.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://sg.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aa.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://of.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ou.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jy.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://vn.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bm.shxzukj.cn

[Q90] 生成序号列
来源：http://rg.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lh.muxihuayi.cn

================================================================================
来源：http://gm.chemitech.net.cn

R. Bash 专题
来源：http://sm.lnxyls.cn

================================================================================
来源：http://hm.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://cv.lnxyls.cn

#!/usr/bin/env bash
来源：http://li.jianghongdianzi.cn

set -euo pipefail
来源：http://as.521024.cn

[R02] 变量赋值与使用
来源：http://jt.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://oy.huanxung.cn

[R03] 只读变量
来源：http://mx.asd995.cn

readonly PI=3.14
来源：http://ns.colortex.cn

[R04] 位置参数
来源：http://qz.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nl.muxihuayi.cn

[R05] 参数默认值
来源：http://kd.9csxet.cn

name="${1:-default}"
来源：http://pk.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://vu.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vn.jctech888.com.cn

[R07] if 判断文件
来源：http://cv.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sz.hnjuh.cn

[R08] 数值比较
来源：http://nn.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xq.muxihuayi.cn

[R09] 字符串比较
来源：http://if.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wj.jctech888.com.cn

[R10] 正则匹配
来源：http://ng.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zw.yuexingan06.cn

[R11] case 多分支
来源：http://aw.newstarts.cn

case "$1" in
来源：http://cg.wgjwhj.cn

start) echo "启动" ;;
来源：http://sf.colortex.cn

stop)  echo "停止" ;;
来源：http://lr.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://je.colortex.cn

esac
来源：http://zr.bjjhwx.cn

[R12] for 遍历文件
来源：http://dg.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://mx.szsharing.cn

[R13] for 计数循环
来源：http://vl.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://yi.shxzskj.cn

[R14] C 风格 for
来源：http://fb.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qt.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://ed.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ee.jianghongdianzi.cn

[R16] until 等待条件
来源：http://kz.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fx.huixiangedu.cn

[R17] 数组定义与取值
来源：http://ia.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://or.huixinmuqiang.cn

[R18] 遍历数组
来源：http://ao.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gc.shtwfgs.cn

[R19] 数组长度
来源：http://mn.szxytkj.cn

echo "${#arr[@]}"
来源：http://ew.nszjky.cn

[R20] 关联数组（字典）
来源：http://mx.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ml.nszjky.cn

[R21] 字符串长度
来源：http://lh.szxytkj.cn

echo "${#s}"
来源：http://eo.bjjhwx.cn

[R22] 截取子串
来源：http://br.hahajie.cn

echo "${s:0:5}"
来源：http://ml.haigaiapp.cn

[R23] 字符串替换
来源：http://dj.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://er.bjjhwx.cn

[R24] 大小写转换
来源：http://zr.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ed.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://lu.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jf.colortex.cn

[R26] 命令替换
来源：http://tk.colortex.cn

now=$(date +%F); echo "$now"
来源：http://ff.huanxung.cn

[R27] 算术展开
来源：http://vg.nicolike.cn

echo $((1 + 2 * 3))
来源：http://us.huixinmuqiang.cn

[R28] 浮点运算
来源：http://kw.521024.cn

echo "scale=2; 10/3" | bc
来源：http://gq.hahajie.cn

[R29] 定义函数
来源：http://bt.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gj.panjiajie.cn

[R30] 函数返回状态码
来源：http://xj.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://pi.nszjky.cn

[R31] 局部变量
来源：http://ue.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://ir.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://jt.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nn.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://zb.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ir.shxzukj.cn

[R34] 退出时清理
来源：http://tl.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vv.panjiajie.cn

[R35] 后台执行并等待
来源：http://ca.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yg.szsharing.cn

[R36] 并发执行多个任务
来源：http://ua.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://al.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://bl.hahajie.cn

files=$(ls -1)
来源：http://ex.521024.cn

[R38] 管道串联
来源：http://ei.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://gr.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://qe.wgjwhj.cn

cmd > out.log 2>&1
来源：http://he.9csxet.cn

[R40] 追加写日志
来源：http://iq.jctech888.com.cn

echo "log" >> out.log
来源：http://tf.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://zt.newstarts.cn

cmd >/dev/null 2>&1
来源：http://nz.wgjwhj.cn

[R42] 输入重定向
来源：http://gg.wgjwhj.cn

wc -l < a.txt
来源：http://jn.yuexingan06.cn

[R43] 按名字查找文件
来源：http://wx.hnjuh.cn

find . -name "*.log" -type f
来源：http://bo.asd995.cn

[R44] 按修改时间查找
来源：http://kz.chemitech.net.cn

find . -mtime -7 -type f
来源：http://wm.9csxet.cn

[R45] 批量删除
来源：http://nh.9csxet.cn

find . -name "*.tmp" -delete
来源：http://by.shxzukj.cn

[R46] 递归替换文件内容
来源：http://oo.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cb.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://on.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zs.yuexingan06.cn

[R48] awk 取指定列
来源：http://ep.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://mm.shtwfgs.cn

[R49] awk 带条件
来源：http://ah.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uu.szsharing.cn

[R50] awk 求和
来源：http://cj.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://av.chemitech.net.cn

[R51] 排序去重取前几
来源：http://xn.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zy.nicolike.cn

[R52] 统计行数
来源：http://mf.nszjky.cn

wc -l a.txt
来源：http://vb.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://vl.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hk.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://hz.huanxung.cn

diff a.txt b.txt
来源：http://fk.hahajie.cn

[R55] 压缩与解压
来源：http://kv.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ad.yuexingan06.cn

[R56] 远程拷贝
来源：http://wh.haigaiapp.cn

scp file user@host:/path/
来源：http://ec.shxzukj.cn

[R57] 远程执行命令
来源：http://gt.huanxung.cn

ssh user@host 'uptime'
来源：http://oy.muxihuayi.cn

[R58] 下载文件
来源：http://dm.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ja.lnxyls.cn

[R59] 发 POST JSON
来源：http://ki.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vc.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://hb.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jx.haigaiapp.cn

[R61] 磁盘占用
来源：http://oj.lnxyls.cn

df -h;  du -sh *
来源：http://an.gzmigu.cn

[R62] 找最占空间的文件
来源：http://pa.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://kf.huixiangedu.cn

[R63] 内存与进程
来源：http://nv.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://la.panjiajie.cn

[R64] 结束进程
来源：http://gg.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://pm.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://qd.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bz.wgjwhj.cn

[R66] 定时任务
来源：http://qd.haigaiapp.cn

crontab -e;  crontab -l
来源：http://ni.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://kq.hahajie.cn

openssl rand -hex 16
来源：http://ym.nszjky.cn

[R68] 计算文件校验值
来源：http://uf.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fn.shtwfgs.cn

[R69] 生成随机密码
来源：http://sp.521024.cn

head -c 16 /dev/urandom | base64
来源：http://ab.shtwfgs.cn

[R70] 时间戳与互转
来源：http://ex.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://ex.panjiajie.cn

[R71] 日期格式化
来源：http://qg.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ju.haigaiapp.cn

[R72] 等待端口就绪
来源：http://tl.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wr.hahajie.cn

[R73] 分割大日志
来源：http://hs.asd995.cn

split -l 1000 big.log part_
来源：http://ag.521024.cn

[R74] 批量重命名
来源：http://kk.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mj.wgjwhj.cn

[R75] 导出环境变量
来源：http://cr.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://gg.bookmarksfly.cn

[R76] 使用临时文件
来源：http://da.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://it.hahajie.cn

[R77] 读取用户输入
来源：http://jh.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://fh.bookmarksfly.cn

[R78] 交互式菜单
来源：http://cb.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pi.szxytkj.cn

[R79] 解析命令行选项
来源：http://mm.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ez.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://ny.szsharing.cn

time ./run.sh
来源：http://qv.haigaiapp.cn

================================================================================
来源：http://xy.jctech888.com.cn

S. C / C++ 专题
来源：http://lf.bjjhwx.cn

================================================================================
来源：http://eo.9csxet.cn

[S01] C：Hello World
来源：http://mj.wgjwhj.cn

#include <stdio.h>
来源：http://aw.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lu.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://ty.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://bx.hnjuh.cn

[S03] C：读入整数
来源：http://av.panjiajie.cn

int x; scanf("%d", &x);
来源：http://ev.huanxung.cn

[S04] C：字符串复制
来源：http://eu.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ga.haigaiapp.cn

[S05] C：字符串长度
来源：http://hn.szsharing.cn

strlen(s)
来源：http://yy.bjjhwx.cn

[S06] C：字符串比较
来源：http://li.huixiangedu.cn

strcmp(a, b) == 0
来源：http://zq.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://af.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ve.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://fd.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nj.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://jj.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rq.muxihuayi.cn

[S10] C：指针与解引用
来源：http://yi.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://qu.hnjuh.cn

[S11] C：逐行读文件
来源：http://ix.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://yp.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rd.lnxyls.cn

fclose(f);
来源：http://xx.panjiajie.cn

[S12] C：写文件
来源：http://tq.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ql.gzmigu.cn

[S13] C：宏定义
来源：http://re.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fm.gzmigu.cn

[S14] C：枚举
来源：http://mv.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://vc.szsharing.cn

[S15] C：类型转换
来源：http://tv.colortex.cn

(double) a / b
来源：http://oy.chemitech.net.cn

[S16] C：位操作置位
来源：http://tn.521024.cn

x |= (1 << 3);
来源：http://kj.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://ad.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nw.bookmarksfly.cn

[S18] C：命令行参数
来源：http://vo.shxzskj.cn

int main(int argc, char **argv)
来源：http://vp.haigaiapp.cn

[S19] C：快速排序
来源：http://kf.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tt.huixinmuqiang.cn

[S20] C：二分查找
来源：http://iz.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kf.gzmigu.cn

[S21] C：字符类别判断
来源：http://fd.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xh.yuexingan06.cn

[S22] C：字符串转数字
来源：http://su.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://du.wgjwhj.cn

[S23] C：随机数
来源：http://aj.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zv.9csxet.cn

[S24] C：获取本地时间
来源：http://zr.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ah.521024.cn

[S25] C：内存拷贝
来源：http://zx.panjiajie.cn

memcpy(dst, src, n);
来源：http://uj.asd995.cn

[S26] C：内存清零
来源：http://qt.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://pk.colortex.cn

[S27] C：定义常量
来源：http://lz.shxzskj.cn

const double PI = 3.14159;
来源：http://qq.shxzskj.cn

[S28] C：静态变量
来源：http://cd.jianghongdianzi.cn

static int counter = 0;
来源：http://oy.muxihuayi.cn

[S29] C：变参函数
来源：http://ip.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rf.szxytkj.cn

[S30] C：头文件保护
来源：http://tr.nicolike.cn

#ifndef X_H
来源：http://oa.chemitech.net.cn

#define X_H
来源：http://bg.shxzskj.cn

#endif
来源：http://te.bjjhwx.cn

[S31] C++：Hello World
来源：http://kt.yuntaijiaju.cn

#include <iostream>
来源：http://ko.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://fm.yuntaijiaju.cn

[S32] C++：字符串
来源：http://dw.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://ph.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://iu.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sy.colortex.cn

[S34] C++：遍历 vector
来源：http://uv.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://yc.wgjwhj.cn

[S35] C++：map
来源：http://fb.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xy.hahajie.cn

[S36] C++：unordered_map
来源：http://uy.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ry.huanxung.cn

[S37] C++：set
来源：http://dm.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rq.gzmigu.cn

[S38] C++：排序
来源：http://lz.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://xp.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://hd.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ai.colortex.cn

[S40] C++：查找元素
来源：http://kq.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://we.szxytkj.cn

[S41] C++：类与构造函数
来源：http://iv.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pe.szsharing.cn

[S42] C++：继承与虚函数
来源：http://ok.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://to.shxzskj.cn

[S43] C++：智能指针
来源：http://iw.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://aw.shtwfgs.cn

[S44] C++：引用传参
来源：http://ta.hahajie.cn

void inc(int &x) { ++x; }
来源：http://sh.jianghongdianzi.cn

[S45] C++：lambda
来源：http://im.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mr.hnjuh.cn

[S46] C++：函数模板
来源：http://ud.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ez.panjiajie.cn


<!-- 参考信息 -->