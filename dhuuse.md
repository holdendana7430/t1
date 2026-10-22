代发 wailian999

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jahenvds.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hivihpvm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2flxcrfya.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lmxcqsoz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2nyjxmxmh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wuaaretp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2kdmtekvo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pctuqqes.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2imlbdbua.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cfybhvwj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xkgkoyml.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2rttqqgcr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2jtkkofnf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ilskdkki.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2aydnavei.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2cvxukuec.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gmomrlsu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lumupbxz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jbgghktl.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gqacfjgn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2dpsnxemt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bgjdopdf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dcjaynef.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2autueqng.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2rczeessl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2josanoaq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nstzhese.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2rjuhjaxc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2nwkygaao.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2lzjhdele.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2acioosqv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hjzavybo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qgncbecs.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zstzsumc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qyfilzvg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ydrtpbnj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2rvjrqgvl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2wfhedynr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2tsoyvexf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ucttlmnq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yezuaxci.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2xlotqxrm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2xjnqasqp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2tuvnfayj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2iovtfuhd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2gxftuncs.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2unnyzmid.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2krlcphsc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2gnovgnbh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jelrmimm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2kmtnjsjs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2xfzugaci.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ibtnqeph.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2iamtnehv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2yfmipirw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fmxadeem.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mzahnpqg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2erbvawbu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ukvzxthm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2rauqvabs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2qzcpjiev.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2rajydohi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vegmcxfb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2cangwvhh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2hbbxbyfp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tttgsamx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2brtupojl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2hbdllglk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2oxaanjgc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ozzdnyjt.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2sgkquebw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2siypuqnd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2uvbdkrxg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hgkoahca.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2spvutndu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ikwymfzm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jtawzirp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ejxixidi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lgfzbpgk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gtupebib.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2dkjcgqot.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ndnluelv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2pjezutnn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vyiozeeo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2hhbxalna.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nkxuockm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2uziuhdcq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2egwdkoum.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2surtypun.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2yzuwkhgw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2duyscftm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2fgtmobgj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ntivycfh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2guvadtzg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kbunrutv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2mjuonmur.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pqmareux.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dcdprrog.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2botcljsq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2nzgkijlz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2grjedniy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ftjkgrlp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2cguxmaak.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ewkpewom.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2dqwqwrtu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kwymrdbj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ipwfsgyh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2zfcbvuwl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2jsetsvdh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zuqvieww.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fpnmoibq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2aeklyykj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ahiydpev.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2dcpoxldz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vevpcmdk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ehdfivel.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vnebbeeg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ixwfsysc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gxmqwhhj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ttaofedr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wimqpkoo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qrjldkdn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2pmykpgpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xlclewoq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2luzkhjuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evubfput.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uktbmbgj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ylpdnqio.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnokrpwt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zjeenyzf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ykwqzfso.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2jeigahph.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2dbkjvjmh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2dftudgfi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2eeaxbbvi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hgsvbozi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2kjalouua.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qrsuktno.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2juytkvxx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2zdpriflm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2dpicaoxu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2vaosvfza.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2nggyxjzt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2sypfisuw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pwgxykhw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2xgryqujr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2favqbtvh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2znowcedg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gquhcdcg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2iymjddtm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2eakrvbyt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ojqxribg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jpvenuys.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pprkegwu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2mmcquktl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tcvxqfma.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2cntgzzqc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gjjosjxv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2bjzpshfw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2elitufow.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2edkvintc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lqmovqxs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2rfrpnwes.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mozvhcyz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zpzyrsdi.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2zfryttri.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gbcxshtm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2otlsiaek.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nmhdsfwr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2fsaqfqlt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2fswqlvgb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zetilsot.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2oejvrebk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2tiwimgsa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2letlzrsr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2imdtjzvc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2jluhtiby.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zkeqklgb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2posuljyf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2tnxsayqc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2edomuxqk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2vnbrplos.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bdijbkzj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kocblehg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2dhjbwlxb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kqgkcvxu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2nwfgxeoo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nuussgwf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2sbstwnrf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zlhenvcu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2omckudbh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mjzpperw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qgekoafr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yghwyxwv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2bjioecye.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2izozefoi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2xjwezjow.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2hgggkzzr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2siqkejuz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2andnwait.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2asfckmwc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rfduenzk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nvxbegzp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mlphsqou.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vuagwjbb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2inghisse.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2wcdgbltq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hlmdhkdk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2tyraioad.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jnybognk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2flzilumi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ofcmrjfm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zqwwowof.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2vkyisvic.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gxyshwvw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rpzjfpuh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2nowsrlso.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jbksnjab.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2hhnifake.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuihuwke.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zdtqwwmf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xpljddsp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wbbznajm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdhhezos.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oylrlung.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2hreuredf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yshkcbzg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2iiobsjvn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ehhwxsou.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2kqhrnokr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jblqqwjl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2qhuoikyr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bfazuicy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ydyhqunv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qyuaqkbk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2trytemmt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2bfguoukw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2henyrjmm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fuaueahd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fjtpsjgc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2utilegym.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2buvevdpo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2rlbpshsz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2jkpumqay.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2aajedfpq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2jpgjqyxn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2srnityea.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kiubqkac.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2skkpdugt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2gambrilw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2tfiwowvs.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rrszojwu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wnynmrqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljuqakii.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dkebhlev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ruklrmsi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vxtonkxu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dpfctade.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2blfmauvf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2faoffunn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dnveobla.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wbnizudp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2mzmjxpwc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2nfqjjrfh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jkfxjkcp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2rdgfgvfb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2czefowum.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hegbxekd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yzyjlylx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yzmohnpg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qvawrslh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wgswkajw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ooetaehu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zdtlxuuu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2cvdfedmw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xvnbmsiy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2aoyidunv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lxkwmxlz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2bpytioez.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xszvtcqa.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2azstiscm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2abebqykc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ysaypomq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nwfysnpe.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2bwopyapp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2eutsjkno.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2muaqxohk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2elhzudrg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2caegqbfg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dkvydxco.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cxvclckv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2sxjbfflm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rckafdsk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2slwfhdhv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2cozihvxb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ywixxkth.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2kcdlvsib.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2venulbye.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mxmyucno.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ydzpdtau.html


<!-- 参考信息 -->