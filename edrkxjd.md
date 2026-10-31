代发 wailian999

[Q82] 字符长度与字节长度
来源：http://lm.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xl.haigaiapp.cn

[Q83] 大小写转换
来源：http://ta.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kn.newstarts.cn

[Q84] 去除首尾空格
来源：http://xv.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://rh.bjjhwx.cn

[Q85] 数值取整
来源：http://dg.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://df.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://lu.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://df.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://zm.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://is.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://br.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xx.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wr.szsharing.cn

[Q89] 判断表是否存在
来源：http://ur.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yj.wgjwhj.cn

[Q90] 生成序号列
来源：http://ne.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jv.asd995.cn

================================================================================
来源：http://cw.panjiajie.cn

R. Bash 专题
来源：http://aq.szxytkj.cn

================================================================================
来源：http://ja.szsharing.cn

[R01] shebang 与严格模式
来源：http://gi.szxytkj.cn

#!/usr/bin/env bash
来源：http://wy.gzmigu.cn

set -euo pipefail
来源：http://cm.colortex.cn

[R02] 变量赋值与使用
来源：http://sr.hnjuh.cn

name="Tom"; echo "$name"
来源：http://qq.shxzukj.cn

[R03] 只读变量
来源：http://ed.chemitech.net.cn

readonly PI=3.14
来源：http://od.newstarts.cn

[R04] 位置参数
来源：http://nb.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bs.nicolike.cn

[R05] 参数默认值
来源：http://lz.9csxet.cn

name="${1:-default}"
来源：http://cb.colortex.cn

[R06] 判断命令是否存在
来源：http://hr.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rw.huixiangedu.cn

[R07] if 判断文件
来源：http://df.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bu.nszjky.cn

[R08] 数值比较
来源：http://sb.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bn.lnxyls.cn

[R09] 字符串比较
来源：http://tm.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dx.wgjwhj.cn

[R10] 正则匹配
来源：http://sj.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gp.huixinmuqiang.cn

[R11] case 多分支
来源：http://op.hnjuh.cn

case "$1" in
来源：http://si.colortex.cn

start) echo "启动" ;;
来源：http://vo.nszjky.cn

stop)  echo "停止" ;;
来源：http://cz.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://ky.szxytkj.cn

esac
来源：http://zd.newstarts.cn

[R12] for 遍历文件
来源：http://pj.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://gh.jianghongdianzi.cn

[R13] for 计数循环
来源：http://hd.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://nf.muxihuayi.cn

[R14] C 风格 for
来源：http://dh.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fw.bjjhwx.cn

[R15] while 逐行读文件
来源：http://gs.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zd.nicolike.cn

[R16] until 等待条件
来源：http://ux.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ut.9csxet.cn

[R17] 数组定义与取值
来源：http://lj.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gb.nicolike.cn

[R18] 遍历数组
来源：http://zp.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://np.lnxyls.cn

[R19] 数组长度
来源：http://nm.asd995.cn

echo "${#arr[@]}"
来源：http://vp.9csxet.cn

[R20] 关联数组（字典）
来源：http://io.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dy.lnxyls.cn

[R21] 字符串长度
来源：http://gw.colortex.cn

echo "${#s}"
来源：http://tb.shxzukj.cn

[R22] 截取子串
来源：http://sg.huixiangedu.cn

echo "${s:0:5}"
来源：http://hh.szxytkj.cn

[R23] 字符串替换
来源：http://ks.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zj.newstarts.cn

[R24] 大小写转换
来源：http://oj.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sp.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://ms.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zr.bookmarksfly.cn

[R26] 命令替换
来源：http://zi.521024.cn

now=$(date +%F); echo "$now"
来源：http://eb.huixiangedu.cn

[R27] 算术展开
来源：http://zo.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://mx.yuntaijiaju.cn

[R28] 浮点运算
来源：http://qb.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://ah.jianghongdianzi.cn

[R29] 定义函数
来源：http://aw.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nh.wgjwhj.cn

[R30] 函数返回状态码
来源：http://fq.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://gw.huixiangedu.cn

[R31] 局部变量
来源：http://iz.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://oq.muxihuayi.cn

[R32] 参数个数校验
来源：http://ay.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fh.colortex.cn

[R33] 捕获错误并提示行号
来源：http://li.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wl.huixinmuqiang.cn

[R34] 退出时清理
来源：http://oo.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zc.lnxyls.cn

[R35] 后台执行并等待
来源：http://ot.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ps.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://ul.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mk.hahajie.cn

