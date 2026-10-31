代发 wailian999

[Q80] 字符串截取
来源：http://ps.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ew.colortex.cn

[Q81] 字符串替换
来源：http://kj.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fz.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://yr.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://io.521024.cn

[Q83] 大小写转换
来源：http://qj.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dy.nicolike.cn

[Q84] 去除首尾空格
来源：http://ex.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://sk.panjiajie.cn

[Q85] 数值取整
来源：http://vm.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vf.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://lg.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ac.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://vg.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tf.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://pb.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yl.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qv.hahajie.cn

[Q89] 判断表是否存在
来源：http://qy.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rv.asd995.cn

[Q90] 生成序号列
来源：http://zu.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vl.wgjwhj.cn

================================================================================
来源：http://ys.shxzskj.cn

R. Bash 专题
来源：http://lm.muxihuayi.cn

================================================================================
来源：http://rw.asd995.cn

[R01] shebang 与严格模式
来源：http://za.521024.cn

#!/usr/bin/env bash
来源：http://ix.gzmigu.cn

set -euo pipefail
来源：http://cs.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://cb.asd995.cn

name="Tom"; echo "$name"
来源：http://ut.bookmarksfly.cn

[R03] 只读变量
来源：http://xr.wgjwhj.cn

readonly PI=3.14
来源：http://cw.huixiangedu.cn

[R04] 位置参数
来源：http://jg.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ea.huixiangedu.cn

[R05] 参数默认值
来源：http://cd.huixinmuqiang.cn

name="${1:-default}"
来源：http://fu.colortex.cn

[R06] 判断命令是否存在
来源：http://zp.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gx.shxzskj.cn

[R07] if 判断文件
来源：http://hk.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ri.nicolike.cn

[R08] 数值比较
来源：http://wh.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iq.hnjuh.cn

[R09] 字符串比较
来源：http://io.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fq.chemitech.net.cn

[R10] 正则匹配
来源：http://tp.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fl.yuexingan06.cn

[R11] case 多分支
来源：http://el.yuntaijiaju.cn

case "$1" in
来源：http://ol.newstarts.cn

start) echo "启动" ;;
来源：http://xd.newstarts.cn

stop)  echo "停止" ;;
来源：http://xg.huixinmuqiang.cn

*)     echo "未知命令" ;;
来源：http://cb.jianghongdianzi.cn

esac
来源：http://ut.521024.cn

[R12] for 遍历文件
来源：http://ue.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://yg.shxzskj.cn

[R13] for 计数循环
来源：http://tk.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://np.521024.cn

[R14] C 风格 for
来源：http://ds.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dl.newstarts.cn

[R15] while 逐行读文件
来源：http://cn.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oz.9csxet.cn

[R16] until 等待条件
来源：http://xb.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://un.hnjuh.cn

[R17] 数组定义与取值
来源：http://yq.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tp.panjiajie.cn

[R18] 遍历数组
来源：http://yr.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lk.hnjuh.cn

[R19] 数组长度
来源：http://km.521024.cn

echo "${#arr[@]}"
来源：http://ay.newstarts.cn

[R20] 关联数组（字典）
来源：http://ei.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oq.521024.cn

[R21] 字符串长度
来源：http://qo.gzmigu.cn

echo "${#s}"
来源：http://ta.bjjhwx.cn

[R22] 截取子串
来源：http://vz.shxzukj.cn

echo "${s:0:5}"
来源：http://rs.jianghongdianzi.cn

[R23] 字符串替换
来源：http://xh.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gy.jctech888.com.cn

[R24] 大小写转换
来源：http://tt.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ei.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://fl.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vq.shtwfgs.cn

[R26] 命令替换
来源：http://ue.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://ne.gzmigu.cn

[R27] 算术展开
来源：http://cu.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://oa.colortex.cn

[R28] 浮点运算
来源：http://fh.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://to.chemitech.net.cn

[R29] 定义函数
来源：http://mc.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bp.shtwfgs.cn

[R30] 函数返回状态码
来源：http://uk.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://gt.wgjwhj.cn

[R31] 局部变量
来源：http://jn.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://ab.jctech888.com.cn

[R32] 参数个数校验
来源：http://gp.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rc.521024.cn

[R33] 捕获错误并提示行号
来源：http://wo.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pa.bjjhwx.cn

[R34] 退出时清理
来源：http://fd.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cz.szsharing.cn

