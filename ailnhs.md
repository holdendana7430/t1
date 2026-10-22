代发 wailian999

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2jmvkcklh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dkqouabi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jmbqgaqu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bhhgegsz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2pwnzjyrn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2iqlzggsn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pofjmfeh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2mfawvacx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jrbhzmsa.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2bdpqntud.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2gkrqjfmm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2qpwtwsyw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zphbixrx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2pudvngqf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2akmwvybt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ionwkpuk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ashwcrvl.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2upvkzndc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2dmlabyny.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ujfnlqxw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2diqfwsfx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2axwrdgnj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruvcwizx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mxvwrkye.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2fejjkhqs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2zzerrcgr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2krrslknw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2adpowoax.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2artwiaiy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2lbqrgtbh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2nxyrdbzt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2oikzlatn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2theitrae.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2wbimfvzc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qqpgfffb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2kcjqzdfb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fmbqqdsh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qwolsfbk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vbpbsjrv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tfvcgekb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ygwzoezd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hervitkj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tawsyyuc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2auggacke.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2egtgisok.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ktouxjij.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2itbbvedi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2bmjlukfe.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2sotbrxcw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fsckhovx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2iynrmkfm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2fslhrppl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2srmjvfso.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lliwbgsu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rzbubxxd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qlqafyvh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2yxpdwgoc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2icpvpdkt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2thdcrtes.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rlhovlhv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wromvevr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lqvyyujg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pbtnqzgr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qxqdriix.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2uhxjojot.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2oxjxpono.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ravxlgax.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2nldlgwbf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2qwqqqycv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cdbyafac.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jjfvaupj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2zijuyxup.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2zmuaqgye.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2bnfnmmps.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2mwbfgccq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2skbelzhu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ffrjlcgv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vslqgxim.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2gicsjfdh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2xurddjhj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ehewcvph.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2qnxvwdqp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2zawqeheh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2afetjdbv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pjwcgezz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2fnrzfjws.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2zzhlzzcn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qkbcnfey.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kcwcpzlb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2uklzpoga.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ctasodzm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2medgewmt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2vyuglsqq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2grksipyk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fjjtjdzv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2prmolvod.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2cqcnjdvj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2mkzlpqam.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2kdervnlk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qxfzlmiy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2hiursosp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2jctzdfmt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2smawumfa.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2byhofmij.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wbrzwdal.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2myfsvmio.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2hfhxtzvd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2epyqxkfa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wslsewtk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2rpdywopw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2itwpracb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wqfoaobq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2qrpawzwh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lqytaheb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fjjvdbrb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2vxkakchh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2uyoklvgp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2vhyihmng.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2nrzmdbhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdrnifls.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ewqpbflc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdkdbzvx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2msuzmpxj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2mawvktve.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2yidbpxjx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gzkglzkq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2jwtqueyc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2oytkyhze.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2cdzxccts.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2dzydqyqx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qvoivcgz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tynbdykv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wazyvtvh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vyprizmn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2yecsqxkz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dlfzhtnl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2usdwcvma.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2kxjvgttp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xencmsmu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2slcoyccn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2laypsvfp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ossyugxb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dwslohwg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yipxoydv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2esckvywv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zmmvltue.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kceddvou.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wkzbdvvr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vvuggsnp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2viyajyci.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zrvmfnuy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jetqwhxm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2wgcidtqt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ziizfhzv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2kgfocuie.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2oidnabwv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2pxotcufy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bjynmtsq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hkvzvtwd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rqoswhap.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2nzkiczir.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ogtrgeon.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2twzfmdyi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2gdwvsaoq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xdorntlq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2hvmqblbo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bvgghliy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rhkhzenw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xaiajhkp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tzdiybef.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2eexzgpil.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2sfprtkmc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2asjretry.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2bximhabc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2viylmdol.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2awrjiioy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qqrgoqwf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2umdkdarg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iodstwhg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2odytfftq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vkhzjezq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2gtwgedgr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ogodxwvy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ktwpuhub.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2nbqjbrdh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2adnhrsml.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2exwgmcnq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ncbsjbva.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2zwndvfva.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2csdsvbce.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rbrhcqug.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tmsvzyiy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2irvwrjhh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2cezxxgqv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vlppalax.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ajftcgzv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2whomblue.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wrvhkhtt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2vcmxgvyl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gblfyxzw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2czicvvrv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gudjoclk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xihcmtxl.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mytbwout.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2dlxkfnzi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2cxwdxftl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ysghtjye.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ghgwyiqf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jhdwxdeu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pqfljuno.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtevcoss.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2qqccnayf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2xeumtmar.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mqgiwweo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2qwoornlf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvhcrwoi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ohswpliq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2mflestfv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2upirnizf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zlvkvlch.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2irovaxsg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2trlyjpin.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fsecboqk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2noybjaio.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pluxqztz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2dqxugqyz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cbgkdywf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vbshhclu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2invfothe.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2edsyetwa.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2yotzfqvh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vtxysdfy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xxdqaarj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2oaursegu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2hajyjwrx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2cjbkindk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xptgevrz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2qvamquun.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2elaijglc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ceanqzlp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2lffnerng.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2fsjgkhgm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pnqbewmv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2btrypicf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2slmvmbxm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2rdrpyxst.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2nhnknhbz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2owhznorn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ywxrfwvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuposqkh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wccikltf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cffzhdei.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pvnimwje.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2agiiwnsq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kddiyywl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gaikzfkm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cgaxwkco.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kzptjumf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cruplcey.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ccnexpto.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2mjtfbvuc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2nwtybbrq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xodztfwx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vhuaheeb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2usoagtpg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2pwdjqjek.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gzbvkrqc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wcytexgf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2iupaiess.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2pmjbxxkt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2dklkxthp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2csiulihs.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2jrncivgp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2hbxaekqq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2vodhizto.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jrzvcirf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kerikwhy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uvkbucqc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ayhfeyrx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2armezmkf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2eulymdoa.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2purixscy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iynnpsjv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qbptbhoq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2aawilagk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2kakubndf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gxgnmupd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ndowivbj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xatscqgj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2wngxpqae.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2acwfhshj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2uafmcfwj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tppargsb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2qgtavugy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2emkalzij.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mjxxlhyj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2uiissrfz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cbbdrvdx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wgtmqlkz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2botagwxl.html


<!-- 参考信息 -->