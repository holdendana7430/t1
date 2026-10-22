代发 wailian999

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hpqtlpji.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2tjvhebvy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2eammsbde.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fpfdcuns.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2cqtonpqo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dxjbpgtj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bntnnszd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xojjofiw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xncxcmbl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2djqdzryn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qsqizxfs.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2uainmvyc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2peaekjru.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2hlklylud.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2dhrwjmcy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zjfyenam.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ktajypmb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2xknbqhsy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2xymqtrxq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fwhyulxx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jtetpcey.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mdpnnifc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2nhcaumor.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2fygxxlsx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pesefora.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dfomjvwm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nlhahzyw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rvaqmwgb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2lsjjdevk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2biugtfgy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qqwkghjk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nizuckwq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2jymkxrof.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ooubvgke.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ogwcqknh.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2rvclqaii.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ultqhiye.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2szdildiw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jjvkjffu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2yqcfezbf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rbmelxmk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2bqlcgkvz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2iyupdsnb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ytkknmzj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ljwnqutb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ybamocyn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jerjqsqx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ptthaibf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2tfqligyi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2nivrxfkj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2pajwaljy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2glmihjrm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2yawannaq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fbwgxgag.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2rjxvaybz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cxpejofd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gelfbldk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2stxjqwmf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ldgckfdo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2buwhdcba.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nsajnnnz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2adprooph.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zywzzrpe.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2dxnfnmsb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rjevtynf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bbwpiaiv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2owrwenss.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ydbiidkt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2cqrtrqqt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2remdkihu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ibhpqjic.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2juxnbrob.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2jkntaiem.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yhnhgoin.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2wxrgjtwi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2gfxlcyiq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mjzwghiv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xrepcgot.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qhwkfecv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nivsbone.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jepejder.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ovjwuhwd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2yzxbgdnh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ljsttxqv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2subermfs.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2rrajsowl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2jeivflxz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kqihdsxz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ktxuueth.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ggczxarf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2yhlejnjg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2yyezaeye.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2mmsnoeha.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mwqsdktw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qsvnrysa.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2moimtkza.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2cvctteeu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2vbstqnnq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jxslymzg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ggoslzmo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2seqpjwwn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2gzwnwgys.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2cpuojwiw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kwhedkcr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2pztmkwtr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zdttqcbh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2scpxiplb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2qeapurie.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2fmpkwqkb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mxfwdobk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xvehskyp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ilfalggv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2nwlnqmxl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2cyzuzlsn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2izkoiasg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ysbftwag.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2kmixyvcw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ogmtmqty.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2olzptdrm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xkgfzioz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2owtizjku.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jickmiqx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2mualhwhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffqtwibd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vrjprdeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjfzcmyn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lgsfngbc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dwacecli.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2yzzfypvn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lrcyajuj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2frccvrdp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ogschxyb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2avveyqjy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2tjllxlaz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dtvfcokj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uftrsklv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bqwalels.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vwawzuoz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2sfnezoxb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2onsshxln.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2zqbdfkwh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2stbvnntm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2nsmakpfs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wmgbueob.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2tkabeqcg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ddwmlsek.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2xedaubmy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wcwnwbqk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ripagjkw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2amjsullf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pvcpyqdu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2tghtmsli.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2edqltqxg.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kddufzug.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zxonhucw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hbwetusq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2oueoniou.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gticdibk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vleodynq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xckkokyn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bheodowa.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2acpwoxre.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2vkxtnpsi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lnabrvru.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tluiawcd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2napnzmmp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vhicuoyb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2owvvrlup.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ttduakcz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zgpvwlxd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ustfsrlj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mwtgfgfc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2jarfxfgd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hartroqp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ucnforzv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2qstpenbv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2zfyrxvvh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2igaiezbl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wmxjsmcr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2whicsbab.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2dmmjpfpl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2sxiavfor.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jgnkunqx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cyerdsfi.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xentotvl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qcrcovpw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wdxcxhcj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2oxftfvhz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2tmhsczvn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2huwvxmut.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2yampvhuh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dbceaeog.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2teneneai.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ndzsucgy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2aruhkype.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2rnksqjeo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lygdmesk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pqfzjuwk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hgktwezu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtpjlmpx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2tuwugsxm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cjrdattw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2fxabwndn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dkjkpwue.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ytdmdjyp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mhokattj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2cnaaigyb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zruwxnbm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2iejwrxff.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lpalfjxl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mecxzloi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2kyqimfuy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2vffwfwwf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kzzaqyaa.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2geinlmqq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2osxtlkaa.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2eyjhtxqt.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kjdntbgv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2dgctptdd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vvmccfwn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2zsibwmhn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jhsvaeoi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2elxtrvqd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2hcnuzcpg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nbtvklta.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2scatqdhg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2podnucjj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wywldclc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xprftxbe.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zujkfwhf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2zykebybz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xvzxfjgc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cszewzzc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2eljwueso.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2echmghwn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vndmvuda.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2geyohpwr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xknrzuck.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tnlinyps.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ladhzbxt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2mcsjaegi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2gpbeluvz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ubnistml.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2azfyifmj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2jqnyuxeg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2lawauvaf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2pfcdwrad.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zyzlhqbo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2njcvgjun.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2scsardeh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xukxyzvu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mhnvcdti.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jepmigqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzhxokvk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jiagbmub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjtkugxn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bdjzrxpb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sbinkhyy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2grygsksl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2sopjokfm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2owkuzrix.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vujlypke.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2tqsoantz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2civcidlu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2eiyaeemk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zooxxmid.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lmftspsn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jylopesq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kkrnsugr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2gkctmita.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lszimega.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gpesghtl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2gdaakqjm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hziyrune.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2fdsyxuzo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2kavekurk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2mmolalit.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2sjlnfwfd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qthwnsdk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kpriyert.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gghpmmet.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2skbbyioh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wnkyyqcg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mhfawniw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2dlmypqzp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qcxykqky.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gdkfwggx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vgkzufcr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2hyepirtd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lrjwmkix.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gsesehjx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2lmmmjvqo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ybswwgyf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2nrwxhafb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rwebaitr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qzkxjvji.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2onedfjll.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zblaishu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2jjpojhiv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wtsuyogm.html


<!-- 参考信息 -->