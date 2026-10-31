代发 wailian999

[Q76] 按天统计
来源：http://bm.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://at.521024.cn

[Q77] 时间加减
来源：http://dg.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zb.haigaiapp.cn

[Q78] 当前时间
来源：http://sq.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wj.nicolike.cn

[Q79] 字符串拼接
来源：http://ro.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://en.bookmarksfly.cn

[Q80] 字符串截取
来源：http://rp.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xm.hnjuh.cn

[Q81] 字符串替换
来源：http://yn.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nu.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://is.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ny.521024.cn

[Q83] 大小写转换
来源：http://dm.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ly.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://pe.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://qs.jianghongdianzi.cn

[Q85] 数值取整
来源：http://hh.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cl.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://ks.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ep.hahajie.cn

[Q87] JSON 字段做条件
来源：http://fn.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hk.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://fp.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lm.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://so.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://ss.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wf.newstarts.cn

[Q90] 生成序号列
来源：http://wd.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ck.shxzskj.cn

================================================================================
来源：http://qb.lnxyls.cn

R. Bash 专题
来源：http://jk.shtwfgs.cn

================================================================================
来源：http://xy.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://qu.huanxung.cn

#!/usr/bin/env bash
来源：http://dr.szsharing.cn

set -euo pipefail
来源：http://au.newstarts.cn

[R02] 变量赋值与使用
来源：http://ak.521024.cn

name="Tom"; echo "$name"
来源：http://ih.jctech888.com.cn

[R03] 只读变量
来源：http://ku.shtwfgs.cn

readonly PI=3.14
来源：http://tx.hnjuh.cn

[R04] 位置参数
来源：http://oo.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://am.hnjuh.cn

[R05] 参数默认值
来源：http://kq.colortex.cn

name="${1:-default}"
来源：http://ko.shxzukj.cn

[R06] 判断命令是否存在
来源：http://sp.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jp.panjiajie.cn

[R07] if 判断文件
来源：http://ml.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mh.wgjwhj.cn

[R08] 数值比较
来源：http://od.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tl.shxzskj.cn

[R09] 字符串比较
来源：http://wv.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lo.gzmigu.cn

[R10] 正则匹配
来源：http://vc.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gx.nicolike.cn

[R11] case 多分支
来源：http://lr.jianghongdianzi.cn

case "$1" in
来源：http://aq.nszjky.cn

start) echo "启动" ;;
来源：http://lx.newstarts.cn

stop)  echo "停止" ;;
来源：http://bc.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://kh.jianghongdianzi.cn

esac
来源：http://rw.lnxyls.cn

[R12] for 遍历文件
来源：http://ap.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://lb.hahajie.cn

[R13] for 计数循环
来源：http://bl.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://dl.yuexingan06.cn

[R14] C 风格 for
来源：http://gp.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ll.newstarts.cn

[R15] while 逐行读文件
来源：http://qf.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cs.muxihuayi.cn

[R16] until 等待条件
来源：http://uq.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pg.521024.cn

[R17] 数组定义与取值
来源：http://qq.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zc.huanxung.cn

[R18] 遍历数组
来源：http://ok.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nz.szxytkj.cn

[R19] 数组长度
来源：http://kw.shxzukj.cn

echo "${#arr[@]}"
来源：http://jv.hahajie.cn

[R20] 关联数组（字典）
来源：http://vc.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xf.shtwfgs.cn

[R21] 字符串长度
来源：http://va.colortex.cn

echo "${#s}"
来源：http://ti.shxzukj.cn

[R22] 截取子串
来源：http://zw.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://kd.jianghongdianzi.cn

[R23] 字符串替换
来源：http://ps.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://an.hnjuh.cn

[R24] 大小写转换
来源：http://uf.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zb.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://cf.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qm.szxytkj.cn

[R26] 命令替换
来源：http://qg.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://va.szsharing.cn

[R27] 算术展开
来源：http://ps.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://mc.nszjky.cn

[R28] 浮点运算
来源：http://km.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://zb.haigaiapp.cn

[R29] 定义函数
来源：http://dl.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wj.lnxyls.cn

[R30] 函数返回状态码
来源：http://du.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://jo.huanxung.cn

[R31] 局部变量
来源：http://rz.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://tk.nicolike.cn

[R32] 参数个数校验
来源：http://rv.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wb.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://jr.szxytkj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wg.yuexingan06.cn

