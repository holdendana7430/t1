代发 wailian999

[Q80] 字符串截取
来源：http://tw.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ga.chemitech.net.cn

[Q81] 字符串替换
来源：http://ou.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ua.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://fc.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ec.hahajie.cn

[Q83] 大小写转换
来源：http://ze.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qp.nszjky.cn

[Q84] 去除首尾空格
来源：http://gh.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://yb.muxihuayi.cn

[Q85] 数值取整
来源：http://lf.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jy.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://ms.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xz.hahajie.cn

[Q87] JSON 字段做条件
来源：http://jc.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wv.huanxung.cn

[Q88] 行转列（条件聚合）
来源：http://lr.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qs.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wy.hnjuh.cn

[Q89] 判断表是否存在
来源：http://ei.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vx.newstarts.cn

[Q90] 生成序号列
来源：http://lc.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tp.hnjuh.cn

================================================================================
来源：http://vm.521024.cn

R. Bash 专题
来源：http://om.bjjhwx.cn

================================================================================
来源：http://cv.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://yy.chemitech.net.cn

#!/usr/bin/env bash
来源：http://uw.huixinmuqiang.cn

set -euo pipefail
来源：http://it.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://cj.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://ip.gzmigu.cn

[R03] 只读变量
来源：http://gc.colortex.cn

readonly PI=3.14
来源：http://qb.bjjhwx.cn

[R04] 位置参数
来源：http://lf.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://is.szsharing.cn

[R05] 参数默认值
来源：http://hr.szxytkj.cn

name="${1:-default}"
来源：http://yc.szxytkj.cn

[R06] 判断命令是否存在
来源：http://ub.bjjhwx.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ci.newstarts.cn

[R07] if 判断文件
来源：http://ki.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://me.bookmarksfly.cn

[R08] 数值比较
来源：http://xf.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cz.newstarts.cn

[R09] 字符串比较
来源：http://bi.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xt.bjjhwx.cn

[R10] 正则匹配
来源：http://bp.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cm.szxytkj.cn

[R11] case 多分支
来源：http://qh.521024.cn

case "$1" in
来源：http://lm.shtwfgs.cn

start) echo "启动" ;;
来源：http://pn.newstarts.cn

stop)  echo "停止" ;;
来源：http://oh.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://ln.huanxung.cn

esac
来源：http://xw.yuexingan06.cn

[R12] for 遍历文件
来源：http://kr.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://wx.wgjwhj.cn

[R13] for 计数循环
来源：http://st.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://fm.hnjuh.cn

[R14] C 风格 for
来源：http://im.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qz.colortex.cn

[R15] while 逐行读文件
来源：http://mk.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zc.newstarts.cn

[R16] until 等待条件
来源：http://vj.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ch.bjjhwx.cn

[R17] 数组定义与取值
来源：http://ji.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tp.newstarts.cn

[R18] 遍历数组
来源：http://ui.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gr.huixinmuqiang.cn

[R19] 数组长度
来源：http://rm.bjjhwx.cn

echo "${#arr[@]}"
来源：http://xi.colortex.cn

[R20] 关联数组（字典）
来源：http://vy.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yn.huixinmuqiang.cn

[R21] 字符串长度
来源：http://dg.yuntaijiaju.cn

echo "${#s}"
来源：http://jf.szxytkj.cn

[R22] 截取子串
来源：http://he.shtwfgs.cn

echo "${s:0:5}"
来源：http://zc.shxzskj.cn

[R23] 字符串替换
来源：http://rk.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tf.jianghongdianzi.cn

[R24] 大小写转换
来源：http://mg.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bd.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://ks.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oy.shtwfgs.cn

[R26] 命令替换
来源：http://me.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://sd.hnjuh.cn

[R27] 算术展开
来源：http://xu.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://vx.lnxyls.cn

[R28] 浮点运算
来源：http://ug.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://tg.lnxyls.cn

[R29] 定义函数
来源：http://bd.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rr.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://sy.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://gd.bjjhwx.cn

[R31] 局部变量
来源：http://rh.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://ep.chemitech.net.cn

[R32] 参数个数校验
来源：http://ar.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qc.colortex.cn

[R33] 捕获错误并提示行号
来源：http://zf.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ze.chemitech.net.cn

[R34] 退出时清理
来源：http://yz.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tn.bjjhwx.cn

