代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zoujrmgy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ynjbmtwt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kcvcgeef.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2pqjrhomk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zgfrdejw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2hacobpcc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2rqrdujko.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2pychuphf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2oegzjsaa.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ybqmkwdi.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ppomblva.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2azeapfff.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2pyhxvgkq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mdqxiwgu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dfobzfcl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jyhchevo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zkveexzl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2wtktcvkl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cyqngtqw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rjkdsmps.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2sezzpjnf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dobzjuyw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kdybgnlz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bcitbjrj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2iozamcde.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2mmplztym.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ftvmhgje.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2hgqaxnzt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zwwlncoh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rtybyehb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2oouhwqli.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2vgzgovlp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ftnkuliy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2tonxlose.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2oafiiivk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pfojesnk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hpnrhsoj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2lpzeodlw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vrvqbcgf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2txybpnxa.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2plfswoym.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2eikpifhu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tjidoemd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2seadzuui.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2mgncksih.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ljqktscg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2efkjmhem.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2gewddzcz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gheqsdtv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2osqwptft.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rwgxcdjb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2laguullf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2uswikbwr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2lsugkitl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fktgbjfl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2uvpttznz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wrnrjnzx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mwhtnpug.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wltekjgt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2hjeztjta.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2bvgvwbwy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mkhmgbyp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qzfwhpks.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jqrmytco.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2sufcocyv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zmwrqsjm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jilmejkq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vzunmezi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2stzhwvoe.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2jvsdofbi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2nkjqzapg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ujmszcbv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2iwqnnkbu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ruwkqgam.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2bxjucirh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zopqzvze.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2thabkhkv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wnrrsddl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2faqzpzto.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kudifdsw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2wntgzyqa.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2hwzzyyxq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rgoznoyp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2mrdffzta.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2vllyclyz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2pmqhgyiq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2kvpfjprl.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2sflrhdvr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2uccfnhyh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ejxtqmuf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2otltxxxk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qxtephlq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jotttrfc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kaaupobx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2brpkfapg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2njqvivjc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2olnwwybf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ajigohco.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zlmlalat.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ttexaqbd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dpmcwobu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jxajurta.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2usopchue.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2moizknxp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2nachlkwz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fvggozly.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lncqjwdm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2sqkqrvnz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ztvqomdh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dkqvgpod.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ktancqfl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2yrqgarjv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2parvdwgt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ufovunml.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2cfiuwhau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgwzjltb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jfnnmtsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tctyynqa.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pisitety.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2iqhylusm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2nheqtexo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gyrupvnb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xhxtrsbc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2iotmqhaj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2aavjnljw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qrtpwuvn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mggcqasa.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bwpslqdr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2izaisoaz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pwdkhehl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2mccsafks.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2wrnwgtgu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2zeugxyks.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2pfzwggap.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2qabjxnch.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2memdtohw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rpvvgagp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2hevenlfp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ouhciatg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fdparhdd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2wpzikqlg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hbphlfsq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bhuvwiep.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjumquvz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2eloxemov.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2zfqysmet.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2sziutcoh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jedvdcgh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2phntrngj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2loxaeaum.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2fswtkfty.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vinhdffj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xgqohnfg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vtxclimn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2jjtdiqsx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2piczobas.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2emxhqxeo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2uiijgzzl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2atsfzepw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2vddvvyos.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bwjthtku.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2fdlwyiby.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2jhsmpgyo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ffvklszw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2mrsutkxe.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2fmvjqobo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pobmrvvk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qehfefnk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2wblkxtnj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ylovlhwt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2jboebmcn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2jfkbqytc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tnjfwqqe.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fazoqzaa.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2khygbuvg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2parzjkag.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2cvwhhfpy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzdvzzih.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ldtlqyrd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2udzbdfem.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jqptpvqm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2tvlwnkie.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2isggaorc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vggjpben.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2kjbdquan.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2xwnqxxpp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ceswplbo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ncbyfzya.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2rhgcgbeh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2msutxwwv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2oldaqhwf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2woqrdhay.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2xmwdvojw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lpgxkmxh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lfohwadh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sdxdrbqo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xpxyoope.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gdombsev.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jtonequg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2aojwtvgt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2hgaohzop.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2gleqsqjf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2lfuiqsrw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qsgclerb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dkudzbsq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qsaumazk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2hayhcznn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vsdqizsl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2frytfjzc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qckruonu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2cwkotpma.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tegzvtxo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lbhymdps.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hsebpaou.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2kjddxfgo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2hotukawj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tyjermqh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqdnfalz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ixgcskxr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hqvjzikt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2yvpxnvva.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nfywlcyk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pmqnxgdt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2cysapzds.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zakqmkrw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vaaisyau.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wvnboqmv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wxxxqmsg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2itpvoccz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gieauziy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qhwipzgm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2trxlckgx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2tuwjfkwe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2gefegbva.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wooltcsc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qkleothu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gfziqeph.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vyrisqjs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vhgvcnba.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2totvgjlh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ymzsjkig.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2smwpnrqu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2rahenikg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2cyjeavws.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pfeatgfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbkzaxuj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2phqwmrjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzqvehpx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yzswrqen.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nfegmiff.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2blooiiuy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2wzztkrxy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2phenjczu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nmhbjraa.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2oatxtpba.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2tdwpjtjk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xhencwbh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2qctramug.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2phkzlopj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zuqkppeu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vrhdxuiw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2owcrvlhf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2barvjfzt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zbdunjhh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2nfbwjlzg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2rokjtzkk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gtuxqnyb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2caghsqth.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2impcmiih.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2tihdtzkc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2bgbdkvcd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iowfahxy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hpqjxfsh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ekpwutaj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wiigbdly.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lbvyxklg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2rtygcbil.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2afsphiqs.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ykcezzyo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zxnranwc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xizzfsfn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ultghprn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zuyflaau.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2wpuzeoel.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2oxfohrca.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zvpeflsq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2vagsfkky.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2snppfzel.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cglwlqvw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zcztisbg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2eeiwbbqt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nesrkqij.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2csmaqupt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nxmsuixi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2xxavteqf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fqapthwl.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lcdifyqy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2sufgazhb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2fhvuhezl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ofhzkagl.html


<!-- 参考信息 -->