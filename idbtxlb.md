代发 wailian999

[Q76] 按天统计
来源：http://up.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ts.shxzukj.cn

[Q77] 时间加减
来源：http://dk.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ts.521024.cn

[Q78] 当前时间
来源：http://wn.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ee.colortex.cn

[Q79] 字符串拼接
来源：http://lu.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ws.huanxung.cn

[Q80] 字符串截取
来源：http://bl.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jz.hahajie.cn

[Q81] 字符串替换
来源：http://gp.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vt.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://up.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uk.yuexingan06.cn

[Q83] 大小写转换
来源：http://in.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oz.shxzukj.cn

[Q84] 去除首尾空格
来源：http://mw.521024.cn

SELECT TRIM(name) FROM users;
来源：http://io.panjiajie.cn

[Q85] 数值取整
来源：http://gu.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vl.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://nv.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kt.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://mq.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qn.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://ev.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fo.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ui.521024.cn

[Q89] 判断表是否存在
来源：http://vr.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gp.szsharing.cn

[Q90] 生成序号列
来源：http://gd.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lg.521024.cn

================================================================================
来源：http://ca.hnjuh.cn

R. Bash 专题
来源：http://mb.shxzukj.cn

================================================================================
来源：http://lb.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://nl.shxzukj.cn

#!/usr/bin/env bash
来源：http://yn.yuexingan06.cn

set -euo pipefail
来源：http://ip.521024.cn

[R02] 变量赋值与使用
来源：http://ro.newstarts.cn

name="Tom"; echo "$name"
来源：http://kk.yuntaijiaju.cn

[R03] 只读变量
来源：http://br.gzmigu.cn

readonly PI=3.14
来源：http://up.lnxyls.cn

[R04] 位置参数
来源：http://le.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yq.521024.cn

[R05] 参数默认值
来源：http://ul.haigaiapp.cn

name="${1:-default}"
来源：http://ls.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://ax.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zy.521024.cn

[R07] if 判断文件
来源：http://jj.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://om.lnxyls.cn

[R08] 数值比较
来源：http://wj.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tr.shxzskj.cn

[R09] 字符串比较
来源：http://jf.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hb.huixinmuqiang.cn

[R10] 正则匹配
来源：http://xr.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dp.gzmigu.cn

[R11] case 多分支
来源：http://lx.panjiajie.cn

case "$1" in
来源：http://vr.gzmigu.cn

start) echo "启动" ;;
来源：http://eg.colortex.cn

stop)  echo "停止" ;;
来源：http://db.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://fx.lnxyls.cn

esac
来源：http://qz.huixiangedu.cn

[R12] for 遍历文件
来源：http://rq.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://sd.nicolike.cn

[R13] for 计数循环
来源：http://zj.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://rz.shtwfgs.cn

[R14] C 风格 for
来源：http://eu.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gt.newstarts.cn

[R15] while 逐行读文件
来源：http://rk.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ud.huixiangedu.cn

[R16] until 等待条件
来源：http://yz.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gp.shxzskj.cn

[R17] 数组定义与取值
来源：http://ce.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sc.bjjhwx.cn

[R18] 遍历数组
来源：http://vi.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eb.chemitech.net.cn

[R19] 数组长度
来源：http://dv.bjjhwx.cn

echo "${#arr[@]}"
来源：http://nz.szsharing.cn

[R20] 关联数组（字典）
来源：http://yc.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ns.huixinmuqiang.cn

[R21] 字符串长度
来源：http://gw.newstarts.cn

echo "${#s}"
来源：http://ka.lnxyls.cn

[R22] 截取子串
来源：http://sx.newstarts.cn

echo "${s:0:5}"
来源：http://of.colortex.cn

[R23] 字符串替换
来源：http://zg.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bo.shxzukj.cn

[R24] 大小写转换
来源：http://nv.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cf.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://jq.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xr.shxzukj.cn

[R26] 命令替换
来源：http://cp.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://vs.gzmigu.cn

[R27] 算术展开
来源：http://it.szsharing.cn

echo $((1 + 2 * 3))
来源：http://pd.hnjuh.cn

[R28] 浮点运算
来源：http://ua.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://rs.chemitech.net.cn

[R29] 定义函数
来源：http://sh.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qq.shxzskj.cn

[R30] 函数返回状态码
来源：http://wa.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://fl.gzmigu.cn

[R31] 局部变量
来源：http://ht.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://bp.hahajie.cn

[R32] 参数个数校验
来源：http://bv.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eb.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://qk.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://di.9csxet.cn

