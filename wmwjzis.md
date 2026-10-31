代发 wailian999

[Q78] 当前时间
来源：http://va.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zj.haigaiapp.cn

[Q79] 字符串拼接
来源：http://ox.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ni.hnjuh.cn

[Q80] 字符串截取
来源：http://bz.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pp.huixiangedu.cn

[Q81] 字符串替换
来源：http://sk.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gp.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://lw.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qo.hnjuh.cn

[Q83] 大小写转换
来源：http://up.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wf.lnxyls.cn

[Q84] 去除首尾空格
来源：http://me.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://oi.panjiajie.cn

[Q85] 数值取整
来源：http://rf.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://it.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://zd.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pk.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://co.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ir.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://bs.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mf.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vz.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://vk.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gz.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://av.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jq.shxzskj.cn

================================================================================
来源：http://fa.9csxet.cn

R. Bash 专题
来源：http://oo.muxihuayi.cn

================================================================================
来源：http://wc.szsharing.cn

[R01] shebang 与严格模式
来源：http://ir.szsharing.cn

#!/usr/bin/env bash
来源：http://vd.hnjuh.cn

set -euo pipefail
来源：http://ig.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://az.hahajie.cn

name="Tom"; echo "$name"
来源：http://xw.jctech888.com.cn

[R03] 只读变量
来源：http://vz.chemitech.net.cn

readonly PI=3.14
来源：http://ec.shxzukj.cn

[R04] 位置参数
来源：http://vz.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ko.colortex.cn

[R05] 参数默认值
来源：http://au.newstarts.cn

name="${1:-default}"
来源：http://lo.szxytkj.cn

[R06] 判断命令是否存在
来源：http://ne.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gi.shxzukj.cn

[R07] if 判断文件
来源：http://az.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tn.lnxyls.cn

[R08] 数值比较
来源：http://tf.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://br.jianghongdianzi.cn

[R09] 字符串比较
来源：http://sw.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oy.jianghongdianzi.cn

[R10] 正则匹配
来源：http://gf.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dj.521024.cn

[R11] case 多分支
来源：http://si.hnjuh.cn

case "$1" in
来源：http://me.colortex.cn

start) echo "启动" ;;
来源：http://hd.nicolike.cn

stop)  echo "停止" ;;
来源：http://bg.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://nb.jctech888.com.cn

esac
来源：http://wr.gzmigu.cn

[R12] for 遍历文件
来源：http://zc.bjjhwx.cn

for f in *.txt; do echo "$f"; done
来源：http://gz.colortex.cn

[R13] for 计数循环
来源：http://se.asd995.cn

for i in {1..10}; do echo "$i"; done
来源：http://ci.yuntaijiaju.cn

[R14] C 风格 for
来源：http://gh.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://og.szxytkj.cn

[R15] while 逐行读文件
来源：http://jj.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jl.shtwfgs.cn

[R16] until 等待条件
来源：http://uc.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tt.newstarts.cn

[R17] 数组定义与取值
来源：http://ry.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qz.shxzukj.cn

[R18] 遍历数组
来源：http://eh.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gd.asd995.cn

[R19] 数组长度
来源：http://dy.asd995.cn

echo "${#arr[@]}"
来源：http://go.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://pg.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ai.shxzukj.cn

[R21] 字符串长度
来源：http://jt.jianghongdianzi.cn

echo "${#s}"
来源：http://xv.521024.cn

[R22] 截取子串
来源：http://ff.gzmigu.cn

echo "${s:0:5}"
来源：http://vn.huixiangedu.cn

[R23] 字符串替换
来源：http://wr.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://is.szsharing.cn

[R24] 大小写转换
来源：http://yg.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sg.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://hx.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://za.hahajie.cn

[R26] 命令替换
来源：http://vm.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://ck.521024.cn

[R27] 算术展开
来源：http://vv.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://bq.chemitech.net.cn

[R28] 浮点运算
来源：http://cl.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://zk.hahajie.cn

[R29] 定义函数
来源：http://fv.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ur.wgjwhj.cn

[R30] 函数返回状态码
来源：http://wl.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://oo.shxzukj.cn

[R31] 局部变量
来源：http://rf.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://tl.wgjwhj.cn

[R32] 参数个数校验
来源：http://gn.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gy.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://fs.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ej.jianghongdianzi.cn

[R34] 退出时清理
来源：http://vr.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nn.newstarts.cn

[R35] 后台执行并等待
来源：http://dv.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oh.nszjky.cn