[R35] 后台执行并等待
来源：http://zw.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nc.huanxung.cn

[R36] 并发执行多个任务
来源：http://wi.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pb.lnxyls.cn

[R37] 把输出赋给变量
来源：http://kc.panjiajie.cn

files=$(ls -1)
来源：http://tt.521024.cn

[R38] 管道串联
来源：http://gr.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://mp.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://wv.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://ub.jctech888.com.cn

[R40] 追加写日志
来源：http://st.bookmarksfly.cn

echo "log" >> out.log
来源：http://hv.yuexingan06.cn

[R41] 丢弃输出
来源：http://bm.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://jz.asd995.cn

[R42] 输入重定向
来源：http://nz.521024.cn

wc -l < a.txt
来源：http://kg.hahajie.cn

[R43] 按名字查找文件
来源：http://uc.panjiajie.cn

find . -name "*.log" -type f
来源：http://cz.lnxyls.cn

[R44] 按修改时间查找
来源：http://tb.panjiajie.cn

find . -mtime -7 -type f
来源：http://dl.chemitech.net.cn

[R45] 批量删除
来源：http://nh.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://hv.szxytkj.cn

[R46] 递归替换文件内容
来源：http://tr.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://av.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://my.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xj.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://ee.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://sv.newstarts.cn

[R49] awk 带条件
来源：http://rm.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uj.huixiangedu.cn

[R50] awk 求和
来源：http://xd.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ue.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://nk.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sk.huanxung.cn

[R52] 统计行数
来源：http://yn.huixiangedu.cn

wc -l a.txt
来源：http://pi.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://lm.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nj.lnxyls.cn

[R54] 比较两个文件
来源：http://cv.huixiangedu.cn

diff a.txt b.txt
来源：http://dd.asd995.cn

[R55] 压缩与解压
来源：http://ou.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ln.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://ki.chemitech.net.cn

scp file user@host:/path/
来源：http://qt.szsharing.cn

[R57] 远程执行命令
来源：http://ys.jctech888.com.cn

ssh user@host 'uptime'
来源：http://vo.jctech888.com.cn

[R58] 下载文件
来源：http://re.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lw.szxytkj.cn

[R59] 发 POST JSON
来源：http://hg.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ip.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://lz.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cy.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://mx.panjiajie.cn

df -h;  du -sh *
来源：http://yy.lnxyls.cn

[R62] 找最占空间的文件
来源：http://xw.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://ld.9csxet.cn

[R63] 内存与进程
来源：http://jl.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://nk.szxytkj.cn

[R64] 结束进程
来源：http://ih.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://if.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://pz.nicolike.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ue.huixiangedu.cn

[R66] 定时任务
来源：http://ad.wgjwhj.cn

crontab -e;  crontab -l
来源：http://uj.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://kl.haigaiapp.cn

openssl rand -hex 16
来源：http://vh.shxzskj.cn

[R68] 计算文件校验值
来源：http://bm.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zz.hahajie.cn

[R69] 生成随机密码
来源：http://ad.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://bp.9csxet.cn

[R70] 时间戳与互转
来源：http://ax.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://kv.newstarts.cn

[R71] 日期格式化
来源：http://yd.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dv.haigaiapp.cn

[R72] 等待端口就绪
来源：http://bd.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dc.shxzukj.cn

[R73] 分割大日志
来源：http://le.hahajie.cn

split -l 1000 big.log part_
来源：http://zf.gzmigu.cn

[R74] 批量重命名
来源：http://yo.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ou.lnxyls.cn

[R75] 导出环境变量
来源：http://ev.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://gh.szxytkj.cn

[R76] 使用临时文件
来源：http://cc.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wl.hahajie.cn

[R77] 读取用户输入
来源：http://pq.huanxung.cn

read -rp "请输入: " ans
来源：http://ab.bjjhwx.cn

[R78] 交互式菜单
来源：http://dp.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yi.nszjky.cn

[R79] 解析命令行选项
来源：http://jh.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tk.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://bb.bjjhwx.cn

time ./run.sh
来源：http://bp.shxzukj.cn

================================================================================
来源：http://qi.yuexingan06.cn

S. C / C++ 专题
来源：http://mv.hnjuh.cn

================================================================================
来源：http://nl.bookmarksfly.cn

[S01] C：Hello World
来源：http://hs.9csxet.cn

