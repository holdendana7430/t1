代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2cnpqdueu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cnpkayxn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2heskmskt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2oggefymn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2zgbyyfag.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jhnubbup.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ykrpguzk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2rsplyuqf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2svqlqaft.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2mnqfafkd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hxfbeyac.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pydhyuqc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xuaainod.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2peficnka.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2sklyulmf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jphketmz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2clgmybzc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ckxhvvrv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pvmgfqvq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2legbrhqr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xqckwtzh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2xdqrqava.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jthqbmlu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ucykuech.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mzksnsoo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2xojnicrm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jqcydoie.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2tjxsihcb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2cvycmcmn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2vvkjajuc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jypwpzxj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2svwptcbe.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fksecphd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ailsbfcf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2uprrmadx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2nofvfuki.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2thjiqjpb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wrikbkza.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jwhuvbqa.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2upwrweyo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zmxvsbei.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ybltulhe.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ahqpbpzl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2atatmuzg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2vltnvfly.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2gzbykris.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2rmzjsuue.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2diohfywj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zhmdornu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ctmbivpd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2edjisqtv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2tidxlxyr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2nsfvovdr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2wvubvvul.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vzklxjut.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2tgnirgbs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2aqluesuu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2evsapnbt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ltnvjebc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2nlidbsbo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ouxvvnwn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wmjnmqky.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xoizwlcs.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wzhurqvo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2assqmjjx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2catkdyfd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2nroqmjlh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xwrktwke.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fldjqqln.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ttdcqbvx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2jfbkpwkh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hlhliwse.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2vtovxpnu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ppcpqjbt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lkiptffq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2kblpzowf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2xaljsnts.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ncttrzyp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2kcmqsqhl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2vlimdedy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2slyyeaqa.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ppvgkkgh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2gcijmwtf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2dwdanraf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hvrzvcwg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ouopxlcb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2bnfjdbhy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xgtfvhhi.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2iwapupuh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2sphmjezs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wsseushv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2pdwuflqa.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2oefqogyz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wsjjcriq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2gnxzdzcr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pdcuyyiz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2hiohkiqb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hjmnvstn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2aadrspdc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ughulpdn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vjdzgnqm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2uyciceth.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xkjxmlge.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xwjkndvs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2prkifhpl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tshtqhdn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fnbngjah.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2qhkefyjh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2jpvbgmon.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2uznwecft.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2cxndglcu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2kjqycsfe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2bpasmsfm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ntbemini.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2mddlhncd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpaaaktn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mhiptbaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvoacfof.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rjjucegk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2umkhhyfi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ifwaxzgl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2innzwpli.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ggaoxqgo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2rnzhspkl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2rsjgqosy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2pybfbrae.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2iuvonjhf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jmxobmrt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2rjeijelg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gztbahxv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2tfodxgxa.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2xcsowfit.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ukmfughx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hmuoyglf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2omkjijbu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2czwdwhqp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2dmvfzowl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2nggeeiov.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mfrgclam.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2haeycfxb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2aygwsdgc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2bxayruki.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pgsagojs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2dtpvopya.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2sbwtifdl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2zoadeypm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2seqawlit.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2awttrzli.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2itjjmtiu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mvxkrbov.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ttwjxjcn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xkopxsct.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2afehvuqf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2djfzovws.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2oedyjcoi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2igspbdvy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2kwpcnojn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2oguymizv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2afwgwmab.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kxyfypvc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qqkrkurb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2odmvtabf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2tzqddrts.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2gtvojbev.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qvtappjn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2wglskgtz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vylylifo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2exyailln.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ckyzczpt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qhddtdmh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2rptwqozw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2vuayxmek.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2asbyfdfi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2tdyacwls.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rzycdoro.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2sygzxjyf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2tuwlupdr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2irbjsaco.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ofvthbup.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2aejrzwez.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eubbtpah.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hnmmbujy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nfjrgiij.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bbmkptyu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ltbvrytc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2znnuchvm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2atakmnhx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2rrspclrw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2pjboqcez.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kuxdwlww.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ibldppbh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2idslaezy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2oopwhzxf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nvyzojil.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dugnizgv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nxjlimlh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ucpneqdt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cgwinggf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jnpmubzn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gimlcypd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2uzzdktpr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2wceahtev.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2tkesgxwa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ifyholcz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhsmwkmf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2tojikjqq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mavdiklg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2kldmxsfc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2aflaztch.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pbdxppzi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2hdiksmcs.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2axztqgic.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lexdjmkz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wmcpugce.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rrigltjj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2wbqdstrx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wmzzmskf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2oufhuojj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pkeivjhm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hhvcrqjq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ryooxsvr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ujmnsfyy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ajmtnjyk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gjirwhxr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bipglhiw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2krvudcrh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2kojdvvpe.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rkuwhpxt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjezxybz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2xuclmmri.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2gxedwkxc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tzgraits.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2rsyesjxk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2yftbmsis.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tecmmjvp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2remnsush.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2sddecvka.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2pedfpltt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ofiwqagi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ibscvbwb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pbeaisos.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2kpphptsx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2wzgklpjc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vxymazkn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kwvrylzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2goxaqper.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cuixhhps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nczrobep.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tsusilgi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2npcczgaa.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2aduxmucx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mlvacmmd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ccrirtmo.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vmcudroi.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rnhlkgre.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2vgzovylu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dcmurxro.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wmdvdxab.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rcetjzqr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dccjzwom.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tpqgjdyz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jdyqokzn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ljhvdmlf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ojyjbixl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2asgppbiv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2abihxyea.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2valheuqh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2pakdrmbc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2zwphflws.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2tejctrce.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2whbqfjax.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vxayxkve.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fbiumhjk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2wqdwqueu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ndbcsbix.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bnfnsyjp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2mfrojzmr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ytmtyxkq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qoespprw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kwtzbsjk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2pjiglhjh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ykvcsais.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ayvkikwb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2hlabeedn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2frhsixpx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rcjvguli.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2smqjfbia.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2crijzjya.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fbrdoyhr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2srytbuih.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2csmaflrz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wqaqjknj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uodxktbi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2tnbnnqrd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2guqbbpxy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2brdgxber.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2prfwmjgc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2jilmgbmd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2cusimhov.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lyyqmzpk.html


<!-- 参考信息 -->