代发 wailian999

[Q82] 字符长度与字节长度
来源：http://qu.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ur.szxytkj.cn

[Q83] 大小写转换
来源：http://ri.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bw.521024.cn

[Q84] 去除首尾空格
来源：http://pu.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://hf.asd995.cn

[Q85] 数值取整
来源：http://xl.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ym.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://xb.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mm.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://ap.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tm.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://ry.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kn.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sr.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://ao.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vr.nicolike.cn

[Q90] 生成序号列
来源：http://py.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zz.hnjuh.cn

================================================================================
来源：http://ez.nicolike.cn

R. Bash 专题
来源：http://fb.bookmarksfly.cn

================================================================================
来源：http://fq.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://px.huixiangedu.cn

#!/usr/bin/env bash
来源：http://zg.szxytkj.cn

set -euo pipefail
来源：http://gx.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://am.colortex.cn

name="Tom"; echo "$name"
来源：http://wf.szsharing.cn

[R03] 只读变量
来源：http://ee.huixinmuqiang.cn

readonly PI=3.14
来源：http://cl.huixiangedu.cn

[R04] 位置参数
来源：http://hr.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vg.lnxyls.cn

[R05] 参数默认值
来源：http://fk.colortex.cn

name="${1:-default}"
来源：http://xt.lnxyls.cn

[R06] 判断命令是否存在
来源：http://yh.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uu.panjiajie.cn

[R07] if 判断文件
来源：http://cu.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gg.shtwfgs.cn

[R08] 数值比较
来源：http://uw.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://om.9csxet.cn

[R09] 字符串比较
来源：http://ba.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fb.huanxung.cn

[R10] 正则匹配
来源：http://pk.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ca.newstarts.cn

[R11] case 多分支
来源：http://ai.9csxet.cn

case "$1" in
来源：http://rw.wgjwhj.cn

start) echo "启动" ;;
来源：http://kh.lnxyls.cn

stop)  echo "停止" ;;
来源：http://ud.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://dg.jianghongdianzi.cn

esac
来源：http://kn.wgjwhj.cn

[R12] for 遍历文件
来源：http://bx.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://fo.nicolike.cn

[R13] for 计数循环
来源：http://jr.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://og.newstarts.cn

[R14] C 风格 for
来源：http://jm.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ks.wgjwhj.cn

[R15] while 逐行读文件
来源：http://fm.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://le.colortex.cn

[R16] until 等待条件
来源：http://wa.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pr.szxytkj.cn

[R17] 数组定义与取值
来源：http://lu.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kg.shxzukj.cn

[R18] 遍历数组
来源：http://ok.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yb.yuexingan06.cn

[R19] 数组长度
来源：http://dz.huanxung.cn

echo "${#arr[@]}"
来源：http://ra.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://vc.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hn.huixinmuqiang.cn

[R21] 字符串长度
来源：http://cf.huixinmuqiang.cn

echo "${#s}"
来源：http://hh.szsharing.cn

[R22] 截取子串
来源：http://yj.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://fg.szxytkj.cn

[R23] 字符串替换
来源：http://tg.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sa.521024.cn

[R24] 大小写转换
来源：http://fd.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ih.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://uj.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rc.wgjwhj.cn

[R26] 命令替换
来源：http://sn.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://zk.shtwfgs.cn

[R27] 算术展开
来源：http://pi.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://ur.lnxyls.cn

[R28] 浮点运算
来源：http://vq.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://ct.nszjky.cn

[R29] 定义函数
来源：http://vb.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jm.gzmigu.cn

[R30] 函数返回状态码
来源：http://ay.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://jn.521024.cn

[R31] 局部变量
来源：http://yx.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://xv.lnxyls.cn

[R32] 参数个数校验
来源：http://js.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pa.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://sr.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://if.jctech888.com.cn

[R34] 退出时清理
来源：http://no.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rq.muxihuayi.cn

[R35] 后台执行并等待
来源：http://pq.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yt.lnxyls.cn

[R36] 并发执行多个任务
来源：http://jf.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dm.hnjuh.cn

[R37] 把输出赋给变量
来源：http://qf.shxzskj.cn

files=$(ls -1)
来源：http://rb.hnjuh.cn

