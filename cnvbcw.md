代发 wailian999

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2mosmxvld.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fgqchqas.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2thlfdevv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kyxlksgx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2jzazkprd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rfonxgzb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2khcchclf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xkjhdfxm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2uuhomirk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2cutppnsi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2inlwpxxa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ioiddrhb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gcamounu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2sfabvwrf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rtjttlhl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ntuxgokp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lzujqnoo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ktzfxmne.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2unhgqpbz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zswhoepv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnanirbj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dzwvhldf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vnhjxuqs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qkrvyves.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2gdlzfgsh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dhubzlgq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2psrewzfg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2lwhcjnpw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2smjktsjh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2grovpjno.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2dptyrrsl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2nfnwkwaq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nbpdyitj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2hjlctizh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2rrhxxgjp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ootzmncx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hjcyuhxz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2kzumiqit.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2combqhyy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pofiarck.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bactotbq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ybmgdgjn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gjpkygar.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2hwyodnmb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ryctxxir.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jeeogjto.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gugztrzh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ndltnrib.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2fyxgoysq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pdvodoxh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2jtcrooxt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fmbzsalw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nscvfkls.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2czycovxs.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2twdzjizs.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jrrbfmhj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2tepcdpdq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zlvibcvf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2opnkmzyo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2iezxrzus.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2fdhakggt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2cqwmpzjz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zmcvqnll.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2vdxnbivl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2feoypjro.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2cwasxkto.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qqsjpzvt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2trgznaib.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2muxzktlp.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cwpyllqw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ukablzot.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2aqckolfp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2yspwypvi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ygecpesd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2tuoynnuc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gyfdfgtz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2soucjvho.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2enopjyow.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2hbgzzxux.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2zuudrmzb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mkzzmbgf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2earrdyfs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2jajckyru.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pdmhrjze.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2cxpwojxg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2cesrqezd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2umyahnnx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xecrlpjy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2fhsnnezz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2psqnrffp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2otpmbanf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2varokybk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2rlnudbel.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2olwlapjq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2krsqjpov.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bfbmjwtp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2yjubnrqi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2yihvjxct.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2hvhzzlhd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qgckttwq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ehrduenq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dypytyua.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2yyosbmlb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2fmjwafam.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2kibmlhmi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lnlcarwx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2wgbfsvnn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2nrpxhmwb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2heboniou.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2woiibqcm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ntxfpqro.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jtrwwsow.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2dvrxnjjn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jifksmys.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gscqdihs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2gtofjcns.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2mzqgxrox.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2mnrkzvjn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2oyuwjgnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ornzguta.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zexlzbww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frypihhj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vnamotwr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mhoxzwbr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2txhhsgqw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zcxskrdg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fghdaxic.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ylltqriq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2iubhkvol.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2fxbwardp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2csjxgrlt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2sdhqqqwz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2qhnllgns.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ntdyhizq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2csjdczon.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lmpaifsk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wpiyamgh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2camwadvv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2onjuahpq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2sqpkfujc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2lqfbavcv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2dbrhxino.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kuelsvmu.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ppwlpabz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2jsshwueg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cmnsaond.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ulseicjl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2htrozuxs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tstlzehy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2uglptfek.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ctrckjen.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zlykzznp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2lyntquoq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2eykulwaq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lybchokj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zyvwtoqu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lwzhyzph.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ohqddhoc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2xjxmhkzf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2szetbjll.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2spulruvr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2hfydymyy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rqdpmfrp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kcvwhded.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bdzqbfvt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dadlebfn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2zynejwsg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yiieqpjh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2dlbgvmlg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jmvrgypj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nzvfeawn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2sgomqtro.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wutnpuyj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2axcsorfo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mphcczps.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2dtespcma.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2jxptbkpq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hvtoqkmc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qiojityz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jgiqatqa.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2njymztlf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2gyireklo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2hhdcrmwn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2yiypwsvz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2fofuaknq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oualoqjr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2hoqkozrz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2thmcvzsp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2xxphsgzc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2awtrurjl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lesjajmn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ggqamecg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2poyzdqjp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rznjpbpn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xprojubu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2dplvdypr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2megfquhv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tbczpyxz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2bgfmkdcp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hzskvnuv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2rhmfedzk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mairkarn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2khycdvwy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mexeoudf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2mabzgakl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wfltuose.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fbihxpdr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2fimvexdk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qygnyapw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jsbuvjxi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2usegstmc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2kvhxgxpr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2rdmxfofn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vpbjywjh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ftauylvp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2xhgpqjyz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ttifgcrs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2funbyppb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2bsetiscy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lecjjlqe.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2gwdhmztr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2saiqeutp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2klylhmer.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vbazcfyo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ypcotafx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2syonogjr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lsvmoxyk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mlttwkue.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jhjbasen.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wsvqordu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ynzauhft.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2yctwqikq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmfcvctn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jycbwipp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2attvdzoe.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2emjbqtzf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wfhvhiil.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qofuxuaz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mtssossw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2hfpaheov.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xwnvyiei.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ncllhroa.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2poypfojt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2cpecdrnk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ituobekf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2glkeestn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zebonldb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2pazbjctd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qbdvwqei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tutccmlf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gbnqyfmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtdbpihm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pyzblvwt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qdqgeyai.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pjryptfw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2jhoucgcj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2lzbspggf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ektvdnop.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nawoeliw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xkmpchid.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zkounnxn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2yimcjvuz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2riolrgex.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2soqfufge.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ibjsmxmf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2iqgtylmn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tfsqycgx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gvfbpwvi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2gtdriwat.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2tzdeprpa.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ssidqsic.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2slabunjb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ojgscyqm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2cvasidnh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ajseryjy.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nghzzxln.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2axutrqso.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2dstjrawl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xwgkcrhu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nnhorekf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zszsnrsx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2slvudhas.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ypmbkwon.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2apllqece.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2smebghic.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2pdyrhalc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cvomyxct.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2lcfwzhgc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2chlluqyz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2bezcytpg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2kixvfqay.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bdggtfdq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ghkfwkcp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ojvjkkrf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2kvtxwqej.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bwpdnrzm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2usgwcdoh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2slgwinqh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tjkjcuuo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sjvclezv.html


<!-- 参考信息 -->