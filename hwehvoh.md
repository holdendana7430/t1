代发 wailian999

[Q82] 字符长度与字节长度
来源：http://mn.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tw.hnjuh.cn

[Q83] 大小写转换
来源：http://ta.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ns.asd995.cn

[Q84] 去除首尾空格
来源：http://as.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://wk.9csxet.cn

[Q85] 数值取整
来源：http://tq.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cu.521024.cn

[Q86] 读取 JSON 字段
来源：http://ba.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ah.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://mc.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jd.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://ef.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gc.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wb.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://qk.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vt.shxzukj.cn

[Q90] 生成序号列
来源：http://fj.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zy.lnxyls.cn

================================================================================
来源：http://yc.szxytkj.cn

R. Bash 专题
来源：http://ws.shtwfgs.cn

================================================================================
来源：http://mt.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://yw.szxytkj.cn

#!/usr/bin/env bash
来源：http://em.9csxet.cn

set -euo pipefail
来源：http://ta.shxzukj.cn

[R02] 变量赋值与使用
来源：http://dn.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://sp.shxzskj.cn

[R03] 只读变量
来源：http://tk.yuexingan06.cn

readonly PI=3.14
来源：http://uy.shtwfgs.cn

[R04] 位置参数
来源：http://te.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zr.szsharing.cn

[R05] 参数默认值
来源：http://av.jianghongdianzi.cn

name="${1:-default}"
来源：http://qc.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://ls.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hr.hnjuh.cn

[R07] if 判断文件
来源：http://nl.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kb.nszjky.cn

[R08] 数值比较
来源：http://ha.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://su.szxytkj.cn

[R09] 字符串比较
来源：http://vp.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ia.szsharing.cn

[R10] 正则匹配
来源：http://cf.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://un.asd995.cn

[R11] case 多分支
来源：http://xd.muxihuayi.cn

case "$1" in
来源：http://ki.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://wd.szsharing.cn

stop)  echo "停止" ;;
来源：http://xl.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://ki.hnjuh.cn

esac
来源：http://rs.521024.cn

[R12] for 遍历文件
来源：http://cg.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://cy.bookmarksfly.cn

[R13] for 计数循环
来源：http://ub.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://xn.hnjuh.cn

[R14] C 风格 for
来源：http://lw.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qa.shxzukj.cn

[R15] while 逐行读文件
来源：http://pl.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gw.nszjky.cn

[R16] until 等待条件
来源：http://dq.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gp.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://bk.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sj.yuntaijiaju.cn

[R18] 遍历数组
来源：http://wf.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vd.szsharing.cn

[R19] 数组长度
来源：http://zy.gzmigu.cn

echo "${#arr[@]}"
来源：http://bo.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://kr.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jk.nszjky.cn

[R21] 字符串长度
来源：http://up.bookmarksfly.cn

echo "${#s}"
来源：http://mz.lnxyls.cn

[R22] 截取子串
来源：http://ez.szxytkj.cn

echo "${s:0:5}"
来源：http://pl.muxihuayi.cn

[R23] 字符串替换
来源：http://pn.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mb.gzmigu.cn

[R24] 大小写转换
来源：http://gq.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wo.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://db.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://id.shxzukj.cn

[R26] 命令替换
来源：http://xo.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://am.bjjhwx.cn

[R27] 算术展开
来源：http://mb.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://ha.colortex.cn

[R28] 浮点运算
来源：http://zs.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://kb.huixiangedu.cn

[R29] 定义函数
来源：http://lc.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://os.bjjhwx.cn

[R30] 函数返回状态码
来源：http://lr.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://tv.yuexingan06.cn

[R31] 局部变量
来源：http://ca.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://vj.asd995.cn

[R32] 参数个数校验
来源：http://rv.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pj.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://ll.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yw.huanxung.cn

[R34] 退出时清理
来源：http://bn.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yy.newstarts.cn

[R35] 后台执行并等待
来源：http://iq.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tl.newstarts.cn

[R36] 并发执行多个任务
来源：http://hx.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jh.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://to.yuntaijiaju.cn

files=$(ls -1)
来源：http://vt.hnjuh.cn

[R38] 管道串联
来源：http://hu.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://cb.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://dr.shxzukj.cn

cmd > out.log 2>&1
来源：http://go.huixinmuqiang.cn

[R40] 追加写日志
来源：http://nm.gzmigu.cn