[R34] 退出时清理
来源：http://ud.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zc.shxzskj.cn

[R35] 后台执行并等待
来源：http://fb.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jj.gzmigu.cn

[R36] 并发执行多个任务
来源：http://kr.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tu.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://ry.colortex.cn

files=$(ls -1)
来源：http://qw.chemitech.net.cn

[R38] 管道串联
来源：http://sk.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://js.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://zx.lnxyls.cn

cmd > out.log 2>&1
来源：http://go.szxytkj.cn

[R40] 追加写日志
来源：http://od.nszjky.cn

echo "log" >> out.log
来源：http://qx.521024.cn

[R41] 丢弃输出
来源：http://yy.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://he.szsharing.cn

[R42] 输入重定向
来源：http://hz.hahajie.cn

wc -l < a.txt
来源：http://qy.shtwfgs.cn

[R43] 按名字查找文件
来源：http://bv.chemitech.net.cn

find . -name "*.log" -type f
来源：http://gz.hahajie.cn

[R44] 按修改时间查找
来源：http://zg.chemitech.net.cn

find . -mtime -7 -type f
来源：http://uj.panjiajie.cn

[R45] 批量删除
来源：http://du.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://bs.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://qx.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ur.9csxet.cn

[R47] sed 单行替换
来源：http://zf.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ox.bookmarksfly.cn

[R48] awk 取指定列
来源：http://qe.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://il.huanxung.cn

[R49] awk 带条件
来源：http://fm.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jq.lnxyls.cn

[R50] awk 求和
来源：http://hs.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cy.shxzskj.cn

[R51] 排序去重取前几
来源：http://il.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tz.gzmigu.cn

[R52] 统计行数
来源：http://ta.chemitech.net.cn

wc -l a.txt
来源：http://lq.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://ak.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://as.panjiajie.cn

[R54] 比较两个文件
来源：http://vd.newstarts.cn

diff a.txt b.txt
来源：http://mn.colortex.cn

[R55] 压缩与解压
来源：http://ss.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cp.bjjhwx.cn

[R56] 远程拷贝
来源：http://cq.nicolike.cn

scp file user@host:/path/
来源：http://mh.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://ec.shxzskj.cn

ssh user@host 'uptime'
来源：http://ye.panjiajie.cn

[R58] 下载文件
来源：http://fb.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pd.lnxyls.cn

[R59] 发 POST JSON
来源：http://cl.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yk.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://xn.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wf.szsharing.cn

[R61] 磁盘占用
来源：http://vg.shxzukj.cn

df -h;  du -sh *
来源：http://iz.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://xr.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://oh.521024.cn

[R63] 内存与进程
来源：http://jq.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://lv.colortex.cn

[R64] 结束进程
来源：http://pa.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://xs.bookmarksfly.cn

[R65] 查看端口占用
来源：http://zi.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ju.huixinmuqiang.cn

[R66] 定时任务
来源：http://ei.hnjuh.cn

crontab -e;  crontab -l
来源：http://ba.nicolike.cn

[R67] 生成随机十六进制串
来源：http://tt.yuexingan06.cn

openssl rand -hex 16
来源：http://ds.newstarts.cn

[R68] 计算文件校验值
来源：http://jc.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://by.shxzukj.cn

[R69] 生成随机密码
来源：http://oa.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://cs.szsharing.cn

[R70] 时间戳与互转
来源：http://uf.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://pn.haigaiapp.cn

[R71] 日期格式化
来源：http://if.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://db.newstarts.cn

[R72] 等待端口就绪
来源：http://ev.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vz.huixiangedu.cn

[R73] 分割大日志
来源：http://zy.hnjuh.cn

split -l 1000 big.log part_
来源：http://uo.gzmigu.cn

[R74] 批量重命名
来源：http://ty.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ys.huanxung.cn

[R75] 导出环境变量
来源：http://vl.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://gl.nszjky.cn

[R76] 使用临时文件
来源：http://qe.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rf.szsharing.cn

[R77] 读取用户输入
来源：http://pv.newstarts.cn

read -rp "请输入: " ans
来源：http://ri.newstarts.cn

[R78] 交互式菜单
来源：http://xe.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pq.szsharing.cn

[R79] 解析命令行选项
来源：http://ha.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ji.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://hd.huanxung.cn

time ./run.sh
来源：http://bj.wgjwhj.cn