[R34] 退出时清理
来源：http://vl.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vf.9csxet.cn

[R35] 后台执行并等待
来源：http://ad.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fq.gzmigu.cn

[R36] 并发执行多个任务
来源：http://fq.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ti.asd995.cn

[R37] 把输出赋给变量
来源：http://kv.colortex.cn

files=$(ls -1)
来源：http://kh.shtwfgs.cn

[R38] 管道串联
来源：http://it.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://kc.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://qw.521024.cn

cmd > out.log 2>&1
来源：http://qk.nszjky.cn

[R40] 追加写日志
来源：http://ib.bookmarksfly.cn

echo "log" >> out.log
来源：http://hu.jctech888.com.cn

[R41] 丢弃输出
来源：http://rp.huanxung.cn

cmd >/dev/null 2>&1
来源：http://pa.bookmarksfly.cn

[R42] 输入重定向
来源：http://cy.shtwfgs.cn

wc -l < a.txt
来源：http://kj.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://ud.bjjhwx.cn

find . -name "*.log" -type f
来源：http://po.muxihuayi.cn

[R44] 按修改时间查找
来源：http://up.nicolike.cn

find . -mtime -7 -type f
来源：http://ja.szxytkj.cn

[R45] 批量删除
来源：http://fz.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://le.hnjuh.cn

[R46] 递归替换文件内容
来源：http://ph.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yu.asd995.cn

[R47] sed 单行替换
来源：http://mt.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vo.bookmarksfly.cn

[R48] awk 取指定列
来源：http://sb.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://rl.bookmarksfly.cn

[R49] awk 带条件
来源：http://vj.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://za.chemitech.net.cn

[R50] awk 求和
来源：http://kj.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zd.haigaiapp.cn

[R51] 排序去重取前几
来源：http://ef.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dw.jctech888.com.cn

[R52] 统计行数
来源：http://th.szsharing.cn

wc -l a.txt
来源：http://om.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://tn.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iw.nszjky.cn

[R54] 比较两个文件
来源：http://nv.nicolike.cn

diff a.txt b.txt
来源：http://ac.shxzskj.cn

[R55] 压缩与解压
来源：http://wb.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mi.muxihuayi.cn

[R56] 远程拷贝
来源：http://ug.hahajie.cn

scp file user@host:/path/
来源：http://ed.chemitech.net.cn

[R57] 远程执行命令
来源：http://mu.jctech888.com.cn

ssh user@host 'uptime'
来源：http://fb.shtwfgs.cn

[R58] 下载文件
来源：http://er.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hx.bjjhwx.cn

[R59] 发 POST JSON
来源：http://ee.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ze.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://fg.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lu.muxihuayi.cn

[R61] 磁盘占用
来源：http://rl.huixinmuqiang.cn

df -h;  du -sh *
来源：http://ob.nszjky.cn

[R62] 找最占空间的文件
来源：http://dz.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://sn.newstarts.cn

[R63] 内存与进程
来源：http://cb.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://mt.yuexingan06.cn

[R64] 结束进程
来源：http://ae.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://mr.shxzukj.cn

[R65] 查看端口占用
来源：http://sw.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ie.panjiajie.cn

[R66] 定时任务
来源：http://dp.521024.cn

crontab -e;  crontab -l
来源：http://jb.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://lw.asd995.cn

openssl rand -hex 16
来源：http://uv.hnjuh.cn

[R68] 计算文件校验值
来源：http://ys.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vs.shxzukj.cn

[R69] 生成随机密码
来源：http://sp.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://wx.huixiangedu.cn

[R70] 时间戳与互转
来源：http://sc.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://jb.szxytkj.cn

[R71] 日期格式化
来源：http://yk.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nv.hnjuh.cn

[R72] 等待端口就绪
来源：http://zd.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xt.newstarts.cn

[R73] 分割大日志
来源：http://at.shxzukj.cn

split -l 1000 big.log part_
来源：http://is.9csxet.cn

[R74] 批量重命名
来源：http://qm.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ar.shxzukj.cn

[R75] 导出环境变量
来源：http://ki.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://mm.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://fc.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dt.hahajie.cn

[R77] 读取用户输入
来源：http://pm.gzmigu.cn

read -rp "请输入: " ans
来源：http://fz.nicolike.cn

[R78] 交互式菜单
来源：http://fn.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://li.shtwfgs.cn

[R79] 解析命令行选项
来源：http://in.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rz.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://jn.hnjuh.cn