echo "log" >> out.log
来源：http://al.lnxyls.cn

[R41] 丢弃输出
来源：http://nl.nicolike.cn

cmd >/dev/null 2>&1
来源：http://mz.chemitech.net.cn

[R42] 输入重定向
来源：http://ns.colortex.cn

wc -l < a.txt
来源：http://ob.nszjky.cn

[R43] 按名字查找文件
来源：http://xu.nszjky.cn

find . -name "*.log" -type f
来源：http://kw.asd995.cn

[R44] 按修改时间查找
来源：http://lm.huixiangedu.cn

find . -mtime -7 -type f
来源：http://dq.szxytkj.cn

[R45] 批量删除
来源：http://jh.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://ah.shxzukj.cn

[R46] 递归替换文件内容
来源：http://iu.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ww.huixiangedu.cn

[R47] sed 单行替换
来源：http://qx.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://um.huanxung.cn

[R48] awk 取指定列
来源：http://dr.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://jq.asd995.cn

[R49] awk 带条件
来源：http://jd.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mr.lnxyls.cn

[R50] awk 求和
来源：http://ni.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gj.szsharing.cn

[R51] 排序去重取前几
来源：http://ki.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tl.hahajie.cn

[R52] 统计行数
来源：http://px.jianghongdianzi.cn

wc -l a.txt
来源：http://ka.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://kg.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jl.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://qs.jctech888.com.cn

diff a.txt b.txt
来源：http://jx.haigaiapp.cn

[R55] 压缩与解压
来源：http://kk.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://si.nszjky.cn

[R56] 远程拷贝
来源：http://mj.nszjky.cn

scp file user@host:/path/
来源：http://ar.huixiangedu.cn

[R57] 远程执行命令
来源：http://nq.lnxyls.cn

ssh user@host 'uptime'
来源：http://xx.nszjky.cn

[R58] 下载文件
来源：http://ri.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zc.szsharing.cn

[R59] 发 POST JSON
来源：http://eb.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lq.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://cz.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ni.newstarts.cn

[R61] 磁盘占用
来源：http://eq.9csxet.cn

df -h;  du -sh *
来源：http://bj.gzmigu.cn

[R62] 找最占空间的文件
来源：http://uw.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://vo.chemitech.net.cn

[R63] 内存与进程
来源：http://cz.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://un.asd995.cn

[R64] 结束进程
来源：http://dr.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://zq.muxihuayi.cn

[R65] 查看端口占用
来源：http://jw.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ma.lnxyls.cn

[R66] 定时任务
来源：http://ns.szxytkj.cn

crontab -e;  crontab -l
来源：http://vv.newstarts.cn

[R67] 生成随机十六进制串
来源：http://gh.haigaiapp.cn

openssl rand -hex 16
来源：http://bn.shxzukj.cn

[R68] 计算文件校验值
来源：http://vf.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cb.shtwfgs.cn

[R69] 生成随机密码
来源：http://cx.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://dp.bjjhwx.cn

[R70] 时间戳与互转
来源：http://ux.huanxung.cn

date +%s;  date -d @1700000000
来源：http://pg.hahajie.cn

[R71] 日期格式化
来源：http://sl.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qt.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://ie.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hk.newstarts.cn

[R73] 分割大日志
来源：http://nn.wgjwhj.cn

split -l 1000 big.log part_
来源：http://ai.9csxet.cn

[R74] 批量重命名
来源：http://pt.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ch.muxihuayi.cn

[R75] 导出环境变量
来源：http://cl.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://oq.panjiajie.cn

[R76] 使用临时文件
来源：http://cw.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://re.gzmigu.cn

[R77] 读取用户输入
来源：http://th.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://qb.wgjwhj.cn

[R78] 交互式菜单
来源：http://mv.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xv.jctech888.com.cn

[R79] 解析命令行选项
来源：http://sa.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://if.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://xp.chemitech.net.cn

time ./run.sh
来源：http://pw.hnjuh.cn

================================================================================
来源：http://rj.panjiajie.cn

S. C / C++ 专题
来源：http://gu.nicolike.cn

================================================================================
来源：http://lm.huixinmuqiang.cn

[S01] C：Hello World
来源：http://zf.hahajie.cn

#include <stdio.h>
来源：http://xs.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vk.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://of.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://no.shtwfgs.cn

[S03] C：读入整数
来源：http://ts.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://cn.521024.cn

[S04] C：字符串复制
来源：http://bd.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://af.chemitech.net.cn