[R35] 后台执行并等待
来源：http://qq.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://us.colortex.cn

[R36] 并发执行多个任务
来源：http://vi.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mx.nszjky.cn

[R37] 把输出赋给变量
来源：http://dh.gzmigu.cn

files=$(ls -1)
来源：http://rs.shxzukj.cn

[R38] 管道串联
来源：http://cq.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://pn.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://to.muxihuayi.cn

cmd > out.log 2>&1
来源：http://lg.bjjhwx.cn

[R40] 追加写日志
来源：http://bc.bjjhwx.cn

echo "log" >> out.log
来源：http://kb.haigaiapp.cn

[R41] 丢弃输出
来源：http://bj.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://qc.wgjwhj.cn

[R42] 输入重定向
来源：http://ap.nicolike.cn

wc -l < a.txt
来源：http://xu.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://dw.jctech888.com.cn

find . -name "*.log" -type f
来源：http://im.szsharing.cn

[R44] 按修改时间查找
来源：http://gj.haigaiapp.cn

find . -mtime -7 -type f
来源：http://sc.nszjky.cn

[R45] 批量删除
来源：http://do.huanxung.cn

find . -name "*.tmp" -delete
来源：http://ng.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://gt.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zs.haigaiapp.cn

[R47] sed 单行替换
来源：http://kw.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qz.bookmarksfly.cn

[R48] awk 取指定列
来源：http://iq.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://jz.chemitech.net.cn

[R49] awk 带条件
来源：http://dt.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cp.yuntaijiaju.cn

[R50] awk 求和
来源：http://lw.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mj.chemitech.net.cn

[R51] 排序去重取前几
来源：http://ky.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qy.gzmigu.cn

[R52] 统计行数
来源：http://tg.shxzskj.cn

wc -l a.txt
来源：http://tt.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://yd.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://al.hahajie.cn

[R54] 比较两个文件
来源：http://gg.panjiajie.cn

diff a.txt b.txt
来源：http://rm.hahajie.cn

[R55] 压缩与解压
来源：http://ai.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uw.muxihuayi.cn

[R56] 远程拷贝
来源：http://cr.shxzukj.cn

scp file user@host:/path/
来源：http://bp.9csxet.cn

[R57] 远程执行命令
来源：http://cp.bjjhwx.cn

ssh user@host 'uptime'
来源：http://hd.huixiangedu.cn

[R58] 下载文件
来源：http://yi.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zm.haigaiapp.cn

[R59] 发 POST JSON
来源：http://xp.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ll.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://aa.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uk.muxihuayi.cn

[R61] 磁盘占用
来源：http://rx.szsharing.cn

df -h;  du -sh *
来源：http://kg.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://jj.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://co.wgjwhj.cn

[R63] 内存与进程
来源：http://fv.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://vx.hahajie.cn

[R64] 结束进程
来源：http://nu.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://hn.haigaiapp.cn

[R65] 查看端口占用
来源：http://on.nicolike.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tk.szsharing.cn

[R66] 定时任务
来源：http://ee.huanxung.cn

crontab -e;  crontab -l
来源：http://ip.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://qs.hahajie.cn

openssl rand -hex 16
来源：http://tb.shtwfgs.cn

[R68] 计算文件校验值
来源：http://ex.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xr.szxytkj.cn

[R69] 生成随机密码
来源：http://sc.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://lo.szxytkj.cn

[R70] 时间戳与互转
来源：http://gf.newstarts.cn

date +%s;  date -d @1700000000
来源：http://ps.huanxung.cn

[R71] 日期格式化
来源：http://mj.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uo.panjiajie.cn

[R72] 等待端口就绪
来源：http://ao.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hj.shxzskj.cn

[R73] 分割大日志
来源：http://mr.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://cq.shtwfgs.cn

[R74] 批量重命名
来源：http://zt.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vj.bjjhwx.cn

[R75] 导出环境变量
来源：http://ul.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://hl.shxzukj.cn

[R76] 使用临时文件
来源：http://ru.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xo.huixiangedu.cn

[R77] 读取用户输入
来源：http://np.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://zl.asd995.cn

[R78] 交互式菜单
来源：http://gf.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pm.wgjwhj.cn

[R79] 解析命令行选项
来源：http://hk.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kl.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://eu.shxzskj.cn

time ./run.sh
来源：http://uz.lnxyls.cn

================================================================================
来源：http://yy.huixinmuqiang.cn