[R37] 把输出赋给变量
来源：http://jm.szxytkj.cn

files=$(ls -1)
来源：http://fc.asd995.cn

[R38] 管道串联
来源：http://oz.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://uz.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://lz.chemitech.net.cn

cmd > out.log 2>&1
来源：http://tr.jianghongdianzi.cn

[R40] 追加写日志
来源：http://gp.shxzskj.cn

echo "log" >> out.log
来源：http://kw.gzmigu.cn

[R41] 丢弃输出
来源：http://wt.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://xs.muxihuayi.cn

[R42] 输入重定向
来源：http://xa.haigaiapp.cn

wc -l < a.txt
来源：http://sw.muxihuayi.cn

[R43] 按名字查找文件
来源：http://no.shtwfgs.cn

find . -name "*.log" -type f
来源：http://sq.hahajie.cn

[R44] 按修改时间查找
来源：http://mk.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://mn.hahajie.cn

[R45] 批量删除
来源：http://jn.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://dn.huanxung.cn

[R46] 递归替换文件内容
来源：http://sy.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://be.yuexingan06.cn

[R47] sed 单行替换
来源：http://dm.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hi.shtwfgs.cn

[R48] awk 取指定列
来源：http://jp.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://dv.huixiangedu.cn

[R49] awk 带条件
来源：http://yi.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mh.szxytkj.cn

[R50] awk 求和
来源：http://id.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hf.9csxet.cn

[R51] 排序去重取前几
来源：http://qt.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hr.hnjuh.cn

[R52] 统计行数
来源：http://ez.asd995.cn

wc -l a.txt
来源：http://rg.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://os.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pz.haigaiapp.cn

[R54] 比较两个文件
来源：http://so.hnjuh.cn

diff a.txt b.txt
来源：http://ya.huanxung.cn

[R55] 压缩与解压
来源：http://on.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ah.asd995.cn

[R56] 远程拷贝
来源：http://vt.bookmarksfly.cn

scp file user@host:/path/
来源：http://uh.yuexingan06.cn

[R57] 远程执行命令
来源：http://cy.bjjhwx.cn

ssh user@host 'uptime'
来源：http://qe.wgjwhj.cn

[R58] 下载文件
来源：http://ok.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dx.panjiajie.cn

[R59] 发 POST JSON
来源：http://av.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fy.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://hh.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mu.9csxet.cn

[R61] 磁盘占用
来源：http://qf.hahajie.cn

df -h;  du -sh *
来源：http://ur.nicolike.cn

[R62] 找最占空间的文件
来源：http://kc.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://kp.bjjhwx.cn

[R63] 内存与进程
来源：http://pd.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://lo.lnxyls.cn

[R64] 结束进程
来源：http://qb.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://gr.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://wy.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eq.chemitech.net.cn

[R66] 定时任务
来源：http://ps.nicolike.cn

crontab -e;  crontab -l
来源：http://ih.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://jw.newstarts.cn

openssl rand -hex 16
来源：http://wn.hahajie.cn

[R68] 计算文件校验值
来源：http://yz.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gi.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://xc.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://rg.newstarts.cn

[R70] 时间戳与互转
来源：http://oj.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://ee.asd995.cn

[R71] 日期格式化
来源：http://kp.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gc.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://th.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://st.szxytkj.cn

[R73] 分割大日志
来源：http://fu.bjjhwx.cn

split -l 1000 big.log part_
来源：http://nc.bjjhwx.cn

[R74] 批量重命名
来源：http://fm.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mr.shxzskj.cn

[R75] 导出环境变量
来源：http://do.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://mw.nicolike.cn

[R76] 使用临时文件
来源：http://pm.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rq.szsharing.cn

[R77] 读取用户输入
来源：http://kg.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://wo.haigaiapp.cn

[R78] 交互式菜单
来源：http://uh.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ev.szxytkj.cn

[R79] 解析命令行选项
来源：http://px.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://su.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://rk.yuntaijiaju.cn

time ./run.sh
来源：http://ro.huixinmuqiang.cn

================================================================================
来源：http://vw.gzmigu.cn

S. C / C++ 专题
来源：http://pr.panjiajie.cn

================================================================================
来源：http://qp.shxzukj.cn

[S01] C：Hello World
来源：http://ct.hahajie.cn

#include <stdio.h>
来源：http://ku.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wm.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://st.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://gg.shxzukj.cn

[S03] C：读入整数
来源：http://un.521024.cn

