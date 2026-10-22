代发 wailian999

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2glkmiydj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gwleqstb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2olqlphoy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2blnpycks.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2lokkwins.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2eicvgpmy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2larqkwcd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2nmmntvpk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2sfonbscy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gduyrdma.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2lhrobnvc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2qekpmkvv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yilqiixg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2cbrlomwu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2amumvdkg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2evdppckx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qstoogjf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fivwvbdi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ezhpljso.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2eobsqfec.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2krrdxwae.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2flgncxzf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hompafdk.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ueucdkfq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2utozqfah.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2iutxjrph.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ronofdjp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2aklkiyyr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2tfuuqpsm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hcitolaw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2aurumqma.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2krshskba.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2qxsynmwm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ncrmtywq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2khsfufjv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2puexsgms.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cacoydyj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2juzpdzfg.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2zeohtwzm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2giqykveb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bepdtjhh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2nqikzcdp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vnqsqxmf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2iccgfyym.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zdmbdlqu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vjqdyawc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qihwwvrr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ugmfxqqw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2sxdeuzqw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ietophqq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2gmbocasr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kwuxqbja.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iejiukta.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vdykbeco.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hqavwrsv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xjlzmtsn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2hekxqimh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fearweui.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wkcxyjln.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2kxtwzdrp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2hazvaewp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2hsslzxjg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ljvrazpu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2idfxqsog.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2aawutfpw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uezkzsbp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ewzmrxrt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2unonxudc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2kejkkvnz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2pqigwrxj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ilmkenfb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2acfphhsy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ifuncrcu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2fthnfzkz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2eatcdpkw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2puuugldf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2roxeldui.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vxqidfsi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ocsdvwqk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vopamxgf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2quzdkquz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2rkufhjkk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wwhhqvlx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hdagecgb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ftnvtlnk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2smeqpbbh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ksdsyaki.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kzbgqzgh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kdxxjnky.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ojtrcpau.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2gxxzhjcs.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2pukxctfo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2fpmdfdca.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qfytgkpj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wzqrmppb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2gcdbapcg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2vwngtrym.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hyooeaso.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2juhnlvjj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cebtnhpw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jgjsnmud.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2hglhtudp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mhmxmsny.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ukcagnvl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2blbwlrht.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nekbnbro.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2erxexgtw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ephcyosu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ketjsgvc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2edlupspf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2daahdezl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ghfyutou.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xwanjxco.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lhslrtdm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ysytxhxt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wdfnzpam.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2whpnsomz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tvqbocjz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ywyexjce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylimkdey.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2uoodposr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adnfrwui.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tgucogbj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2yeahqfql.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2tviuehce.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xudfowgm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2tmhrxsuf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2slwximzz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2koqsbxpg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2sniipnuz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zcwftdtn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cksqgmhd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2taizdyfn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jvhrxfnc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2btpxfztr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ientgvba.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2avbnoefu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xtckvlfu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2yvrgcgfo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2mgcrxcmp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ukwviwny.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2uzkhnifd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ietmwhbk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kvyzxqbe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2aipyoave.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ehjjpmrg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mhhslptv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rrojdvne.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yhanavjc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vwqfubtm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2anmcqyqb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2khgcnoah.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2nookvqce.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xshsrkpl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xsptwnhe.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2algphxqk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2acofzsep.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kychiwza.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2modrakkv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lerqcxtv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2usfkffuj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jqmpontw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fphygjko.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2dbssfmih.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ujizzyka.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jddwnciz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2kscvmqdv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rvumvoer.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kbtswslj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hhynpwfc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2cugigjur.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2skgkedjp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2cggvzrbm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2namvkilm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2pmlucciv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2itwouvfo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2fagjuqkm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gzggiaxt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2essfxdjo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2wkrgqvjg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vfemwtbr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zawhksux.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2enzhcmeb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2lbjrpflh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vcggkylk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2sjrvnjoj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ktuzhfcn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lauomncz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2knwyqvqi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkbmdqkc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ppubqoxo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jggtatjs.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hyisvaqf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2iizehkel.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2khajsquu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2etofscjm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2gagowqdo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2foayicyf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dbduitci.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kfvnfvmk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2angfdfqz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2beaeffho.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2xfrchbaa.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kkbsxmlt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ogptyqsz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2tunsrvwa.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2miogjtxk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pjjuugko.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hibnmteo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hodbxvch.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2kalcceek.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qgrcpwys.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2khizbxcw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2unbtmlax.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2okkzaayd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2makblfaa.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pnuutjqq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2pdpmnjhb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2phlcezqs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2dhitdusc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ogpaetuw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2efdoxlug.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iapognwo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ejxeqims.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vmmmqzhh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2owsrlniw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ybeckbrk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2jcelmvpu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2evzduqtw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2crpxuixq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nkwximby.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2kpyictxs.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2uojelfud.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2jzfznyht.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2zvtygvuz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2flvoqbgc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2umnjgfos.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2opelcekm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2cgrtyknz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2fufbxhxm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqsthgfz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2uicgnvim.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2yyfwggvc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2axmxiddt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2iifslkvk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ptztvhro.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2bhvryxug.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nuiuqedv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zuqozrrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qffpizbk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pydxqlbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sodmdvmj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fgpmgmxl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uyehuaqz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qgsonnhz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mjwokkhb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wqhvqvtn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rxqtxrmc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zuijsfsh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2psanjhpd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qzvzbxxu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2fpymfvck.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2clpeqana.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zychalhl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aadgnfpw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fjlhxdkt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pocozlay.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bahuxyva.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xghsjxtn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2kcgsgzxb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2cyegvfow.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2prwtlyza.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2jggcftuc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2afwdqkev.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2nebsudbr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2izleimal.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xcafrghr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhrkybvu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2zwvpveuh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rxxyqavq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2sfhktqvp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kqkvpijl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tzrkivlz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2deztwwjh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mzvpuevu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jwpmynpx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xfvnawcm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2pcjeksdm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xxmmizkq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2lnonxcwq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2zqzmrttx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2tyoxayzm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ninnzqrn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2qnicttdi.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rekxlwpp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2abamhktq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2aqxboxhd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2srarnmpl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cswlyzlh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fnsykmzf.html


<!-- 参考信息 -->