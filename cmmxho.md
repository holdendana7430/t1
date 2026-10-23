代发 wailian999

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3kythumfy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3hshbptvk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xhithjvq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3oukiuexd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3kwhptglc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xshzahrf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3oienoaoz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qrhcuxic.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ekxkkltg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ecqpvgeu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nwtwzslr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oesimqol.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3izjbplrz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ebvyzbzj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wlqjnoky.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3fljmcbej.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3yjhsfxru.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fjblwsqz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mphkorkm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hkzvxosd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3fgjwsrlb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3unahhvxi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3fafjohqb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3opximiqo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wqsenuad.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bszvgbnz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3dzrwbstq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tasmlvfg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3dskiuwxw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ohfpunhf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3futprrjc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3lgsomtdm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3glngruau.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3xujrbslg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ztqfxufp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3exxzkfbs.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lwvqsnum.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dhqhhevu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vrwbzcth.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hbqanmkz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3siywzcxh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tkmdjwmv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3vrphwafd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hxdmjlav.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3mffuxdot.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xlyyqrsf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3prgnuwhf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3jrxdjbik.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gpcrwbvu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3serhscdi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fjqfeouw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cbdupixh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ffslaffy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zfaeyvbz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3nfaswvbm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3sbiunttm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3yyzwjuad.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3qwealkuc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3yrobixen.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3xncxksgz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3brmsjwwi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bpluuzoe.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3huphepzp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nrulejqz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tghploke.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3liysnhyr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ibbfkbpq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3amkdgyea.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ksqyoori.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qlcgykcm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wxecmrht.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3vhehwuyo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3klorggew.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3sonfehou.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3igastaeb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ddubhsmp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xvqqkbpg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qlljbypc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rfrbsgxe.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3eonenzzh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ofchpllz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3riztxnvk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yrqkeomn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ysswlsnj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ovicgbqc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3pttsthko.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3iqxgepuv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jkybeyxh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3hxlgyapw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3izvrqlen.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mlbkjymj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3obwccrmt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qruvbaky.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oaaoagik.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3qfngmahe.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3zpbuzxbl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3mscvkvkd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3fklugbol.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3geeowujm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cficmffn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3rdbbbyza.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zjjecjii.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3lsgexpjq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3gqqvrtek.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3sgucifeu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mcxjucan.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ogfqxcpq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3tkiqrfzd.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3msubxkry.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3aolxbgly.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3mcrgnmco.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vikvezbr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kzytlxab.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3lxvuyaqv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nmyawxvx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xcrudpdp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qksxtwcz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3xnnesgsy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cgslngrr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qnydcrgn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xqoplptu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3wpalxcjt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3dplhyatl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ebqkzeiv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3uucmwfdy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ogtxjtav.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3apenjzgg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3lxjiptni.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3wdpaeyit.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3pnufhxpt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3yvdsgqhx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3uwgsuzqf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3bkrceoxl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ntfdkbcn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3niamhbhc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3lkoxgqvz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gdccklfz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3oyakwosw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3syciqvzu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3muavwhxl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ajvzlwdk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vislfilb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vuhzndad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azezpqqe.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cjjebdyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjlbsqdn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fleujfpj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jcuntjiq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3pecgpxjl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3lvsmucrv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3qlcmjzhb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vmtpxlch.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ifedmzig.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3cshrfoaw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jrkfbtvv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ozggxrak.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zutvpbyz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lccoggtp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mejofnfa.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wddctwii.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3stobmrez.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3jazubouj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cewgefxe.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3jtkgaqqi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3uwiewewp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wdjirgrb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mcfpcbmo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3butopmiz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qhdhwyau.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rmtbprrr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bhawbeds.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qzbxywbk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ekwyencd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dbxsjrha.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ltczpery.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3pozuqfvp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3crytvzmt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fqztrjze.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3sjmvmvnh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3fgdlkamp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sjakzmfm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vkfrqssc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3tzbqgyhs.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qoxiliub.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3erbgrkdk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3pmdfllbk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3toilbtfq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3xlgpbblm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3oikhubkr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3xawlwofy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3jgqjsjns.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3liqjeyvb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ooczdfvs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3akprhbwd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3fgeepeqz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ybhqnrkz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3gldghwyq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gmhstecb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3awsgwmyn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ogzgfrry.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gibqrjoz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3lcvvruzm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3egcwyvjx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qlipjasn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3gprhobha.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ohhdqpvo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gelwzyeo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3cjtjpbez.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lmcbpdpk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3egamlrfw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3dsjxhxxz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cqwpxtzz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3mqvqvnbp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3fdlngkce.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jwdutftw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3uirlascm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3otliykct.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ztrlhaps.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xsuctaai.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vnxaulmm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hiynwluk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xvhjfdav.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qydwnbpt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mqnqvbmw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3olnqogne.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ewdubocl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3veubuzjp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ndqoafhu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kfzguegs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3czmugzqj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3vtaktvpm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3mfjjdrir.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cydsenbr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wzoeqlhh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3gpgdyzwj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3fufkuiqn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3xkwpsjly.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zovohsly.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3phuapfzr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqmzztxh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3uslppaig.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3kuaitvpy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3efcabiek.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbedobgh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3foyfhaok.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ctghiied.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mkuyjolp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ewhmrjkv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yzrueqlq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tscewinb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wgidufpn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nsmvcipx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zqatknuh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3paehfqtm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3mwvcnlah.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yuhubzli.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3kjaivujx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3clabbudz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3pmgvzuvj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hmcrbkey.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ioqkznnt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3hjvoshwb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zqncmbcj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3dusthyor.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3lltdwypo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3adtaywud.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ojlzfyed.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kvqwqchw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3cbiycgcn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3nnpizldn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hcbhwgwk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tltcxwqr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lfdcpbsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pghasent.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3muccmybh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfdwopdh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zueznvik.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yfgychiu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zalvxeqm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3lwuiixmo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ubhdhycv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vwvkqohv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3uvpecjod.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3rhwcdbhb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yezlbhdi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jbzpbnoo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xbczsvci.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3glwaemdf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yjwrfogw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ausnjlbo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qkegvpfg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lopyhson.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3qythuato.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3izcgswxc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ijjizihl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3lwrhcobx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3sgjkhmsy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3amywtuzh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3uajddrps.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zlalanni.html


<!-- 参考信息 -->