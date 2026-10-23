代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3axmdfwao.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nfhqwurr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3nkffmkww.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3thdunufv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ludegksf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3kalcptvm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vzslosbn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vtzbrejq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kaogkrxd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mijnmsbk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3lrggqizx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3utfyxnun.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rpzsohyd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fahvecac.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bamjgptg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3eyoezbrh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3cabbimpj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rfkycoxl.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3xqiwugjg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3avtmhgcj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jjymettf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3teznxopm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dbtnphst.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lsgwdbye.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xvltjnuc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ngagtjba.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3udpdytkn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gclaetim.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3trybdzvg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wwuvkbru.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyjxzzxm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3cwqzpnsg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3pyrcduez.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vwjlgmfc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yfyypooe.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3csbnigua.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3rtthqvgb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3wbvmwypy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3bcpboelb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3gohcucsj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwbznidm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3opmrihkk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3lbskpotk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3vxwsejhw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jracngrs.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3xbqvdfan.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rwdltody.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jsnvcgaa.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qqvpbddz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wvosbudc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3txctycpv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3owcszwmo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gziqlqiv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3fdxjlaca.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zyrtdhgf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3tkqwoyzl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nujozmmh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3lnnsclzg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3seaaunce.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jufphvcp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rvyjqbdy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3vdxlpdso.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pvldbhbh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3litwapki.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3kmsxhepg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3cimpcqlo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mcccuezg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hneazzcw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3jgdobgan.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3cyzeflpd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mexnkwyu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3lbnxvlkx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3rzqqorrc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3asxpvnvp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fkrsivgz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qrylzllq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3toeqmwtp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3fbpqsoii.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3anjxacul.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ukmtvget.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qrqdhubk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3otzunrrg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3nkaitxbe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xcsnnfsc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3akifaijp.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qcajjzyq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3zrxpxeic.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ulcjgvzl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3dclrwshi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3humjyqht.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3txcgliff.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3enqmauug.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3qmexyqxu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zssqcrih.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3fwckzwfp.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3bjosyqcy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3svzqlkpg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3sscfyscn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cfviguvg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3jtlmrzel.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3rezwnrjt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3yzsdklpk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xnqimwhb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3yhgawrzn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vmppzmxl.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qizqnlnq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fcfkuhpl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3klykugle.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wmosguwp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3lwutvqmy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kqkzkeop.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3eujsevyi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rgwqbhvd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3mgecbovu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3duezsyfr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3zblgwrlw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3tbwpvgxm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3icijjqoy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gmlgferd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3cjckgntl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3kycqycdw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3boxamyps.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lahohzub.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3pcaznwug.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3xqnrcoxe.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qiuuzzxd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3kpbdpxkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odsebeod.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zcnylfkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnnrzmyj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hmliuedo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gcucbmod.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3sybszuuw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3oyfkpaob.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vjzqdysg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3hfsrlzel.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3vraasnux.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ioejbvzp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3oumjogrv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vrysgiui.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gbvuxlnp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qukrfxth.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hafwisrj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rhiideub.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vqtvfsui.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3cklperkt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3yocifzcd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3yrbcsiws.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3knrghtuc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3yadshcfr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qtglfsvb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3veqszwdv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3krfwxbkp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jlanipuu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wtznmvpu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhljbqfb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xuronyud.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3acxvddad.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hpjgpqpg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dlgxqwza.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ctcrowvd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ubognfcv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3yrkvjfpx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3skvkzyfh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rmbljceq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xchxfegi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tucufgqu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bpczhfab.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3dqxanroy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hdtzjary.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hrhzzmjn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3pwvpwxfr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ljfpegwp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3wwjuqrsb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vyjutvku.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vcxfhgcl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wngmzykx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vynlqlkv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kehsfucd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qdcrezth.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jaicrjfd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3dygijgbq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3cypceids.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3trtznpia.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3eeqmlduc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3exwehsjh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pfuviuge.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ajjhktel.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vwmloagf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3dhloutee.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3urisyvez.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3crjtwyju.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3pjpifwoa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3bahmtdvs.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3gvaufdwt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zlbryhrn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qpzjiukl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3tgsbnkug.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3scbbkpfh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3msitzdwj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3nddfmmhh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3cfulijsj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3udxbqbfn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hggrwzxu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rpnofnpd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ruopvhwm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3evdevrjf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mtepuclc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3nhhkthna.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aqmkmgbf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jewgrbot.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lxdqrmzn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lziqljow.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3yzmwobwq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3cruurkws.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3crplclgu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3haestguo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vjyniykg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3gaqlgjxg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dypnhlrs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3hqktivuj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ehbtgcja.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3fwwknsii.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3svagrboa.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3zsmsahbn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3spzgyfzm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3clxnqgin.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3feuumend.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ckwlfjvi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3vymrszre.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvwvkfcs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ymeistys.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wzoiajvf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ittmjfkf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3xpjezeov.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3avjgbqlx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3useycriw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lzwwyzqw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3mubeetca.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fdsqrcvk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivbuvdvj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3uypcrlst.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3llxucvmc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3flgnlbwi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3tmlwhoel.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3mbkkihml.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xkaklrno.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ussyullx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3lehogile.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ftmmiyxa.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zckuruay.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3uolryqqk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3dxadtehn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3xcqzbxrp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3sagbbybw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3twzasmhv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nyqaajhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxmmhiud.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dthxyuby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhadfxmk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gxpxlptd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3npnyiunx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3auxusicd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3nmxgfgcx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qclesndh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vhvygzut.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3mmowmzuc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3srsytvpw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tltvdboi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3rulxygjp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rnuavfxe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vhyqhazt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dminuumn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3kdiarfly.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3vhnydwld.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3subajkkh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ilveyiuj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3veksgqkj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kkaniioz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zyxcylft.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nerygnjh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3zsawybya.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ypfgqclx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pdgwjbei.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3fvapzpdc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbcpipxt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ektmrrmn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qqzcnrmp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3pslugmxp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yofiyaoc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gqarfsqg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jkzqrpql.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3mqbsuexw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3erwigvke.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ovipltdi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ndviosff.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lkpmmrig.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3nkwwewaz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zvqtsekl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rkdvmiha.html


<!-- 参考信息 -->