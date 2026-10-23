代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3btcnxizf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3yuebngkc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lpddzcdl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tqqoddgb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3attozqty.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wubswmkx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3egjzunce.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fvzdobhu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ckxemtwv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gsvprlkl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3qrzhcsgd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qersxyzi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3pqzvojzw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iqzznpiq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3fofsvuam.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3gnjeufwh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3cnonfvzw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3kexihdwn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zblummqn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3idbcfmoz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tumespde.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3htdsiphz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3nbpynavg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gefvjrmp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3dffxaqjv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dapdvcir.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3cqqdfpmz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ncnpuhjd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3gmyngnat.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3redrhxdy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcrtgfdo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3svwzsxvk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ummcokgu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3igtnmaip.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ocdyhhgv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3osoidrdp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zseeqius.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3eouhubxy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ynsgfyde.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3kzvleovl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3snktiyjn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3lbdzqzvq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3uasyqyen.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3whwetsot.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fjbcqvfo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3yknipiid.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ocwxinnk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ytbvxibt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jtidodgr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3gemdfrxj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3phiqzkce.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ptdbqpgm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hofjcqfm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3sogiaavz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dgsksulv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3xussodcw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3oludalbc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3whheyiyk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ptmjbaif.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3hywollwz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xrqjurxk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gyxxmmrp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ekfpxzgi.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3wvfnmglv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ocqysnzo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3labqxkfd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3twvovhmk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jzufdvqp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3uxutrwqs.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3zvddwstq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hxbmozms.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3heqhyubd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3bfqqtoui.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3aqkzkiyz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qhiiryef.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3umoratzp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3outsfxqz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3blmwzzgo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qpcoztsl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3eufootpl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ptmcwkzt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zjkvdmhh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wvuqncnq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3glcwdeax.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vyhhgibg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cxmovxvr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3dcfaupaj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3kppqdkfu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xyjpoaki.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3zingbxug.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ncedjusr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3heexzkag.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3omklofou.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mxzcporx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3oxhilcuj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3lvmnozwx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3egzshcmp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kcwylpae.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3gdwugkod.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ikjhjjgv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3aickhjpk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3hkqzqxok.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yrroqkzt.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3igrrlmec.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zfhryxfl.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zxqimsfq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3sigfhgmw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tnregmcb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3zszgvnju.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ftzyelzf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yknnpriv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ejpaxxsg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jzgzjbue.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kstwdglc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ggptgggk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ycyvlkbz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3fznollak.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lvcundvi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jqpnrbsr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3fxmajyah.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3rvwupvpc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3cihmuejf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3fwnmwzcy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3mahptbjl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3klhrdtvj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3cuhyuuyl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hxapsopb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xisnthpg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3nwicgxnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdvbsygk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tuacyxar.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3kgglpszc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3yitetzwq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kotjoxda.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3rzfxbrkz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zhnwvlaw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3zjegngzl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3svwrwobi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fkbpnioj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3umyzhppc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imeexfxt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ehjthfbe.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3edvgzbbz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mhtypjub.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ymzlnmqh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3rvcfwanu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hviqggsq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mmnrtawl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vqqoeevd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3uublehbp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zujlwuwz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xbptwtnq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hzyvtiuz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3bueuuvrt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mwiyuzfu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ygzvggsq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nmctzawk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3mtogiccr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3olccmecd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ycbfvkar.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3axjjvtzu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3atotkjhl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3aqghxilu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3utzrqfip.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rkyiyndt.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vwyrrbyl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3xvehsdkx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qlyakdnr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3qdawqexy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vjokfiah.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gikhquct.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3xijsgagp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tiiyfotu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bxjpokjr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tllobzgd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3whwleppo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ffeeexdg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3nkbwkqhn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ebgiqqfv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yvkfrdhb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bvnrsbhr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rvmfywpu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zuklderd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3haoaazkc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3qbovdddo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ydopruyl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ojuhqsmn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ktoyrcfz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3utbgujrj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xeeguoda.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3rzlcziij.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3dwtfjcgb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3pelgoemx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zcrknqqa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3sxxnnmto.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pbcvevok.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ktjpqlfr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcqjimty.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3sschtpok.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bjatvdon.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xxqelfuv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zjrnttmx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3cimytkbh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ntlshsma.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3rgkknglj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ofvfukeq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ftriffbv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zkwvmtas.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ybbymdra.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3aygmwnny.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nmbxuoio.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xgylfmuy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3zzgxpchv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3adplhcbq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3jnmftpfs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3srrkobfb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3bdtyjirk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3evagazit.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3dvlirfpv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3fihpxoiz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ghzfjtgx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zjzffgqf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3yiujiotn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggxjbwue.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3nnjymvxz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3mnkulavo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wmbdueif.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3bnqmmtkl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3iatjgkki.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3lzmakdbo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pdhwlhtv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rbrbqcrd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lbcbhijp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3bwgrukqd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ezrsvgsd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3hjnkmxuk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wneuygsp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3clycubrw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3osllsjku.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vukjpudd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouwjqphg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xzhodcun.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3zjcoraia.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3sgnftoua.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rkhxlysx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qpgiyhef.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3jjmwxlum.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3zbhppqru.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3egquwpxs.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jsdkdtnf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tgixwssu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3bdwlozbk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gruxswnf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fymfsias.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lttzbxeg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3kwhyqyot.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ljdlvnyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkvmttle.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cfmodlsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xszwoxss.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hcprttkp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xtafxybc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3kkbduckn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3nbiudhtr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3hdfjgqbo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3apfjmqnu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ufmegxox.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hfpteocp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mdqflldx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3tvalmiep.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3emhdmcqf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3keeqzfed.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gjqkunxd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3osqdyxqu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3rmleuddr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ovoruobb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cqlqbtbx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3yowciqld.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ltcrubcv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3rophxqud.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3czsbxztx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3mixtikui.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3xqlaaqvu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gzgorkbu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3yidfgxjf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3boqdmclc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mhwqhbbf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3aemixdso.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3iqsgvdpt.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gvkbrugo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3byjibirp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cisuerlc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3sbkoystp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3umovpsap.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dblkqsmj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ptzvimja.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3sojkdawf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3clxaojhl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zsetiucl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ybsmdgoc.html


<!-- 参考信息 -->