#include <stdio.h>
来源：http://on.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sg.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://qh.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://tp.yuexingan06.cn

[S03] C：读入整数
来源：http://vy.newstarts.cn

int x; scanf("%d", &x);
来源：http://qu.szsharing.cn

[S04] C：字符串复制
来源：http://gr.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gy.huixiangedu.cn

[S05] C：字符串长度
来源：http://xb.jctech888.com.cn

strlen(s)
来源：http://vo.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://xm.colortex.cn

strcmp(a, b) == 0
来源：http://br.shxzukj.cn

[S07] C：数组遍历求和
来源：http://kv.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tl.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://ca.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rj.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://on.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://da.asd995.cn

[S10] C：指针与解引用
来源：http://nb.colortex.cn

int *p = &a;  *p = 5;
来源：http://ts.newstarts.cn

[S11] C：逐行读文件
来源：http://eg.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://bv.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yn.shxzskj.cn

fclose(f);
来源：http://dv.lnxyls.cn

[S12] C：写文件
来源：http://wg.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nz.hahajie.cn

[S13] C：宏定义
来源：http://ps.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nj.panjiajie.cn

[S14] C：枚举
来源：http://db.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://cj.haigaiapp.cn

[S15] C：类型转换
来源：http://vh.bjjhwx.cn

(double) a / b
来源：http://rt.szsharing.cn

[S16] C：位操作置位
来源：http://px.haigaiapp.cn

x |= (1 << 3);
来源：http://ot.newstarts.cn

[S17] C：安全拼接字符串
来源：http://vo.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://za.bookmarksfly.cn

[S18] C：命令行参数
来源：http://pw.nszjky.cn

int main(int argc, char **argv)
来源：http://ew.gzmigu.cn

[S19] C：快速排序
来源：http://pt.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://op.nicolike.cn

[S20] C：二分查找
来源：http://cq.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fq.chemitech.net.cn

[S21] C：字符类别判断
来源：http://fl.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lb.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://kc.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nv.huanxung.cn

[S23] C：随机数
来源：http://nr.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://si.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://mx.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xf.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://is.gzmigu.cn

memcpy(dst, src, n);
来源：http://el.huanxung.cn

[S26] C：内存清零
来源：http://st.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://jw.huixiangedu.cn

[S27] C：定义常量
来源：http://ei.9csxet.cn

const double PI = 3.14159;
来源：http://cm.huixinmuqiang.cn

[S28] C：静态变量
来源：http://sp.wgjwhj.cn

static int counter = 0;
来源：http://fx.asd995.cn

[S29] C：变参函数
来源：http://zn.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kv.hnjuh.cn

[S30] C：头文件保护
来源：http://ht.huixiangedu.cn

#ifndef X_H
来源：http://fo.haigaiapp.cn

#define X_H
来源：http://tb.hahajie.cn

#endif
来源：http://xi.wgjwhj.cn

[S31] C++：Hello World
来源：http://rg.panjiajie.cn

#include <iostream>
来源：http://jz.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://qp.shxzukj.cn

[S32] C++：字符串
来源：http://md.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://fd.lnxyls.cn

[S33] C++：vector 增删
来源：http://gu.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jz.shxzukj.cn

[S34] C++：遍历 vector
来源：http://nd.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://bg.panjiajie.cn

[S35] C++：map
来源：http://yu.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ad.jctech888.com.cn

[S36] C++：unordered_map
来源：http://kk.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wf.newstarts.cn

[S37] C++：set
来源：http://bo.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mr.huixiangedu.cn

[S38] C++：排序
来源：http://lf.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://ix.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://oe.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mr.shxzskj.cn

[S40] C++：查找元素
来源：http://le.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fx.9csxet.cn

[S41] C++：类与构造函数
来源：http://rh.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pa.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://ax.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://xz.gzmigu.cn

[S43] C++：智能指针
来源：http://op.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://gg.huixiangedu.cn

[S44] C++：引用传参
来源：http://ae.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://mj.huanxung.cn

[S45] C++：lambda
来源：http://lc.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ss.yuexingan06.cn

[S46] C++：函数模板
来源：http://rp.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aw.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://an.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xt.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://jq.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tm.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://ln.jianghongdianzi.cn

[S49] C++：写文件
来源：http://si.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bt.hahajie.cn

[S50] C++：格式化数字
来源：http://nd.nicolike.cn


<!-- 参考信息 -->