[R38] 管道串联
来源：http://ub.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://mb.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://dg.shtwfgs.cn

cmd > out.log 2>&1
来源：http://yt.panjiajie.cn

[R40] 追加写日志
来源：http://hl.jianghongdianzi.cn

echo "log" >> out.log
来源：http://hi.gzmigu.cn

[R41] 丢弃输出
来源：http://sp.nicolike.cn

cmd >/dev/null 2>&1
来源：http://zb.lnxyls.cn

[R42] 输入重定向
来源：http://hy.lnxyls.cn

wc -l < a.txt
来源：http://cw.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://wf.shtwfgs.cn

find . -name "*.log" -type f
来源：http://gs.9csxet.cn

[R44] 按修改时间查找
来源：http://lv.gzmigu.cn

find . -mtime -7 -type f
来源：http://mi.asd995.cn

[R45] 批量删除
来源：http://jg.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://qa.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://xj.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yz.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://cs.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mp.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://dh.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://db.muxihuayi.cn

[R49] awk 带条件
来源：http://sc.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yd.asd995.cn

[R50] awk 求和
来源：http://kd.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wh.lnxyls.cn

[R51] 排序去重取前几
来源：http://qv.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gt.newstarts.cn

[R52] 统计行数
来源：http://yt.asd995.cn

wc -l a.txt
来源：http://hg.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://te.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lf.szxytkj.cn

[R54] 比较两个文件
来源：http://qp.haigaiapp.cn

diff a.txt b.txt
来源：http://wi.muxihuayi.cn

[R55] 压缩与解压
来源：http://vy.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hw.wgjwhj.cn

[R56] 远程拷贝
来源：http://hs.yuntaijiaju.cn

scp file user@host:/path/
来源：http://lz.9csxet.cn

[R57] 远程执行命令
来源：http://dw.nicolike.cn

ssh user@host 'uptime'
来源：http://ox.asd995.cn

[R58] 下载文件
来源：http://jp.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dc.hahajie.cn

[R59] 发 POST JSON
来源：http://jw.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hr.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://wx.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vr.newstarts.cn

[R61] 磁盘占用
来源：http://ac.jctech888.com.cn

df -h;  du -sh *
来源：http://gr.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://fn.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://bm.bookmarksfly.cn

[R63] 内存与进程
来源：http://np.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://he.shxzukj.cn

[R64] 结束进程
来源：http://lb.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://ro.szsharing.cn

[R65] 查看端口占用
来源：http://cd.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vk.shxzskj.cn

[R66] 定时任务
来源：http://az.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://je.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://dt.newstarts.cn

openssl rand -hex 16
来源：http://ry.shtwfgs.cn

[R68] 计算文件校验值
来源：http://ie.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sd.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://of.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://ry.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://eo.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://my.panjiajie.cn

[R71] 日期格式化
来源：http://ni.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vr.nszjky.cn

[R72] 等待端口就绪
来源：http://rd.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tc.hnjuh.cn

[R73] 分割大日志
来源：http://nw.szsharing.cn

split -l 1000 big.log part_
来源：http://kr.jctech888.com.cn

[R74] 批量重命名
来源：http://hc.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oh.9csxet.cn

[R75] 导出环境变量
来源：http://ev.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://ha.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://iz.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gr.szxytkj.cn

[R77] 读取用户输入
来源：http://cz.asd995.cn

read -rp "请输入: " ans
来源：http://ju.colortex.cn

[R78] 交互式菜单
来源：http://oq.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pi.jctech888.com.cn

[R79] 解析命令行选项
来源：http://fh.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ri.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://vu.huanxung.cn

time ./run.sh
来源：http://st.yuntaijiaju.cn

================================================================================
来源：http://ld.jianghongdianzi.cn

S. C / C++ 专题
来源：http://ye.huanxung.cn

================================================================================
来源：http://os.colortex.cn

[S01] C：Hello World
来源：http://md.jianghongdianzi.cn

#include <stdio.h>
来源：http://iz.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ab.nszjky.cn

[S02] C：变量与格式化输出
来源：http://wa.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://xm.newstarts.cn

[S03] C：读入整数
来源：http://ck.colortex.cn

int x; scanf("%d", &x);
来源：http://wk.chemitech.net.cn