================================================================================
来源：http://rm.nicolike.cn

S. C / C++ 专题
来源：http://gb.shxzskj.cn

================================================================================
来源：http://wf.panjiajie.cn

[S01] C：Hello World
来源：http://zs.huixinmuqiang.cn

#include <stdio.h>
来源：http://ul.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fe.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://ki.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://bd.chemitech.net.cn

[S03] C：读入整数
来源：http://le.shxzukj.cn

int x; scanf("%d", &x);
来源：http://mv.521024.cn

[S04] C：字符串复制
来源：http://yt.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kw.gzmigu.cn

[S05] C：字符串长度
来源：http://tm.jctech888.com.cn

strlen(s)
来源：http://oq.gzmigu.cn

[S06] C：字符串比较
来源：http://tj.shtwfgs.cn

strcmp(a, b) == 0
来源：http://id.asd995.cn

[S07] C：数组遍历求和
来源：http://th.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zg.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://jb.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://td.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://rr.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sh.shtwfgs.cn

[S10] C：指针与解引用
来源：http://ly.newstarts.cn

int *p = &a;  *p = 5;
来源：http://pj.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://bk.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://tb.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tb.shxzskj.cn

fclose(f);
来源：http://yw.huanxung.cn

[S12] C：写文件
来源：http://an.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ff.newstarts.cn

[S13] C：宏定义
来源：http://mv.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yt.yuexingan06.cn

[S14] C：枚举
来源：http://nb.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://ap.panjiajie.cn

[S15] C：类型转换
来源：http://xw.szxytkj.cn

(double) a / b
来源：http://hl.newstarts.cn

[S16] C：位操作置位
来源：http://wg.yuexingan06.cn

x |= (1 << 3);
来源：http://jn.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://rr.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yr.haigaiapp.cn

[S18] C：命令行参数
来源：http://es.colortex.cn

int main(int argc, char **argv)
来源：http://xe.bookmarksfly.cn

[S19] C：快速排序
来源：http://gy.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://du.bjjhwx.cn

[S20] C：二分查找
来源：http://sr.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://io.9csxet.cn

[S21] C：字符类别判断
来源：http://gn.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ou.nszjky.cn

[S22] C：字符串转数字
来源：http://ww.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ox.shtwfgs.cn

[S23] C：随机数
来源：http://hc.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gt.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://qp.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sl.muxihuayi.cn

[S25] C：内存拷贝
来源：http://cy.newstarts.cn

memcpy(dst, src, n);
来源：http://ed.newstarts.cn

[S26] C：内存清零
来源：http://ky.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://fl.huixiangedu.cn

[S27] C：定义常量
来源：http://yq.9csxet.cn

const double PI = 3.14159;
来源：http://qx.yuntaijiaju.cn

[S28] C：静态变量
来源：http://ca.lnxyls.cn

static int counter = 0;
来源：http://vk.huanxung.cn

[S29] C：变参函数
来源：http://wz.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yw.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://na.wgjwhj.cn

#ifndef X_H
来源：http://wy.lnxyls.cn

#define X_H
来源：http://se.szxytkj.cn

#endif
来源：http://oi.haigaiapp.cn

[S31] C++：Hello World
来源：http://zp.nicolike.cn

#include <iostream>
来源：http://ru.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://qo.haigaiapp.cn

[S32] C++：字符串
来源：http://pj.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://bm.521024.cn

[S33] C++：vector 增删
来源：http://dw.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gt.lnxyls.cn

[S34] C++：遍历 vector
来源：http://hf.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://ox.yuexingan06.cn

[S35] C++：map
来源：http://ds.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nr.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://uv.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://af.9csxet.cn

[S37] C++：set
来源：http://bo.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hb.shxzskj.cn

[S38] C++：排序
来源：http://kf.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://zi.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://eh.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://js.panjiajie.cn

[S40] C++：查找元素
来源：http://dg.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dg.panjiajie.cn

[S41] C++：类与构造函数
来源：http://ce.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vf.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://pz.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://yu.nszjky.cn

[S43] C++：智能指针
来源：http://xn.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://id.muxihuayi.cn

[S44] C++：引用传参
来源：http://gw.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://pl.nszjky.cn

[S45] C++：lambda
来源：http://sj.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kx.nszjky.cn

[S46] C++：函数模板
来源：http://kb.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pa.nszjky.cn


<!-- 参考信息 -->