time ./run.sh
来源：http://xr.muxihuayi.cn

================================================================================
来源：http://od.yuexingan06.cn

S. C / C++ 专题
来源：http://iv.shxzskj.cn

================================================================================
来源：http://so.haigaiapp.cn

[S01] C：Hello World
来源：http://wo.chemitech.net.cn

#include <stdio.h>
来源：http://cg.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ik.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://zw.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://da.newstarts.cn

[S03] C：读入整数
来源：http://hq.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://ap.jctech888.com.cn

[S04] C：字符串复制
来源：http://ee.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fh.huixiangedu.cn

[S05] C：字符串长度
来源：http://oc.chemitech.net.cn

strlen(s)
来源：http://mw.asd995.cn

[S06] C：字符串比较
来源：http://gq.wgjwhj.cn

strcmp(a, b) == 0
来源：http://vu.gzmigu.cn

[S07] C：数组遍历求和
来源：http://jo.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ey.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://tj.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://db.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://ds.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xe.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://hn.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://rm.huixiangedu.cn

[S11] C：逐行读文件
来源：http://mn.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://ui.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wr.yuntaijiaju.cn

fclose(f);
来源：http://cf.wgjwhj.cn

[S12] C：写文件
来源：http://cj.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rb.shtwfgs.cn

[S13] C：宏定义
来源：http://bi.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yw.huanxung.cn

[S14] C：枚举
来源：http://ca.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ec.bookmarksfly.cn

[S15] C：类型转换
来源：http://do.yuexingan06.cn

(double) a / b
来源：http://ff.hahajie.cn

[S16] C：位操作置位
来源：http://fd.nszjky.cn

x |= (1 << 3);
来源：http://ys.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://go.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gj.hnjuh.cn

[S18] C：命令行参数
来源：http://dy.colortex.cn

int main(int argc, char **argv)
来源：http://pw.muxihuayi.cn

[S19] C：快速排序
来源：http://lq.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yq.yuexingan06.cn

[S20] C：二分查找
来源：http://jh.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wq.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://ya.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xl.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://el.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vm.huixiangedu.cn

[S23] C：随机数
来源：http://tg.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lq.hahajie.cn

[S24] C：获取本地时间
来源：http://jm.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gr.colortex.cn

[S25] C：内存拷贝
来源：http://wr.bjjhwx.cn

memcpy(dst, src, n);
来源：http://dw.hahajie.cn

[S26] C：内存清零
来源：http://tw.szsharing.cn

memset(a, 0, sizeof a);
来源：http://yz.jctech888.com.cn

[S27] C：定义常量
来源：http://wg.jctech888.com.cn

const double PI = 3.14159;
来源：http://yj.bookmarksfly.cn

[S28] C：静态变量
来源：http://mz.huixiangedu.cn

static int counter = 0;
来源：http://jy.panjiajie.cn

[S29] C：变参函数
来源：http://qn.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hi.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://rb.jctech888.com.cn

#ifndef X_H
来源：http://us.jctech888.com.cn

#define X_H
来源：http://li.szsharing.cn

#endif
来源：http://ic.lnxyls.cn

[S31] C++：Hello World
来源：http://bc.bookmarksfly.cn

#include <iostream>
来源：http://mp.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://ue.yuexingan06.cn

[S32] C++：字符串
来源：http://pw.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://oc.muxihuayi.cn

[S33] C++：vector 增删
来源：http://rj.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wd.shxzskj.cn

[S34] C++：遍历 vector
来源：http://tb.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://it.huanxung.cn

[S35] C++：map
来源：http://qg.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wg.szxytkj.cn

[S36] C++：unordered_map
来源：http://sr.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ki.lnxyls.cn

[S37] C++：set
来源：http://zv.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ja.jctech888.com.cn

[S38] C++：排序
来源：http://bs.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://ij.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://rl.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mh.hnjuh.cn

[S40] C++：查找元素
来源：http://si.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jg.szxytkj.cn

[S41] C++：类与构造函数
来源：http://ny.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xm.nicolike.cn

[S42] C++：继承与虚函数
来源：http://bt.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://nk.shxzukj.cn

[S43] C++：智能指针
来源：http://wk.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://un.panjiajie.cn

[S44] C++：引用传参
来源：http://th.szsharing.cn

void inc(int &x) { ++x; }
来源：http://bz.huixiangedu.cn

[S45] C++：lambda
来源：http://nt.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ph.huanxung.cn

[S46] C++：函数模板
来源：http://qd.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lw.521024.cn


<!-- 参考信息 -->