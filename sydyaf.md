代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hmqrvgsj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2zfocnpuf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ckhcrxku.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2hyvyffnf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2emmncjos.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2dehshmqx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2rotyziwq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mldneamf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2rzmnsslj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2affwxymi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2zgcghezy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qbureyhr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2bvdubbyk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2oqyqflxe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jblzspgb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2pdycwdpp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ukvnqthq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2fbknwqyp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kmfxypuw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2feinhbhg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ksdundej.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fnwuofbn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2viynimzv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2umrecxce.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qdrzsijn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2sbzrpiqi.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vhnpuztp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2netjrcsp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nthipsiy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ctcwpxpq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2cwthiufj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2oowhkwvp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2olfqgbhj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2rqbevlfn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vaskewlj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2wcuvxixe.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fnvaptob.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rnvjwnvd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2cxwpesed.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2wciuydfu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2upmnuyxj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2omldbhzz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2rswgxwmt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ikjwchpe.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2skyjqyop.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hcquvcan.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gvaeqrts.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2uwnzlgrn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2arahnrlf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rkbcmizk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iotpiqjn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qtpjjitr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2xelteebc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qtmgybjp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2suuqbbdn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2fbrectxh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2sjzijguj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2mwzpzpkd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dwotsyov.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ouawitgt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zooudhdt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2sazcsmuc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2wprgmplt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ifbfwkfi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vgxrcgfa.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2qbdqijrj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ytuvljqo.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zutoohmv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jmsovjqo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zujdwfye.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2cuyszepa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wylijvqn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2sducwuvf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ncqtdtdg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dkexnfwt.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2yykvnzzx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2pmqrnvyr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2yjrkxpgk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2sxdkikcg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wjilmbpi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hsduathd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2sdoygsyc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2lenrkgds.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2gkrsjdao.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2kwapvazc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dybdelie.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2sioaewcz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2hucdmbgf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ggtmrquj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kctjsiyx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2awieynjb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bwrpoajy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ayfegiae.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2bzvhglif.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hffyzfrl.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2lmvqadur.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2txtaogrn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wkygutkf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jwtvcuvl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2qlaxspmn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2yanztyab.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2izrgyovi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2aznwrnpd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2urdsymjo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ukliusjo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ngumlgxw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2laeucgof.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2knsntsgs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ikjnuagz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2juntzwdr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2kbdroyln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncfqihcz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2meersicc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqnvzlzs.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bwvrasrj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qjadynlz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2otiznojs.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qzrzzhas.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2iiahtyfy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2wolwvddr.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2vgaivngw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ytbmuvzk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wkncxcrn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zsxyiwaf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jnrykqcw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2quevtbbs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2mhpvntgu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2etxrpple.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2yufeokpw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2rgjpyozr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ikenwlyo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2lpukvhvf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ctqrybnt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zeufwxkk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2clegljnp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zvckxeph.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ypqsayez.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2agpudrav.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nnsgtxlz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfriyapz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rtlxdjve.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2rkfbpysk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2yvuqpevo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2amoxcyuo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ajemahxt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2npefxmjd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2pyvethjn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2xebeprzx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2irpkfvjy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2brrxkwwc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2erckmypj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lchczehm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zxdpkzgg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ntwrfrcn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ypybhxrc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2uljpzcny.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nmzymzxr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2lqdeeqvl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zlxdvddu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ktfbzwku.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qngelxzq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2oyaszbvk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nmnejhwt.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2oqirrnms.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vvkecusz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2dnmlnbtr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2aynjbyqj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2mysbatoo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hbsmypik.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ywvwgnck.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ynwxygry.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ntlzfsro.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2jqprouon.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qyluidhn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2khwdvcil.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2idgdxzip.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2udhmipfq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mkysjtmh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2jslsutdr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2swpsmqzk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2xcymbngy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2gpelsozf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2nnjyhmqk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2tnaoblpe.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2yquqeycc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ndzaprpr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jxxrgvdy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jjtipbam.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ytmvnnli.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hmlqribq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2hszpvtoc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xrabewtr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2sxvvvvum.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uijzkmgw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2nokfbjlt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vcxlefkj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2odqbuogx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2hivaeppn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2irrfqwrl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fhwvvldj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lwfeigtj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ufkbgjth.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2gfnagdle.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ofxtlblb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ykeacvkw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2snxskgok.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2bboajsga.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2oaicgkpc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jvsjyoce.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2vsuemdmk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ptrkrekn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbdgifvn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vrvuvduo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2qivqjctn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tglxruhl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gpspqywp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zqueyjks.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2okgqjykk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gmhmtulk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ffdypilg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uvjztssa.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cybbrtxl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ourielba.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2giqfubkq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2txjoyyyi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2afukynja.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2dhoyvtoe.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2khtbenqr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2oevnhovs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2qgfnvhqn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lhosoyca.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xywrusrw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2opncnukn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2tbhwtmpo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sgzjttql.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2xzfephhf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2nnlellzf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2rcbmhhuf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2qlyhzwde.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2gzsdiktr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gpufpori.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2getbymjy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ucgxkcxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rpmbhyow.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ykalesee.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2blweevdp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vossijpz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ddnqkxbj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2pnznmmld.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cankjaxl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2znmiffzw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hbxvuapd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2iinstpgv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2iokbmqxn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zbjfpaom.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2goqzhzkn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rowewhlp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dubsnimc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2crtrsxvb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uvimngpd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vhfdomoz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2rskwppqh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jmbnygfg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xbilmbfb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2axlgvfof.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2nroruckw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2opurcncy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jigrckra.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gjcvlrbe.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qfnviffk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2qflbohia.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2uedjqsij.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2yqitpdfn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2fxfzryoc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tkjxlmea.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ougtcfcg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2cazwvfev.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2fnomijga.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gzloijjn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ttxontqb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2qyoojbby.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2dudtjsii.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2enbwrrwv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2tiyjflsm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2flfheela.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2cvjwycif.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2msbmamvl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2uqnibefw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2rgawojik.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2oolwwohh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ivcavcbp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2irwcdvgs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jcotrzqn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2zjucyeha.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pxzkqzzd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qctxgyaq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jpftixpu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2eqsgjzwr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lscvduzf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2dgamrrii.html


<!-- 参考信息 -->