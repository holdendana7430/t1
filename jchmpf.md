代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3oncptacg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3odzznnyp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3gacaxzrq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wzkhavww.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3dopbynzb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3nnwiuwuo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ogpvmyvk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wopnmnvq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ilpcrlzf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cxszffmk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lehtotli.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ugrowavw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3yxoiurbl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3asbguwik.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3dbdmxgnm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3bvebtkpr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3hrobfdmr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3bklknyzz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3actsmnhp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ipshcmjc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3oidbybwb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3tplzrgqc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xdhvoaou.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xltziris.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ecogmedf.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rlxkacig.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3uopvltqj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ucqqfzyy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lexcnxen.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3iygphaud.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zamyrlif.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3nlbmfxou.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lzkcmueq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nuikougw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qvaynxbs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3hkdhzyel.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3bjbkdewx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3uecvytfn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3gtvgadii.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3imirbtvc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3atswkeys.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3lrhfrrlc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3amvjzlha.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3gcuyyamg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kfbebzei.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3xfpwrenw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3mlzvbafm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nrmsrtrd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kykxtmgq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3yclwaybu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dxftvbne.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3kaeagurg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3iotezrsq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ralhbeyx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3lyzvwnyo.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3uxeqbxco.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3vqyuiric.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bdeizshn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3dkybunaa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3kgaxqxac.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ixekvdbg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3trodvedw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3urgnnozs.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3pmznxogj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hyposvhi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3mpigxner.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hbvyyawy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3uwkxaucr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3wfqdkhlf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3cfuvycjx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xuvkrlzw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3pwuzhtqw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ztozpxan.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dyujwtmn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3djxqbmzu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3jmrfcqbb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ctcevruo.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3culmzzla.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3kbwxtmzt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3tscncios.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3iwtxiiow.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3svyvvuxh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3izgvsked.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zjcgogxi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wajdthor.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3klpmzguz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rdsyiyfv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qemppxjp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3mkwtdwnb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ogbgareb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ibocagei.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3gujimycp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3rmhvxprn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3rajednac.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3kmgspvzz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3uebaxatg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3jugvoapa.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3hrexqvjl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ozhzgazc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3osuxbldf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3mefoqjrn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xjqvsiba.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cxqhdnhe.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ykvruowy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gwcdyvci.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gqngnswa.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3neukskti.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3staymxzk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3twjlemyq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3cybxlyez.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rklgepva.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3sypeqqdd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3viocoscr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3adlcstbt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wblfkkmz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ekjxcyhk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3aqwygvir.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ygoncmah.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yezylzni.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ydeuafsz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3aovqsjif.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jytliymi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3kuyfxtkv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3irrpojxn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3whzgdttv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3zexuxvvw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vhqfywdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfeofznz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kulgaojz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfexiosg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aibeyrhw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jgrddibc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fjcukdmm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3lrjzzrxl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3yygnazzs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jgurysuw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3flebtoch.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3cvpitxgs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3skdqobov.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ywgoiqno.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3atzdjdte.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fotrwfdn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zpkzmctx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fzxhkmmw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3cellmign.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3lvaljwvq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3agsqhcgn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dxgojaay.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3htiegdfq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ylqcbrdg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wgiweedr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aeezrayf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tbczariu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qbnbqppz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rldsktsh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3otctoaig.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hxqkzjti.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3pouwfhtz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ttrjsoyi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3aodvqsyw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jmudecyk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ldrrgihb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pqtjlgmh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ntprkncz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wfkeewze.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3govrwjba.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3tkbtntei.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jlqcdlsl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3mclxfeni.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zdvmmfjr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qrxthqcd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3dwcctasx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kefovxhz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bcuxnoil.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3aqvirufg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xfrwruly.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ubzllwpn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3sucdpboa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3uoraxupk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3nnclrnmn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3llgngrgq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qmkdnuvz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3szganhqu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3psjxvjha.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gzolxoea.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3demxeyui.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3oxwgudix.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3urnppuoi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3bloqpkvs.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qoltltnz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3djbuacis.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3bcvkghzm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3cwbkinfd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ivrthffo.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3lbinneyr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3srwmvnpb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3hmkyjhzb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3qneyjxrs.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kvyrlhve.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3twjticng.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3bsrikbqj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xulidavd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qaqkqoiv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcvogyii.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3szfzldwu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tcxvzecr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3cmhzsein.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dnowznsq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3sbjxhgxo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3kzbcbeqz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3uvsedwth.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ntucgpcz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3mhjalcsl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vluhttop.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3nimwmzhn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vyabojrl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dagftgqk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3eoyllsma.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3sccdhfeb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3etvxatmy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3edaqmoeg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ajyqolfx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rxodvumu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nycdbmju.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vluilbde.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qlswvtwc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dezrossy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbfodkno.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3rjzutvob.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzpvvdns.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rjiwaicm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3nujvsqfr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gofaslix.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qvmziedd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kiugdfxk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dkdwdsqy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uhunymjq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rtfvadqc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ecfqwoak.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3aywaitxs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3egrteqhx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3eayxwmid.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xgiuibkl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3bavexfeh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3teyihrpa.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cvrmechv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tqtvvfiv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3pcfrtcoq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3imjjijdc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3pgswjltw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3beeqwsim.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rrvxxlwh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3klqywqkx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3iztkched.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ljdgreav.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3bwtyiuyf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mnjskujr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnygnuag.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qvzgmsvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sowxnhxl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iittefyl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jrqxbjik.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kxnwvlkr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3frphzxdk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mgwuywvt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ygtnftyo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3griwsnfq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ioaynrde.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jjwflkxq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3yqomdegj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3eqtqurun.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tuanitlb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bafzrjtn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3pbeeuyij.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hmahldpf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jytpbyrt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3koroefxn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3xriczmpc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3nqljidus.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3awssrenp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3svxtkjlv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3vjjigybl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3nnezbrzn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jpytvdau.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mgrnqoxe.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bcykmdje.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ibddffno.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tdetybjp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3wbtdftgo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3bwsylirw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qtbwghnh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3buglesza.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3zybpkvcd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mzkkjpny.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qqwnzngu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nuszuycz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hgrhuxuz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3crgebemd.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3fgvbdgww.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xwsfdpov.html


<!-- 参考信息 -->