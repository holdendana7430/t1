代发 wailian999

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3qizqoypp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3yadedwzf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3jtnlhgjb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hzdfebxq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ennbgyti.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dzvubeow.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3xcfwiymq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3yrfkosna.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3toiguqmt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3fpxrkdhn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3dtulcfiq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3oxkcvuph.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3shnczbrz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3wndqtdal.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wscnowmr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewpufewl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3mscsallt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3tcjopdss.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ccnlgwep.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3mutkuepq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fjbypwnu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ykidnfdr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rfnqjjzr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3lkaflhkg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3lcwgpenu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3iadnfyfi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lxxdrzas.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3aojkspsy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3kttkcpvk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3vxhwyzsq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3iuupkrop.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3msxazrat.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3imwctadn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3orfeigbd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3lgmjlklk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3upqirzft.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3piudtxhi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3usfykpzz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qihuimtc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3tczfdymu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wnoqfzkm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3irdsnqzu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ermfvvrx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3bmgjrhqv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3eohmgvha.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qtdvcdss.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gxeeunxb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3riknqhgf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3cryvpxuv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3nvcmycmq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3lajfnjqd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3krbbkdaw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3paywzote.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3eyyvdfgr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fkrefknx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ktlgfjbv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ssbthoog.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3tqqhsalq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wdshxjml.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3iptisqaf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3efuexveo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3eibqfxdb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wburxzhn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3azxvkulv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3bjurepum.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3urysnwoj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3skxzvrgm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3seuszqdz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3xdwzwmfm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wnjedfli.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ajtxtuyk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3aunsdyxu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3zgzhnhvs.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3fctdxtwb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3djioiqkb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ssyldbvz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3aqsryivw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jztzhudy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3qxxwgkfy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3shvdtkba.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3pptfenox.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dcuciwjt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xxtszpyz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ydbjehwg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3pqqoifer.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ioxgvhgt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3dvlnkykb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3qfmrpvia.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3mzuaderg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3yvfxshak.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3netpnbcv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3kxtjjtzh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3siddbswh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ovixlgdp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yemwzpft.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3iircjomb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3acazthkg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3tdzuxmlm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ihbiysvd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jvspsqng.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3kkbfuira.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fffvelmt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ruvyespy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3yzpwivoq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3pswldnth.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ovexxmzz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3gucntsih.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3bykehwts.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3grxsgepb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vyupyepc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kwbqlpec.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3cubrmtol.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wxpemvia.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3pauabgsq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ospprsfs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3hhuolakb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3irhkrpax.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3civjphsp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ulamrdao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pyonofgw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3nqxptybw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lthwonsh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ctxwbalm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3pitnxksp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3rldngffn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3cloifquh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3olyyczid.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gsjwjpzr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3igitkkin.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tvpitqrb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3mlelhuxa.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lvhqomkq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qdazeffx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3flbbvbju.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3tbfiibph.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xkpectve.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3gmyndwtu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3qhavipxx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jgnouurc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3opabxxbq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3moddtmbc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zsczfybg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3huzwlctn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmnsolkq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3obxgktgt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hqatzbso.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zcvgadub.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ktpyzbto.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uyfqyquf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3riaiazas.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3pejatguh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ehxdovob.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3sqjjfbnc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sltguemv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3vqntfyal.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3mooseiqf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lwjwtaqx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3davgtzcd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3frfxriun.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3znpcggdd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vxnpduac.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3kbuuyeus.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fkihejoe.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3stamegih.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3criyhhch.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vitwjuwn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3jhzqymwd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qhwpjdwj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3idvidtot.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jfroburr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pkzbamqf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3rgjfbyhs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vbivhhrb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3eenixaes.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nvbbyroc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3cfwzsseg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ziqdrsyx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3lycoxgoz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vwywnpem.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3esspyvix.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3klemfmsy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ktqslbof.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3npwafeey.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3iewlqxnv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xclflevt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wcxvbnsq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3bappdrbw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kpzsulsq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3cvenzooz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3hfeezxub.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mdmigzxr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3okkpkspe.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3desvmjbx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3gedeebwz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ccwzzxfa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptauzfbc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ydelqisu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mslctgix.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3wktctwua.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wczqglrh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3teruztbc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gbngixpv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3tjrqnrau.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wayrxlvt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3utkevpgm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3caizntea.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3bemxnxvh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ftkhahaa.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3pubzpxwb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3oylltxrj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xxrpzalb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pmfgoxkt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vcsvxlmt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hphvqahk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3wsvfjpio.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3klsxvrnz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mayhldrk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gcoxgsjk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3lzjhpkdz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3icuhffyr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3nowcbkyy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qukoduew.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eriskcrl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3yntmrhhu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3dcwaquue.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3yktwoukh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mpvdublk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nynbxxhu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3daopjaaq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fitnjsdx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3revwjggk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fexocmcw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dtiwnrab.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3wjviypcz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3awffqekk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3nhkzhrta.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3rvzzlpyt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3prnxzdmr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3fjaikrmj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3apxohfnd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3uqvmafdh.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3pfersxst.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3iwposnfq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mvhmmmoj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gigjeiko.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ywyktccc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3gdlisapf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rzseovmh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3guqtwawt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocuxshzt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kdzqcvib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxwledsq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lahsplef.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3imlmzrrj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3wtkdaedn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hyzgfbur.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ehznuspp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cobaybpy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3momudgwo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kuompbgy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cadxryyr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3mflcuusl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fnmssjld.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pciwclrb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kbfmvkhc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mndedlbf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3relgomti.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3syonpuux.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gvpzsrcn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ycrcgyif.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ftgrecym.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3tsnchray.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3mtaelbnx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3udfntuwz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jrtmwfkm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vpmnrutv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tyudbzgg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hdrweqrc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3sgwjryjh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3smonisvw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3eejzvdsp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3trttigln.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bladifiv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iutfclff.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qtiozruj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3leaxwidz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dzqhqfbu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3zwcrqqjs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xxbdovlo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jirudizw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3jwthhlya.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3yhtlwnbj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tcbukkci.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3pdqczxtq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3xsiedtnr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3nhohpyal.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3eiavheqv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3faobemgw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3rlazoeem.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bxmcnjdj.html


<!-- 参考信息 -->