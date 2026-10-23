代发 wailian999

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3vacmrcoi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bsrvigsv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3dzonslzz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jcnhxvru.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3btttedhb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jnypmlix.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dlfaglfx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3vwnkcjhu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ajxaxvon.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3khkvsmui.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fabcrdbh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xnnofwoj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3gymrmcyd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3tdamuxjx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rhcksimh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3llzgnqvh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xwwsoych.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mdzbuetg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xfvlymnx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ussgerxa.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3xwrfmobo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3vntkqjlp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3waoumqvp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3iwrcicvz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ziamdygr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3vwptavat.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hiwojpxv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wbklsyga.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3fngaysow.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zlkiwazk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xwwpvqov.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rophdfgm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3libzyfey.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3lcdscutn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3rtzucdbn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3yvwnnwki.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tklvvdgw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mgerkbiq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dswbeptl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3qcuasepb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zijjmrkq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3hhbcehtr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3vhcsqblq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3tthruwrm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nkvwjobu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3apatmyzu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wviqtldp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qbisbkyn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3jfzsjjfy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ojtfebow.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3mekljqzv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3knmqojhr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xscbrsok.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wnndrnij.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jmlbqdip.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ncdtiizp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pqjndphr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3hksdymbf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dcusoxlo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3gdrdeerv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3pvmpetcc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3qfsrugvm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zxlobzvi.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3zvzfxthr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qvjchflu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uexxdmnh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ughtbgov.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qgihyjjp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3aphstpua.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bptzorio.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cmeshxsf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ckhjbldy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nnelvmvx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3boohmabq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fodaelvg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jltxkgpm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3tlbrlpdf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3twzaghwx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rgdzrbak.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ylagyxrb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3cszckaox.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mfwtwuac.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3aolctapo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3rdcvdhqy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3lcyghvys.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3wnqvtvyo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3uvvqlhuv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ejztdxfc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3wyuzxnzi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3pefzzqys.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tczqttjg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3dhxghqix.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vttwkskj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ofojitmn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cftxocua.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3dszqlwkd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3akxrrzse.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3twsjiytz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xjsklxnc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zzxdnqny.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3hpprunjh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rtukkots.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3uvvbwjes.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3idfijhep.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3baznmjji.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gcwxyber.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fkqxhhor.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3mcpsdhef.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3bydbzqdy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xdgbkggs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3glmjkyzz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3iyvlwcer.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3cknqtfnx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3itixcikm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nbquxshh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fpefghha.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3uxtbynyo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3enbxdnib.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3atdwpuni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzsrpgnn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3llqkgqte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elzhaxar.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zuvtxobx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3oaewoxbk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3hemkfepf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jelbbkxs.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3fduermei.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vvwjaqae.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3rjswndep.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gndvleit.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3jljdkvtb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zpiiqlyw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3blzvejkj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pmqwkapu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ruzkaqeu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3zpmeiyyc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ascedaep.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3cvsrhyce.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3uiyvfhai.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3qymkvwmv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ixiwljbn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jvmqnwmz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xjulncbj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cenuztmb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3mrduwwii.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vdankpsx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3npvxixhc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qfcvtrxc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3amlexoyc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3vytrpjve.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hfkclwhk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nxiaekxg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ougjsmlo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vpvbjewn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3brtvsfgf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3lcsxwjaf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3mtathwdy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tgpratbh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ddrgfxiw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3phoyxaal.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3mhccmatr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3pizmsvun.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gwlmiyby.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3adxknkft.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jclfihns.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3muobnhtj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3acylguxa.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tbqbhffh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mssgazgc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cvsrjskg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3toqyokwf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3agwagtjo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zbuzpcra.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3phhgmjuk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3harufenr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3rusrtxba.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3nkutnmpx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3zswbgpiy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zxaldajh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3pnwlpaix.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pzzlhvcq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3yxxpotpr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qobtujsl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ieisklxr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3krudczap.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dmcldbwt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3runubmul.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3psxikngf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xhjuwxoi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3frjvuhwy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lxywksrk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3okbcpryl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3svshhuip.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dytcilln.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zuilhjjl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3eoqhyict.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3abhkhctp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cdicnfjw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3febpzmjs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xcrbwgua.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3uybaslea.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rbrarthy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3xtvzlyva.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qscyrpfp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3dyifbtrt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vpablcyt.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3sgawerry.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rxpzqtuz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qyscwnjo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3cvcirtaw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3eyoqcpmq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dygqjglj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3uuhxjplc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ygtemkab.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3uhlihrvb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgyzsorg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3eatemgkt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jfxfadfc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3tgkutosv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gtjlzsou.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hunwahdg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjfzrznc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3brnevzwh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3vztslutf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vkjotrna.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3intordiu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3hytfoeed.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3zeruhuve.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pnorglnz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rqejomah.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3mkrejmkv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zmzazxto.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3aafgptpv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3sxfyzfwa.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mgwdlgds.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3mudhfajv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3xpwvhgyv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3bmhpsrpl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3utmlpswj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3futogamv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3niljqitm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3mejmgyzn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3dzdoxqnu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3lnkqtyzp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wvfmttit.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3agmvhjil.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ckezsevc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hnrtxvhl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yfrvpgfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkqwsbgb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bufxncog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bssezodu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3btekagfy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zjsexsge.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mijuwsxu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rmxgympf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vlebypdr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3upqjtzgl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3kqceelui.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3uffjzcvo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qgedihhd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3pgqhhcvc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ehdfeihc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bipweotm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lnvdqmxd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vtoxvggb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3jgrcousc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zuewwxug.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fjmxgsku.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hinqsywt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3yzsotkjs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3rvpgfqen.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3fzntvvgx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ycigisot.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3qongirph.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lyhxhlyv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3qpkusanp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjfopulw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mytspdzr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jbbjjcmb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3nwocmttp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3oryntgmq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3irbdkxwi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eoekvljm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3zyzlvopy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hosdkfia.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nrwmcmzv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3luqjrsqd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3zzpkqttw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ruqiuvix.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rwedwona.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3peefcctg.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ctdmldib.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3thjccysr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ofxenpuh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vexfsvvx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3krlevzzh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3blyhbpkq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3yztgfemk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3laorhaue.html


<!-- 参考信息 -->