S. C / C++ 专题
来源：http://ca.colortex.cn

================================================================================
来源：http://pn.shtwfgs.cn

[S01] C：Hello World
来源：http://js.wgjwhj.cn

#include <stdio.h>
来源：http://dq.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://we.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://vy.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://pv.szsharing.cn

[S03] C：读入整数
来源：http://qf.shxzukj.cn

int x; scanf("%d", &x);
来源：http://zk.jctech888.com.cn

[S04] C：字符串复制
来源：http://mg.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uu.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://kx.haigaiapp.cn

strlen(s)
来源：http://ve.shtwfgs.cn

[S06] C：字符串比较
来源：http://ql.asd995.cn

strcmp(a, b) == 0
来源：http://rp.hahajie.cn

[S07] C：数组遍历求和
来源：http://xd.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vk.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://kc.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qb.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://xf.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ws.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://ob.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://pb.colortex.cn

[S11] C：逐行读文件
来源：http://rq.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://xo.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yf.asd995.cn

fclose(f);
来源：http://ph.newstarts.cn

[S12] C：写文件
来源：http://ac.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fm.huanxung.cn

[S13] C：宏定义
来源：http://pg.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wa.jctech888.com.cn

[S14] C：枚举
来源：http://er.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://bi.szsharing.cn

[S15] C：类型转换
来源：http://io.muxihuayi.cn

(double) a / b
来源：http://jq.521024.cn

[S16] C：位操作置位
来源：http://bn.asd995.cn

x |= (1 << 3);
来源：http://ws.szsharing.cn

[S17] C：安全拼接字符串
来源：http://ed.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dt.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://ux.huanxung.cn

int main(int argc, char **argv)
来源：http://vp.shxzukj.cn

[S19] C：快速排序
来源：http://fk.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fc.yuexingan06.cn

[S20] C：二分查找
来源：http://it.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vr.szxytkj.cn

[S21] C：字符类别判断
来源：http://yx.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cn.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://yi.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ed.521024.cn

[S23] C：随机数
来源：http://bw.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vx.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://fp.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ee.9csxet.cn

[S25] C：内存拷贝
来源：http://sq.colortex.cn

memcpy(dst, src, n);
来源：http://lc.bjjhwx.cn

[S26] C：内存清零
来源：http://ty.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://so.jctech888.com.cn

[S27] C：定义常量
来源：http://th.szxytkj.cn

const double PI = 3.14159;
来源：http://qr.huixinmuqiang.cn

[S28] C：静态变量
来源：http://ku.huixiangedu.cn

static int counter = 0;
来源：http://mw.muxihuayi.cn

[S29] C：变参函数
来源：http://ze.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dp.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://kt.huanxung.cn

#ifndef X_H
来源：http://zv.lnxyls.cn

#define X_H
来源：http://gm.521024.cn

#endif
来源：http://tz.nicolike.cn

[S31] C++：Hello World
来源：http://tq.gzmigu.cn

#include <iostream>
来源：http://hd.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://rz.bookmarksfly.cn

[S32] C++：字符串
来源：http://yj.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://gk.szsharing.cn

[S33] C++：vector 增删
来源：http://ev.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ku.asd995.cn

[S34] C++：遍历 vector
来源：http://nh.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://zc.szxytkj.cn

[S35] C++：map
来源：http://ns.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://md.shxzskj.cn

[S36] C++：unordered_map
来源：http://sy.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://am.szsharing.cn

[S37] C++：set
来源：http://dt.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xf.wgjwhj.cn

[S38] C++：排序
来源：http://ew.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://ty.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://xs.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://og.9csxet.cn

[S40] C++：查找元素
来源：http://jo.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kq.newstarts.cn

[S41] C++：类与构造函数
来源：http://mr.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sl.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://zz.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://xy.newstarts.cn

[S43] C++：智能指针
来源：http://ep.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://su.asd995.cn

[S44] C++：引用传参
来源：http://yn.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://hu.asd995.cn

[S45] C++：lambda
来源：http://zl.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pw.nszjky.cn

[S46] C++：函数模板
来源：http://dg.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yr.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://nw.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mb.9csxet.cn

[S48] C++：逐行读文件
来源：http://zr.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vw.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://kh.shxzskj.cn

[S49] C++：写文件
来源：http://we.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gv.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://ce.haigaiapp.cn


<!-- 参考信息 -->