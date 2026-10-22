代发 wailian999

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2lbgasnsi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dfdnwwda.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2tvpjkvge.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uvjzauua.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2nhnheiph.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2auzbibpu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rhxasjik.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mfkuvfxl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2xxurazrd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vdkdgquv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ldegavjj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wjwejvlf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2becvfrkk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2mmxeiebj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2oqoxifsk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wsubzbdl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2rmvlzois.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wchxrbot.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ezxeibqm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2viiutoco.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2egwfpcpa.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2seuxxwqd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvzgvtwi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2iqbcqzpk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2owfbstwy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rnxszaqk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pdywfstw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2iqbritdx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vrcgntss.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2qkdfbofx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2gjlwhhww.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2iipsuakr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nqwcrgqh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2crotlrkj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2axgjhdcv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2qnljrqbg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wmffumyb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2eetwwtpg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ycrekibp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2bzjvikmp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2imhdvfua.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2zsusitqg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2imoapsjr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2skehvuhp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2gguhgtah.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2uzmclaii.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vzegjvvx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ulznlkwd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rspbjdij.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2acqfiate.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2krejomqj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2oktkgxrh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cvkcmtea.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fztragbn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ofsricol.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2whrujhui.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ifxsywer.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2joumcidy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2txhspbck.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zjygcxvr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qotlziie.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wbvwkfbw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2oywhyvpc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2yiuppxap.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2nzevblyq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hznucium.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wiogeocw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2vsrauydq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pnnvwsoi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ebiqgnrr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ppxynejm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ohnxjoon.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2vivvwxgx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xguqcetc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2svwulcuz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zetrqoxm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2enucqfhc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xxjhdefs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2pdahoxae.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2pkluuasn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2tbuksoxl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2vdveprft.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2yrbioyzr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vgwzbnes.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ezigboqw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xehqeodj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ylotrauz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2jtjszxtm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lcnnhsdo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2rstehegr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ryfmrygd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cwnjazjw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2vtmuxzyk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2fyldttqu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2npkrmpql.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2dvukwpno.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2vdgsttin.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2nzzgpcge.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ydcbsijn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vlplmncg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2clhztavw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2axsmhgkf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bqfjsuxw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2speshobd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2segadbeu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2hmivxcty.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ejkzeacq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fmgtbeab.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2tcjuyuky.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2genyfnmh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fdmtbbyi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ranuhpkh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2oiqqivbe.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2rrrrwdgi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2kncrfbyu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xlcosijf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2twevhtix.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vlsprsxv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2vccteokg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqjtomgv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ffhbletn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2liiiuqsv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jebgcyuy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2hiiwmlcy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjidzlno.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2eojzteho.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2brhyaygu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2eibaveoj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2zwgsnpjr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vlezhecr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2plqiamou.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ovfiehgg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2smhatyra.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xtrbcgoc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2uspninzq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kybvcgsn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wsqqymmb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2yvyfhxjn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2senllpzo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mzckwsve.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ouqxtnau.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2yqsildud.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pvxkqgjv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2atkicgoz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dmghszcl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lnqrsouf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bsnjytek.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2bywpijde.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yaumqxtc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2yjykffga.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cggroivu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lkgemlvw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rsqkbfww.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wzscwvkb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ykllqsze.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2mclzsagd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2eowgqruk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tidokzbz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hfqruexk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2sygtyhwl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2mukbzbrs.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2szvzfutz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2impdonqg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2srhzgzdc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2amckfxcm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ulvutmxn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dipxcsta.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kyjmutwr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2kpiwxxvt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ohsrjlux.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2eanafxqc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2igehcuyv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2hvjeqrxl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sjbeytuy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2umlvtumx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2yoogxzzg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2iblrtsid.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qkhlggoy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eslnpvew.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2parjjtof.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2vymjjugj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2zpoxysnp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hguehkws.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2oxkopezi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ypvyrcwe.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lyvtinpm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2oshrtovh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lglcwmdy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2csjdtyhy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltabjyph.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rokklurz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jjicpgbu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hncfbmaq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ecvngjfu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2gojyfsru.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2dpgwxklo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2kkrjbrqp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xcjtlhjv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xewzsptu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kozpxllh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2phukkzdc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gippebou.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2wsgszdzu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fvovcqro.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ilqnahlx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2mbvjqrcd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2lhamfxbu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zgoyuytf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dzvdxcmk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2txolurdo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lwcdodly.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2yqfnnecl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2rxqzbuzw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2cfxkdgis.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2qkntjxdg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbbnejyb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qzvsywmm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2pzpamowl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lqzpqrry.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2smglhywj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hqpcfgjz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2afzyhsaa.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2epieprpx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lydypxru.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2unvgtmdc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2twvqqkiz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2uqcdrcxi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qvqccado.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fmzpszuj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jiuwgggo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2zcjzzpva.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2jqxjhqzm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2csxcmokd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2wcmgxcfp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2pupvjtuk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ikfcauhw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2driscbvt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fowfguaq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2innqtlvt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2klzpqcxt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xylxhfuo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gjrryttd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2tepdhcdn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2fizyhxgl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2njvmnwec.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2lztqnicz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zpummopd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2fwxkgcek.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dxzibhru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqxoexna.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ambmrpmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsfmvzjq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dlfgzykm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qmmukoti.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2mzfuhyvt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2vjmdpkra.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2epwdwejk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2orjjbuut.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2rmzadlbv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2arujdail.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hmqsxsms.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2xbyswmyp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pvjgqmtu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zpafhiba.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nhzcymlq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2uxbfnktg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qdnqtczf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yyruwxug.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bsgttilp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2rgddfuxu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sjqgrlsc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zmincslq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2rgksepmt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dztxpvfy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2rsrrjgmr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kcfytrcp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zbtidldi.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2yggctzec.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xblvzqdi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2obdpzfre.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2kjdslpzp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ejdqabdd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hdtgqkic.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bsitrkxc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rteozkop.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2yylyesij.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qsdxcudj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cscnjcdr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xikdajqf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2yvpyppen.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2inxurhft.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gwrzwacc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vkpzgvfh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2wwbrbliv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2xkairdlq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ihrsfxkd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2thdwiekg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jwwdugth.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2iicwinid.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wswssfnd.html


<!-- 参考信息 -->