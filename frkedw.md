代发 wailian999

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fpibtkzd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qexqawjv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ouabadqo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mzjodtvw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3evaxoulq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xziacozk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3dokkynls.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nimydpwf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3suhapuyr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ytgyhbwl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rzxnxycs.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3cdztnedq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3byersmyy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3dqtkaffy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3igytvvyk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3lfoxokjx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3aipbtzvt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qzrgmmmv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3nkhaprvn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ijaptbmz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3cmieixgb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3eynthlrp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3eclqcbsp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3psmiryzv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3riamfocb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3gqfwovhs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyudygjx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ikffynzi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3glwfumpa.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3spmwfyll.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hkvdimyu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3dwfactsj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3becyorgs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ycrtspeh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ehdotmsw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3voiapmvl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3urajusom.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3iutqdinr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3nnjfxreh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3khuirifs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ggxjfnzl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ejhjklcm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xowwbdny.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3pwvanffk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zhppmkyg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3qqghutaf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cjkhsdmd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wdbibnty.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vryczjpd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kcntqhfm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3kaqcvdyn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3hjxzwrxy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gsxqqzcu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3xzabrorq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3pjmmgvfx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3toiknhba.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cwivcwcv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gwdbqers.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kvkkellk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gcnabanl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ukxvvzbt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3fhnzhdsu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3avortdjh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3kpwbtkuc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3vxgeixim.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3nkrcwvvc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ubgooeoh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3hosifjgj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3rgilmodd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vtgtxmmg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3norfliaa.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3iolorgor.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3nwtsxrxl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3rgfzdvjx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3knwadwyc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3olbergqj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3awafwkqc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3qdxzdrbv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ykmcsuan.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fjguphsi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3dqmdgnpz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mxuikvri.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3kwxgbpxf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3rxouysim.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3muioxhpb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3uhbotiit.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3bvbgurpx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hwrmhmdo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3yyucrvkp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3fgqwkofy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3afwdeatr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zrsouukk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3nlcmftic.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xcyhrlmv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3xqqhzpgr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wbejddec.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qiidlxlo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3wnfxyenp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pjkikxaj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gidxvync.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ummynlib.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3tssaanei.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ceijbqqn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3neiofjxu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3kvjsvnvc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3hdzcyntb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3otuxyvee.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3dcruujxq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3txbzgfve.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3iexixzif.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wivvhrbi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3xbrhxzll.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3zenzbzni.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ztuekeqk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hcavgwgr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ouxbhbmg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3shsmunbs.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3mbhdfxyf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3mfegrvdm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3cppdiiqi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ukopmmct.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3quvwdqvx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3dlxtmcnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzgjzqfo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3imcancka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eawqyjyq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dbjivhiq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3aimfsxeg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3icjfbjyu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3duadnwpl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ikvgniys.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3hbspydzk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fmnyxfwz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3onzqbyhq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3snixmzip.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3aygmyuyq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3crfqwfgt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zfplyhso.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pzyudykr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3goazduxb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3uncpacwk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3csgsojlp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bjojmkhs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3tabvdeuw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3chkzbhws.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3bqzehqjd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rnadonqk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fjhfysgd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3tqiljomb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3exfvgzzs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ywfnucxo.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3nxmcugzo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vafqjkbf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hcuyxpvf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3jloradgd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ndjfxcgi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3rubmjcog.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pfxyzrjc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3livnmggv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3prgcntul.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3zpbulecy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lyyshpcv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3jaekboio.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lamoebtq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3imjasemc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3akvvyjqs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ahuqjjkv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3yylfbnke.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vvsrrtah.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3yulocglx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3giuhwiea.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ofypilpg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3mfzkqnqv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xshrjpwz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qhsjfcgd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kbaekuyc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wohddlnt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oaooxhln.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xpbpnwih.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3rpwwkain.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3riqbhpqz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3tkrcolmw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gwmspimi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3fxsiscpp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3nmqnjthl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3sprnxrzs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3sloyityb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3hqglynhw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3mlpmdlij.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tgisgxsj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3zvsdcizh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mvosyvhj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xcfbsurw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xiolvcdc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3gwrehnmq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mkhlezyd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3gqvdasna.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3defdoahv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yfrwegvt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3oqvgmrom.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zytgvpcx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3udugpcrt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tjvpkcdc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3axmfffay.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3dkvzojay.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vjbmxrfw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pnqzcmsg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rckowvvm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lzfxzxjj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ibaqlyoq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3cjorxbdj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tlzyjckp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3crbmcxng.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3uxtxxxit.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3dcnlowmn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xhdsglbk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3whcokfjn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qehbrgud.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3yhqyyeuc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3gltpagql.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hipskmuv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3zwtgbtyr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3pvqpvtii.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tadpbgpb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xgwnqnwe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kunxcshl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jwtzfmpl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3fkegangl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3arnquvzy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3glsxknkw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3dbzyhisu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3vfstydwv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xsuongwd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nebosdxc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3tukgqahm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ggtwyduj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3foltcsad.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3jxeiilys.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3apdlevkm.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hkzcfqji.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dltrfryi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3axzxmnkx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lgxdxjtf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ibteqzzu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3rucjeymc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ilplaspv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wahwgpda.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mdrknqis.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eqjubhxs.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ptzbchgz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wqwnwdjm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ikiptkur.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uqauyuly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvnrfuse.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wtnxankx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwizlerf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3occcfbwz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3imnpiocv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3donjzszb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3szoqlmdi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3orypcczk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ofkmjfod.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3thivkyeo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ydpmoslt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wqwjvufs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3tresxhqm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ytehlngr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kvucxwra.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3teqodnqa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3yqvwmhzx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3tgpqdpot.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3honuyeoc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3mwpzhcom.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3azahlsvx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ngfhiowe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ywtzokcf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3lzdfkznk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3lpezmodh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rwhnotwu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptqoateh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3eiyslald.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zsjhpvkn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ftawqytq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kwkkqlzg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ztlqgulk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jtuuqmet.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3npqorwet.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3omxduraa.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3lhfxtmrq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jjbwrgqw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3leqxaayw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3prntipge.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3imjqvycy.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3wradekoe.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hsxcbbfk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3icfmhcel.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ryyalwkm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zubkxvbt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ewuprpbi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tyfqsofw.html


<!-- 参考信息 -->