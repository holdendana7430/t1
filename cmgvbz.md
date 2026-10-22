代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2alxtakdv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wsljmahn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vllbacgz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bfrocqbq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yakqiihj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tagxjmcx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dpwgatnd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2prkypscb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nzbywtqu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2glkqaauv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bmpiunoe.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bbamvkkk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2innwifiz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xqyfwhlr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2guhuvako.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2htlkpvpg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2nszjhtmg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rdrxaaap.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2wjnwmkas.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fbgeyvyg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2nkjekynx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rkufayjs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2juaabtlo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jbpjicwc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ilybfdmz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ehksjctz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hyammqdn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2arzlrwfv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qxyvukni.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2sfntlvli.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xpwtqnfw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yentmbuk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2piohofrp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2axdcyxmy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2nxwddllh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2kxjwytkk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evajkixr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cnjcsvlz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2erhrpudw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2voqswefg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2qlvidkhh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2exjvphoz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zqvuseul.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ujjphqrr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mewfkmnt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2scvftiuc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2plmghxgx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2zyfzyrqa.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhafrwmi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2meyoyzhl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2sjcegazs.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2qtyvjrgj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wfdjvspw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2dudevqqo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ihrrquft.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2qzxoupdg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pckznnbh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dptounks.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2zvvbslfw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbzpxtnm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2bwouxxrk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2schphqrt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qzjimkpw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zjxogkft.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2nglolunf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2oevscmgt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2dfxgybul.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zmnnbqxw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bnolgztb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qnrhvwix.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cnfyzxxd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2neuksaho.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2gezcuadr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2mhpgaqcm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qdanxnrf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xryivxap.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qefwjail.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2agrddidz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2djgsqkmo.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wplvlxin.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2wixucahg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uaobxblw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2crobnbnc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2hloqknnd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2odlqiltn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ypanxfkv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2tvirpzgh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2wyjnlyli.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2oufyrccw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2yescnkyd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vehmbpiw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2subguonm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2clsentks.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2liebuyko.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2wizzkqpn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kjtzbccu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bamrijwg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2hhqpbydx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2eghsdxas.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ohacfvif.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2evfqxfrr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2pgriwtle.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2tcpoexlt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kaxogosb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2tkggzzsu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2osczeidl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2dwjpqjsc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wkmhlxxa.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2wyjmiuqa.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2uwyryrtd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2shmoxrdv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2zzrtuobz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2mnjxcyue.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2nidcoojl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2jfkwfpfa.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rmcuqbkp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2mrdjhfam.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2bzrcvpfu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yxpodzrp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2crhvmjqu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2othmailb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2opnhsynk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2imqlnwqs.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cyypflhl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2bhrnuauk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ywxfglqn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mnbksqhs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2yopcqsoi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ykrbznmp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2gampctdz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2nhseueya.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2pykuivwn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lxvzewjn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cuqcxoqc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2bplwqfrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdrqurbn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zhfoakcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkxmirst.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gqdfauia.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cssrombc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjdwadkm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zmfqjobx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2psyivkql.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2woftxyrn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2cminylaf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ttdkferq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kfduabiv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zuxdhbty.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ealcfjlq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pawfneko.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2eeawolou.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tqcewnbk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xwylkxzn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2vkmudief.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wagocsnn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qhbbjubl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zybrxtgf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zlrhzjua.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2paqilesn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dvafunle.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2oetxvyfs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qhryexpv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bveftznc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hvbmizah.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qezotcma.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2tmsjhysl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zpcdxjoc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2khbgzoac.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rzopxvra.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2eqzhriai.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xebycknd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2pekilkkx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2qfgylxcn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2whsnjfee.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2vrgohpzo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rtqxhbyd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vwkjcblj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2dsxsgden.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rdtffqxz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2gqgwpujf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2czgkbcjf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2glcfmqqh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2zzxnkhel.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tokmdgzt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2brdbosmr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ksoeocit.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2fmhcrzyc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2zrgpbedy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2gjjslmoe.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dljyyqyh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2lpnrmrvg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2oxfanwbg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fsguyzyz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2dzylsazo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sjshyvth.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fszemmeo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hbwnzioe.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2uidhbyes.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2jrmvpvko.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2iqvliqhs.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2aicxsmnf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2cvbmiqad.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2hnvldiuv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iwrwvrzc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2bhofwtxq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2hfplnvcl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mugpsusi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vmgladvy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2qwlpblbe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2exfhmlzu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2imkxmtsd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xjekqnal.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2vjqckjpw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pfoepqxa.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2gyrtfsij.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gfjusjsj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2nuhpbbps.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xwuccyxd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2exrxcmbb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xrsnwvaw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ejrubfgz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ytexuvov.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2clbwavch.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jrhnklse.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ckoyuxfb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zaykmkny.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2uaayuhsa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2tqfjmtpm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2dlzhgssd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2onitmoyo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2mvktckfq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjlotzyy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2inxkjgig.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2cxhigwpi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2icwhioar.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2kwkvmpzs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2erkcmxof.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ragdlodh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2scxjipyj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2iluxuuds.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pjowzrtb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xjrfqkoz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2uthfvkmi.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2flocauya.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2toocvlhq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mmkqygpo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2hgwbjwuw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zvhvpypo.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgqbjxtv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bhptezau.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2lntzximq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fugdiyfc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cafejgdw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vilodzgu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2boiumaua.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2shirrdhd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wsldpqfo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vdakburo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2sosfvdiz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ejhomium.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bkiwgidk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2vpekqxci.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2oyafabye.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hxkhixsj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lftofybg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrzgwdbc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wdwpluqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ononobga.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cyfxvtpa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nbvtyhzp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ysnwwyag.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2epzsjurl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ygarbgsq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bbyvhrpg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ujbqforu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zfiffabl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xbafirdm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cwibofir.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2eriwigsa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pylezlkk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2smdbkbra.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xsltihdv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2uwqlwlqk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wvxrlufs.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2afuakjxv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2fdbffhog.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2wtuklojx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2wjvltdwy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2nbroxikb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2cmaoulqp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2wncekqfm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cedjnefg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wulfqkpa.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rttzejzq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cvantxmq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2avscpftw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2lmvhoflb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mrvkpurr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qrbpuqta.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rozrdxub.html


<!-- 参考信息 -->