[R36] 并发执行多个任务
来源：http://uu.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wk.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://bx.jctech888.com.cn

files=$(ls -1)
来源：http://sq.colortex.cn

[R38] 管道串联
来源：http://gk.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://gl.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://ey.asd995.cn

cmd > out.log 2>&1
来源：http://rp.muxihuayi.cn

[R40] 追加写日志
来源：http://zj.shxzukj.cn

echo "log" >> out.log
来源：http://do.panjiajie.cn

[R41] 丢弃输出
来源：http://gv.9csxet.cn

cmd >/dev/null 2>&1
来源：http://qp.jianghongdianzi.cn

[R42] 输入重定向
来源：http://gj.chemitech.net.cn

wc -l < a.txt
来源：http://zp.521024.cn

[R43] 按名字查找文件
来源：http://tz.bjjhwx.cn

find . -name "*.log" -type f
来源：http://ct.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://xi.yuexingan06.cn

find . -mtime -7 -type f
来源：http://tr.shtwfgs.cn

[R45] 批量删除
来源：http://qt.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://yv.hahajie.cn

[R46] 递归替换文件内容
来源：http://oo.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bo.huanxung.cn

[R47] sed 单行替换
来源：http://js.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oe.hnjuh.cn

[R48] awk 取指定列
来源：http://ms.521024.cn

awk '{print $1, $3}' a.txt
来源：http://yr.jianghongdianzi.cn

[R49] awk 带条件
来源：http://bn.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ii.colortex.cn

[R50] awk 求和
来源：http://hp.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ek.huixiangedu.cn

[R51] 排序去重取前几
来源：http://sv.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://me.szxytkj.cn

[R52] 统计行数
来源：http://xk.huixinmuqiang.cn

wc -l a.txt
来源：http://po.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://sw.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kf.huixiangedu.cn

[R54] 比较两个文件
来源：http://gp.muxihuayi.cn

diff a.txt b.txt
来源：http://ok.chemitech.net.cn

[R55] 压缩与解压
来源：http://uj.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://to.nicolike.cn

[R56] 远程拷贝
来源：http://rr.colortex.cn

scp file user@host:/path/
来源：http://ba.gzmigu.cn

[R57] 远程执行命令
来源：http://vq.hahajie.cn

ssh user@host 'uptime'
来源：http://iy.shtwfgs.cn

[R58] 下载文件
来源：http://fu.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ys.nszjky.cn

[R59] 发 POST JSON
来源：http://ab.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://df.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://um.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pi.asd995.cn

[R61] 磁盘占用
来源：http://au.hahajie.cn

df -h;  du -sh *
来源：http://yd.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://md.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://pz.jctech888.com.cn

[R63] 内存与进程
来源：http://ny.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://kn.szsharing.cn

[R64] 结束进程
来源：http://jk.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://yp.huixiangedu.cn

[R65] 查看端口占用
来源：http://jt.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fc.bjjhwx.cn

[R66] 定时任务
来源：http://lr.newstarts.cn

crontab -e;  crontab -l
来源：http://vq.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://gw.huixinmuqiang.cn

openssl rand -hex 16
来源：http://pc.colortex.cn

[R68] 计算文件校验值
来源：http://gv.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nj.hnjuh.cn

[R69] 生成随机密码
来源：http://lt.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://co.hahajie.cn

[R70] 时间戳与互转
来源：http://gi.szsharing.cn

date +%s;  date -d @1700000000
来源：http://ac.chemitech.net.cn

[R71] 日期格式化
来源：http://tg.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nx.szsharing.cn

[R72] 等待端口就绪
来源：http://gv.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dm.gzmigu.cn

[R73] 分割大日志
来源：http://mz.asd995.cn

split -l 1000 big.log part_
来源：http://yt.9csxet.cn

[R74] 批量重命名
来源：http://fk.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wh.asd995.cn

[R75] 导出环境变量
来源：http://ry.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://dy.chemitech.net.cn

[R76] 使用临时文件
来源：http://eh.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lj.asd995.cn

[R77] 读取用户输入
来源：http://av.wgjwhj.cn

read -rp "请输入: " ans
来源：http://gc.asd995.cn

[R78] 交互式菜单
来源：http://me.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ys.9csxet.cn

[R79] 解析命令行选项
来源：http://af.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xj.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://xu.nicolike.cn

time ./run.sh
来源：http://es.chemitech.net.cn

================================================================================
来源：http://vi.shxzskj.cn

S. C / C++ 专题
来源：http://he.panjiajie.cn

================================================================================
来源：http://gk.newstarts.cn

