代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vztwgoup.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2kozicudf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2lqdtfzdq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2fgxkaspw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2quedpybe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2pobjcope.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bkuzwrdq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xvzojswo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kwtexkka.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2vspsjfce.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2yuscdkbp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lgaggjie.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mxicvoql.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zzocqxrn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2fsrontfh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ppodsfyx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kunpmkkq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2acwqjvnz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wxvhdsjc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hvspmitt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2kzlvzytz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ltfebjgi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2gzzibwfd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xfdgcuen.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mtvzuuoc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2gfioxdqg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2aawhplao.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qjxzpiuk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2foxyiajx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2neyhpzzr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2oqfyjakp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tkrjhsdu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2whjwwomh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2bofphxpm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ylthtqyd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fxxhwoqi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2pcitvazs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2shpckhgk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tnatcqap.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xxwnlqph.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2aqldwgtu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2pofpdxzf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hckmoqti.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2tmexxwvu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nvewsmpt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gyysadqn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2hhuzhqxs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2isgkhioy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hrjblpmn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2tshhagrp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2xpouptiw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bbayyujw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pptdacfn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2vmwtshbd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2fitvrbhy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kczvwiwd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zsmdgmsm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2scotzdpr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2htkosgns.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2dlgtdhos.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hnoxrrkr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2lxwwooqb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kbmvbnvi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2lmjlzdnm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vdunrnhz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xvofszdy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tfgmzuid.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hbjlnpka.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2jshxhkif.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2luaxeadk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bjmypoyx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2cosejrau.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2tweozyae.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2yoxxuqae.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zmuarfdn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2kiqfgtcx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2iuezprsc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2dbbpjcxl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2pzwbljnw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2zpctkilg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2nbvpywjr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cjvviofy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2mnsnenzd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2aicivpzf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2havbhnse.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ldrthzbu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cmvdpazw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2oeiphavt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ryohokbc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kqjakrbf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vkodzgyb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2pspcetoi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2jffslbdo.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2hbdzpaan.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2eegythyx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2lvxurest.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2mjpksamb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2bzrcglww.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2cwyeynwo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vtwhmlfo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2foprkhnb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vmtfuzqn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2cynuackd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2pdwwbsso.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2dqgnuopt.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2tgnlgprb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uktslqkb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2jnybziut.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bnphozee.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2afagwndw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2tbxzjlqr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2icuhhgff.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2wqnnvvyf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rnfnbbed.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2lgincmlz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2tabgxeqf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2isudpibm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2xdmqkhrj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nmquqnsi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ryvdtwye.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2kaeqcdcn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2seyjqoje.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vryuvqbx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qykwewlq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zzctyvtd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2sfdfenxu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jhdnehwq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wxpqgtkq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2himjxolj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2dtsslxdi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ruwzeiok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyqfcptx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mlsptlev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axyzixcn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lxoqhmls.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2jdpgwiig.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2leohuori.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jeujjngn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2afkcjtvn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vwghssbg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2erossomf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2uyzajeil.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ygbrrvmz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2heuofcms.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2hglelzwt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tqwiyfiq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2wrxhdpgk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2gedmwvtf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cjnvamjx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2pxhyclwr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2psiywzur.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zymagcgc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ksjikjtj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2owhjtxtp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2telsslvg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kktyrtmo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2tgwycnqq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2teqpohpx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vwwnwnhp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nnrvowbg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gcbkhkke.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2teyamrfo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2rbiumiyx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gddjzyaj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2egsowdlf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jqllljsg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2uanwoirs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2sajryqha.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2htuolwhf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zjjsyypc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ouslqgvz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gwpvfhul.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2sazviesz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ihedgjnv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2asbdwboe.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2knvlhksh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hxiduwhs.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2mtrkybcr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2vwgrmstb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wkgnrirq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2hsxtxhuj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jvgboyao.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2tijmotcx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qhhlpzap.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2rsypsvfi.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jqqfrmgy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wrmuzxoh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2vjzotwwp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yuhsekbo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2mafeqkhw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eguwchek.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tsreslfe.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qbzscehi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tlsqddeq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fmxkarsn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ndfmopjb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2yehmwjzx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2bqwfqwut.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ulprpmva.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2voadqizd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2pmjstbrd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2tzsskcgf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hkqbnoia.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2gygbzngb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2drpwyysv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2svupowhh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jngbdoze.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2nlmqwbgu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2iafhsevp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ldqwjkuf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2esmjifqc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kddstgzh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2bemeadze.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pehlnupo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2uywvzqtt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vykinncw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kvdrbigt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xvtpvlyh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2hmkymata.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2pcadliuj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2tpwwpcnf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vvgzlobr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2atciljkq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xqulllbr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ysxhcsym.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mwhfmprj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nmepqewq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2lbknmfsk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2pdezvswq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qfqveqsh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gkodkjsd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2vgkmwfde.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ozeghavb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2nqspleee.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2swvajmvq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2lmczdvmg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2imyrpwgc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2eodbzhnk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ozqkpxeg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ubgclgag.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mrykgxgs.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mpaapxat.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2qcxrtmdr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2eyxdleac.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2cnngsarh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2plupgqcs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dtjumneu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lhlcbfqo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ducsiuig.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2cwltapjj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nkoapkpb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2wgcpzvrt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2mjkagllm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2bxwyqoed.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xwaxhqnd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2sbbiyrxu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bixullmk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2stqxgfov.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2phdnwqhh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2katpgpvr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yfcnslsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omkslrdb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2hqjlfmab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwbrsoiw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dkgrxrqc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2txkxwifp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zavwzjqe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2blgrjabm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ekmazzrf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kazppirn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2mladxeiz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ebhqstcg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2voldrjsx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2dwmvghgd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bdfcaxns.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bwvpspwq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cutaullq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tammxfet.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2znxxzuiw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ngsiaovc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zatnvttt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lbjsssoy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2upkrqnaz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2pcanlotz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ldplehhd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2gmbdefto.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2iwjqhmep.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hcabbjkb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2dhttxqce.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ntepqveo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2djjeaeii.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2byjggowm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2epbmmkpv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ygbsbukf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2swxpxbji.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2racfydph.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2hpfnsnri.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2imeshzbd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qipbgbfu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2wlahzbtx.html


<!-- 参考信息 -->