int x; scanf("%d", &x);
来源：http://er.jctech888.com.cn

[S04] C：字符串复制
来源：http://bt.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dx.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://ns.shtwfgs.cn

strlen(s)
来源：http://it.bookmarksfly.cn

[S06] C：字符串比较
来源：http://rm.nicolike.cn

strcmp(a, b) == 0
来源：http://bq.lnxyls.cn

[S07] C：数组遍历求和
来源：http://us.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yo.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://fm.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://md.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://on.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dh.hnjuh.cn

[S10] C：指针与解引用
来源：http://zh.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://id.chemitech.net.cn

[S11] C：逐行读文件
来源：http://vw.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://tt.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dq.shxzskj.cn

fclose(f);
来源：http://ya.chemitech.net.cn

[S12] C：写文件
来源：http://uq.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pd.jctech888.com.cn

[S13] C：宏定义
来源：http://gw.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bc.haigaiapp.cn

[S14] C：枚举
来源：http://rx.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://on.nicolike.cn

[S15] C：类型转换
来源：http://kn.szsharing.cn

(double) a / b
来源：http://xx.wgjwhj.cn

[S16] C：位操作置位
来源：http://cy.asd995.cn

x |= (1 << 3);
来源：http://gy.newstarts.cn

[S17] C：安全拼接字符串
来源：http://uj.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vq.bookmarksfly.cn

[S18] C：命令行参数
来源：http://xj.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://yw.haigaiapp.cn

[S19] C：快速排序
来源：http://df.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ny.lnxyls.cn

[S20] C：二分查找
来源：http://xa.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://au.lnxyls.cn

[S21] C：字符类别判断
来源：http://wk.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wq.chemitech.net.cn

[S22] C：字符串转数字
来源：http://nt.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ui.colortex.cn

[S23] C：随机数
来源：http://ct.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bu.nicolike.cn

[S24] C：获取本地时间
来源：http://xd.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wi.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://ii.9csxet.cn

memcpy(dst, src, n);
来源：http://ma.szsharing.cn

[S26] C：内存清零
来源：http://uq.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://kh.wgjwhj.cn

[S27] C：定义常量
来源：http://ik.huanxung.cn

const double PI = 3.14159;
来源：http://pj.muxihuayi.cn

[S28] C：静态变量
来源：http://pm.szsharing.cn

static int counter = 0;
来源：http://sq.521024.cn

[S29] C：变参函数
来源：http://mm.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sc.bjjhwx.cn

[S30] C：头文件保护
来源：http://si.szsharing.cn

#ifndef X_H
来源：http://en.szsharing.cn

#define X_H
来源：http://ak.shxzukj.cn

#endif
来源：http://im.jctech888.com.cn

[S31] C++：Hello World
来源：http://lt.huixiangedu.cn

#include <iostream>
来源：http://mr.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://tk.hnjuh.cn

[S32] C++：字符串
来源：http://vy.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://sn.hahajie.cn

[S33] C++：vector 增删
来源：http://rm.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zc.nszjky.cn

[S34] C++：遍历 vector
来源：http://ke.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://cv.jianghongdianzi.cn

[S35] C++：map
来源：http://ff.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ek.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://si.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fb.wgjwhj.cn

[S37] C++：set
来源：http://gn.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tt.panjiajie.cn

[S38] C++：排序
来源：http://fl.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://wg.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://um.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lm.asd995.cn

[S40] C++：查找元素
来源：http://cl.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kc.asd995.cn

[S41] C++：类与构造函数
来源：http://kd.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oj.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://du.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://ep.shtwfgs.cn

[S43] C++：智能指针
来源：http://pm.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://hg.shxzskj.cn

[S44] C++：引用传参
来源：http://al.nszjky.cn

void inc(int &x) { ++x; }
来源：http://tp.shxzukj.cn

[S45] C++：lambda
来源：http://oc.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nv.gzmigu.cn

[S46] C++：函数模板
来源：http://ed.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mp.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://ug.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bo.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://qw.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gx.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://zb.szxytkj.cn

[S49] C++：写文件
来源：http://am.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vg.panjiajie.cn

[S50] C++：格式化数字
来源：http://xb.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tp.colortex.cn

[S51] C++：显式类型转换
来源：http://xo.szsharing.cn

static_cast<double>(a) / b
来源：http://pr.colortex.cn

[S52] C++：const 与 noexcept
来源：http://mt.jianghongdianzi.cn


<!-- 参考信息 -->