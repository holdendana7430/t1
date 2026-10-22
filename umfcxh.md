代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qorehlmr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2crfrcaee.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ftadrukj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2noxkshwc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2wbbtryqf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2okbzyjmv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2szwwtfhj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qjobiags.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tntsesmk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2svdgmryo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sycohrqe.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xpbrbkjv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2hotdtden.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2doyvxfwj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2blrnjaxf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2atvrpixw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jxmrseen.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nfrmepen.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ijsfxngv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hahujykq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2tnirxbpz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ippfajav.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2uohjmckv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2mlhibyhd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2cjyqpqcd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ryvvqkqe.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2lchxclrh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pvccecsf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2gflzyiim.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2iwnkhqud.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ilanujxr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hbylxztb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2snragnma.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zvxqarsc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nrpgtuwk.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mknlazgz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2szjezmhx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rizahego.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jmpskaxm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hgswsgmw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2girjlzwa.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2xjjklqdt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2iukblxwl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ylvjttzx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2btgnhlnb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2opuycoim.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vtwbaizw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2stsvhnxu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hjkocyer.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mkedvflc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2wdgpsdyq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2sgvukevq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jvtsgpgo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qcpjlurp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lkglaafy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2howpjtbc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2onldqgxp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2pwkzrawa.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2jeiguwjw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ovppifxg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2jviumifr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2nyjotbzj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vdpwyhnl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2sxwxpvre.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pndkalae.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2gsoufpkx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ddcmiqhi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2cqhlfjoc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2nzdgbdgb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2jwaginbo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rjyokhqq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2cvosechn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ummckegw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wgaiehgh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2drtsezje.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2fetpspku.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2sickgddi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2oguytapr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qcbrqchm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2tliirtdp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2qiquokxz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ywmejwpo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ismlhvsi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ohqlrwcb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ynwylnqv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zopleyht.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2pybkdtmh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vnkkgwxx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2fkneqzpr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zeirbgrz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2cocxwfev.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2eibjoxrs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hpbdmlqd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ziudaayg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2hpgashhk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2rqlavyvp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2wmxmtyrx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2vcathprt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2cwsrrasf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2glnovgic.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2zpydcfgv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nutbigng.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2juttzdxz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2sxhrocfe.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ihjllaud.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fsouidgi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2fyblssyr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2lburpazy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2qjlgwbzp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2rccmjiez.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2xkfhdjwk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cbmqyzme.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lkuebyln.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ojhiidvt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2agdputir.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2uxgstcyr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2kunrfozi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dvaypakk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fznqlmte.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2usmzodmg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2bxjpimmk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2rdsrmqxy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vbjsgdzq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2plbjdyxa.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2maajivlb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nfmosvut.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rnulkrrr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2vlimllng.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2pydfxfkf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2xwqburao.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2jnqzbqdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzplwvzq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yvqcreay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tecxjvzg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uoklarjj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ijuiyazy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2coawetww.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2cjlimoon.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ypyhhtxn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2skpelvcm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2pivpuhun.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2bomahrbj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ktiiwaow.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gxetetil.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bmbdvrbt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uzgyumpz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2hgmnixjk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2tszlaqcm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2miubrutj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2syrhjlcc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2kaglfreo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2bsegzixs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2hqjgfhav.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qxcbpgei.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pvocmqtq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2crvwyagf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2zediuhcd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ewepapyn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ffddbzvj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gffyszkw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ckgpnzfp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2dbctoozv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bmkhfhwu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jedxjuzc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2crhjlisp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2axyobkme.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2sqqhaogu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ttpzeacl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2udjgrvwb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hjryywik.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2fbegpwul.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mwjzotsw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2lykdghba.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qtjixoww.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hrtzsvca.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2gkdhsdcu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pvqolxwr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vayqwxcj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dfbijbnp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2raswdwqp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2dahcxvhb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xvddjgai.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2eesujqgu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qurskjjx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wlztvauq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2dgeoizky.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2qmizrpsh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2thzeytze.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lntygijq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xmkpuuek.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2unxayjcn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lxalclvi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2frkuuwrp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ztcmidgc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2hfovypiy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2bxfyhvhq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zziglwuu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ovpbrsgt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ikphkzem.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kvjkxdec.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2uvqhlbja.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2vcqvdgec.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2asxmqaiv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ouvvihkt.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2sbbhftmu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2osbqsxph.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2yvcakyfz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yidcueyz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rcnziswz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ehcdlzyf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2anbtopvv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lfuryecq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2iogbvpsi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jcloiqtg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2rvrmjbye.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jpskfruf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zzkcppie.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2mfriyuzv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2nzfksafh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2uwnirknb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eqjbrjun.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2dixeemvp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2lauzxxiq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2nkpbquhj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2grsdnmpb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2uqxmpytf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2velxdvky.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2uddjgwgw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2fpeduuwl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wjnsbfpz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2gbfagvgq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2vxhtpobk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ojvgmtpf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnqqqqpg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nttfqpaq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2sdtyttju.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2lduqurok.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2sfdtxebu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xfbvvewp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ttfvffqu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vuinguzc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vogjgnsw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tnxlvary.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2lisdkgod.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcqeqnbp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2xqxeyfud.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mnmknrtf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2srfqerkb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hgdvbxom.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2umslwkip.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2heyjbijo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2teyezrfw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2dpuvtafq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2mvuoytvy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2spvctqhh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wyhdmmfk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vpqjitao.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xdngwuse.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2fwrffitf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2weptyywf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yocmvpbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zshddnze.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gzdsqopj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rkiypodh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yfrhdrbx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wlyzqstw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2cxtooxul.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ugnslott.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qjishcft.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fhyawngd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2kzgzxzrp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2aytfzgkk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hdccjgqv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2crewmuxi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ecyrwzvb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2paqupczc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xsnqmtnb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2eathpecj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qxtovzsg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ignhlipv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2syknnlqq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2naexfevc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2nszadkqu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2fubcgwow.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2clphkrmu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2grmjvuoi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lveamerd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fapfwvvj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2evigswcx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tdpxgfhl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2udzedsft.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hyzzszyv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2efryttur.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2aikbcien.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dsicsegb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vosxbgbi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2tppaakur.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vqbceomp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sznoshdo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2syfzeozg.html


<!-- 参考信息 -->