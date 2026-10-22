代发 wailian999

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2jzhpcxnw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pybqxhms.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2nrfeafop.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vijgqeag.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qziblthr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2iorommpw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2oihbampd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2kcgdguem.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jipkgmem.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ntolrtvy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2sarusvjj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fzravpsk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2vttusujz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2bjqpvles.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2odgchgwn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ndliuyqd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2aphoogti.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2pailxebt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2yzitomdr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qvishuoe.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ppbutxoz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2iqpezfml.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dlhlhvnx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2sjgvnmga.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2mvmmaxmf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2opcdetce.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hwdzatka.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ltsyaagc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2smmwadrm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2kffvbpwi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wxbqkohg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2rusotoza.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vsogvmse.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2nvrashug.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2sngmhreu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2qrrjimmc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wxufmuls.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mybldxie.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2pmkllhck.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2eeedosfx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xuszggfz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2phxgfrea.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ulcyoibv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2iycuofms.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2udcymmdb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qytsipck.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2euqlvfrr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ckqfnlvy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2nhxfqkzp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2apjmdvjp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qqysckuj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fnzxyzby.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lppwwmzo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2gxrwvlpt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rxzwrbou.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2bkyejewk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ofdkkvzk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2bsirdvoz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mgoigtqo.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2dwztydch.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jdarftbo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2rfywgyag.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qzwetgsg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2wkbsfwfv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2pliuwxsn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2lgqofjts.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ohbcrrao.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2matxtjsy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2hirttioh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2efyzbywx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2wllrqpon.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2arcbqsky.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2gjfbngyp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2fibiqdla.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wdkmxtdh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2sqtjszxz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2thmmptms.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dwvrdriv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2spstzqbi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2eimaqskb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2qtmpmpth.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2furwwucd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2bbybleii.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tfztcynu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ktrcwipd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2unzbkukz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tchaiqvl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2babalzds.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2mnhyonci.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2waygvixm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2pbsyhdcp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ajrlwmgw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2soimeipq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ywskzotr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2avzldidb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2wcjnfmkv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ehgfqput.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zrwvdcfq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2knseobie.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cluknyvj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2azvzviiz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2okftyhek.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2trzsdnlx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2cdrbcyjm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wrbuekca.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2klrfuhzv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lkyqaicl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rqfmhvfc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2boscnrqd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2cvghuwky.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ompurzkv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ygenohrr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2delgnezi.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2oqkemddz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hpgjzdjq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mdyagnwr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2dowgelim.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2vfvgttgm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2stcbafoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtgqrrzy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wwlsmclj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqrfadtv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xvstmhyy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lyslwqzo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2yxorlxbn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ddobzsrb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2mrmrjtpq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2cyrtvjzu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2jljltvtu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2humhsymd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qypadbsp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2htasqjre.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2mivjddhj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ylhmseio.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kurzivlm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mvyuttdd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2bhajggry.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zbqcrkzn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2bsdjfakn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2gixbzbnk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wjnpiiqs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2yvzvgyxk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2cdpszlns.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2apkjurjq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xqddkrux.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yztexlcl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vjgqpqew.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vrubglkm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zqkbasmf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2egbgmsie.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2idzrnfwg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aoidwpgy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2adppcasj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2safnzumq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wyblpdhw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2oqzcccmt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zhrdrhaf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ajrvdcaa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zogmrwlw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vkqkbepu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wpagymoo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hvapggxt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rkftlmoz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2aavdjkah.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gqrlqohm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nukyvmvq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2lxrtfnqq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2aoirkbsi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2evuchwcv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2cvyjfgyw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2binlbzoq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bfayjtiy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2bslpjoox.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dfdaahwq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qmmddycf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2pagwsehz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fsfowutq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2yzmvgzkm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wlgnlada.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2xmkgtxyi.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fyskxwtp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bavzslif.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2xsvbtnig.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jogtyite.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vhmiltmi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ckbmawzu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2juuzpdgq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lqrgscps.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ealreokv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2enxtkvit.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2egebybjm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yfeoosqp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2mjbyqunc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2anoclgnz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zywkotsp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnazvnsx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2hcdayqxo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mfkrsrua.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ymjtjuow.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bdzbnjiv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2fqfbuzre.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2sixrgmxu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2enwveysu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vjnymsmz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2wnvbmxfk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2bvcnydxn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2eaugulus.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jrzmdrdu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2xyptzgyf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2yjpwerrt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2avbbyiqk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2szgxejms.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2appbehai.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xoogyjci.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ckphqifl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2bezebhvb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gtdpebcv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hgzosaes.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hxnflnlb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ailulqze.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qyipsrqo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2yscytfsb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sgfmhryg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2dflhwrrl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2atumlgkd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ysnfgmpa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2geyplgwx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2txkjqerm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aocmzzpr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jgyvtwhr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ukadaicn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ronqptya.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2tdedvdxj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2uiefpase.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2eajozgcv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vpnebxox.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2djqyzbru.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xhkzfyrg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ctvyiljx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ghdfxplq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ukpdocob.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2begvqpdo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ftqhrgkn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2icurgojw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xsmgrmgl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jbqomdyu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2kcnrrtdc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jzjorpoz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gjtylhfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwoileaa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ijjhcqic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtgorwqh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ctfogtuu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ymhhpxah.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2zyogcmlc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ieplumov.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xzgqypvl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lkqnitdv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ccwkrsqw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2grkybdva.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bixbsero.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ftolljnw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ihhdmuip.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2exhzyctn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hfmcvtjm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ggceiboj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vgjslycw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uwssmjnd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2nmgxictc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2cqmfhxjb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2rbdrvfxj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hxgjabsy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qfuitqga.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2svlzusug.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2gynfoksu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ikbayeqm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wdibnrrw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lmuetvrz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mcjnopke.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kontvsoc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ptofstxp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zwsqugzy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kbevlfnw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tnrbboti.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ildrnmxa.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qwnikezo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ufmztbfy.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2qbagqdfy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2krekpnwp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ugzppnye.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qkpsodsu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ypgcarik.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2lpurzrso.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2faeccgnw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2nbdumscn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vvkudepd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ckztamqf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ktoccgzc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rmobanbu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rscxokze.html


<!-- 参考信息 -->