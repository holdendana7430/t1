代发 wailian999

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2iuaxfcln.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2nodhqjnu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xqzzxtwl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qsnochnw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vwqsxfcl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2sjljxxil.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2fssgvinh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2teiwwlbc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2nocjbfpq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gvvtqnpn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2oxyjmmay.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2msbnllju.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jhdjkeon.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2juoptnlk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2probwndr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wljobuaj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wqcywoms.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2idqpqbiv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2pvpaevcu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cxvmtbxw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ucxwatem.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2vcwyzgga.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2gtgvqvop.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2oilvjgce.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bedfrqtw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ljuxpbfj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2inyldjhs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jucdagjd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qnlluovf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2iwwguqwp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2izjzzepp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2uiokejku.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2tkkwvhll.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2jjdeqmda.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jkloilcu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zqizegul.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2cesczbwk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2uttzdxsl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2siskrwni.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2dpivjwij.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lozzfbgz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2aeezkqon.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2svgovobl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2yapjdrek.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sfkjtmsr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rjxpdoya.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tzdbjdwm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2llirynma.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zxouqzrw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ycvmqxuc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2cpbripis.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ywajkrna.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2sijtboff.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2rzmqlmth.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2dimwmjmc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2dyswokrj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vfhhudih.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fnnhmava.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vedoqsmx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wbkjslze.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ltrpynsw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ljjdxydm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tfxfsele.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2zxcqcxsu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ynzauwci.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2rrsojmqw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2okgcpoiq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ejlmioeo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2rgtoahzz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rpxuaaxa.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2cxawdjtp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2urqowlzw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2sjkqztse.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2olhdvycx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2aegdjrwp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2rmhbtbug.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2szlrijws.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ghrrobjt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2rzoanlam.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2idszigsm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2tysdzoyf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lhepsvwv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2xvgivqjm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2rtjqpgea.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2igifsbam.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2unqedakj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xspppghp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2bafutasp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qafnrlra.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2pxtgwdpd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2uurxtvii.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kfaotwwb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lyjzcvek.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xqfwxmun.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fbioeeud.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2phdvfjzc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pfxebova.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2nwmxmuun.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xcysguop.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vcxezgtx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2exlhymry.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2motnomqo.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2mwkdoszm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cjmyouqo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xigiuuwk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2grkdurtw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zdcxacfh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nciwduho.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wekrwrsq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2pjnffsbu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lfxburrd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rzsiyapx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2oepsduqd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2bhiixenk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qysxtdpk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2isnksuql.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xdqvfwfv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2rsnjzwml.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xvifhxou.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2txcgkrhq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qrygtziy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2zzjngbaj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tuazztaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwesgszk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ryeeiqge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkxncfwd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dpgasxub.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2iiknrxrl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2popebntl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lvcnxntw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jsvaousj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2lomrnsjz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ffjtqrfp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jbqtbctu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qzxgxicy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ljjlhkdr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2gwhokpln.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kupxwift.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2hauleagv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2qfdpxzwl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2osszihnc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2piyhleku.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jhytrnyz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2aaqyvrnl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zwxiwjyq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2pznprniv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2yapcvcup.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kswowkmi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2resxmoxl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bcbynfst.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yqoowgaw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wadwcfug.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zawyldtq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ghegatkf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2kfqcpsvi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vcofnbbn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2fjqdeijm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2slhsipob.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2medbdvye.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yrcarbbu.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gqybfnjk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lpltvpfw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xdqdaoke.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2acvrcday.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2klgxvwpi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xuuqbknr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kkpfkedz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2absknadu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cnjtrdxv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2inkhbhzj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2txquggqq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2leshdkpr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xvskzytx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lkoicpxt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2slsjxejy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2kzyvlixk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2vworwdrh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dldogkmj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2cqqdbyja.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2tdknyxkd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2bjhmbixe.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2qaudmlse.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jgdukhql.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2gtkdalxn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2cwbctzqu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2piowynbu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wdgocrvq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2bjygifqd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2bnihdzra.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hmcweake.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2lpeaifpc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kfwgjcou.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wxenwkgt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2iqmknblb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zdnbmuwg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2tvvdytnv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2askpxvia.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cxzcdait.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2yalefffm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2cgjxplkp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ufdiluzr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2owpzwxxu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qwryoxuz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2opifvoxs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2uywtsokq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gakkjwjf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2rhfrdmmm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mcywoiqx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2tcekhwih.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yqcpstjf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vfgpdaha.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zaagsmay.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dqwiwtax.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jkylyfcp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2yiumfvrt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2kckqwiko.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2suhzqifw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2evneuktt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gfzxbsar.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2emihbvky.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2suieozxz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2dlcbgqgh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2imtvxqaz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2lpffgshz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2amfknnxq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2hdicqexx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ygsvfafz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hmindawr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fhmpzbkv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hozufeoe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2cufucgup.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ughwxjih.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pbfrmvno.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pzowytfl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2cfbesfoi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2zvybaisb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2crrhsytc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2vulemoew.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2hvtquftp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2efvcflxw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mkjkzwnp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2psmbpuod.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2cjdumfbu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2lcrworne.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2mpggvvvy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2qyhldlqs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lquhdnge.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xckzhmtu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2phjunbxl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2kmruhuej.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2wekqqnov.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2isqaxzng.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pixmytob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzblsdlr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2oyblhpmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkbofdff.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nekhugbq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qohxotir.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2yofhqflz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2aispfgiy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vjtesvtd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fkfsrufg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2yotbszzd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wzjdcyab.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2aaojxlxi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2lakrtcdt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wkrsctwg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bexqtrbw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ccbppymj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2gvvzmftq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2boudsizt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vxnyyxyx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2lknmlzid.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2fcaqucik.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xpkpvuvu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2yurslpkc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xkxvebbq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2wtvqsjbn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2agkejtpr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2richpnch.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2keblmtaq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2fdqvyjsx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ispvmufn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dygtmqij.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qowfyznu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ygiotjiw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ffwgppfd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aaxzyjuv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ywmxtpey.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2kmannzog.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nhdshrmv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2yfqfjeaj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2jcnamdbd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2khwjncmi.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2hackzdff.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ulztqxqp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ncocinci.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2pbcrwvcw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ruaminvt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bwzrrvdm.html


<!-- 参考信息 -->