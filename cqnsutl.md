代发 wailian999

[Q78] 当前时间
来源：http://vd.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gq.521024.cn

[Q79] 字符串拼接
来源：http://kz.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ii.newstarts.cn

[Q80] 字符串截取
来源：http://ax.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ft.haigaiapp.cn

[Q81] 字符串替换
来源：http://bf.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lz.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://zn.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pk.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://si.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://va.521024.cn

[Q84] 去除首尾空格
来源：http://yg.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://iy.muxihuayi.cn

[Q85] 数值取整
来源：http://ty.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wg.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://od.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ee.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://hr.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jw.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://rp.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hg.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qt.huanxung.cn

[Q89] 判断表是否存在
来源：http://nu.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oh.chemitech.net.cn

[Q90] 生成序号列
来源：http://fg.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://de.jianghongdianzi.cn

================================================================================
来源：http://rp.wgjwhj.cn

R. Bash 专题
来源：http://rw.shtwfgs.cn

================================================================================
来源：http://sr.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://eh.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://hb.szxytkj.cn

set -euo pipefail
来源：http://dl.nszjky.cn

[R02] 变量赋值与使用
来源：http://zn.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://jh.yuexingan06.cn

[R03] 只读变量
来源：http://rs.shxzukj.cn

readonly PI=3.14
来源：http://lr.asd995.cn

[R04] 位置参数
来源：http://ah.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kb.bjjhwx.cn

[R05] 参数默认值
来源：http://jf.shxzskj.cn

name="${1:-default}"
来源：http://qr.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://ee.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nf.huixinmuqiang.cn

[R07] if 判断文件
来源：http://th.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ze.szsharing.cn

[R08] 数值比较
来源：http://se.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fr.shxzskj.cn

[R09] 字符串比较
来源：http://vb.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hm.shtwfgs.cn

[R10] 正则匹配
来源：http://lv.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sy.jctech888.com.cn

[R11] case 多分支
来源：http://to.chemitech.net.cn

case "$1" in
来源：http://qo.colortex.cn

start) echo "启动" ;;
来源：http://kj.hahajie.cn

stop)  echo "停止" ;;
来源：http://kb.huixinmuqiang.cn

*)     echo "未知命令" ;;
来源：http://wo.yuexingan06.cn

esac
来源：http://fb.muxihuayi.cn

[R12] for 遍历文件
来源：http://pf.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://jt.newstarts.cn

[R13] for 计数循环
来源：http://wh.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://ns.wgjwhj.cn

[R14] C 风格 for
来源：http://qo.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ws.shxzskj.cn

[R15] while 逐行读文件
来源：http://nl.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vg.newstarts.cn

[R16] until 等待条件
来源：http://vd.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wk.hnjuh.cn

[R17] 数组定义与取值
来源：http://gt.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ou.gzmigu.cn

[R18] 遍历数组
来源：http://my.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rk.wgjwhj.cn

[R19] 数组长度
来源：http://rq.lnxyls.cn

echo "${#arr[@]}"
来源：http://cn.newstarts.cn

[R20] 关联数组（字典）
来源：http://cg.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gw.bjjhwx.cn

[R21] 字符串长度
来源：http://fa.huanxung.cn

echo "${#s}"
来源：http://um.panjiajie.cn

[R22] 截取子串
来源：http://tu.panjiajie.cn

echo "${s:0:5}"
来源：http://yn.nicolike.cn

[R23] 字符串替换
来源：http://oj.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cc.chemitech.net.cn

[R24] 大小写转换
来源：http://pd.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vv.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://nd.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://df.newstarts.cn

[R26] 命令替换
来源：http://hs.521024.cn

now=$(date +%F); echo "$now"
来源：http://np.shxzskj.cn

[R27] 算术展开
来源：http://kx.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://zd.bookmarksfly.cn

[R28] 浮点运算
来源：http://ki.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://vx.521024.cn

[R29] 定义函数
来源：http://oi.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fy.nszjky.cn

[R30] 函数返回状态码
来源：http://io.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://ha.9csxet.cn

[R31] 局部变量
来源：http://tw.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://ve.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://wf.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jo.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://sa.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zv.wgjwhj.cn

[R34] 退出时清理
来源：http://fj.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vd.nszjky.cn

[R35] 后台执行并等待
来源：http://db.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qq.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://rw.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lb.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://af.huixiangedu.cn

files=$(ls -1)
来源：http://cr.bookmarksfly.cn

