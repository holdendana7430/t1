代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2uyyyjfyz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vobdfoqo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2izlxsuop.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2veztadqz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2zhegcrpy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qsxzoanc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2pxapheuv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nbyhsgrj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2qeomffpb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wtpiyvbe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qjlfoksz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qfkjisft.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cajefxfd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tlfovvpj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaruusfv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2omhmunoz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2gjokwixn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2dulomuyq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hsvyghlf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zdhgmvnr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cbqoavfj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2syolsvfq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2iiapzhez.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2cfaxrhrq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvseltpm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2kmkyuwxu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2yrcyupfn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ijjgohqp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jvwspyil.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hjhinlmm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2lxqyanku.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qdcfhkow.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nmkhdczo.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2whckhrlm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2injrgkby.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jyipjmsj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2twmkfolw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2gzqchoai.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fwmnsxfd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2tsgpzyuu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2slwutgkc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2orjipusq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hhcjifzk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2vdgicejy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pzmwqfld.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bumtsiik.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zviwketp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2rdvdltqo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2kuvdoiwu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2dxjgpbnv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sznobava.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ujqgvwag.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2btpvrblk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2unextdtf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mkeyysfn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qbwnlkmd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2splovftj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rabrrpnh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rndcpumf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2eouuiacr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2pyrzqlhl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cvfaweqo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jdxvvwqf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2aheanuyg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ldtwuirv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvshfqpi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2oiuqrfor.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lztqyukz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2veldenrx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rymlaupf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2olewnuhx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2bgivctyh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2lrsmexbs.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2zfcwtsgi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2btmwfwdt.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qqhzlvbp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zyuqbhiw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2pdpvrcjd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2plzgarjw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2dogjxlxq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2xowfmlch.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ivmfenko.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2hyhfdkbj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jszadyzj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2vqptmslf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rqruvzxt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vnwpgqvp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bqqiinfr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2pxvnltoq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2exbykduw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2vocjwgct.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2unhpgzbl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bdzootqt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2jhjotvyg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2medeuxga.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2kvpvjmyq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zgxvvbnd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2klrgxgpu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2asohspqc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fgzlujbf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2fqlsmbgs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxmeqszt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2phbfxccp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2bzrtcbnz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2njgmfrrz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2fdcecqmg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qepilqgu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2nduioonp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ngobmtuo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ybapouox.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2lcsqzplo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbpkrofo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xmivkdsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahexgwfy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hhnikyqv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2jjlaareb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucvvzpxh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xxgglsaq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2triumvdd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2qkyfdeut.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2mxxpvslj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2iunwoslw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gutgaion.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2euejoaey.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2uzufatyh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uqfwulbi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2zswhpkoj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2cosxpyiz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2oddvyjat.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ybezhssu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2cpxrffil.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2auqlrgws.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ivmhcjln.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2kvikeesh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2agjpmzaf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ouugkspa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2euodkaof.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2kltgxrmk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zgxamovs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2nuhisjna.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jetrqflj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2smcxqeyx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2sujlhnhc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uougmrxq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2mdqrlfvi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2upvqcqle.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2bsghcvni.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2fjyyldrh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wvikasnk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jauaxjqd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2phyqsxxi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fkfponnq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2iwpvrbue.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2andracfd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yqasoeoj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2qhyiegfq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ppkhzxxz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2iatswojl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2nzcmvogc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vrqzlogu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2dcsnwyya.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2newcgfsu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tdrmodti.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2uuyczkrx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2mltmqorm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wwgzqbby.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2avqscdwl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2azgqpfcg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kqeckyti.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2dnzfwnxt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2anvhjxrl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2imoulych.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xkhrsmyt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dpktytbx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2dswrrxab.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2fwdcnseh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qzvrufet.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2tkeqkekh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ivpaoiax.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ggqqojpi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2lbqlluuq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2cyeqhxmn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2odlccdbp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ftxuzdhn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ptgshxck.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iaunbmfn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2blsinzbk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmfyqjai.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2yfnyvdme.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kqlxjsoe.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2shbypygm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fhtndrgw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2wolbksjg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2lfxgnavd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zvzmbvns.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2szxqbjbt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ojlrpsnl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2xhgtboes.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hazwcelv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yykilpud.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nrmsltzi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kggnofgh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2fckrdyzu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2nldeiqlg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2houchfep.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2rwshagbz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2mfierlwd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihfbaqsc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2vvdtgwug.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2rgmkpvgl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ivebuils.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfjjjegr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uksxvdfu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyryasuu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dnmhmzqa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2bzuaktjv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fqxkjxrr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2blqhugeg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ykjrpvig.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ejeqhfly.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aomaloma.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yzshrpjd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vdzpjffx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2elhfsuqa.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2cpbgfvtq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bdrzthrr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qgdhkuod.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2neexliks.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2iqjxawou.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2bkinjrjl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vfbmvfdf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jresxbcv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2emtxigbc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2asfgqsqs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lxabphur.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2owygxfex.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jjaseobs.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mxqxgaoq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2pjlcrofo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oorpkulx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ftnkjduv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ippyzmag.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jmpjwbes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vktkarwv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gzzxhwbd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ghkoaqva.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ffvtavyj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2nxdbceaa.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ukqdbero.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fmnavqnb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2hdcbblul.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2authqaem.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2toqypdnh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2dbyleztt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kbtiopzy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2axuoyzvl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lguzmetd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wjebdouy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2uciwjwud.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vrxmdbcj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2qxigiddp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ppdoaqyf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ckxtuoty.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2jfklrpwg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2powjnzyn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2zexzlajn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2nivjsfjo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2njagtuph.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nxxbxzkw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hevrmaqf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wvjwavqo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sujyikpm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2vpzvpmnb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bfvgcols.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hmdtsdxt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qdyuizab.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2smfyreza.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ngqibjwx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2afoyxhld.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2hqvhryvu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yjcyixsa.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qskvwqnx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2frfwifyu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wpppbgzu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2djeoawtm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2wdzaufgr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qktwifyi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2otrjguxb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2mnhcgngg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2fkhtjamq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gzymicec.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wrgwpsif.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2zyrkvqzp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2krrkxups.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2gfhurtjg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zlyfyedj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nhlsxefn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2desylxlo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2vrrldbcj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2epctowiu.html


<!-- 参考信息 -->