代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ehewepbi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2asnxkuon.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2giujilkl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2oftthrts.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wdnihwrh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2dhzpjzza.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2zmwwmyfd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ddkuofah.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2rjxwklqw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2zdaxwpzu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2wcibhevi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hmjlecou.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydlaxspa.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2cdafjwet.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilgqevch.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2kabxwhuf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2sqhvgegy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vkqelnvo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zmwsayjk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ollbjscw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qawdnjzx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rytmvdlp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2aujcbmkj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2fkcwzilo.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2rssflgnn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2dktaaibt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2tktwgszq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2bkgmuuzh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qctgfiwa.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2khzrcpld.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2igvfjprn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bnvqklcc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zprnlwxo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2gbctpqsn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2saubipdq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikzhjgig.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ykatojxw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2zgzjglxd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2odjefwug.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ffgxxhyx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2clvfzgit.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2bntzdwjk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2fpdxujax.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2qajhhsfz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fhjwprzh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hhbggehj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tiwtkzrw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ahpghjsn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ctxkzqpw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hvjpdgtn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nbtbqanm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ktglfush.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fzgrtojf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2wkweluye.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2uktvmkov.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2sxnynozk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zjfxxuci.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mucagptr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kwdkuunm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2bxwyhwqr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2iuilmpim.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lvksuscc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2epfkrgqc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2mwjwrmvl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fidwyztc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2trsvbfys.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2xryjltoh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2uzdufpok.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hakjtyim.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jbunxusd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ngigugdc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zbdkansb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2tjedoyfy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2bmyloucs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rgtudihy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2cooiwbkb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2haticaxx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2iqtrofaq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2bdgihfkh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2fubbibvg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2amsqanuy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kjdffisz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2qzuceawx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2svprouqg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2suzvwjhm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2npubdjog.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2abiwzslw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2qdpwzfhq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2rvilthop.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2dajechjb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2gyhkqlck.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nadzpmou.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ufowwsgx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xpnubpvf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2epkkbbrz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2twaqriqo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wlkbdhvx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ildlwmya.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2nfmhxort.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zrvkvkuz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2foasxmup.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2skgjshyx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2invbnmud.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2lfhfhcvz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2emdkiocx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2uykwexnm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2prqucisd.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2gtzbcwld.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2zqbumojg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ohewyhdv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2egwhkvdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szfcheru.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hdvxsjlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gegxnehm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ybcdxilh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2zvwmjdkz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2qutnctnh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vewbgwrq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2whxhahol.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2gochhxry.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ndbahcxe.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2cyyhlgvj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2pvmkzunt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bnfspdtl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nnjvhjyw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lqkafyfs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2yoldsfox.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pvprvpos.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2kjzbpwyo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hjcthhuo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2dtgcotiy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ahjwwogk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ozfxobdp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2rnksowos.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pgfbtgbv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2auaddgel.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2qcghibrh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2actzcanq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zixdxagv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2oxnfoxew.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mimtotgd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xzwknnkl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2iqxckuhy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lwxlaeul.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2xncvqeyo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2earkxdwv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2rgjqafbd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2dygfcwmy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ropgcqat.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yjtnaogr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jiipfvvc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tnufnuuw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ltbldzxs.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vyhupjlc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ufuytxpi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2tlvchrcq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qovamabt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ltepcqct.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2sedgdkma.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2sosavhaf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2afxdtfnl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2rmnjpfsh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ktztxzfd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ukzsjsib.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ddtrzmsi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2tkhgbndu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2vhdlkdfm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ghgeojnv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ehcltime.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2funktdmc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hssabith.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rtablcoi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2fwccgbyl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hfbwveqz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vugncdfz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2otavjpke.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zvovbnxy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gbprukhb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wavfynmh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yhvtyimn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2gnxroopd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixmduwca.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qlsoxmsh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ruqvtsxd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ckuxuudc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bhtgnire.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jriieqap.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jekciukb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ofqevrbb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mdmxvixm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xncapkrv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vvvpkfmh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2uhygiurn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tgqpbpal.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2oslryhpe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kwzuaiwk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vizxnnxi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ydbbefyt.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2lbezcrns.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vbczuvol.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2raniwyqq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vlhqaijs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2uupxgwcr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wnqiczpk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2cusoiypr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2djazafis.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jlvhdnlv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdidqinh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cbhbrvwi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2srbqjbzo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xizbkcfh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2atqqqkiv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cyzchffg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2qayzjrjv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tffkmamz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ivagrssm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dleepibf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gxtvrouz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2fivcgpzx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2kugvwxxz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nqcskfaw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2vminpjwr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2qncwfllq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ayivytfd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2mxafaipk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2jnqwfurl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2reaqumyf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ifbzzqef.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jhotrati.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wxtimebi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pfwcsbsm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2rpmvaafu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lacbhdot.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xomzyehy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2httzgyce.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ncodzqzv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2joybrquq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2pnukiiwf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2jcskxcmx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2bypintii.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gmbkmpue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yiyieejz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2iwujxxwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgnxguvj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2otmcvncf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xtjftdhk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2mbxxiejg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ipccrntm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2sxfexvwv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pvnrbenc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ldkecuky.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2mzeypzsw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vopbqguf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2bojyatpi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ruivitwd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bvioablc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oihaivbp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wkyktwle.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2picgpsje.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2juxfuqko.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2riyiefov.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2kuqafohf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2qqaxeiws.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ggcovorx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2yhaisgoo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2luxyoxid.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2cughwwjw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wvbcueag.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2sdjongcs.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2bjzwipjn.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fdwwtcxx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qurdnqbx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zghnbixy.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ybupwjyz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2runoegan.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uipjljvp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2jtmvojpp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2racjzlza.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vmhipnkj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2codrjodj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xoximacm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rwizgmfl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2jioubpdn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2aimpgvxk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kstgnxea.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ycjsfouq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2fdwotgit.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wqptqbmh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mxnlzced.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hltaknsa.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jqoilkdx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ouxvphxh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yvzlxfrd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2pzcxsrvw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2lpgwkepr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2hkxugvlj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gqphnssz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kvqsdayr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ytlqhlvq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qsjpxnyu.html


<!-- 参考信息 -->