[R38] 管道串联
来源：http://wz.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://la.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://qm.asd995.cn

cmd > out.log 2>&1
来源：http://fn.szsharing.cn

[R40] 追加写日志
来源：http://yd.jctech888.com.cn

echo "log" >> out.log
来源：http://tv.gzmigu.cn

[R41] 丢弃输出
来源：http://ac.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://pi.huanxung.cn

[R42] 输入重定向
来源：http://ia.lnxyls.cn

wc -l < a.txt
来源：http://hl.szsharing.cn

[R43] 按名字查找文件
来源：http://cd.hahajie.cn

find . -name "*.log" -type f
来源：http://aw.haigaiapp.cn

[R44] 按修改时间查找
来源：http://pb.wgjwhj.cn

find . -mtime -7 -type f
来源：http://dt.panjiajie.cn

[R45] 批量删除
来源：http://vu.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://tj.shxzskj.cn

[R46] 递归替换文件内容
来源：http://jq.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yv.nszjky.cn

[R47] sed 单行替换
来源：http://yh.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hf.gzmigu.cn

[R48] awk 取指定列
来源：http://ne.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://oj.bjjhwx.cn

[R49] awk 带条件
来源：http://jx.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bd.bookmarksfly.cn

[R50] awk 求和
来源：http://oo.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yy.521024.cn

[R51] 排序去重取前几
来源：http://pa.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ec.asd995.cn

[R52] 统计行数
来源：http://ha.wgjwhj.cn

wc -l a.txt
来源：http://am.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://hk.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uq.bjjhwx.cn

[R54] 比较两个文件
来源：http://lh.jctech888.com.cn

diff a.txt b.txt
来源：http://kf.huixiangedu.cn

[R55] 压缩与解压
来源：http://eu.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kf.huixiangedu.cn

[R56] 远程拷贝
来源：http://uu.huanxung.cn

scp file user@host:/path/
来源：http://cy.szxytkj.cn

[R57] 远程执行命令
来源：http://sd.yuexingan06.cn

ssh user@host 'uptime'
来源：http://rb.huixiangedu.cn

[R58] 下载文件
来源：http://zw.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fr.szxytkj.cn

[R59] 发 POST JSON
来源：http://my.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ku.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://tu.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://at.nszjky.cn

[R61] 磁盘占用
来源：http://du.9csxet.cn

df -h;  du -sh *
来源：http://le.hahajie.cn

[R62] 找最占空间的文件
来源：http://je.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://pu.gzmigu.cn

[R63] 内存与进程
来源：http://dn.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://lp.newstarts.cn

[R64] 结束进程
来源：http://jp.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://xk.panjiajie.cn

[R65] 查看端口占用
来源：http://ll.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fy.colortex.cn

[R66] 定时任务
来源：http://mv.hahajie.cn

crontab -e;  crontab -l
来源：http://sl.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://lx.newstarts.cn

openssl rand -hex 16
来源：http://mm.nszjky.cn

[R68] 计算文件校验值
来源：http://ly.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zu.szsharing.cn

[R69] 生成随机密码
来源：http://om.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://mg.haigaiapp.cn

[R70] 时间戳与互转
来源：http://il.newstarts.cn

date +%s;  date -d @1700000000
来源：http://xz.gzmigu.cn

[R71] 日期格式化
来源：http://ls.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ve.9csxet.cn

[R72] 等待端口就绪
来源：http://zs.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wd.newstarts.cn

[R73] 分割大日志
来源：http://vj.bjjhwx.cn

split -l 1000 big.log part_
来源：http://et.nszjky.cn

[R74] 批量重命名
来源：http://lq.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ri.521024.cn

[R75] 导出环境变量
来源：http://pr.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://iq.jctech888.com.cn

[R76] 使用临时文件
来源：http://ju.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vi.yuexingan06.cn

[R77] 读取用户输入
来源：http://hx.bjjhwx.cn

read -rp "请输入: " ans
来源：http://xe.shtwfgs.cn

[R78] 交互式菜单
来源：http://iw.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hi.lnxyls.cn

[R79] 解析命令行选项
来源：http://du.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ce.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://jq.huanxung.cn

time ./run.sh
来源：http://dw.szsharing.cn

================================================================================
来源：http://us.yuexingan06.cn

S. C / C++ 专题
来源：http://eo.asd995.cn

================================================================================
来源：http://gq.nszjky.cn

[S01] C：Hello World
来源：http://nl.lnxyls.cn