[S04] C：字符串复制
来源：http://py.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yr.shxzukj.cn

[S05] C：字符串长度
来源：http://yp.shxzukj.cn

strlen(s)
来源：http://it.szsharing.cn

[S06] C：字符串比较
来源：http://ik.nszjky.cn

strcmp(a, b) == 0
来源：http://iq.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://ma.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ss.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://ob.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://av.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://od.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ty.hahajie.cn

[S10] C：指针与解引用
来源：http://rd.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://dn.huixiangedu.cn

[S11] C：逐行读文件
来源：http://bu.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://pf.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nn.521024.cn

fclose(f);
来源：http://hy.colortex.cn

[S12] C：写文件
来源：http://sz.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gs.521024.cn

[S13] C：宏定义
来源：http://ii.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xx.shxzukj.cn

[S14] C：枚举
来源：http://uj.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://kp.huixiangedu.cn

[S15] C：类型转换
来源：http://ci.chemitech.net.cn

(double) a / b
来源：http://qd.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://qp.asd995.cn

x |= (1 << 3);
来源：http://st.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://rh.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ff.chemitech.net.cn

[S18] C：命令行参数
来源：http://bf.hahajie.cn

int main(int argc, char **argv)
来源：http://ld.yuexingan06.cn

[S19] C：快速排序
来源：http://of.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nd.shxzukj.cn

[S20] C：二分查找
来源：http://pd.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fa.jctech888.com.cn

[S21] C：字符类别判断
来源：http://gv.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hw.panjiajie.cn

[S22] C：字符串转数字
来源：http://dw.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ia.nszjky.cn

[S23] C：随机数
来源：http://oo.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ma.lnxyls.cn

[S24] C：获取本地时间
来源：http://pf.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ky.newstarts.cn

[S25] C：内存拷贝
来源：http://wz.gzmigu.cn

memcpy(dst, src, n);
来源：http://sx.lnxyls.cn

[S26] C：内存清零
来源：http://hd.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://qp.shxzskj.cn

[S27] C：定义常量
来源：http://ap.chemitech.net.cn

const double PI = 3.14159;
来源：http://qc.gzmigu.cn

[S28] C：静态变量
来源：http://tx.huixinmuqiang.cn

static int counter = 0;
来源：http://kq.huixinmuqiang.cn

[S29] C：变参函数
来源：http://op.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kh.hnjuh.cn

[S30] C：头文件保护
来源：http://we.hahajie.cn

#ifndef X_H
来源：http://yp.huixiangedu.cn

#define X_H
来源：http://ni.muxihuayi.cn

#endif
来源：http://kk.hnjuh.cn

[S31] C++：Hello World
来源：http://kx.yuexingan06.cn

#include <iostream>
来源：http://cb.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://wr.shtwfgs.cn

[S32] C++：字符串
来源：http://ws.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://gp.newstarts.cn

[S33] C++：vector 增删
来源：http://xv.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dn.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://ll.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://am.muxihuayi.cn

[S35] C++：map
来源：http://to.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jd.wgjwhj.cn

[S36] C++：unordered_map
来源：http://xi.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yk.bookmarksfly.cn

[S37] C++：set
来源：http://oo.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ap.haigaiapp.cn

[S38] C++：排序
来源：http://wa.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://jr.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://gs.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yt.lnxyls.cn

[S40] C++：查找元素
来源：http://vo.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hr.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://al.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iy.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://qg.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://st.huanxung.cn

[S43] C++：智能指针
来源：http://nm.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://pc.muxihuayi.cn

[S44] C++：引用传参
来源：http://qg.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://sj.shtwfgs.cn

[S45] C++：lambda
来源：http://ts.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ej.colortex.cn

[S46] C++：函数模板
来源：http://rq.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jl.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://mo.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ov.colortex.cn

[S48] C++：逐行读文件
来源：http://ps.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ji.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://zh.szsharing.cn

[S49] C++：写文件
来源：http://lq.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dh.521024.cn

[S50] C++：格式化数字
来源：http://ly.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cx.colortex.cn

[S51] C++：显式类型转换
来源：http://yb.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://jk.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://wl.shxzskj.cn


<!-- 参考信息 -->