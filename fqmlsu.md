代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ckcqanuw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2nivlsmrw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2dxpvksmh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2udmcumwu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mejovcvs.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2flqihplc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fxqqpzuw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kjpldbho.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ubhqsnft.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vyciebcb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2wiairkdr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ugjtpbno.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kleahfib.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dokrdcir.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kikyggkq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2dxsmazcu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2pgldcfqa.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2gdiajgac.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ysvhsnir.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2snjjlzaj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hahndmgo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vxqbnyib.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2grfoeqol.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2joxeobmg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hmdqzrvu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lopiqvzv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2pompixeu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jtrtvufb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2cnkfjjoo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2myayeqbx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2brofnosc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2njqhcwsh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rajjeuxs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2itcybzfs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yehrcslo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2uliktzgt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2eqwogsvp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ckgdnrtz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2yipjcgsc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2dqwxzicu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qveblgqu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2sshsxjub.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ozegfirx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2oohsxxux.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ygcavsuj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2drahfwpt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2nutzhalt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tpjshzvu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mamwrmpq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rzfahjtf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2cttbpojk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2axdwfevs.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fbemizpn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2pgshocre.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fxbzsrqe.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2augglqym.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2pmqdwwpt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2xakkqmtk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qxcfpvua.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2oruuqvia.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2owzpmzpc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2beiuzczg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fclwcjnk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hrrgrqrf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2aqmtvfpk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hvfgkxpy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2amlcaqns.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2zigcuqru.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2oggkwzrg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2riveuyhz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dswkpzwa.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ludqhybg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2kcyhyqjz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2moacojgm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2swfsshdq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2rgqbkpft.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ecdvzpid.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2fppqawzd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xfmmqcqz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2yuhyyksi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qtbzixdf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2kuesgcsy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2xiprkavy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cocchvvy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xathymfs.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2yjakybdt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ceccfbvf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vuhqoeiw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gzjaofdj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ritpalln.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2chbwshae.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tyonaqkn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2uwymsoqz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2btrbauhj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2dlweofyf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kikdtase.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2brgafkep.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fqocgcpy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2rvrdbudl.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2vezwoubw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2oypsnzui.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jwtkurqs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xaeojnle.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ofbxbtkg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2npaotatf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2pusbgwcf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2cbwutgzi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xpqmjkka.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2yxjseofs.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2rkcolikc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ezzdobun.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ucxnbwdk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2fyzwwtkl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ymqylocm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2kibsjsed.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pgwcwxrb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2rfowwshq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2kevnzknz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wadwthuo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2wbrbhqgo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2yuchymsw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2lkmvkxdh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dsmigzek.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2cflejpcc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ikiyggop.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2xryrjsom.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mutehruz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyiwlfbn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qabuueme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbswdvgz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kucrxwgm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2cetdlkqk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyqmwobf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ezpqtpos.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2wrntqdfe.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wrbnoaqe.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gqftlzdl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2itanidmx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2whnoybtp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dsjiujvq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jepjbtce.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dcenaren.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ycjxboww.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2jwvvvxnf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hluuylsl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2jpasbbnn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pwwcodru.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2iugmwpif.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jiypcwen.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2heobyhhd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2odxppyqh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugirpzlg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2uquvtnku.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jwpzyvpi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zyaurwoo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yivmfpvs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wsqpmwvr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2hkldmxiw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ejcezxxa.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lzkzbhgf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2mnttwmna.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2txykizdo.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2cfehnsgi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ognzqxhd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fbmgvkpd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rktofnyh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2wcghvpdz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2iehobxsg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2rkysgmkk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2vhievyuq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oisrzyhy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2uphllwlq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vptbymyl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2nsuiuncz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2nmehcmtu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jzumpvzn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2brveudfa.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2evwacdju.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2mkvgceef.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vvomlgsy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2btgvjffi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2cpvibubb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2snmfwxhm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2glrchbep.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2giwvshtz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2dalfscpk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tztfqrmy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ykujocgt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ixuzevog.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2jfitovqe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2jjeiqghw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2dcsulqyt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ngdrvyhf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rnnuvebm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2owavwgfj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2misjiwno.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fjnhgqod.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxmkcrjs.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dxkqvbar.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zeguxfug.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2cyphnwxh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lloyttke.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2fptxbhwh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sakqggtq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mfcsscqx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kceyjrao.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2azhrlcej.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wunmiqwq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zjaxffvf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2djdmkmxf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2immcjbir.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vcnltikx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2dhqdklwv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2dqzrjonq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2vqyrsmhi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2vformnbk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpxnjonv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2dknrmmbq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2claglvvu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2tzyrkhgr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2whwqvcuo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qoyyyyny.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2iqrwgyqw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgwbkaky.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vpsgcyrd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2fmnvluki.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2enysbtdb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehbwvdap.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2afddepfz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2oizwrgtd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ifnlkuub.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ridtnpku.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rilsxqse.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zvhnctvz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2cutqexgl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2nymzgghr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zyluxxsi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cbqlroam.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2xlzruzhc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tteigpxh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zqnyblbx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2oskknpyc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2bipkpeax.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ozysnfpp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2porecpdx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jlpzzcrw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cbynsumh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2uunjmkwc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2agieweyj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2pjfjqakf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kjxpuzdb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lagljfts.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zpztrpym.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jnkcpjzj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lkctnlgn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2fnsrzwwy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gvnofecy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gftrbshi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2yeafcdtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbbewhto.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fuylkfpk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wusmerdi.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2pjxbkvja.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2pmuoyyxk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2jyezllnk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2znbnacik.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2xnyublnb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wefznyqt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tztexjrt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2yfvwsxfp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hzkfsdrd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rtijhzmk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ziwcgzab.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yvdlwehf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fbdfabfi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2sqyogpdx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2scffcdjl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2tgbsvefe.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ktuqkczy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2lqcfcntw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2pexzgosf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2umzlhnyf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ablmayoj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vvxrvuph.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lylwffuf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gwdblbmm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mackvbrx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vuhiahsh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2lwxtpiaa.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2yppsfrrj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iluskhsw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hpquulvp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2yvjycvlh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fmfbktjz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cglkebqr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2bvdtmfnl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2mkyqsqcc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2gynlvpcr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qxdkoekw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ehdmutol.html


<!-- 参考信息 -->