#include <stdio.h>
来源：http://sw.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bh.asd995.cn

[S02] C：变量与格式化输出
来源：http://bp.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://ka.huanxung.cn

[S03] C：读入整数
来源：http://tt.hnjuh.cn

int x; scanf("%d", &x);
来源：http://cn.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://wb.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cz.hahajie.cn

[S05] C：字符串长度
来源：http://fk.hnjuh.cn

strlen(s)
来源：http://fp.huixiangedu.cn

[S06] C：字符串比较
来源：http://zl.nszjky.cn

strcmp(a, b) == 0
来源：http://hp.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://jy.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ac.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://bb.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mm.521024.cn

[S09] C：结构体定义与初始化
来源：http://ty.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lg.haigaiapp.cn

[S10] C：指针与解引用
来源：http://rk.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://no.lnxyls.cn

[S11] C：逐行读文件
来源：http://vi.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://da.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gf.szxytkj.cn

fclose(f);
来源：http://bv.shxzskj.cn

[S12] C：写文件
来源：http://hf.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://or.haigaiapp.cn

[S13] C：宏定义
来源：http://ab.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pj.hahajie.cn

[S14] C：枚举
来源：http://qm.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://ga.huixinmuqiang.cn

[S15] C：类型转换
来源：http://fn.lnxyls.cn

(double) a / b
来源：http://te.jctech888.com.cn

[S16] C：位操作置位
来源：http://pk.9csxet.cn

x |= (1 << 3);
来源：http://ln.9csxet.cn

[S17] C：安全拼接字符串
来源：http://ip.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ix.bjjhwx.cn

[S18] C：命令行参数
来源：http://vj.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://bh.panjiajie.cn

[S19] C：快速排序
来源：http://tx.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ml.jianghongdianzi.cn

[S20] C：二分查找
来源：http://jj.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uo.szsharing.cn

[S21] C：字符类别判断
来源：http://ks.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hr.huixiangedu.cn

[S22] C：字符串转数字
来源：http://wu.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hv.bjjhwx.cn

[S23] C：随机数
来源：http://cr.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vg.521024.cn

[S24] C：获取本地时间
来源：http://ew.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ji.shtwfgs.cn

[S25] C：内存拷贝
来源：http://lq.gzmigu.cn

memcpy(dst, src, n);
来源：http://tl.shtwfgs.cn

[S26] C：内存清零
来源：http://iw.newstarts.cn

memset(a, 0, sizeof a);
来源：http://ch.shxzukj.cn

[S27] C：定义常量
来源：http://oq.lnxyls.cn

const double PI = 3.14159;
来源：http://lf.gzmigu.cn

[S28] C：静态变量
来源：http://ql.gzmigu.cn

static int counter = 0;
来源：http://jt.huixinmuqiang.cn

[S29] C：变参函数
来源：http://ua.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gz.gzmigu.cn

[S30] C：头文件保护
来源：http://in.huixiangedu.cn

#ifndef X_H
来源：http://kz.shxzskj.cn

#define X_H
来源：http://hk.huixinmuqiang.cn

#endif
来源：http://tl.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://gb.nicolike.cn

#include <iostream>
来源：http://pg.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://fb.bjjhwx.cn

[S32] C++：字符串
来源：http://vn.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://ot.muxihuayi.cn

[S33] C++：vector 增删
来源：http://wf.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ox.szxytkj.cn

[S34] C++：遍历 vector
来源：http://uw.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://xm.nicolike.cn

[S35] C++：map
来源：http://we.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wj.wgjwhj.cn

[S36] C++：unordered_map
来源：http://mj.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eh.shxzukj.cn

[S37] C++：set
来源：http://rz.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ye.jianghongdianzi.cn

[S38] C++：排序
来源：http://wp.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://aw.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://mq.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yk.chemitech.net.cn

[S40] C++：查找元素
来源：http://lf.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vn.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://eg.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oa.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://gm.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://lp.jctech888.com.cn

[S43] C++：智能指针
来源：http://sp.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://yo.nszjky.cn

[S44] C++：引用传参
来源：http://mu.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://hc.gzmigu.cn

[S45] C++：lambda
来源：http://gs.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qt.shxzskj.cn

[S46] C++：函数模板
来源：http://jb.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://il.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://lg.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://js.newstarts.cn

[S48] C++：逐行读文件
来源：http://yc.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tl.szxytkj.cn


<!-- 参考信息 -->