[S05] C：字符串长度
来源：http://as.haigaiapp.cn

strlen(s)
来源：http://ly.bookmarksfly.cn

[S06] C：字符串比较
来源：http://yp.chemitech.net.cn

strcmp(a, b) == 0
来源：http://za.hahajie.cn

[S07] C：数组遍历求和
来源：http://fo.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ca.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://vo.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ps.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://uw.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bw.9csxet.cn

[S10] C：指针与解引用
来源：http://la.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://wt.asd995.cn

[S11] C：逐行读文件
来源：http://pt.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://tq.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eg.shxzskj.cn

fclose(f);
来源：http://ea.yuntaijiaju.cn

[S12] C：写文件
来源：http://cc.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gu.lnxyls.cn

[S13] C：宏定义
来源：http://pr.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yk.nicolike.cn

[S14] C：枚举
来源：http://vc.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://ne.hahajie.cn

[S15] C：类型转换
来源：http://ye.szxytkj.cn

(double) a / b
来源：http://le.huixiangedu.cn

[S16] C：位操作置位
来源：http://cg.szsharing.cn

x |= (1 << 3);
来源：http://hd.nicolike.cn

[S17] C：安全拼接字符串
来源：http://zy.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vy.lnxyls.cn

[S18] C：命令行参数
来源：http://wi.szxytkj.cn

int main(int argc, char **argv)
来源：http://ug.shtwfgs.cn

[S19] C：快速排序
来源：http://de.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bi.yuntaijiaju.cn

[S20] C：二分查找
来源：http://qs.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uc.bjjhwx.cn

[S21] C：字符类别判断
来源：http://ux.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ky.nszjky.cn

[S22] C：字符串转数字
来源：http://qj.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fw.lnxyls.cn

[S23] C：随机数
来源：http://nv.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zq.yuexingan06.cn

[S24] C：获取本地时间
来源：http://fw.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pu.wgjwhj.cn

[S25] C：内存拷贝
来源：http://qh.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://qo.jctech888.com.cn

[S26] C：内存清零
来源：http://gc.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://ad.bookmarksfly.cn

[S27] C：定义常量
来源：http://ur.gzmigu.cn

const double PI = 3.14159;
来源：http://ta.gzmigu.cn

[S28] C：静态变量
来源：http://im.521024.cn

static int counter = 0;
来源：http://su.newstarts.cn

[S29] C：变参函数
来源：http://zv.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rx.gzmigu.cn

[S30] C：头文件保护
来源：http://zy.hahajie.cn

#ifndef X_H
来源：http://hk.newstarts.cn

#define X_H
来源：http://fj.hnjuh.cn

#endif
来源：http://po.shxzskj.cn

[S31] C++：Hello World
来源：http://ib.wgjwhj.cn

#include <iostream>
来源：http://sd.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://go.jctech888.com.cn

[S32] C++：字符串
来源：http://jn.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://bz.shtwfgs.cn

[S33] C++：vector 增删
来源：http://su.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pb.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://qm.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://ef.9csxet.cn

[S35] C++：map
来源：http://es.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vt.gzmigu.cn

[S36] C++：unordered_map
来源：http://tr.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ea.9csxet.cn

[S37] C++：set
来源：http://go.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dy.jctech888.com.cn

[S38] C++：排序
来源：http://hd.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://fq.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://ur.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yo.muxihuayi.cn

[S40] C++：查找元素
来源：http://hc.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sp.9csxet.cn

[S41] C++：类与构造函数
来源：http://vn.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qn.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://bj.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://gz.gzmigu.cn

[S43] C++：智能指针
来源：http://du.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://eq.szxytkj.cn

[S44] C++：引用传参
来源：http://qt.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://bh.colortex.cn

[S45] C++：lambda
来源：http://ga.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uq.huanxung.cn

[S46] C++：函数模板
来源：http://eb.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tu.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://ss.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fz.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://pi.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lo.asd995.cn

while (std::getline(in, line)) { }
来源：http://lv.szxytkj.cn

[S49] C++：写文件
来源：http://lt.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iz.jctech888.com.cn

[S50] C++：格式化数字
来源：http://tt.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ht.szxytkj.cn

[S51] C++：显式类型转换
来源：http://tc.panjiajie.cn

static_cast<double>(a) / b
来源：http://ms.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://wg.shxzukj.cn


<!-- 参考信息 -->