[S01] C：Hello World
来源：http://xw.wgjwhj.cn

#include <stdio.h>
来源：http://rm.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gj.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://cn.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://oa.yuntaijiaju.cn

[S03] C：读入整数
来源：http://oh.hahajie.cn

int x; scanf("%d", &x);
来源：http://wu.muxihuayi.cn

[S04] C：字符串复制
来源：http://hl.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://od.hahajie.cn

[S05] C：字符串长度
来源：http://ow.panjiajie.cn

strlen(s)
来源：http://dt.shtwfgs.cn

[S06] C：字符串比较
来源：http://jr.huixiangedu.cn

strcmp(a, b) == 0
来源：http://mf.newstarts.cn

[S07] C：数组遍历求和
来源：http://wm.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yk.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://ws.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ml.colortex.cn

[S09] C：结构体定义与初始化
来源：http://pv.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jh.asd995.cn

[S10] C：指针与解引用
来源：http://mr.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://uc.jctech888.com.cn

[S11] C：逐行读文件
来源：http://ee.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://kw.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ms.521024.cn

fclose(f);
来源：http://sv.chemitech.net.cn

[S12] C：写文件
来源：http://vk.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bf.gzmigu.cn

[S13] C：宏定义
来源：http://fq.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uq.chemitech.net.cn

[S14] C：枚举
来源：http://xx.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://ue.9csxet.cn

[S15] C：类型转换
来源：http://eg.gzmigu.cn

(double) a / b
来源：http://rt.hahajie.cn

[S16] C：位操作置位
来源：http://ow.panjiajie.cn

x |= (1 << 3);
来源：http://ne.newstarts.cn

[S17] C：安全拼接字符串
来源：http://im.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wy.newstarts.cn

[S18] C：命令行参数
来源：http://bv.521024.cn

int main(int argc, char **argv)
来源：http://ls.newstarts.cn

[S19] C：快速排序
来源：http://gl.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ad.wgjwhj.cn

[S20] C：二分查找
来源：http://wx.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zz.bjjhwx.cn

[S21] C：字符类别判断
来源：http://kk.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kv.muxihuayi.cn

[S22] C：字符串转数字
来源：http://bn.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ey.szxytkj.cn

[S23] C：随机数
来源：http://jx.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://is.nszjky.cn

[S24] C：获取本地时间
来源：http://xs.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cp.shxzskj.cn

[S25] C：内存拷贝
来源：http://cw.muxihuayi.cn

memcpy(dst, src, n);
来源：http://xg.hahajie.cn

[S26] C：内存清零
来源：http://do.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://ze.bookmarksfly.cn

[S27] C：定义常量
来源：http://ft.nicolike.cn

const double PI = 3.14159;
来源：http://hz.hahajie.cn

[S28] C：静态变量
来源：http://qm.szxytkj.cn

static int counter = 0;
来源：http://ik.shxzskj.cn

[S29] C：变参函数
来源：http://en.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ut.nszjky.cn

[S30] C：头文件保护
来源：http://gw.haigaiapp.cn

#ifndef X_H
来源：http://us.bookmarksfly.cn

#define X_H
来源：http://md.haigaiapp.cn

#endif
来源：http://ix.shtwfgs.cn

[S31] C++：Hello World
来源：http://rh.yuexingan06.cn

#include <iostream>
来源：http://ah.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://jp.nszjky.cn

[S32] C++：字符串
来源：http://ms.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://nc.yuexingan06.cn

[S33] C++：vector 增删
来源：http://gr.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xd.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://mq.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://hk.huanxung.cn

[S35] C++：map
来源：http://ba.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mu.yuexingan06.cn

[S36] C++：unordered_map
来源：http://gi.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lp.shtwfgs.cn

[S37] C++：set
来源：http://ws.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bg.asd995.cn

[S38] C++：排序
来源：http://hn.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://mr.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://mb.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uq.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://tq.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vd.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://kl.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oi.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://xc.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://dv.nicolike.cn

[S43] C++：智能指针
来源：http://kv.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://ym.huanxung.cn

[S44] C++：引用传参
来源：http://yr.asd995.cn

void inc(int &x) { ++x; }
来源：http://aj.hahajie.cn

[S45] C++：lambda
来源：http://un.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://we.shxzskj.cn

[S46] C++：函数模板
来源：http://yv.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nb.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://qi.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ju.gzmigu.cn

[S48] C++：逐行读文件
来源：http://ed.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lx.hahajie.cn


<!-- 参考信息 -->